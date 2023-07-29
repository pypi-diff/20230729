# Comparing `tmp/deepdoctection-0.25.tar.gz` & `tmp/deepdoctection-0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdoctection-0.25.tar", last modified: Fri Jun 30 11:37:43 2023, max compression
+gzip compressed data, was "deepdoctection-0.26.tar", last modified: Sat Jul 29 17:06:16 2023, max compression
```

## Comparing `deepdoctection-0.25.tar` & `deepdoctection-0.26.tar`

### file list

```diff
@@ -1,270 +1,271 @@
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.855733 deepdoctection-0.25/
--rw-rw-r--   0 janis     (1000) janis     (1000)    11351 2022-06-16 05:58:47.000000 deepdoctection-0.25/LICENSE
--rw-rw-r--   0 janis     (1000) janis     (1000)    10653 2023-06-30 11:37:43.855733 deepdoctection-0.25/PKG-INFO
--rw-rw-r--   0 janis     (1000) janis     (1000)     9929 2023-06-22 12:40:19.000000 deepdoctection-0.25/README.md
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.783733 deepdoctection-0.25/deepdoctection/
--rw-rw-r--   0 janis     (1000) janis     (1000)    11919 2023-06-30 11:36:14.000000 deepdoctection-0.25/deepdoctection/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.783733 deepdoctection-0.25/deepdoctection/analyzer/
--rw-rw-r--   0 janis     (1000) janis     (1000)      706 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/analyzer/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    14920 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/analyzer/dd.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.783733 deepdoctection-0.25/deepdoctection/configs/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/configs/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1971 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/configs/conf_dd_one.yaml
--rw-rw-r--   0 janis     (1000) janis     (1000)       35 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/configs/conf_tesseract.yaml
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.787733 deepdoctection-0.25/deepdoctection/dataflow/
--rw-rw-r--   0 janis     (1000) janis     (1000)      845 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/dataflow/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6806 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/dataflow/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10039 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/dataflow/common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6736 2023-02-23 18:53:18.000000 deepdoctection-0.25/deepdoctection/dataflow/custom.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    20342 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/dataflow/custom_serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15599 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/dataflow/parallel_map.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4526 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/dataflow/serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9604 2023-02-23 18:53:12.000000 deepdoctection-0.25/deepdoctection/dataflow/stats.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.787733 deepdoctection-0.25/deepdoctection/datapoint/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1643 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datapoint/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19089 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/datapoint/annotation.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    23341 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/datapoint/box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6824 2023-02-23 18:53:12.000000 deepdoctection-0.25/deepdoctection/datapoint/convert.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    27294 2023-05-23 14:43:35.000000 deepdoctection-0.25/deepdoctection/datapoint/image.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    31183 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/datapoint/view.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.787733 deepdoctection-0.25/deepdoctection/datasets/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1154 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7421 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/datasets/adapter.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    18887 2023-02-23 18:53:12.000000 deepdoctection-0.25/deepdoctection/datasets/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4105 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/dataflow_builder.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    20603 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/datasets/info.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.791733 deepdoctection-0.25/deepdoctection/datasets/instances/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1388 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/datasets/instances/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12014 2023-02-23 18:53:12.000000 deepdoctection-0.25/deepdoctection/datasets/instances/doclaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11968 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/datasets/instances/fintabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6938 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/instances/funsd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6491 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/instances/iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4675 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/instances/layouttest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5193 2023-02-20 09:20:02.000000 deepdoctection-0.25/deepdoctection/datasets/instances/publaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11948 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/datasets/instances/pubtables1m.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8509 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/datasets/instances/pubtabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6608 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/instances/rvlcdip.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7715 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/instances/xfund.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.791733 deepdoctection-0.25/deepdoctection/datasets/instances/xsl/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/datasets/instances/xsl/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1952 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/datasets/instances/xsl/pascal_voc.xsl
--rw-rw-r--   0 janis     (1000) janis     (1000)     2543 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3326 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/save.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.795733 deepdoctection-0.25/deepdoctection/eval/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1006 2022-06-30 08:30:21.000000 deepdoctection-0.25/deepdoctection/eval/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19509 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/eval/accmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4804 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/eval/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8755 2023-06-28 06:38:28.000000 deepdoctection-0.25/deepdoctection/eval/cocometric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19097 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/eval/eval.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1051 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/eval/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9069 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/eval/tedsmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5713 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/eval/tp_eval_callback.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.799733 deepdoctection-0.25/deepdoctection/extern/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1140 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/extern/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11989 2023-06-28 06:38:28.000000 deepdoctection-0.25/deepdoctection/extern/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11010 2023-05-07 17:37:06.000000 deepdoctection-0.25/deepdoctection/extern/d2detect.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1866 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/deskew.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12381 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/extern/doctrocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2999 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/fastlang.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9319 2023-05-07 17:37:06.000000 deepdoctection-0.25/deepdoctection/extern/hfdetr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    39403 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/extern/hflayoutlm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    46449 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/extern/model.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3692 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/pdftext.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.799733 deepdoctection-0.25/deepdoctection/extern/pt/
--rw-rw-r--   0 janis     (1000) janis     (1000)      699 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/extern/pt/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1372 2022-06-22 06:44:07.000000 deepdoctection-0.25/deepdoctection/extern/pt/ptutils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12292 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/extern/tessocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5654 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/extern/texocr.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.803733 deepdoctection-0.25/deepdoctection/extern/tp/
--rw-rw-r--   0 janis     (1000) janis     (1000)      706 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/extern/tp/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1479 2022-06-22 06:44:07.000000 deepdoctection-0.25/deepdoctection/extern/tp/tfutils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5054 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpcompat.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.803733 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3664 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/common.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.803733 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/config/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/config/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11284 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/config/config.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.807733 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9362 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13545 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7061 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5685 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11006 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17743 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4597 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4215 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/predict.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11947 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/preproc.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.807733 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/utils/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/utils/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2203 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3539 2023-02-13 13:44:17.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7525 2023-05-07 17:37:06.000000 deepdoctection-0.25/deepdoctection/extern/tpdetect.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.811733 deepdoctection-0.25/deepdoctection/mapper/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1390 2023-02-13 13:44:17.000000 deepdoctection-0.25/deepdoctection/mapper/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15505 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/mapper/cats.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6055 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/mapper/cocostruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8537 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/mapper/d2struct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5593 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/mapper/hfstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    35638 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/mapper/laylmstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7775 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/mapper/maputils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7912 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/mapper/match.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6520 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/mapper/misc.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3844 2022-09-21 17:02:22.000000 deepdoctection-0.25/deepdoctection/mapper/pascalstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6876 2022-09-27 06:19:11.000000 deepdoctection-0.25/deepdoctection/mapper/prodigystruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    23583 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/mapper/pubstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5090 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/mapper/tpstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8808 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/mapper/xfundstruct.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.819733 deepdoctection-0.25/deepdoctection/pipe/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1121 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/pipe/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13961 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/pipe/anngen.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13245 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/pipe/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11062 2023-05-23 14:43:35.000000 deepdoctection-0.25/deepdoctection/pipe/cell.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13942 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/pipe/common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9425 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/pipe/concurrency.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8872 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/pipe/doctectionpipe.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5579 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/pipe/language.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5262 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/pipe/layout.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    18031 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/pipe/lm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    32279 2023-06-29 09:06:33.000000 deepdoctection-0.25/deepdoctection/pipe/order.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    22418 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/pipe/refine.py
--rw-rw-r--   0 janis     (1000) janis     (1000)      902 2022-08-12 12:59:53.000000 deepdoctection-0.25/deepdoctection/pipe/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    50554 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/pipe/segment.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10977 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/pipe/text.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3138 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/pipe/transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/py.typed
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.819733 deepdoctection-0.25/deepdoctection/train/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1196 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/train/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15612 2023-02-23 18:53:12.000000 deepdoctection-0.25/deepdoctection/train/d2_frcnn_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10538 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/train/hf_detr_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    21125 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/train/hf_layoutlm_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12968 2023-02-23 18:53:12.000000 deepdoctection-0.25/deepdoctection/train/tp_frcnn_train.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.827733 deepdoctection-0.25/deepdoctection/utils/
--rw-rw-r--   0 janis     (1000) janis     (1000)     2238 2022-09-27 06:16:10.000000 deepdoctection-0.25/deepdoctection/utils/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4612 2023-01-05 12:44:38.000000 deepdoctection-0.25/deepdoctection/utils/concurrency.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3998 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/utils/context.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2022-09-12 13:32:10.000000 deepdoctection-0.25/deepdoctection/utils/detection_types.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3441 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/utils/develop.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17992 2023-02-23 18:53:12.000000 deepdoctection-0.25/deepdoctection/utils/file_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7626 2022-09-27 06:19:11.000000 deepdoctection-0.25/deepdoctection/utils/fs.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2159 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/utils/identifier.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8627 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/utils/logger.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5203 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/utils/metacfg.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7564 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/utils/pdf_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11954 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/utils/settings.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1923 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/utils/systools.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1813 2022-09-12 13:32:10.000000 deepdoctection-0.25/deepdoctection/utils/tqdm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8247 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/utils/transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5323 2022-09-27 06:19:11.000000 deepdoctection-0.25/deepdoctection/utils/utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10115 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/utils/viz.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.783733 deepdoctection-0.25/deepdoctection.egg-info/
--rw-rw-r--   0 janis     (1000) janis     (1000)    10653 2023-06-30 11:37:43.000000 deepdoctection-0.25/deepdoctection.egg-info/PKG-INFO
--rw-rw-r--   0 janis     (1000) janis     (1000)     7958 2023-06-30 11:37:43.000000 deepdoctection-0.25/deepdoctection.egg-info/SOURCES.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)        1 2023-06-30 11:37:43.000000 deepdoctection-0.25/deepdoctection.egg-info/dependency_links.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)     2260 2023-06-30 11:37:43.000000 deepdoctection-0.25/deepdoctection.egg-info/requires.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)       30 2023-06-30 11:37:43.000000 deepdoctection-0.25/deepdoctection.egg-info/top_level.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)     2368 2023-06-30 11:37:43.859732 deepdoctection-0.25/setup.cfg
--rw-rw-r--   0 janis     (1000) janis     (1000)     6406 2023-06-30 11:37:35.000000 deepdoctection-0.25/setup.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.827733 deepdoctection-0.25/tests/
--rw-rw-r--   0 janis     (1000) janis     (1000)      725 2022-09-18 14:33:32.000000 deepdoctection-0.25/tests/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.827733 deepdoctection-0.25/tests/analyzer/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/analyzer/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5326 2023-06-30 07:04:23.000000 deepdoctection-0.25/tests/analyzer/test_dd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17378 2023-05-03 16:43:31.000000 deepdoctection-0.25/tests/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    64681 2022-11-28 15:25:21.000000 deepdoctection-0.25/tests/data.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.831733 deepdoctection-0.25/tests/dataflow/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/dataflow/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2342 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/dataflow/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5389 2023-05-07 15:01:33.000000 deepdoctection-0.25/tests/dataflow/test_common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1632 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/dataflow/test_custom.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4274 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/dataflow/test_custom_serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/dataflow/test_parallel_map.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2836 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/dataflow/test_stats.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.831733 deepdoctection-0.25/tests/datapoint/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/datapoint/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7468 2022-09-06 06:55:23.000000 deepdoctection-0.25/tests/datapoint/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4860 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/datapoint/test_annotation.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12861 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/datapoint/test_box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1534 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/datapoint/test_convert.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12141 2023-05-07 15:01:33.000000 deepdoctection-0.25/tests/datapoint/test_image.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3670 2023-06-22 12:40:28.000000 deepdoctection-0.25/tests/datapoint/test_view.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.835733 deepdoctection-0.25/tests/datasets/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/datasets/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.835733 deepdoctection-0.25/tests/datasets/instances/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/datasets/instances/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)      974 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/datasets/instances/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1285 2022-11-03 14:05:55.000000 deepdoctection-0.25/tests/datasets/instances/test_doclaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2514 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/datasets/instances/test_fintabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2091 2023-05-07 15:01:33.000000 deepdoctection-0.25/tests/datasets/instances/test_funsd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1263 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/datasets/instances/test_iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1911 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/datasets/instances/test_layouttest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1922 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/datasets/instances/test_publaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1921 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/datasets/instances/test_pubtables1m.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1924 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/datasets/instances/test_pubtabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1464 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/datasets/instances/test_rvlcdip.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2704 2022-06-29 12:05:00.000000 deepdoctection-0.25/tests/datasets/test_adapter.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8598 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/datasets/test_info.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2153 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/datasets/test_registry.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.839733 deepdoctection-0.25/tests/eval/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/eval/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3244 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/eval/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12696 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/eval/test_accmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3803 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/eval/test_cocometric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2952 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/eval/test_eval.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2418 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/eval/test_registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1253 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/eval/test_tedsmetric.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.843732 deepdoctection-0.25/tests/extern/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/extern/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2393 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/extern/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5426 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/extern/data.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1652 2022-11-03 14:06:59.000000 deepdoctection-0.25/tests/extern/test_deskew.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4973 2023-05-07 15:01:33.000000 deepdoctection-0.25/tests/extern/test_doctrocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2142 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/extern/test_fastlang.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3781 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/extern/test_hfdetr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19460 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/extern/test_hflayoutlm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2066 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/extern/test_pdftext.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3438 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/extern/test_tessocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1734 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/extern/test_texocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4372 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/extern/test_tpdetect.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.847733 deepdoctection-0.25/tests/mapper/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/mapper/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7056 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/mapper/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    81693 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/mapper/data.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10518 2023-06-09 06:48:22.000000 deepdoctection-0.25/tests/mapper/test_cats.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3621 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/mapper/test_cocostruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1907 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/mapper/test_d2struct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2050 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/mapper/test_hfstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2382 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/mapper/test_iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5556 2023-06-09 06:48:22.000000 deepdoctection-0.25/tests/mapper/test_laylmstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/mapper/test_misc.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2867 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/mapper/test_prodigystruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6679 2023-05-07 15:01:33.000000 deepdoctection-0.25/tests/mapper/test_pubstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/mapper/test_tpstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/mapper/test_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2555 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/mapper/test_xfundstruct.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.855733 deepdoctection-0.25/tests/pipe/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/pipe/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6290 2022-10-24 07:01:39.000000 deepdoctection-0.25/tests/pipe/test_anngen.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4498 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/pipe/test_cell.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3449 2023-02-13 13:44:17.000000 deepdoctection-0.25/tests/pipe/test_common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2676 2023-06-22 12:40:28.000000 deepdoctection-0.25/tests/pipe/test_language.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1955 2022-10-24 07:01:39.000000 deepdoctection-0.25/tests/pipe/test_layout.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4604 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/pipe/test_lm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7862 2023-06-22 12:40:28.000000 deepdoctection-0.25/tests/pipe/test_order.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9676 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/pipe/test_refine.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1784 2023-05-07 15:01:33.000000 deepdoctection-0.25/tests/pipe/test_registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    14433 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/pipe/test_segment.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7862 2023-06-22 12:40:28.000000 deepdoctection-0.25/tests/pipe/test_text.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1892 2022-11-03 14:06:59.000000 deepdoctection-0.25/tests/pipe/test_transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2260 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/test_utils.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.855733 deepdoctection-0.25/tests/train/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/train/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3239 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/train/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1854 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/train/test_d2_frcnn_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3540 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/train/test_tp_frcnn_train.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.855733 deepdoctection-0.25/tests_d2/
--rw-rw-r--   0 janis     (1000) janis     (1000)      761 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests_d2/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1580 2022-09-21 17:02:23.000000 deepdoctection-0.25/tests_d2/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3226 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests_d2/test_d2detect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.484120 deepdoctection-0.26/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11351 2022-06-16 05:58:47.000000 deepdoctection-0.26/LICENSE
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12470 2023-07-29 17:06:16.484120 deepdoctection-0.26/PKG-INFO
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11746 2023-07-29 12:41:17.000000 deepdoctection-0.26/README.md
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.468120 deepdoctection-0.26/deepdoctection/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11968 2023-07-29 17:04:15.000000 deepdoctection-0.26/deepdoctection/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.468120 deepdoctection-0.26/deepdoctection/analyzer/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      706 2023-05-07 15:01:33.000000 deepdoctection-0.26/deepdoctection/analyzer/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    16030 2023-07-29 12:41:17.000000 deepdoctection-0.26/deepdoctection/analyzer/dd.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.468120 deepdoctection-0.26/deepdoctection/configs/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.26/deepdoctection/configs/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2168 2023-07-29 12:41:17.000000 deepdoctection-0.26/deepdoctection/configs/conf_dd_one.yaml
+-rw-rw-r--   0 janis     (1000) janis     (1000)       35 2022-06-16 05:58:47.000000 deepdoctection-0.26/deepdoctection/configs/conf_tesseract.yaml
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.472120 deepdoctection-0.26/deepdoctection/dataflow/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      845 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/dataflow/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6806 2023-05-07 15:01:33.000000 deepdoctection-0.26/deepdoctection/dataflow/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10018 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/dataflow/common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6720 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/dataflow/custom.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    20325 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/dataflow/custom_serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15583 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/dataflow/parallel_map.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4526 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/dataflow/serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9560 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/dataflow/stats.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.472120 deepdoctection-0.26/deepdoctection/datapoint/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1643 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/datapoint/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19073 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/datapoint/annotation.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    23341 2023-06-22 12:40:28.000000 deepdoctection-0.26/deepdoctection/datapoint/box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6879 2023-07-29 12:41:17.000000 deepdoctection-0.26/deepdoctection/datapoint/convert.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    27291 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/datapoint/image.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    33600 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/datapoint/view.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.472120 deepdoctection-0.26/deepdoctection/datasets/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1154 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/datasets/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7405 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/datasets/adapter.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    18887 2023-02-23 18:53:12.000000 deepdoctection-0.26/deepdoctection/datasets/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4105 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/datasets/dataflow_builder.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    20603 2023-06-09 06:48:22.000000 deepdoctection-0.26/deepdoctection/datasets/info.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.472120 deepdoctection-0.26/deepdoctection/datasets/instances/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1388 2023-02-09 09:34:37.000000 deepdoctection-0.26/deepdoctection/datasets/instances/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12014 2023-02-23 18:53:12.000000 deepdoctection-0.26/deepdoctection/datasets/instances/doclaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11968 2023-05-07 15:01:33.000000 deepdoctection-0.26/deepdoctection/datasets/instances/fintabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6938 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/datasets/instances/funsd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6628 2023-07-29 12:41:17.000000 deepdoctection-0.26/deepdoctection/datasets/instances/iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4675 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/datasets/instances/layouttest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5193 2023-02-20 09:20:02.000000 deepdoctection-0.26/deepdoctection/datasets/instances/publaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12231 2023-07-29 12:41:17.000000 deepdoctection-0.26/deepdoctection/datasets/instances/pubtables1m.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8509 2023-05-07 15:01:33.000000 deepdoctection-0.26/deepdoctection/datasets/instances/pubtabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6608 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/datasets/instances/rvlcdip.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7715 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/datasets/instances/xfund.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.472120 deepdoctection-0.26/deepdoctection/datasets/instances/xsl/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.26/deepdoctection/datasets/instances/xsl/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1952 2022-06-16 05:58:47.000000 deepdoctection-0.26/deepdoctection/datasets/instances/xsl/pascal_voc.xsl
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2543 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/datasets/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3326 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/datasets/save.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.472120 deepdoctection-0.26/deepdoctection/eval/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1006 2022-06-30 08:30:21.000000 deepdoctection-0.26/deepdoctection/eval/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19554 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/eval/accmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4803 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/eval/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8755 2023-06-28 06:38:28.000000 deepdoctection-0.26/deepdoctection/eval/cocometric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19078 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/eval/eval.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1051 2022-06-16 05:58:47.000000 deepdoctection-0.26/deepdoctection/eval/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9069 2023-07-29 12:41:17.000000 deepdoctection-0.26/deepdoctection/eval/tedsmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5713 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/eval/tp_eval_callback.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.472120 deepdoctection-0.26/deepdoctection/extern/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1194 2023-07-29 12:41:17.000000 deepdoctection-0.26/deepdoctection/extern/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11989 2023-06-28 06:38:28.000000 deepdoctection-0.26/deepdoctection/extern/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    18725 2023-07-29 12:41:17.000000 deepdoctection-0.26/deepdoctection/extern/d2detect.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1866 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/deskew.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12380 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/extern/doctrocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2999 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/fastlang.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9319 2023-05-07 17:37:06.000000 deepdoctection-0.26/deepdoctection/extern/hfdetr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    39398 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/extern/hflayoutlm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    48853 2023-07-29 12:41:17.000000 deepdoctection-0.26/deepdoctection/extern/model.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3692 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/pdftext.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.472120 deepdoctection-0.26/deepdoctection/extern/pt/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      771 2023-07-29 12:41:17.000000 deepdoctection-0.26/deepdoctection/extern/pt/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1458 2023-07-29 12:41:17.000000 deepdoctection-0.26/deepdoctection/extern/pt/nms.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1372 2022-06-22 06:44:07.000000 deepdoctection-0.26/deepdoctection/extern/pt/ptutils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12292 2023-06-22 12:40:28.000000 deepdoctection-0.26/deepdoctection/extern/tessocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5654 2023-05-07 15:01:33.000000 deepdoctection-0.26/deepdoctection/extern/texocr.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.472120 deepdoctection-0.26/deepdoctection/extern/tp/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      706 2022-06-16 05:58:47.000000 deepdoctection-0.26/deepdoctection/extern/tp/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1479 2022-06-22 06:44:07.000000 deepdoctection-0.26/deepdoctection/extern/tp/tfutils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5054 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpcompat.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.476120 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3664 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/common.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.476120 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/config/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/config/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11284 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/config/config.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.476120 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9362 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13545 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7061 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5685 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11006 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17743 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4597 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4215 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/predict.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11947 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/preproc.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.476120 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/utils/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/utils/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2203 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3539 2023-02-13 13:44:17.000000 deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7525 2023-05-07 17:37:06.000000 deepdoctection-0.26/deepdoctection/extern/tpdetect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.476120 deepdoctection-0.26/deepdoctection/mapper/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1294 2023-07-29 12:41:17.000000 deepdoctection-0.26/deepdoctection/mapper/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15505 2023-06-09 06:48:22.000000 deepdoctection-0.26/deepdoctection/mapper/cats.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6054 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/mapper/cocostruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8589 2023-07-29 12:41:17.000000 deepdoctection-0.26/deepdoctection/mapper/d2struct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5593 2023-02-09 09:34:37.000000 deepdoctection-0.26/deepdoctection/mapper/hfstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    35638 2023-07-04 16:42:30.000000 deepdoctection-0.26/deepdoctection/mapper/laylmstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7775 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/mapper/maputils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7912 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/mapper/match.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6520 2023-05-07 15:01:33.000000 deepdoctection-0.26/deepdoctection/mapper/misc.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3844 2022-09-21 17:02:22.000000 deepdoctection-0.26/deepdoctection/mapper/pascalstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6876 2022-09-27 06:19:11.000000 deepdoctection-0.26/deepdoctection/mapper/prodigystruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    23567 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/mapper/pubstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5090 2023-05-07 15:01:33.000000 deepdoctection-0.26/deepdoctection/mapper/tpstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8807 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/mapper/xfundstruct.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.476120 deepdoctection-0.26/deepdoctection/pipe/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1121 2023-06-22 12:40:28.000000 deepdoctection-0.26/deepdoctection/pipe/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13961 2023-06-22 12:40:28.000000 deepdoctection-0.26/deepdoctection/pipe/anngen.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13245 2023-06-09 06:48:22.000000 deepdoctection-0.26/deepdoctection/pipe/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11062 2023-05-23 14:43:35.000000 deepdoctection-0.26/deepdoctection/pipe/cell.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13941 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/pipe/common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9531 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/pipe/concurrency.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8872 2023-06-22 12:40:28.000000 deepdoctection-0.26/deepdoctection/pipe/doctectionpipe.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5579 2023-06-22 12:40:28.000000 deepdoctection-0.26/deepdoctection/pipe/language.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5262 2023-06-30 07:04:23.000000 deepdoctection-0.26/deepdoctection/pipe/layout.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    18031 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/pipe/lm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    32277 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/pipe/order.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    22410 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/pipe/refine.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)      902 2022-08-12 12:59:53.000000 deepdoctection-0.26/deepdoctection/pipe/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    50446 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/pipe/segment.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10985 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/pipe/text.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3138 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/pipe/transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-05-07 15:01:33.000000 deepdoctection-0.26/deepdoctection/py.typed
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.476120 deepdoctection-0.26/deepdoctection/train/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1196 2023-02-09 09:34:37.000000 deepdoctection-0.26/deepdoctection/train/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15612 2023-02-23 18:53:12.000000 deepdoctection-0.26/deepdoctection/train/d2_frcnn_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10538 2023-02-09 09:34:37.000000 deepdoctection-0.26/deepdoctection/train/hf_detr_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    21141 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/train/hf_layoutlm_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12952 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/train/tp_frcnn_train.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.480120 deepdoctection-0.26/deepdoctection/utils/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2238 2022-09-27 06:16:10.000000 deepdoctection-0.26/deepdoctection/utils/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4583 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/utils/concurrency.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3998 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/utils/context.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2022-09-12 13:32:10.000000 deepdoctection-0.26/deepdoctection/utils/detection_types.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3441 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/utils/develop.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17938 2023-07-29 12:41:17.000000 deepdoctection-0.26/deepdoctection/utils/file_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7626 2022-09-27 06:19:11.000000 deepdoctection-0.26/deepdoctection/utils/fs.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2159 2022-06-16 05:58:47.000000 deepdoctection-0.26/deepdoctection/utils/identifier.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8650 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/utils/logger.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5203 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/utils/metacfg.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7530 2023-07-29 12:41:17.000000 deepdoctection-0.26/deepdoctection/utils/pdf_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11979 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/utils/settings.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1923 2023-01-27 07:53:16.000000 deepdoctection-0.26/deepdoctection/utils/systools.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1830 2023-07-25 15:18:42.000000 deepdoctection-0.26/deepdoctection/utils/tqdm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8273 2023-07-28 11:28:58.000000 deepdoctection-0.26/deepdoctection/utils/transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5323 2022-09-27 06:19:11.000000 deepdoctection-0.26/deepdoctection/utils/utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10113 2023-07-04 16:45:21.000000 deepdoctection-0.26/deepdoctection/utils/viz.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.468120 deepdoctection-0.26/deepdoctection.egg-info/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12470 2023-07-29 17:06:16.000000 deepdoctection-0.26/deepdoctection.egg-info/PKG-INFO
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7990 2023-07-29 17:06:16.000000 deepdoctection-0.26/deepdoctection.egg-info/SOURCES.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)        1 2023-07-29 17:06:16.000000 deepdoctection-0.26/deepdoctection.egg-info/dependency_links.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1783 2023-07-29 17:06:16.000000 deepdoctection-0.26/deepdoctection.egg-info/requires.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)       30 2023-07-29 17:06:16.000000 deepdoctection-0.26/deepdoctection.egg-info/top_level.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2325 2023-07-29 17:06:16.484120 deepdoctection-0.26/setup.cfg
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6477 2023-07-29 17:04:15.000000 deepdoctection-0.26/setup.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.480120 deepdoctection-0.26/tests/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      725 2022-09-18 14:33:32.000000 deepdoctection-0.26/tests/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.480120 deepdoctection-0.26/tests/analyzer/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.26/tests/analyzer/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12802 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/analyzer/test_dd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17402 2023-07-25 15:18:42.000000 deepdoctection-0.26/tests/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    64681 2022-11-28 15:25:21.000000 deepdoctection-0.26/tests/data.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.480120 deepdoctection-0.26/tests/dataflow/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.26/tests/dataflow/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2342 2022-06-16 05:58:47.000000 deepdoctection-0.26/tests/dataflow/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5389 2023-05-07 15:01:33.000000 deepdoctection-0.26/tests/dataflow/test_common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1632 2022-10-12 13:27:51.000000 deepdoctection-0.26/tests/dataflow/test_custom.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4274 2022-10-12 13:27:51.000000 deepdoctection-0.26/tests/dataflow/test_custom_serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.26/tests/dataflow/test_parallel_map.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2836 2022-10-12 13:27:51.000000 deepdoctection-0.26/tests/dataflow/test_stats.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.480120 deepdoctection-0.26/tests/datapoint/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.26/tests/datapoint/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7468 2022-09-06 06:55:23.000000 deepdoctection-0.26/tests/datapoint/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4860 2023-01-27 07:53:16.000000 deepdoctection-0.26/tests/datapoint/test_annotation.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12861 2023-02-09 09:34:37.000000 deepdoctection-0.26/tests/datapoint/test_box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1534 2022-09-29 09:12:15.000000 deepdoctection-0.26/tests/datapoint/test_convert.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12141 2023-05-07 15:01:33.000000 deepdoctection-0.26/tests/datapoint/test_image.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3670 2023-06-22 12:40:28.000000 deepdoctection-0.26/tests/datapoint/test_view.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.480120 deepdoctection-0.26/tests/datasets/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.26/tests/datasets/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.480120 deepdoctection-0.26/tests/datasets/instances/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.26/tests/datasets/instances/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)      974 2022-06-16 05:58:47.000000 deepdoctection-0.26/tests/datasets/instances/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1285 2022-11-03 14:05:55.000000 deepdoctection-0.26/tests/datasets/instances/test_doclaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2514 2022-10-12 13:27:51.000000 deepdoctection-0.26/tests/datasets/instances/test_fintabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2091 2023-05-07 15:01:33.000000 deepdoctection-0.26/tests/datasets/instances/test_funsd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1268 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/datasets/instances/test_iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1911 2022-09-29 09:12:15.000000 deepdoctection-0.26/tests/datasets/instances/test_layouttest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1922 2022-10-12 13:27:51.000000 deepdoctection-0.26/tests/datasets/instances/test_publaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/datasets/instances/test_pubtables1m.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1924 2022-10-12 13:27:51.000000 deepdoctection-0.26/tests/datasets/instances/test_pubtabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1464 2022-10-12 13:27:51.000000 deepdoctection-0.26/tests/datasets/instances/test_rvlcdip.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2782 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/datasets/test_adapter.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8598 2023-01-27 07:53:16.000000 deepdoctection-0.26/tests/datasets/test_info.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2153 2023-02-09 09:34:37.000000 deepdoctection-0.26/tests/datasets/test_registry.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.480120 deepdoctection-0.26/tests/eval/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.26/tests/eval/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3244 2023-01-27 07:53:16.000000 deepdoctection-0.26/tests/eval/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12696 2023-01-27 07:53:16.000000 deepdoctection-0.26/tests/eval/test_accmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3818 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/eval/test_cocometric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2933 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/eval/test_eval.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2418 2022-10-12 13:27:51.000000 deepdoctection-0.26/tests/eval/test_registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1258 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/eval/test_tedsmetric.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.480120 deepdoctection-0.26/tests/extern/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.26/tests/extern/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2393 2023-02-09 09:34:37.000000 deepdoctection-0.26/tests/extern/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5426 2023-02-09 09:34:37.000000 deepdoctection-0.26/tests/extern/data.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1645 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/extern/test_deskew.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4956 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/extern/test_doctrocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2135 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/extern/test_fastlang.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3777 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/extern/test_hfdetr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19412 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/extern/test_hflayoutlm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2052 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/extern/test_pdftext.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3438 2022-10-12 13:27:51.000000 deepdoctection-0.26/tests/extern/test_tessocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1621 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/extern/test_texocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4360 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/extern/test_tpdetect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.484120 deepdoctection-0.26/tests/mapper/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.26/tests/mapper/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7056 2023-01-27 07:53:16.000000 deepdoctection-0.26/tests/mapper/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    81517 2023-07-25 15:18:42.000000 deepdoctection-0.26/tests/mapper/data.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10518 2023-06-09 06:48:22.000000 deepdoctection-0.26/tests/mapper/test_cats.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3621 2022-10-12 13:27:51.000000 deepdoctection-0.26/tests/mapper/test_cocostruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1903 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/mapper/test_d2struct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2046 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/mapper/test_hfstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2381 2023-07-25 15:18:42.000000 deepdoctection-0.26/tests/mapper/test_iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5552 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/mapper/test_laylmstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.26/tests/mapper/test_misc.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2867 2022-09-29 09:12:15.000000 deepdoctection-0.26/tests/mapper/test_prodigystruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6679 2023-05-07 15:01:33.000000 deepdoctection-0.26/tests/mapper/test_pubstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.26/tests/mapper/test_tpstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.26/tests/mapper/test_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2555 2023-01-27 07:53:16.000000 deepdoctection-0.26/tests/mapper/test_xfundstruct.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.484120 deepdoctection-0.26/tests/pipe/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.26/tests/pipe/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6290 2022-10-24 07:01:39.000000 deepdoctection-0.26/tests/pipe/test_anngen.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4498 2023-02-09 09:34:37.000000 deepdoctection-0.26/tests/pipe/test_cell.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3445 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/pipe/test_common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2676 2023-06-22 12:40:28.000000 deepdoctection-0.26/tests/pipe/test_language.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1955 2022-10-24 07:01:39.000000 deepdoctection-0.26/tests/pipe/test_layout.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4596 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/pipe/test_lm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7862 2023-06-22 12:40:28.000000 deepdoctection-0.26/tests/pipe/test_order.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9646 2023-07-25 15:18:42.000000 deepdoctection-0.26/tests/pipe/test_refine.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1784 2023-05-07 15:01:33.000000 deepdoctection-0.26/tests/pipe/test_registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    14449 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/pipe/test_segment.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7862 2023-06-22 12:40:28.000000 deepdoctection-0.26/tests/pipe/test_text.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1892 2022-11-03 14:06:59.000000 deepdoctection-0.26/tests/pipe/test_transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2244 2023-07-25 15:18:42.000000 deepdoctection-0.26/tests/test_utils.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.484120 deepdoctection-0.26/tests/train/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.26/tests/train/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3239 2023-01-27 07:53:16.000000 deepdoctection-0.26/tests/train/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1854 2022-09-29 09:12:15.000000 deepdoctection-0.26/tests/train/test_d2_frcnn_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3532 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests/train/test_tp_frcnn_train.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-07-29 17:06:16.484120 deepdoctection-0.26/tests_d2/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      761 2022-06-16 05:58:47.000000 deepdoctection-0.26/tests_d2/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1554 2023-06-30 12:58:23.000000 deepdoctection-0.26/tests_d2/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3220 2023-07-29 12:41:17.000000 deepdoctection-0.26/tests_d2/test_d2detect.py
```

### Comparing `deepdoctection-0.25/LICENSE` & `deepdoctection-0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/PKG-INFO` & `deepdoctection-0.26/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: deepdoctection
-Version: 0.25
-Summary: Repository for Document AI
-Home-page: https://github.com/deepdoctection/deepdoctection
-Author: Dr. Janis Meyer
-License: Apache License 2.0
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tf
-Provides-Extra: pt
-Provides-Extra: docs
-Provides-Extra: dev
-Provides-Extra: test
-Provides-Extra: hf
-License-File: LICENSE
-
 
 <p align="center">
   <img src="https://github.com/deepdoctection/deepdoctection/blob/master/docs/tutorials/_imgs/dd_logo.png" alt="Deep Doctection Logo" width="60%">
   <h3 align="center">
   A Document AI Package
   </h3>
 </p>
@@ -52,21 +29,25 @@
  - OCR with support of [**Tesseract**](https://github.com/tesseract-ocr/tesseract), [**DocTr**](https://github.com/mindee/doctr)
    (Tensorflow and PyTorch implementations available) and a wrapper to an API for a commercial solution, 
  - Text mining for native PDFs with  [**pdfplumber**](https://github.com/jsvine/pdfplumber), 
  - Language detection with [**fastText**](https://github.com/facebookresearch/fastText),
  - Deskewing and rotating images with [**jdeskew**](https://github.com/phamquiluan/jdeskew). 
  - Document and token classification with all LayoutLM models provided by the Transformer library. 
    (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!).
-   Table detection and table structure recognition with 
-   [**table-transformer**](https://github.com/microsoft/table-transformer). You can try a pipeline using 
-   [**this script**](https://github.com/deepdoctection/deepdoctection/discussions/116).  
- - [**new!**] There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE)
+ - Table detection and table structure recognition with 
+   [**table-transformer**](https://github.com/microsoft/table-transformer). 
+ - There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE)
    and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v2_on_custom_token_classification.ipynb) 
    to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3.
-   
+ - Comprehensive configuration of **analyzer** like choosing different models, output parsing, OCR selection.
+   Check this [notebook](https://github.com/deepdoctection/notebooks/blob/main/Analyzer_Configuration.ipynb) or the 
+   [docs](https://deepdoctection.readthedocs.io/en/latest/tutorials/analyzer_configuration_notebook/) for more infos.
+ - [**new**] Document layout analysis and table recognition now runs with Torchscript (CPU) as well and Detectron2 is 
+   not required anymore for basic inference. 
+
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself. 
      
 Have a look at the [**introduction notebook**](https://github.com/deepdoctection/notebooks/blob/main/Get_Started.ipynb) in the 
 [notebook repo](https://github.com/deepdoctection/notebooks) for an easy start.
 
@@ -125,15 +106,15 @@
 HTML(page.tables[0].html)
 ```
 
 ![table](./docs/tutorials/_imgs/dd_rm_table.png)
 
 
 ```
-print(page.get_text())
+print(page.text)
 ```
 
 ![table](./docs/tutorials/_imgs/dd_rm_text.png)
  
 
 ## Documentation
 
@@ -149,33 +130,58 @@
 ![requirements](./docs/tutorials/_imgs/requirements_deepdoctection.png)
 
 Everything in the overview listed below the **deep**doctection layer are necessary requirements and have to be installed 
 separately. 
 
 - Linux or macOS. (Windows is not supported but there is a [Dockerfile](./docker/pytorch-cpu-jupyter/Dockerfile) available)
 - Python >= 3.8
-- PyTorch >= 1.8 **or** Tensorflow >= 2.9 and CUDA. If you want to run the models provided by Tensorpack a GPU is
+- 1.8 <= PyTorch < 2.0 **or** Tensorflow >= 2.9 and CUDA. If you want to run the models provided by Tensorpack a GPU is
   required. You can run on PyTorch with a CPU only.
 - **deep**doctection uses Python wrappers for [Poppler](https://poppler.freedesktop.org/) to convert PDF documents into 
 images. 
 - With respect to the Deep Learning framework, you must decide between [Tensorflow](https://www.tensorflow.org/install?hl=en)
   and [PyTorch](https://pytorch.org/get-started/locally/).
 - [Tesseract](https://github.com/tesseract-ocr/tesseract) OCR engine will be used through a Python wrapper. The core 
   engine has to be installed separately.
 
+The following overview shows the availability of the models in conjunction with the DL framework.
+
+| Task                                          | PyTorch | Torchscript    |  Tensorflow  |
+|-----------------------------------------------|:-------:|----------------|:------------:|
+| Layout detection via Detectron2/Tensorpack    |    ✅    | ✅ (CPU only)   | ✅ (GPU only) |
+| Table recognition via Detectron2/Tensorpack   |    ✅    | ✅ (CPU only)   | ✅ (GPU only) |
+| Table transformer via Transformers            |    ✅    | ❌              |      ❌       |
+| DocTr                                         |    ✅    | ❌              |      ✅       |
+| LayoutLM (v1, v2, v3, XLM) via Transformers   |    ✅    | ❌              | ❌            |
+
 
 
 ## Installation
 
-We recommend using a virtual environment. You can install the package via pip or from source. Bug fixes or enhancements
-will be deployed to PyPi every 4 to 6 weeks.
+We recommend using a virtual environment. You can install the package via pip or from source. 
 
 ### Install with pip from PyPi
 
-Depending on which Deep Learning library you have available, use the following installation option:
+#### Minimal installation 
+
+If you want to get started with a minimal setting (e.g. running the **deep**doctection analyzer with 
+default configuration or trying the 'Get started notebook'), install **deep**doctection with
+
+```
+pip install deepdoctection
+```
+
+If you want to use the Tensorflow framework, please install Tensorpack separately. Detectron2 will not be installed 
+and layout models/ table recognition models will run with Torchscript on a CPU.
+
+#### Full installation
+
+The following installation will give you ALL models available within the Deep Learning framework as well as all models
+that are independent of Tensorflow/PyTorch. Please note, that the dependencies are very complex. We try hard to keep 
+the requirements up to date though.
 
 For **Tensorflow**, run
 
 ```
 pip install deepdoctection[tf]
 ```
 
@@ -230,15 +236,16 @@
 
 We thank all libraries that provide high quality code and pre-trained models. Without, it would have been impossible 
 to develop this framework.
 
 ## Problems
 
 We try hard to eliminate bugs. We also know that the code is not free of issues. We welcome all issues relevant to this
-repo and try to address them as quickly as possible.
+repo and try to address them as quickly as possible. Bug fixes or enhancements will be deployed in a new release every 4 
+to 6 weeks.
 
 ## If you like **deep**doctection ...
  
  ...you can easily support the project by making it more visible. Leaving a star or a recommendation will help. 
 
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deepdoctection-0.25/README.md` & `deepdoctection-0.26/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: deepdoctection
+Version: 0.26
+Summary: Repository for Document AI
+Home-page: https://github.com/deepdoctection/deepdoctection
+Author: Dr. Janis Meyer
+License: Apache License 2.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: tf
+Provides-Extra: pt
+Provides-Extra: docs
+Provides-Extra: dev
+Provides-Extra: test
+Provides-Extra: hf
+License-File: LICENSE
+
 
 <p align="center">
   <img src="https://github.com/deepdoctection/deepdoctection/blob/master/docs/tutorials/_imgs/dd_logo.png" alt="Deep Doctection Logo" width="60%">
   <h3 align="center">
   A Document AI Package
   </h3>
 </p>
@@ -29,21 +52,25 @@
  - OCR with support of [**Tesseract**](https://github.com/tesseract-ocr/tesseract), [**DocTr**](https://github.com/mindee/doctr)
    (Tensorflow and PyTorch implementations available) and a wrapper to an API for a commercial solution, 
  - Text mining for native PDFs with  [**pdfplumber**](https://github.com/jsvine/pdfplumber), 
  - Language detection with [**fastText**](https://github.com/facebookresearch/fastText),
  - Deskewing and rotating images with [**jdeskew**](https://github.com/phamquiluan/jdeskew). 
  - Document and token classification with all LayoutLM models provided by the Transformer library. 
    (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!).
-   Table detection and table structure recognition with 
-   [**table-transformer**](https://github.com/microsoft/table-transformer). You can try a pipeline using 
-   [**this script**](https://github.com/deepdoctection/deepdoctection/discussions/116).  
- - [**new!**] There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE)
+ - Table detection and table structure recognition with 
+   [**table-transformer**](https://github.com/microsoft/table-transformer). 
+ - There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE)
    and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v2_on_custom_token_classification.ipynb) 
    to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3.
-   
+ - Comprehensive configuration of **analyzer** like choosing different models, output parsing, OCR selection.
+   Check this [notebook](https://github.com/deepdoctection/notebooks/blob/main/Analyzer_Configuration.ipynb) or the 
+   [docs](https://deepdoctection.readthedocs.io/en/latest/tutorials/analyzer_configuration_notebook/) for more infos.
+ - [**new**] Document layout analysis and table recognition now runs with Torchscript (CPU) as well and Detectron2 is 
+   not required anymore for basic inference. 
+
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself. 
      
 Have a look at the [**introduction notebook**](https://github.com/deepdoctection/notebooks/blob/main/Get_Started.ipynb) in the 
 [notebook repo](https://github.com/deepdoctection/notebooks) for an easy start.
 
@@ -102,15 +129,15 @@
 HTML(page.tables[0].html)
 ```
 
 ![table](./docs/tutorials/_imgs/dd_rm_table.png)
 
 
 ```
-print(page.get_text())
+print(page.text)
 ```
 
 ![table](./docs/tutorials/_imgs/dd_rm_text.png)
  
 
 ## Documentation
 
@@ -126,33 +153,58 @@
 ![requirements](./docs/tutorials/_imgs/requirements_deepdoctection.png)
 
 Everything in the overview listed below the **deep**doctection layer are necessary requirements and have to be installed 
 separately. 
 
 - Linux or macOS. (Windows is not supported but there is a [Dockerfile](./docker/pytorch-cpu-jupyter/Dockerfile) available)
 - Python >= 3.8
-- PyTorch >= 1.8 **or** Tensorflow >= 2.9 and CUDA. If you want to run the models provided by Tensorpack a GPU is
+- 1.8 <= PyTorch < 2.0 **or** Tensorflow >= 2.9 and CUDA. If you want to run the models provided by Tensorpack a GPU is
   required. You can run on PyTorch with a CPU only.
 - **deep**doctection uses Python wrappers for [Poppler](https://poppler.freedesktop.org/) to convert PDF documents into 
 images. 
 - With respect to the Deep Learning framework, you must decide between [Tensorflow](https://www.tensorflow.org/install?hl=en)
   and [PyTorch](https://pytorch.org/get-started/locally/).
 - [Tesseract](https://github.com/tesseract-ocr/tesseract) OCR engine will be used through a Python wrapper. The core 
   engine has to be installed separately.
 
+The following overview shows the availability of the models in conjunction with the DL framework.
+
+| Task                                          | PyTorch | Torchscript    |  Tensorflow  |
+|-----------------------------------------------|:-------:|----------------|:------------:|
+| Layout detection via Detectron2/Tensorpack    |    ✅    | ✅ (CPU only)   | ✅ (GPU only) |
+| Table recognition via Detectron2/Tensorpack   |    ✅    | ✅ (CPU only)   | ✅ (GPU only) |
+| Table transformer via Transformers            |    ✅    | ❌              |      ❌       |
+| DocTr                                         |    ✅    | ❌              |      ✅       |
+| LayoutLM (v1, v2, v3, XLM) via Transformers   |    ✅    | ❌              | ❌            |
+
 
 
 ## Installation
 
-We recommend using a virtual environment. You can install the package via pip or from source. Bug fixes or enhancements
-will be deployed to PyPi every 4 to 6 weeks.
+We recommend using a virtual environment. You can install the package via pip or from source. 
 
 ### Install with pip from PyPi
 
-Depending on which Deep Learning library you have available, use the following installation option:
+#### Minimal installation 
+
+If you want to get started with a minimal setting (e.g. running the **deep**doctection analyzer with 
+default configuration or trying the 'Get started notebook'), install **deep**doctection with
+
+```
+pip install deepdoctection
+```
+
+If you want to use the Tensorflow framework, please install Tensorpack separately. Detectron2 will not be installed 
+and layout models/ table recognition models will run with Torchscript on a CPU.
+
+#### Full installation
+
+The following installation will give you ALL models available within the Deep Learning framework as well as all models
+that are independent of Tensorflow/PyTorch. Please note, that the dependencies are very complex. We try hard to keep 
+the requirements up to date though.
 
 For **Tensorflow**, run
 
 ```
 pip install deepdoctection[tf]
 ```
 
@@ -207,15 +259,16 @@
 
 We thank all libraries that provide high quality code and pre-trained models. Without, it would have been impossible 
 to develop this framework.
 
 ## Problems
 
 We try hard to eliminate bugs. We also know that the code is not free of issues. We welcome all issues relevant to this
-repo and try to address them as quickly as possible.
+repo and try to address them as quickly as possible. Bug fixes or enhancements will be deployed in a new release every 4 
+to 6 weeks.
 
 ## If you like **deep**doctection ...
  
  ...you can easily support the project by making it more visible. Leaving a star or a recommendation will help. 
 
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deepdoctection-0.25/deepdoctection/__init__.py` & `deepdoctection-0.26/deepdoctection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typing import TYPE_CHECKING
 
 from packaging import version
 
 from .utils.file_utils import _LazyModule, get_tf_version, pytorch_available, tf_available
 from .utils.logger import logger
 
-__version__ = 0.25
+__version__ = 0.26
 
 _IMPORT_STRUCTURE = {
     "analyzer": ["get_dd_analyzer", "build_analyzer"],
     "configs": [],
     "dataflow": [
         "DataFlowTerminated",
         "DataFlowResetStateNotCalled",
@@ -147,14 +147,15 @@
         "SequenceClassResult",
         "LMTokenClassifier",
         "LMSequenceClassifier",
         "LanguageDetector",
         "ImageTransformer",
         "InferenceResize",
         "D2FrcnnDetector",
+        "D2FrcnnTracingDetector",
         "Jdeskewer",
         "DoctrTextlineDetector",
         "DoctrTextRecognizer",
         "FasttextLangDetector",
         "HFDetrDerivedDetector",
         "HFLayoutLmTokenClassifierBase",
         "HFLayoutLmTokenClassifier",
@@ -168,15 +169,15 @@
         "print_model_infos",
         "ModelDownloadManager",
         "PdfPlumberTextDetector",
         "TesseractOcrDetector",
         "TextractOcrDetector",
         "TPFrcnnDetector",
     ],
-    "extern.pt": ["set_torch_auto_device", "get_num_gpu"],
+    "extern.pt": ["set_torch_auto_device", "get_num_gpu", "batched_nms"],
     "extern.tp": ["disable_tfv2", "ModelDescWithConfig", "TensorpackPredictor"],
     "extern.tp.tpfrcnn": ["CustomResize", "anchors_and_labels", "augment"],
     "extern.tp.tpfrcnn.utils": ["area", "pairwise_intersection", "pairwise_iou"],
     "extern.tp.tpfrcnn.config": ["model_frcnn_config", "train_frcnn_config"],
     "extern.tp.tpfrcnn.modeling": ["ResNetFPNModel"],
     "mapper": [
         "cat_to_sub_cat",
```

### Comparing `deepdoctection-0.25/deepdoctection/analyzer/__init__.py` & `deepdoctection-0.26/deepdoctection/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/analyzer/dd.py` & `deepdoctection-0.26/deepdoctection/analyzer/dd.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 -factory build_analyzer for a given config
 
 -user factory with a reduced config setting
 """
 
 import os
+from os import environ
 from shutil import copyfile
 from typing import List, Optional, Tuple, Union
 
 from ..extern.base import ObjectDetector
 from ..extern.doctrocr import DoctrTextlineDetector, DoctrTextRecognizer
 from ..extern.model import ModelCatalog, ModelDownloadManager
 from ..extern.pdftext import PdfPlumberTextDetector
@@ -38,15 +39,21 @@
 from ..pipe.common import MatchingService, PageParsingService
 from ..pipe.doctectionpipe import DoctectionPipe
 from ..pipe.layout import ImageLayoutService
 from ..pipe.order import TextOrderService
 from ..pipe.refine import TableSegmentationRefinementService
 from ..pipe.segment import PubtablesSegmentationService, TableSegmentationService
 from ..pipe.text import TextExtractionService
-from ..utils.file_utils import pytorch_available, tensorpack_available, tf_available
+from ..utils.file_utils import (
+    boto3_available,
+    detectron2_available,
+    pytorch_available,
+    tensorpack_available,
+    tf_available,
+)
 from ..utils.fs import mkdir_p
 from ..utils.logger import logger
 from ..utils.metacfg import AttrDict, set_config_by_yaml
 from ..utils.settings import LayoutType
 from ..utils.systools import get_configs_dir_path, get_package_path
 from ..utils.transform import PadTransform
 
@@ -55,17 +62,20 @@
 
     from ..extern.tp.tfutils import disable_tp_layer_logging
     from ..extern.tpdetect import TPFrcnnDetector
 
 if pytorch_available():
     from torch import cuda
 
-    from ..extern.d2detect import D2FrcnnDetector
+    from ..extern.d2detect import D2FrcnnDetector, D2FrcnnTracingDetector
     from ..extern.hfdetr import HFDetrDerivedDetector
 
+if boto3_available():
+    from botocore.config import Config  # type: ignore
+
 
 __all__ = ["get_dd_analyzer", "build_analyzer"]
 
 _DD_ONE = "deepdoctection/configs/conf_dd_one.yaml"
 _TESSERACT = "deepdoctection/configs/conf_tesseract.yaml"
 
 
@@ -103,45 +113,59 @@
         copyfile(absolute_path_source, absolute_path)
     return absolute_path
 
 
 def _config_sanity_checks(cfg: AttrDict) -> None:
     if cfg.USE_PDF_MINER and cfg.USE_OCR and cfg.OCR.USE_DOCTR:
         raise ValueError("Configuration USE_PDF_MINER= True and USE_OCR=True and USE_DOCTR=True is not allowed")
+    if cfg.OCR.USE_TESSERACT and (cfg.OCR.USE_DOCTR or cfg.OCR.USE_TEXTRACT):
+        raise ValueError(
+            "Configuration OCR.USE_TESSERACT=True and OCR.USE_DOCTR=True or OCR.USE_TEXTRACT=True is not "
+            "allowed. Only one OCR system can be activated."
+        )
 
 
-def _build_detector(cfg: AttrDict, mode: str) -> Union["D2FrcnnDetector", "TPFrcnnDetector", "HFDetrDerivedDetector"]:
-    weights = getattr(cfg.TF, mode).WEIGHTS if cfg.LIB == "TF" else getattr(cfg.PT, mode).WEIGHTS
+def _build_detector(
+    cfg: AttrDict, mode: str
+) -> Union["D2FrcnnDetector", "TPFrcnnDetector", "HFDetrDerivedDetector", "D2FrcnnTracingDetector"]:
+    weights = (
+        getattr(cfg.TF, mode).WEIGHTS
+        if cfg.LIB == "TF"
+        else (getattr(cfg.PT, mode).WEIGHTS if detectron2_available() else getattr(cfg.PT, mode).WEIGHTS_TS)
+    )
     filter_categories = (
         getattr(getattr(cfg.TF, mode), "FILTER") if cfg.LIB == "TF" else getattr(getattr(cfg.PT, mode), "FILTER")
     )
     config_path = ModelCatalog.get_full_path_configs(weights)
     weights_path = ModelDownloadManager.maybe_download_weights_and_configs(weights)
     profile = ModelCatalog.get_profile(weights)
     categories = profile.categories
     assert categories is not None
     if profile.model_wrapper in ("TPFrcnnDetector",):
         return TPFrcnnDetector(config_path, weights_path, categories, filter_categories=filter_categories)
     if profile.model_wrapper in ("D2FrcnnDetector",):
         return D2FrcnnDetector(
             config_path, weights_path, categories, device=cfg.DEVICE, filter_categories=filter_categories
         )
+    if profile.model_wrapper in ("D2FrcnnTracingDetector",):
+        return D2FrcnnTracingDetector(config_path, weights_path, categories, filter_categories=filter_categories)
     if profile.model_wrapper in ("HFDetrDerivedDetector",):
         preprocessor_config = ModelCatalog.get_full_path_preprocessor_configs(weights)
         return HFDetrDerivedDetector(
             config_path,
             weights_path,
             preprocessor_config,
             categories,
             device=cfg.DEVICE,
             filter_categories=filter_categories,
         )
     raise TypeError(
         f"You have chosen profile.model_wrapper: {profile.model_wrapper} which is not allowed. Please check "
-        f"compatability with your deep learning framework")
+        f"compatability with your deep learning framework"
+    )
 
 
 def _build_padder(cfg: AttrDict, mode: str) -> PadTransform:
     top, right, bottom, left = (
         getattr(cfg.PT, mode).PAD.TOP,
         getattr(cfg.PT, mode).PAD.RIGHT,
         getattr(cfg.PT, mode).PAD.BOTTOM,
@@ -169,25 +193,31 @@
         detector, [LayoutType.table, LayoutType.table_rotated], None, detect_result_generator, padder
     )
 
 
 def _build_ocr(cfg: AttrDict) -> Union[TesseractOcrDetector, DoctrTextRecognizer, TextractOcrDetector]:
     if cfg.OCR.USE_TESSERACT:
         ocr_config_path = get_configs_dir_path() / cfg.OCR.CONFIG.TESSERACT
-        return TesseractOcrDetector(ocr_config_path,config_overwrite=[f"LANGUAGES={cfg.LANGUAGE}"] if
-        cfg.LANGUAGE is not None else None)
+        return TesseractOcrDetector(
+            ocr_config_path, config_overwrite=[f"LANGUAGES={cfg.LANGUAGE}"] if cfg.LANGUAGE is not None else None
+        )
     if cfg.OCR.USE_DOCTR:
         weights = cfg.OCR.WEIGHTS.DOCTR_RECOGNITION.TF if cfg.LIB == "TF" else cfg.OCR.WEIGHTS.DOCTR_RECOGNITION.PT
         weights_path = ModelDownloadManager.maybe_download_weights_and_configs(weights)
         profile = ModelCatalog.get_profile(weights)
         if profile.architecture is None:
             raise ValueError("model profile.architecture must be specified")
         return DoctrTextRecognizer(profile.architecture, weights_path, cfg.DEVICE)
     if cfg.OCR.USE_TEXTRACT:
-        return TextractOcrDetector()
+        credentials_kwargs = {
+            "aws_access_key_id": environ.get("ACCESS_KEY"),
+            "aws_secret_access_key": environ.get("SECRET_KEY"),
+            "config": Config(region_name=environ.get("REGION")),
+        }
+        return TextractOcrDetector(**credentials_kwargs)
     raise ValueError("You have set USE_OCR=True but any of USE_TESSERACT, USE_DOCTR, USE_TEXTRACT is set to False")
 
 
 def _build_doctr_word(cfg: AttrDict) -> DoctrTextlineDetector:
     weights = cfg.OCR.WEIGHTS.DOCTR_WORD.TF if cfg.LIB == "TF" else cfg.OCR.WEIGHTS.DOCTR_WORD.PT
     weights_path = ModelDownloadManager.maybe_download_weights_and_configs(weights)
     profile = ModelCatalog.get_profile(weights)
@@ -273,14 +303,15 @@
         pipe_component_list.append(text)
 
         match = MatchingService(
             parent_categories=cfg.WORD_MATCHING.PARENTAL_CATEGORIES,
             child_categories=LayoutType.word,
             matching_rule=cfg.WORD_MATCHING.RULE,
             threshold=cfg.WORD_MATCHING.THRESHOLD,
+            max_parent_only=cfg.WORD_MATCHING.MAX_PARENT_ONLY,
         )
         pipe_component_list.append(match)
 
         order = TextOrderService(
             text_container=LayoutType.word,
             text_block_categories=cfg.TEXT_ORDERING.TEXT_BLOCK_CATEGORIES,
             floating_text_block_categories=cfg.TEXT_ORDERING.FLOATING_TEXT_BLOCK_CATEGORIES,
@@ -298,15 +329,15 @@
         include_residual_text_container=cfg.TEXT_ORDERING.INCLUDE_RESIDUAL_TEXT_CONTAINER,
     )
     pipe = DoctectionPipe(pipeline_component_list=pipe_component_list, page_parsing_service=page_parsing_service)
 
     return pipe
 
 
-def get_dd_analyzer(reset_config_file: bool = True, config_overwrite: Optional[List[str]] = None) -> DoctectionPipe:
+def get_dd_analyzer(reset_config_file: bool = False, config_overwrite: Optional[List[str]] = None) -> DoctectionPipe:
     """
     Factory function for creating the built-in **deep**doctection analyzer.
 
     The Standard Analyzer is a pipeline that comprises the following analysis components:
 
     - Document layout analysis
```

### Comparing `deepdoctection-0.25/deepdoctection/configs/__init__.py` & `deepdoctection-0.26/deepdoctection/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/configs/conf_dd_one.yaml` & `deepdoctection-0.26/deepdoctection/configs/conf_dd_one.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -9,30 +9,33 @@
       FILTER:
    ITEM:
       WEIGHTS: item/model-1620000_inf_only.data-00000-of-00001
       FILTER:
 PT:
    LAYOUT:
       WEIGHTS: layout/d2_model_0829999_layout_inf_only.pt
+      WEIGHTS_TS: layout/d2_model_0829999_layout_inf_only.ts
       FILTER:
       PAD:
         TOP: 60
         RIGHT: 60
         BOTTOM: 60
-        LEFT": 60
+        LEFT: 60
    ITEM:
      WEIGHTS: item/d2_model_1639999_item_inf_only.pt
+     WEIGHTS_TS: item/d2_model_1639999_item_inf_only.ts
      FILTER:
      PAD:
         TOP: 60
         RIGHT: 60
         BOTTOM: 60
-        LEFT": 60
+        LEFT: 60
    CELL:
       WEIGHTS: cell/d2_model_1849999_cell_inf_only.pt
+      WEIGHTS_TS: cell/d2_model_1849999_cell_inf_only.ts
       FILTER:
 SEGMENTATION:
   ASSIGNMENT_RULE: ioa
   THRESHOLD_ROWS: 0.4
   THRESHOLD_COLS: 0.4
   FULL_TABLE_TILING: True
   REMOVE_IOU_THRESHOLD_ROWS: 0.001
@@ -63,14 +66,15 @@
     - cell
     - column_header
     - projected_row_header
     - spanning
     - row_header
   RULE: ioa
   THRESHOLD: 0.6
+  MAX_PARENT_ONLY: False
 TEXT_ORDERING:
   TEXT_BLOCK_CATEGORIES:
     - title
     - text
     - list
     - cell
     - column_header
```

### Comparing `deepdoctection-0.25/deepdoctection/dataflow/__init__.py` & `deepdoctection-0.26/deepdoctection/dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/dataflow/base.py` & `deepdoctection-0.26/deepdoctection/dataflow/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/dataflow/common.py` & `deepdoctection-0.26/deepdoctection/dataflow/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,22 +45,22 @@
 
     def start(self) -> None:
         """
         Start testing with a progress bar.
         """
         if not self._reset_called:
             self.df.reset_state()
-        itr = self.df.__iter__()
+        itr = iter(self.df)
         if self.warmup:
             for _ in tqdm.trange(self.warmup, **get_tqdm_default_kwargs()):  # type: ignore
                 next(itr)
         # add smoothing for speed benchmark
         with get_tqdm(total=self.test_size, leave=True, smoothing=0.2) as pbar:
             for idx, _ in enumerate(itr):
-                pbar.update()  # type: ignore
+                pbar.update()
                 if idx == self.test_size - 1:
                     break
 
 
 class FlattenData(ProxyDataFlow):
     """
     Flatten an iterator within a datapoint. Will flatten the datapoint if it is a list or a tuple.
```

### Comparing `deepdoctection-0.25/deepdoctection/dataflow/custom.py` & `deepdoctection-0.26/deepdoctection/dataflow/custom.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         get the cache of the whole dataflow as a list
 
         :return: list of datapoints
         """
         self.reset_state()
         with get_tqdm() as status_bar:
             for _ in self:
-                status_bar.update()  # type: ignore
+                status_bar.update()
             if self.shuffle:
                 self.rng.shuffle(self.buffer)
             return self.buffer
 
 
 class CustomDataFromList(DataFromList):
     """
```

### Comparing `deepdoctection-0.25/deepdoctection/dataflow/custom_serialize.py` & `deepdoctection-0.26/deepdoctection/dataflow/custom_serialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,14 @@
     A simplified version of the Microsoft COCO helper class for reading  annotations. It currently supports only
     bounding box annotations
 
     :param annotation_file: location of annotation file
     """
 
     def __init__(self, annotation_file: Optional[Pathlike] = None) -> None:
-
         self.dataset: JsonDict = {}
         self.anns: Dict[int, JsonDict] = {}
         self.cats: Dict[int, JsonDict] = {}
         self.imgs: Dict[int, JsonDict] = {}
 
         self.img_to_anns: DefaultDict[int, List[int]] = defaultdict(list)
         self.cat_to_imgs: DefaultDict[int, List[int]] = defaultdict(list)
@@ -480,15 +479,15 @@
             coco = CocoParser(path)
             img_ids = coco.get_image_ids()
             imgs = coco.load_imgs(img_ids)
 
             with get_tqdm(total=len(imgs)) as status_bar:
                 for img in imgs:
                     img["annotations"] = coco.img_to_anns[img["id"]]
-                    status_bar.update()  # type: ignore
+                    status_bar.update()
 
         df = CustomDataFromList(imgs, max_datapoints=max_datapoints)
         return df
 
     @staticmethod
     def save() -> None:
         """
```

### Comparing `deepdoctection-0.25/deepdoctection/dataflow/parallel_map.py` & `deepdoctection-0.26/deepdoctection/dataflow/parallel_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 @no_type_check
 def del_weakref(x):
     """delete weakref"""
     instance = x()
     if instance is not None:
-        instance.__del__()
+        del instance
 
 
 @no_type_check
 @contextmanager
 def _zmq_catch_error(name):
     try:
         yield
@@ -86,15 +86,15 @@
 
     def reset_state(self) -> None:
         super().reset_state()
         if not self._strict:
             df = RepeatedData(self.df, -1)
         else:
             df = self.df  # type: ignore
-        self._iter = df.__iter__()
+        self._iter = iter(df)
 
     @no_type_check
     @abstractmethod
     def _recv(self):
         raise NotImplementedError
 
     @no_type_check
@@ -133,15 +133,15 @@
 
     def get_data_strict(self) -> Any:
         """data strict"""
         self._fill_buffer()
         for dp in self._iter:
             self._send(dp)
             yield self._recv_filter_none()
-        self._iter = self.df.__iter__()  # refresh
+        self._iter = iter(self.df)  # refresh
 
         # first clear the buffer, then fill
         for k in range(self._buffer_size):
             dp = self._recv_filter_none()
             self._buffer_occupancy -= 1
             if k == self._buffer_size - 1:
                 self._fill_buffer()
```

### Comparing `deepdoctection-0.25/deepdoctection/dataflow/serialize.py` & `deepdoctection-0.26/deepdoctection/dataflow/serialize.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/dataflow/stats.py` & `deepdoctection-0.26/deepdoctection/dataflow/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,30 +89,29 @@
     def start(self) -> npt.NDArray[Any]:
         """
         Start calculating the mean with a progress bar.
         """
 
         if not self._reset_called:
             self.df.reset_state()
-        itr = self.df.__iter__()
+        itr = iter(self.df)
 
         logger.info("Calculating mean")
 
         len_df: Optional[int]
         try:
             len_df = len(self.df)
         except NotImplementedError:
             len_df = None
         if len_df is not None and self.max_datapoints is not None:
             len_df = min(len_df, self.max_datapoints)
 
         with get_tqdm(total=len_df) as status_bar:
             n = None
             for n, dp in enumerate(itr, 1):
-
                 if isinstance(dp, dict):
                     assert isinstance(self.key, str), self.key
                     val = dp[self.key]
                 elif isinstance(dp, list):
                     val = dp
                 else:
                     assert isinstance(self.key, str), self.key
@@ -131,15 +130,15 @@
                         mean_shape = tuple(val.shape[i] for i in range(len(val.shape)) if i not in inner_axis)
                         self.mean = np.zeros(mean_shape)
 
                 if val.ndim == val_0_ndim:
                     x = np.mean(val, axis=self.axis if inner_axis is None else inner_axis)
                     self.mean += (x - self.mean) / n
 
-                status_bar.update()  # type: ignore
+                status_bar.update()
                 if self.max_datapoints is not None:
                     if n == self.max_datapoints:
                         break
 
         logger.info("Mean from %s datapoints along axis %s: %s", n, self.axis, self.mean)
 
         return self.mean
@@ -211,27 +210,26 @@
         """
         Start calculating the mean with a progress bar.
         """
         len_df: Optional[int]
 
         if not self._reset_called:
             self.df.reset_state()
-        itr = self.df.__iter__()
+        itr = iter(self.df)
 
         logger.info("Calculating standard deviation")
         try:
             len_df = len(self.df)
         except NotImplementedError:
             len_df = None
         if len_df is not None and self.max_datapoints is not None:
             len_df = min(len_df, self.max_datapoints)
         n = None
         with get_tqdm(total=len_df) as status_bar:
             for n, dp in enumerate(itr, 1):
-
                 if isinstance(dp, dict):
                     assert isinstance(self.key, str), self.key
                     val = dp[self.key]
                 elif isinstance(dp, list):
                     val = dp
                 else:
                     assert isinstance(self.key, str), self.key
@@ -256,15 +254,15 @@
                     x = np.mean(val, axis=self.axis if inner_axis is None else inner_axis)
                     if n == 1:
                         k = x
 
                     ex += x - k
                     ex2 += (x - k) * (x - k)
 
-                status_bar.update()  # type: ignore
+                status_bar.update()
                 if self.max_datapoints is not None:
                     if n == self.max_datapoints:
                         break
 
             var = (ex2 - (ex * ex) / n) / (n - 1)
             self.std = np.sqrt(var)
```

### Comparing `deepdoctection-0.25/deepdoctection/datapoint/__init__.py` & `deepdoctection-0.26/deepdoctection/datapoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datapoint/annotation.py` & `deepdoctection-0.26/deepdoctection/datapoint/annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     if isinstance(kwargs.get("relationships"), dict):
         for key, values in kwargs["relationships"].items():
             for value in values:
                 ann.dump_relationship(key, value)
     return ann
 
 
-@dataclass  # type: ignore
+@dataclass
 class Annotation(ABC):
     """
     Abstract base class for all types of annotations. This abstract base class only implements general methods for
     correctly assigning annotation_ids. It also has an active flag which is set to True. Only active annotations will be
     returned when querying annotations from image containers.
 
     Annotation id should never be assigned by yourself. One possibility of assigning an id depending on an external
```

### Comparing `deepdoctection-0.25/deepdoctection/datapoint/box.py` & `deepdoctection-0.26/deepdoctection/datapoint/box.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datapoint/convert.py` & `deepdoctection-0.26/deepdoctection/datapoint/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 Conversion functions associated to functionalities of datapoint classes
 """
 import base64
 import copy
 from dataclasses import fields, is_dataclass
 from io import BytesIO
 from shutil import which
-from typing import Any, Optional, Union
+from typing import Any, Optional, Union, no_type_check
 
 import cv2
 import numpy as np
 from numpy import uint8
 from numpy.typing import NDArray
-from PyPDF2 import PdfFileReader
+from PyPDF2 import PdfReader
 
 from ..utils.detection_types import ImageType
 from ..utils.develop import deprecated
 from ..utils.pdf_utils import pdf_to_np_array
 
 __all__ = [
     "convert_b64_to_np_array",
@@ -62,15 +62,15 @@
             value = as_dict(getattr(obj, attribute.name), dict_factory)
             if hasattr(obj, "remove_keys"):
                 if attribute.name in obj.remove_keys():
                     continue
             result.append((attribute.name, value))
         return dict_factory(result)
     if isinstance(obj, (list, tuple)):
-        return type(obj)(as_dict(v, dict_factory) for v in obj)  # pylint:disable=E0110
+        return type(obj)(as_dict(v, dict_factory) for v in obj)
     if isinstance(obj, dict):
         return type(obj)((as_dict(k, dict_factory), as_dict(v, dict_factory)) for k, v in obj.items())
     if isinstance(obj, (np.float32, np.float64)):
         obj = obj.astype(float)
     return copy.deepcopy(obj)
 
 
@@ -90,18 +90,19 @@
     """
     Converts an image from numpy array into a base64 string encoding representation
 
     :param np_image: An image as numpy array.
     :return: An image as base64 string.
     """
     np_encode = cv2.imencode(".png", np_image)
-    image = base64.b64encode(np_encode[1]).decode("utf-8")
+    image = base64.b64encode(np_encode[1]).decode("utf-8")  # type: ignore
     return image
 
 
+@no_type_check
 def convert_np_array_to_b64_b(np_image: ImageType) -> bytes:
     """
     Converts an image from numpy array into a base64 bytes encoding representation
 
     :param np_image: An image as numpy array.
     :return: An image as base64 bytes.
     """
@@ -124,22 +125,21 @@
     :return: Image as numpy array.
     """
     from pdf2image import convert_from_bytes  # type: ignore # pylint: disable=C0415, E0401
 
     assert which("pdftoppm") is not None, "convert_pdf_bytes_to_np_array requires poppler to be installed"
 
     with BytesIO(pdf_bytes) as pdf_file:
-        pdf = PdfFileReader(pdf_file).getPage(0)
-    shape = pdf.mediaBox
+        pdf = PdfReader(pdf_file).pages[0]
+    shape = pdf.mediabox  # pylint: disable=E1101
     height = shape[3] - shape[1]
     width = shape[2] - shape[0]
     buffered = BytesIO()
 
     if dpi is None:
-
         image = convert_from_bytes(pdf_bytes, size=(width, height))[0]
     else:
         image = convert_from_bytes(pdf_bytes, dpi=dpi)[0]
 
     image.save(buffered, format="JPEG")
     image = base64.b64encode(buffered.getvalue()).decode("utf-8")
     np_array = convert_b64_to_np_array(image)
@@ -155,16 +155,16 @@
     :param pdf_bytes: A pdf as bytes object. A byte representation can from a pdf file can be generated e.g. with
                       `utils.fs.load_bytes_from_pdf_file`
     :param dpi: The dpi value of the resulting output image. For high resolution set dpi=300.
     :return: Image as numpy array.
     """
 
     with BytesIO(pdf_bytes) as pdf_file:
-        pdf = PdfFileReader(pdf_file).getPage(0)
-    shape = pdf.mediaBox
+        pdf = PdfReader(pdf_file).pages[0]
+    shape = pdf.mediabox  # pylint: disable=E1101
     height = shape[3] - shape[1]
     width = shape[2] - shape[0]
 
     if dpi is None:
         return pdf_to_np_array(pdf_bytes, size=(int(width), int(height)))
     return pdf_to_np_array(pdf_bytes, dpi=dpi)
```

### Comparing `deepdoctection-0.25/deepdoctection/datapoint/image.py` & `deepdoctection-0.26/deepdoctection/datapoint/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -483,15 +483,15 @@
             (box[0] < points[:, 0]) & (box[1] < points[:, 1]) & (box[2] > points[:, 0]) & (box[3] > points[:, 1])
         )[0]
         selected_ids = ann_ids[indices]
         sub_images = self.get_annotation(annotation_ids=selected_ids.tolist())
         for sub_image in sub_images:
             if sub_image.image is None:
                 raise ValueError(
-                    "When setting an embedding to ImageAnnotation then ImageAnnotation.image must not " "be None"
+                    "When setting an embedding to ImageAnnotation then ImageAnnotation.image must not be None"
                 )
             sub_image.image.set_embedding(
                 annotation_id,
                 global_to_local_coords(
                     sub_image.image.get_embedding(self.image_id), ann.image.get_embedding(self.image_id)
                 ),
             )
```

### Comparing `deepdoctection-0.25/deepdoctection/datapoint/view.py` & `deepdoctection-0.26/deepdoctection/datapoint/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,32 @@
 
 """
 Subclasses for ImageAnnotation and Image objects with various properties. These classes
 simplify consumption
 """
 
 from copy import copy
-from typing import Any, Dict, List, Optional, Sequence, Set, Tuple, Type, Union, no_type_check
+from typing import Any, Dict, List, Mapping, Optional, Sequence, Set, Tuple, Type, Union, no_type_check
 
 import cv2
 import numpy as np
 
 from ..utils.detection_types import ImageType, JsonDict, Pathlike
 from ..utils.logger import logger
-from ..utils.settings import CellType, LayoutType, ObjectTypes, PageType, Relationships, TableType, WordType, get_type
+from ..utils.settings import (
+    CellType,
+    LayoutType,
+    ObjectTypes,
+    PageType,
+    Relationships,
+    TableType,
+    TokenClasses,
+    WordType,
+    get_type,
+)
 from ..utils.viz import draw_boxes, interactive_imshow
 from .annotation import ContainerAnnotation, ImageAnnotation, SummaryAnnotation, ann_from_dict
 from .box import BoundingBox
 from .image import Image
 
 
 class ImageAnnotationBaseView(ImageAnnotation):
@@ -101,15 +111,15 @@
                     if item != sub_cat.category_name:
                         return sub_cat.category_name
                     if isinstance(sub_cat, ContainerAnnotation):
                         return sub_cat.value
                     return int(sub_cat.category_id)
         return None
 
-    def get_attribute_names(self) -> Set[str]:  # pylint: disable=R0201
+    def get_attribute_names(self) -> Set[str]:
         """
         :return: A set of registered attributes. When sub classing modify this method accordingly.
         """
         return {"bbox"}
 
     @classmethod
     def from_dict(cls, **kwargs: JsonDict) -> "ImageAnnotationBaseView":
@@ -306,14 +316,40 @@
             annotation_id_list.extend(cell.text_["annotation_ids"])  # type: ignore
         return {
             "text": " ".join([cell.text for cell in cells]),  # type: ignore
             "text_list": text_list,
             "annotation_ids": annotation_id_list,
         }
 
+    @property
+    def words(self) -> List[ImageAnnotationBaseView]:
+        """
+        Get a list of `ImageAnnotationBaseView` objects with `LayoutType` defined by `text_container`.
+        It will only select those among all annotations that have an entry in `Relationships.child` .
+        """
+        all_words: List[ImageAnnotationBaseView] = []
+        cells = self.cells
+        if not cells:
+            return super().words
+        for cell in cells:
+            all_words.extend(cell.words)  # type: ignore
+        return all_words
+
+    def get_ordered_words(self) -> List[ImageAnnotationBaseView]:
+        """Returns a list of words order by reading order. Words with no reading order will not be returned"""
+        try:
+            cells = self.cells
+            all_words = []
+            cells.sort(key=lambda x: (x.row_number, x.column_number))
+            for cell in cells:
+                all_words.extend(cell.get_ordered_words())  # type: ignore
+            return all_words
+        except TypeError:
+            return super().get_ordered_words()
+
 
 IMAGE_ANNOTATION_TO_LAYOUTS: Dict[ObjectTypes, Type[Union[Layout, Table, Word]]] = {
     **{i: Layout for i in LayoutType if (i not in {LayoutType.table, LayoutType.word, LayoutType.cell})},
     LayoutType.table: Table,
     LayoutType.table_rotated: Table,
     LayoutType.word: Word,
     LayoutType.cell: Cell,
@@ -592,14 +628,15 @@
         self,
         show_tables: bool = True,
         show_layouts: bool = True,
         show_cells: bool = True,
         show_table_structure: bool = True,
         show_words: bool = False,
         show_token_class: bool = True,
+        ignore_default_token_class: bool = False,
         interactive: bool = False,
     ) -> Optional[ImageType]:
         """
         Display a page detected bounding boxes. One can select bounding boxes of tables or other layout components.
 
         **Example:**
 
@@ -612,14 +649,16 @@
         :param show_layouts: Will display all other layout components.
         :param show_cells: Will display cells within tables. (Only available if `show_tables=True`)
         :param show_table_structure: Will display rows and columns
         :param show_words: Will display bounding boxes around words labeled with token class and bio tag (experimental)
         :param show_token_class: Will display token class instead of token tags (i.e. token classes with tags)
         :param interactive: If set to True will open an interactive image, otherwise it will return a numpy array that
                             can be displayed differently.
+        :param ignore_default_token_class: Will ignore displaying word bounding boxes with default or None token class
+                                           label
         :return: If interactive will return nothing else a numpy array.
         """
 
         category_names_list: List[Union[str, None]] = []
         box_stack = []
         cells_found = False
 
@@ -662,20 +701,29 @@
 
         if show_words:
             all_words = []
             for layout in self.layouts:
                 all_words.extend(layout.words)
             if not all_words:
                 all_words = self.get_annotation(category_names=LayoutType.word)
-            for word in all_words:
-                box_stack.append(word.bbox)
-                if show_token_class:
-                    category_names_list.append(word.token_class.value if word.token_class is not None else None)
-                else:
-                    category_names_list.append(word.token_tag.value if word.token_tag is not None else None)
+            if not ignore_default_token_class:
+                for word in all_words:
+                    box_stack.append(word.bbox)
+                    if show_token_class:
+                        category_names_list.append(word.token_class.value if word.token_class is not None else None)
+                    else:
+                        category_names_list.append(word.token_tag.value if word.token_tag is not None else None)
+            else:
+                for word in all_words:
+                    if word.token_class is not None and word.token_class != TokenClasses.other:
+                        box_stack.append(word.bbox)
+                        if show_token_class:
+                            category_names_list.append(word.token_class.value if word.token_class is not None else None)
+                        else:
+                            category_names_list.append(word.token_tag.value if word.token_tag is not None else None)
 
         if self.image is not None:
             if box_stack:
                 boxes = np.vstack(box_stack)
                 if show_words:
                     img = draw_boxes(
                         self.image,
@@ -750,7 +798,19 @@
         :param floating_text_block_categories: A list of top level layout objects
         :param include_residual_text_container: This will regard synthetic text line annotations as floating text
                                                 blocks and therefore incorporate all image annotations of category
                                                 `word` when building text strings.
         """
         image = Image.from_file(file_path)
         return cls.from_image(image, text_container, floating_text_block_categories, include_residual_text_container)
+
+    def get_token(self) -> List[Mapping[str, str]]:
+        """Return a list of tuples with word and non default token tags"""
+        block_with_order = self._order("layouts")
+        all_words = []
+        for block in block_with_order:
+            all_words.extend(block.get_ordered_words())  # type: ignore
+        return [
+            {"word": word.characters, "entity": word.token_tag}
+            for word in all_words
+            if word.token_tag not in (TokenClasses.other, None)
+        ]
```

### Comparing `deepdoctection-0.25/deepdoctection/datasets/__init__.py` & `deepdoctection-0.26/deepdoctection/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/adapter.py` & `deepdoctection-0.26/deepdoctection/datasets/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
                         else:
                             cat_ids = [ann.get_sub_category(WordType.token_class).category_id for ann in anns]
 
                     if _data_statistics:
                         summarizer.dump(cat_ids)
 
                     datapoints.append(dp)
-                    status_bar.update()  # type: ignore
+                    status_bar.update()
 
             if _data_statistics:
                 summarizer.print_summary_histogram()
             self.number_datapoints = len(datapoints)
 
             df = CustomDataFromList(datapoints, shuffle=True)
             if not image_to_framework_func:
```

### Comparing `deepdoctection-0.25/deepdoctection/datasets/base.py` & `deepdoctection-0.26/deepdoctection/datasets/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/dataflow_builder.py` & `deepdoctection-0.26/deepdoctection/datasets/dataflow_builder.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/info.py` & `deepdoctection-0.26/deepdoctection/datasets/info.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/instances/__init__.py` & `deepdoctection-0.26/deepdoctection/datasets/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/instances/doclaynet.py` & `deepdoctection-0.26/deepdoctection/datasets/instances/doclaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/instances/fintabnet.py` & `deepdoctection-0.26/deepdoctection/datasets/instances/fintabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/instances/funsd.py` & `deepdoctection-0.26/deepdoctection/datasets/instances/funsd.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/instances/iiitar13k.py` & `deepdoctection-0.26/deepdoctection/datasets/instances/iiitar13k.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,14 +120,17 @@
         `load_image:` Will load the image for each datapoint.  Default: `False`
 
         `fake_score:` Will add a fake score so that annotations look like predictions
 
         :return: dataflow
         """
 
+        if not lxml_available():
+            raise ModuleNotFoundError("IIITar13KBuilder.build requires lxml but it is not installed.")
+
         split = str(kwargs.get("split", "val"))
         load_image = kwargs.get("load_image", False)
         max_datapoints = kwargs.get("max_datapoints")
         fake_score = kwargs.get("fake_score", False)
 
         if max_datapoints is not None:
             max_datapoints = int(max_datapoints)
```

### Comparing `deepdoctection-0.25/deepdoctection/datasets/instances/layouttest.py` & `deepdoctection-0.26/deepdoctection/datasets/instances/layouttest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/instances/publaynet.py` & `deepdoctection-0.26/deepdoctection/datasets/instances/publaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/instances/pubtables1m.py` & `deepdoctection-0.26/deepdoctection/datasets/instances/pubtables1m.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,17 @@
         `load_image:` Will load the image for each datapoint.  Default: `False`
 
         `fake_score:` Will add a fake score so that annotations look like predictions
 
         :return: dataflow
         """
 
+        if not lxml_available():
+            raise ModuleNotFoundError("Pubtables1MBuilder.build requires lxml but it is not installed.")
+
         split = str(kwargs.get("split", "val"))
         load_image = kwargs.get("load_image", False)
         max_datapoints = kwargs.get("max_datapoints")
         fake_score = kwargs.get("fake_score", False)
 
         if max_datapoints is not None:
             max_datapoints = int(max_datapoints)
@@ -239,14 +242,16 @@
         `split:` Split of the dataset. Can be `train`, `val` or `test`. Default: `val`
         `max_datapoints:` Will stop iterating after max_datapoints. Default: `None`
         `load_image:` Will load the image for each datapoint.  Default: `False`
         `fake_score:` Will add a fake score so that annotations look like predictions
 
         :return: dataflow
         """
+        if not lxml_available():
+            raise ModuleNotFoundError("Pubtables1MBuilderStruct.build requires lxml but it is not installed.")
 
         split = str(kwargs.get("split", "val"))
         load_image = kwargs.get("load_image", False)
         max_datapoints = kwargs.get("max_datapoints")
         fake_score = kwargs.get("fake_score", False)
 
         if max_datapoints is not None:
```

### Comparing `deepdoctection-0.25/deepdoctection/datasets/instances/pubtabnet.py` & `deepdoctection-0.26/deepdoctection/datasets/instances/pubtabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/instances/rvlcdip.py` & `deepdoctection-0.26/deepdoctection/datasets/instances/rvlcdip.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/instances/xfund.py` & `deepdoctection-0.26/deepdoctection/datasets/instances/xfund.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/instances/xsl/__init__.py` & `deepdoctection-0.26/deepdoctection/datasets/instances/xsl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/instances/xsl/pascal_voc.xsl` & `deepdoctection-0.26/deepdoctection/datasets/instances/xsl/pascal_voc.xsl`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/registry.py` & `deepdoctection-0.26/deepdoctection/datasets/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/datasets/save.py` & `deepdoctection-0.26/deepdoctection/datasets/save.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/eval/__init__.py` & `deepdoctection-0.26/deepdoctection/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/eval/accmetric.py` & `deepdoctection-0.26/deepdoctection/eval/accmetric.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,14 @@
     _sub_cats: Optional[Union[Mapping[ObjectTypes, ObjectTypes], Mapping[ObjectTypes, Sequence[ObjectTypes]]]] = None
     _summary_sub_cats: Optional[Sequence[ObjectTypes]] = None
 
     @classmethod
     def dump(
         cls, dataflow_gt: DataFlow, dataflow_predictions: DataFlow, categories: DatasetCategories
     ) -> Tuple[Any, Any]:
-
         dataflow_gt.reset_state()
         dataflow_predictions.reset_state()
 
         cls._category_sanity_checks(categories)
         if cls._cats is None and cls._sub_cats is None:
             cls._cats = categories.get_categories(as_dict=False, filtered=True)
         mapper_with_setting = cls.mapper(cls._cats, cls._sub_cats, cls._summary_sub_cats)
@@ -230,17 +229,17 @@
         labels_predictions: Dict[str, List[int]] = {}
 
         # returned images of gt and predictions are likely not in the same order. We therefore first stream all data
         # into a dict and generate our result vectors thereafter.
         labels_per_image_gt = {}
         labels_per_image_predictions = {}
         for dp_gt, dp_pd in zip(dataflow_gt, dataflow_predictions):
-            dp_labels_gt, image_id_gt = mapper_with_setting(dp_gt)
+            dp_labels_gt, image_id_gt = mapper_with_setting(dp_gt)  # pylint: disable=E1102
             labels_per_image_gt[image_id_gt] = dp_labels_gt
-            dp_labels_predictions, image_id_pr = mapper_with_setting(dp_pd)
+            dp_labels_predictions, image_id_pr = mapper_with_setting(dp_pd)  # pylint: disable=E1102
             labels_per_image_predictions[image_id_pr] = dp_labels_predictions
 
         for image_id, dp_labels_gt in labels_per_image_gt.items():
             dp_labels_predictions = labels_per_image_predictions[image_id]
             for key in dp_labels_gt.keys():
                 if key not in labels_gt:
                     labels_gt[key] = dp_labels_gt[key]
@@ -251,15 +250,14 @@
 
         return labels_gt, labels_predictions
 
     @classmethod
     def get_distance(
         cls, dataflow_gt: DataFlow, dataflow_predictions: DataFlow, categories: DatasetCategories
     ) -> List[JsonDict]:
-
         labels_gt, labels_pr = cls.dump(dataflow_gt, dataflow_predictions, categories)
 
         results = []
         for key in labels_gt:  # pylint: disable=C0206
             res = cls.metric(labels_gt[key], labels_pr[key])
             results.append(
                 {
@@ -392,15 +390,14 @@
     name = "Confusion"
     metric = confusion
 
     @classmethod
     def get_distance(
         cls, dataflow_gt: DataFlow, dataflow_predictions: DataFlow, categories: DatasetCategories
     ) -> List[JsonDict]:
-
         labels_gt, labels_pr = cls.dump(dataflow_gt, dataflow_predictions, categories)
 
         results = []
         for key in labels_gt:  # pylint: disable=C0206
             confusion_matrix = cls.metric(labels_gt[key], labels_pr[key])
             number_labels: TypeCounter[int] = Counter(labels_gt[key])
             for row_number, row in enumerate(confusion_matrix, 1):
@@ -440,15 +437,14 @@
     name = "Precision"
     metric = precision
 
     @classmethod
     def get_distance(
         cls, dataflow_gt: DataFlow, dataflow_predictions: DataFlow, categories: DatasetCategories
     ) -> List[JsonDict]:
-
         labels_gt, labels_pr = cls.dump(dataflow_gt, dataflow_predictions, categories)
 
         results = []
         for key in labels_gt:  # pylint: disable=C0206
             score = cls.metric(labels_gt[key], labels_pr[key])
             number_labels: TypeCounter[int] = Counter(labels_gt[key])
             for label_id, val in enumerate(score, 1):
@@ -493,15 +489,14 @@
     name = "Micro Precision "
     metric = precision
 
     @classmethod
     def get_distance(
         cls, dataflow_gt: DataFlow, dataflow_predictions: DataFlow, categories: DatasetCategories
     ) -> List[JsonDict]:
-
         labels_gt, labels_pr = cls.dump(dataflow_gt, dataflow_predictions, categories)
 
         results = []
         for key in labels_gt:  # pylint: disable=C0206
             score = cls.metric(labels_gt[key], labels_pr[key], micro=True)
             results.append(
                 {
```

### Comparing `deepdoctection-0.25/deepdoctection/eval/base.py` & `deepdoctection-0.26/deepdoctection/eval/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,14 @@
         :return: Dict with metric results.
         """
         output: JsonDict = {}
         for res in results:
             new_key = ""
             new_val = 0.0
             for k, val in res.items():
-
                 if str(val) != "":
                     if k != "val":
                         if k != "key":
                             new_key += k + "/" + str(val) + "/"
                         else:
                             new_key += str(val) + "/"
                     else:
```

### Comparing `deepdoctection-0.25/deepdoctection/eval/cocometric.py` & `deepdoctection-0.26/deepdoctection/eval/cocometric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/eval/eval.py` & `deepdoctection-0.26/deepdoctection/eval/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
                     run,
                     self.dataset.dataset_info.name,
                     50,
                     self.dataset.dataflow.categories.get_categories(filtered=True),
                 )
             elif self.dataset.dataset_info.type == DatasetType.token_classification:
                 if hasattr(self.metric, "sub_cats"):
-                    sub_cat_key, sub_cat_val_list = list(self.metric.sub_cats.items())[0]  # type: ignore
+                    sub_cat_key, sub_cat_val_list = list(self.metric.sub_cats.items())[0]
                     sub_cat_val = sub_cat_val_list[0]
                     sub_cats = {sub_cat_key: sub_cat_val}
                     self.wandb_table_agent = WandbTableAgent(
                         run,
                         self.dataset.dataset_info.name,
                         50,
                         self.dataset.dataflow.categories.get_categories(filtered=True),
@@ -162,15 +162,15 @@
                             values_as_dict=True,
                             name_as_key=False,
                         )[sub_cat_key][sub_cat_val],
                         sub_cats,
                     )
                 else:
                     raise AttributeError(
-                        "metric has no attribute sub_cats and cannot be used for token classification " "datasets"
+                        "metric has no attribute sub_cats and cannot be used for token classification datasets"
                     )
             else:
                 raise NotImplementedError
 
         else:
             self.wandb_table_agent = None
```

### Comparing `deepdoctection-0.25/deepdoctection/eval/registry.py` & `deepdoctection-0.26/deepdoctection/eval/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/eval/tedsmetric.py` & `deepdoctection-0.26/deepdoctection/eval/tedsmetric.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -146,14 +146,15 @@
             return new_node
         return None
 
     def evaluate(self, inputs: Tuple[str, str]) -> float:
         """Computes TEDS score between the prediction and the ground truth of a
         given sample
         """
+
         ground_truth, pred = inputs[0], inputs[1]
         if (not pred) or (not ground_truth):
             return 0.0
         parser = etree.XMLParser()
         try:
             ground_truth_tr = etree.XML(ground_truth, parser)
         except etree.XMLSyntaxError:
@@ -214,15 +215,14 @@
     mapper = Page.from_image
     structure_only = False
 
     @classmethod
     def dump(
         cls, dataflow_gt: DataFlow, dataflow_predictions: DataFlow, categories: DatasetCategories
     ) -> Tuple[List[str], List[str]]:
-
         dataflow_gt.reset_state()
         dataflow_predictions.reset_state()
 
         # gt and predictions are not necessarily in same order. Will need to reorder
         gt_dict = defaultdict(list)
         pred_dict = defaultdict(list)
         for dp_gt, dp_pred in zip(dataflow_gt, dataflow_predictions):
```

### Comparing `deepdoctection-0.25/deepdoctection/eval/tp_eval_callback.py` & `deepdoctection-0.26/deepdoctection/eval/tp_eval_callback.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/__init__.py` & `deepdoctection-0.26/deepdoctection/extern/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Wrappers for models of external libraries as well as implementation of the Cascade-RCNN model of Tensorpack.
 """
 
-from ..utils.file_utils import tensorpack_available
+from ..utils.file_utils import detectron2_available, tensorpack_available
 from .base import *
-from .d2detect import *
 from .deskew import *
 from .doctrocr import *
 from .fastlang import *
 from .hfdetr import *
 from .hflayoutlm import *
 from .model import *
 from .pdftext import *
 from .tessocr import *
 from .texocr import *  # type: ignore
 
 if tensorpack_available():
     from .tpdetect import *
+
+if detectron2_available():
+    from .d2detect import *
```

### Comparing `deepdoctection-0.25/deepdoctection/extern/base.py` & `deepdoctection-0.26/deepdoctection/extern/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/d2detect.py` & `deepdoctection-0.26/deepdoctection/extern/doctrocr.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# File: d2detect.py
+# File: doctrocr.py
 
 # Copyright 2021 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -12,251 +12,277 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-D2 GeneralizedRCNN model as predictor for deepdoctection pipeline
+Deepdoctection wrappers for DocTr OCR text line detection and text recognition models
 """
 
-from copy import copy
 from pathlib import Path
-from typing import Dict, List, Literal, Mapping, Optional, Sequence
+from typing import Any, List, Literal, Mapping, Optional, Tuple
+from zipfile import ZipFile
 
 from ..utils.detection_types import ImageType, Requirement
 from ..utils.file_utils import (
-    detectron2_available,
-    get_detectron2_requirement,
+    doctr_available,
+    get_doctr_requirement,
     get_pytorch_requirement,
+    get_tensorflow_requirement,
+    get_tf_addons_requirements,
     pytorch_available,
+    tf_addons_available,
+    tf_available,
 )
-from ..utils.settings import ObjectTypes, TypeOrStr, get_type
-from ..utils.transform import InferenceResize
-from .base import DetectionResult, ObjectDetector, PredictorBase
+from ..utils.settings import LayoutType, ObjectTypes, TypeOrStr
+from .base import DetectionResult, ObjectDetector, PredictorBase, TextRecognizer
 from .pt.ptutils import set_torch_auto_device
 
+if doctr_available() and ((tf_addons_available() and tf_available()) or pytorch_available()):
+    from doctr.models.detection.predictor import DetectionPredictor  # pylint: disable=W0611
+    from doctr.models.detection.zoo import detection_predictor
+    from doctr.models.recognition.predictor import RecognitionPredictor  # pylint: disable=W0611
+    from doctr.models.recognition.zoo import recognition_predictor
+
 if pytorch_available():
     import torch
-    import torch.cuda
-    from torch import nn  # pylint: disable=W0611
 
-if detectron2_available():
-    from detectron2.checkpoint import DetectionCheckpointer
-    from detectron2.config import CfgNode, get_cfg  # pylint: disable=W0611
-    from detectron2.layers import batched_nms
-    from detectron2.modeling import GeneralizedRCNN, build_model  # pylint: disable=W0611
-    from detectron2.structures import Instances  # pylint: disable=W0611
+if tf_available():
+    import tensorflow as tf  # type: ignore  # pylint: disable=E0401
+
+
+def _set_device_str(device: Optional[str] = None) -> str:
+    if device is not None:
+        if tf_available():
+            device = "/" + device.replace("cuda", "gpu") + ":0"
+    elif pytorch_available():
+        device = set_torch_auto_device()
+    else:
+        device = "/gpu:0"  # we impose to install tensorflow-gpu because of Tensorpack models
+    return device
+
+
+def _load_model(path_weights: str, doctr_predictor: Any, device: str) -> None:
+    if pytorch_available():
+        state_dict = torch.load(path_weights, map_location=device)
+        for key in list(state_dict.keys()):
+            state_dict["model." + key] = state_dict.pop(key)
+        doctr_predictor.load_state_dict(state_dict)
+        doctr_predictor.to(device)
+    elif tf_available():
+        # Unzip the archive
+        params_path = Path(path_weights).parent
+        is_zip_path = path_weights.endswith(".zip")
+        if is_zip_path:
+            with ZipFile(path_weights, "r") as file:
+                file.extractall(path=params_path)
+                doctr_predictor.model.load_weights(params_path / "weights")
+        else:
+            doctr_predictor.model.load_weights(path_weights)
 
 
-def _d2_post_processing(
-    predictions: Dict[str, "Instances"], nms_thresh_class_agnostic: float
-) -> Dict[str, "Instances"]:
+def doctr_predict_text_lines(np_img: ImageType, predictor: "DetectionPredictor", device: str) -> List[DetectionResult]:
     """
-    D2 postprocessing steps, so that detection outputs are aligned with outputs of other packages (e.g. Tensorpack).
-    Apply a class agnostic NMS.
+    Generating text line DetectionResult based on Doctr DetectionPredictor.
 
-    :param predictions: Prediction outputs from the model.
-    :param nms_thresh_class_agnostic: Nms being performed over all class predictions
-    :return: filtered predictions outputs
+    :param np_img: Image in np.array.
+    :param predictor: `doctr.models.detection.predictor.DetectionPredictor`
+    :param device: Will only be used in tensorflow settings. Either /gpu:0 or /cpu:0
+    :return: A list of text line detection results (without text).
     """
-    instances = predictions["instances"]
-    class_masks = torch.ones(instances.pred_classes.shape, dtype=torch.uint8)
-    keep = batched_nms(instances.pred_boxes.tensor, instances.scores, class_masks, nms_thresh_class_agnostic)
-    fg_instances_keep = instances[keep]
-    return {"instances": fg_instances_keep}
+    if tf_available() and device is not None:
+        with tf.device(device):
+            raw_output = predictor([np_img])
+    else:
+        raw_output = predictor([np_img])
+    detection_results = [
+        DetectionResult(
+            box=box[:4].tolist(), class_id=1, score=box[4], absolute_coords=False, class_name=LayoutType.word
+        )
+        for box in raw_output[0]
+    ]
+    return detection_results
 
 
-def d2_predict_image(
-    np_img: ImageType,
-    predictor: "nn.Module",
-    preproc_short_edge_size: int,
-    preproc_max_size: int,
-    nms_thresh_class_agnostic: float,
+def doctr_predict_text(
+    inputs: List[Tuple[str, ImageType]], predictor: "RecognitionPredictor", device: str
 ) -> List[DetectionResult]:
     """
-    Run detection on one image, using the D2 model callable. It will also handle the preprocessing internally which
-    is using a custom resizing within some bounds.
+    Calls Doctr text recognition model on a batch of numpy arrays (text lines predicted from a text line detector) and
+    returns the recognized text as DetectionResult
 
-    :param np_img: ndarray
-    :param predictor: torch nn module implemented in Detectron2
-    :param preproc_short_edge_size: the short edge to resize to
-    :param preproc_max_size: upper bound of one edge when resizing
-    :param nms_thresh_class_agnostic: class agnostic nms threshold
-    :return: list of DetectionResult
+    :param inputs: list of tuples containing the annotation_id of the input image and the numpy array of the cropped
+                   text line
+    :param predictor: `doctr.models.detection.predictor.RecognitionPredictor`
+    :param device: Will only be used in tensorflow settings. Either /gpu:0 or /cpu:0
+    :return: A list of DetectionResult containing recognized text.
     """
-    height, width = np_img.shape[:2]
-    resizer = InferenceResize(preproc_short_edge_size, preproc_max_size)
-    resized_img = resizer.get_transform(np_img).apply_image(np_img)
-    image = torch.as_tensor(resized_img.astype("float32").transpose(2, 0, 1))
-
-    with torch.no_grad():
-        inputs = {"image": image, "height": height, "width": width}
-        predictions = predictor([inputs])[0]
-        predictions = _d2_post_processing(predictions, nms_thresh_class_agnostic)
-    instances = predictions["instances"]
-    results = [
-        DetectionResult(
-            box=instances[k].pred_boxes.tensor.tolist()[0],
-            score=instances[k].scores.tolist()[0],
-            class_id=instances[k].pred_classes.tolist()[0],
-        )
-        for k in range(len(instances))
+
+    uuids, images = list(zip(*inputs))
+    if tf_available() and device is not None:
+        with tf.device(device):
+            raw_output = predictor(list(images))
+    else:
+        raw_output = predictor(list(images))
+    detection_results = [
+        DetectionResult(score=output[1], text=output[0], uuid=uuid) for uuid, output in zip(uuids, raw_output)
     ]
-    return results
+    return detection_results
 
 
-class D2FrcnnDetector(ObjectDetector):
+class DoctrTextlineDetector(ObjectDetector):
     """
-    D2 Faster-RCNN implementation with all the available backbones, normalizations throughout the model
-    as well as FPN, optional Cascade-RCNN and many more.
+    A deepdoctection wrapper of DocTr text line detector. We model text line detection as ObjectDetector
+    and assume to use this detector in a ImageLayoutService.
+    DocTr supports several text line detection implementations but provides only a subset of pre-trained models.
+    The most usable one for document OCR for which a pre-trained model exists is DBNet as described in “Real-time Scene
+    Text Detection with Differentiable Binarization”, with a ResNet-50 backbone. This model can be used in either
+    Tensorflow or PyTorch.
+    Some other pre-trained models exist that have not been registered in `ModelCatalog`. Please check the DocTr library
+    and organize the download of the pre-trained model by yourself.
+
+    **Example:**
+
+                 path_weights_tl = ModelDownloadManager.maybe_download_weights_and_configs("doctr/db_resnet50/pt
+                 /db_resnet50-ac60cadc.pt")
+                 # Use "doctr/db_resnet50/tf/db_resnet50-adcafc63.zip" for Tensorflow
+
+                 categories = ModelCatalog.get_profile("doctr/db_resnet50/pt/db_resnet50-ac60cadc.pt").categories
+                 det = DoctrTextlineDetector("db_resnet50",path_weights_tl,categories,"cpu")
+                 layout = ImageLayoutService(det,to_image=True, crop_image=True)
+
+                 path_weights_tr = dd.ModelDownloadManager.maybe_download_weights_and_configs("doctr/crnn_vgg16_bn
+                 /pt/crnn_vgg16_bn-9762b0b0.pt")
+                 rec = DoctrTextRecognizer("crnn_vgg16_bn", path_weights_tr, "cpu")
+                 text = TextExtractionService(rec, extract_from_roi="word")
 
-    Currently, masks are not included in the data model.
+                 analyzer = DoctectionPipe(pipeline_component_list=[layout,text])
 
-    There are no adjustment to the original implementation of Detectron2. Only one post-processing step is followed by
-    the standard D2 output that takes into account of the situation that detected objects are disjoint. For more infos
-    on this topic, see <https://github.com/facebookresearch/detectron2/issues/978> .
+                 path = "/path/to/image_dir"
+                 df = analyzer.analyze(path = path)
 
-        config_path = ModelCatalog.get_full_path_configs("dd/d2/item/CASCADE_RCNN_R_50_FPN_GN.yaml")
-        weights_path = ModelDownloadManager.maybe_download_weights_and_configs("item/d2_model-800000-layout.pkl")
-        categories = ModelCatalog.get_profile("item/d2_model-800000-layout.pkl").categories
+                 for dp in df:
+                     ...
 
-        d2_predictor = D2FrcnnDetector(config_path,weights_path,categories,device="cpu")
 
-        detection_results = d2_predictor.predict(bgr_image_np_array)
     """
 
     def __init__(
         self,
-        path_yaml: str,
+        architecture: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
-        config_overwrite: Optional[List[str]] = None,
         device: Optional[Literal["cpu", "cuda"]] = None,
-        filter_categories: Optional[Sequence[TypeOrStr]] = None,
-    ):
-        """
-        Set up the predictor.
-
-        The configuration of the model uses the full stack of build model tools of D2. For more information
-        please check <https://detectron2.readthedocs.io/en/latest/tutorials/models.html#build-models-from-yacs-config>.
-
-        :param path_yaml: The path to the yaml config. If the model is built using several config files, always use
-                          the highest level .yaml file.
-        :param path_weights: The path to the model checkpoint.
-        :param categories: A dict with key (indices) and values (category names). Index 0 must be reserved for a
-                           dummy 'BG' category. Note, that this convention is different from the builtin D2 framework,
-                           where models in the model zoo are trained with 'BG' class having the highest index.
-        :param config_overwrite:  Overwrite some hyperparameters defined by the yaml file with some new values. E.g.
-                                 ["OUTPUT.FRCNN_NMS_THRESH=0.3","OUTPUT.RESULT_SCORE_THRESH=0.6"].
-        :param device: "cpu" or "cuda". If not specified will auto select depending on what is available
-        :param filter_categories: The model might return objects that are not supposed to be predicted and that should
-                                  be filtered. Pass a list of category names that must not be returned
-        """
-
-        self.name = "_".join(Path(path_weights).parts[-3:])
-        self._categories_d2 = self._map_to_d2_categories(copy(categories))
-        if config_overwrite is None:
-            config_overwrite = []
+    ) -> None:
+        self.name = "doctr_text_detector"
+        self.architecture = architecture
         self.path_weights = path_weights
-        d2_conf_list = ["MODEL.WEIGHTS", path_weights]
-        for conf in config_overwrite:
-            key, val = conf.split("=", maxsplit=1)
-            d2_conf_list.extend([key, val])
-
-        self.path_yaml = path_yaml
-        self.categories = copy(categories)  # type: ignore
-        self.config_overwrite = config_overwrite
-        if device is not None:
-            self.device = device
-        else:
-            self.device = set_torch_auto_device()
-        if filter_categories:
-            filter_categories = [get_type(cat) for cat in filter_categories]
-        self.filter_categories = filter_categories
-        self.cfg = self._set_config(path_yaml, d2_conf_list, device)
-        self.d2_predictor = D2FrcnnDetector.set_model(self.cfg)
-        self._instantiate_d2_predictor()
-
-    @staticmethod
-    def _set_config(
-        path_yaml: str, d2_conf_list: List[str], device: Optional[Literal["cpu", "cuda"]] = None
-    ) -> "CfgNode":
-        cfg = get_cfg()
-        # additional attribute with default value, so that the true value can be loaded from the configs
-        cfg.NMS_THRESH_CLASS_AGNOSTIC = 0.1
-        cfg.merge_from_file(path_yaml)
-        cfg.merge_from_list(d2_conf_list)
-        if not torch.cuda.is_available() or device == "cpu":
-            cfg.MODEL.DEVICE = "cpu"
-        cfg.freeze()
-        return cfg
-
-    @staticmethod
-    def set_model(config: "CfgNode") -> "GeneralizedRCNN":
-        """
-        Build the D2 model. It uses the available builtin tools of D2
-
-        :param config: Model config
-        :return: The GeneralizedRCNN model
-        """
-        return build_model(config.clone()).eval()
-
-    def _instantiate_d2_predictor(self) -> None:
-        checkpointer = DetectionCheckpointer(self.d2_predictor)
-        checkpointer.load(self.cfg.MODEL.WEIGHTS)
+        self.doctr_predictor = detection_predictor(
+            arch=self.architecture, pretrained=False, pretrained_backbone=False
+        )  # we will be loading the model
+        # later because there is no easy way in doctr to load a model by giving only a path to its weights
+        self.categories = categories  # type: ignore
+        self.device_input = device
+        self.device = _set_device_str(device)
+        self.load_model()
 
     def predict(self, np_img: ImageType) -> List[DetectionResult]:
         """
         Prediction per image.
 
         :param np_img: image as numpy array
         :return: A list of DetectionResult
         """
-        detection_results = d2_predict_image(
-            np_img,
-            self.d2_predictor,
-            self.cfg.INPUT.MIN_SIZE_TEST,
-            self.cfg.INPUT.MAX_SIZE_TEST,
-            self.cfg.NMS_THRESH_CLASS_AGNOSTIC,
-        )
-        return self._map_category_names(detection_results)
+        detection_results = doctr_predict_text_lines(np_img, self.doctr_predictor, self.device)
+        return detection_results
+
+    @classmethod
+    def get_requirements(cls) -> List[Requirement]:
+        if tf_available():
+            return [get_tensorflow_requirement(), get_doctr_requirement(), get_tf_addons_requirements()]
+        if pytorch_available():
+            return [get_pytorch_requirement(), get_doctr_requirement()]
+        raise ModuleNotFoundError("Neither Tensorflow nor PyTorch has been installed. Cannot use DoctrTextlineDetector")
 
-    def _map_category_names(self, detection_results: List[DetectionResult]) -> List[DetectionResult]:
+    def clone(self) -> PredictorBase:
+        return self.__class__(self.architecture, self.path_weights, self.categories, self.device_input)
+
+    def possible_categories(self) -> List[ObjectTypes]:
+        return [LayoutType.word]
+
+    def load_model(self) -> None:
+        """Loading model weights"""
+        _load_model(self.path_weights, self.doctr_predictor, self.device)
+
+
+class DoctrTextRecognizer(TextRecognizer):
+    """
+    A deepdoctection wrapper of DocTr text recognition predictor. The base class is a TextRecognizer that takes
+    a batch of sub images (e.g. text lines from a text detector) and returns a list with text spotted in the sub images.
+    DocTr supports several text recognition models but provides only a subset of pre-trained models.
+
+    This model that is most suitable for document text recognition is the CRNN implementation with a VGG-16 backbone as
+    described in “An End-to-End Trainable Neural Network for Image-based Sequence Recognition and Its Application to
+    Scene Text Recognition”. It can be used in either Tensorflow or PyTorch.
+
+    For more details please check the official DocTr documentation by Mindee: https://mindee.github.io/doctr/
+
+    **Example:**
+
+                 path_weights_tl = ModelDownloadManager.maybe_download_weights_and_configs("doctr/db_resnet50/pt
+                 /db_resnet50-ac60cadc.pt")
+                 # Use "doctr/db_resnet50/tf/db_resnet50-adcafc63.zip" for Tensorflow
+
+                 categories = ModelCatalog.get_profile("doctr/db_resnet50/pt/db_resnet50-ac60cadc.pt").categories
+                 det = DoctrTextlineDetector("db_resnet50",path_weights_tl,categories,"cpu")
+                 layout = ImageLayoutService(det,to_image=True, crop_image=True)
+
+                 path_weights_tr = dd.ModelDownloadManager.maybe_download_weights_and_configs("doctr/crnn_vgg16_bn
+                 /pt/crnn_vgg16_bn-9762b0b0.pt")
+                 rec = DoctrTextRecognizer("crnn_vgg16_bn", path_weights_tr, "cpu")
+                 text = TextExtractionService(rec, extract_from_roi="word")
+
+                 analyzer = DoctectionPipe(pipeline_component_list=[layout,text])
+
+                 path = "/path/to/image_dir"
+                 df = analyzer.analyze(path = path)
+
+                 for dp in df:
+                     ...
+
+    """
+
+    def __init__(self, architecture: str, path_weights: str, device: Optional[Literal["cpu", "cuda"]] = None) -> None:
+        self.name = "doctr_text_recognizer"
+        self.architecture = architecture
+        self.path_weights = path_weights
+        self.device_input = device
+        self.device = _set_device_str(device)
+        self.doctr_predictor = recognition_predictor(arch=self.architecture, pretrained=True)
+        self.load_model()
+
+    def predict(self, images: List[Tuple[str, ImageType]]) -> List[DetectionResult]:
         """
-        Populating category names to detection results
+        Prediction on a batch of text lines
 
-        :param detection_results: list of detection results. Will also filter categories
-        :return: List of detection results with attribute class_name populated
+        :param images: list of tuples with the annotation_id of the sub image and a numpy array
+        :return: A list of DetectionResult
         """
-        filtered_detection_result: List[DetectionResult] = []
-        for result in detection_results:
-            result.class_name = self._categories_d2[str(result.class_id)]
-            if isinstance(result.class_id, int):
-                result.class_id += 1
-            if self.filter_categories:
-                if result.class_name not in self.filter_categories:
-                    filtered_detection_result.append(result)
-            else:
-                filtered_detection_result.append(result)
-        return filtered_detection_result
+        if images:
+            return doctr_predict_text(images, self.doctr_predictor, self.device)
+        return []
 
     @classmethod
     def get_requirements(cls) -> List[Requirement]:
-        return [get_pytorch_requirement(), get_detectron2_requirement()]
-
-    @classmethod
-    def _map_to_d2_categories(cls, categories: Mapping[str, TypeOrStr]) -> Dict[str, ObjectTypes]:
-        return {str(int(k) - 1): get_type(v) for k, v in categories.items()}
+        if tf_available():
+            return [get_tensorflow_requirement(), get_doctr_requirement(), get_tf_addons_requirements()]
+        if pytorch_available():
+            return [get_pytorch_requirement(), get_doctr_requirement()]
+        raise ModuleNotFoundError("Neither Tensorflow nor PyTorch has been installed. Cannot use DoctrTextRecognizer")
 
     def clone(self) -> PredictorBase:
-        return self.__class__(
-            self.path_yaml,
-            self.path_weights,
-            self.categories,
-            self.config_overwrite,
-            self.device,
-            self.filter_categories,
-        )
+        return self.__class__(self.architecture, self.path_weights, self.device_input)
 
-    def possible_categories(self) -> List[ObjectTypes]:
-        return list(self.categories.values())
+    def load_model(self) -> None:
+        """Loading model weights"""
+        _load_model(self.path_weights, self.doctr_predictor, self.device)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deepdoctection-0.25/deepdoctection/extern/deskew.py` & `deepdoctection-0.26/deepdoctection/extern/deskew.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/fastlang.py` & `deepdoctection-0.26/deepdoctection/extern/fastlang.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/hfdetr.py` & `deepdoctection-0.26/deepdoctection/extern/hfdetr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/hflayoutlm.py` & `deepdoctection-0.26/deepdoctection/extern/hflayoutlm.py`

 * *Files 0% similar despite different names*

```diff
@@ -615,15 +615,14 @@
         if device is not None:
             self.device = device
         else:
             self.device = set_torch_auto_device()
         self.model.to(self.device)
 
     def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> SequenceClassResult:
-
         input_ids = encodings.get("input_ids")
         attention_mask = encodings.get("attention_mask")
         token_type_ids = encodings.get("token_type_ids")
         boxes = encodings.get("bbox")
 
         if isinstance(input_ids, torch.Tensor):
             input_ids = input_ids.to(self.device)
@@ -660,15 +659,14 @@
 
     def clone(self) -> "HFLayoutLmSequenceClassifierBase":
         return self.__class__(self.path_config, self.path_weights, self.categories, self.device)
 
     def _validate_encodings(
         self, **encodings: Union[List[List[str]], "torch.Tensor"]
     ) -> Tuple["torch.Tensor", "torch.Tensor", "torch.Tensor", "torch.Tensor"]:
-
         input_ids = encodings.get("input_ids")
         attention_mask = encodings.get("attention_mask")
         token_type_ids = encodings.get("token_type_ids")
         boxes = encodings.get("bbox")
 
         if isinstance(input_ids, torch.Tensor):
             input_ids = input_ids.to(self.device)
@@ -728,15 +726,14 @@
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
         device: Optional[Literal["cpu", "cuda"]] = None,
     ):
-
         config = PretrainedConfig.from_pretrained(pretrained_model_name_or_path=path_config_json)
         self.model = LayoutLMForSequenceClassification.from_pretrained(
             pretrained_model_name_or_path=path_weights, config=config
         )
         super().__init__(path_config_json, path_weights, categories, device)
 
     def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> SequenceClassResult:
@@ -789,15 +786,14 @@
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
         device: Optional[Literal["cpu", "cuda"]] = None,
     ):
-
         config = LayoutLMv2Config.from_pretrained(pretrained_model_name_or_path=path_config_json)
         self.model = LayoutLMv2ForSequenceClassification.from_pretrained(
             pretrained_model_name_or_path=path_weights, config=config
         )
         super().__init__(path_config_json, path_weights, categories, device)
 
     def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> SequenceClassResult:
@@ -857,15 +853,14 @@
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
         device: Optional[Literal["cpu", "cuda"]] = None,
     ):
-
         config = LayoutLMv3Config.from_pretrained(pretrained_model_name_or_path=path_config_json)
         self.model = LayoutLMv3ForSequenceClassification.from_pretrained(
             pretrained_model_name_or_path=path_weights, config=config
         )
         super().__init__(path_config_json, path_weights, categories, device)
 
     def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> SequenceClassResult:
```

### Comparing `deepdoctection-0.25/deepdoctection/extern/model.py` & `deepdoctection-0.26/deepdoctection/extern/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,14 +233,33 @@
                 "3": LayoutType.list,
                 "4": LayoutType.table,
                 "5": LayoutType.figure,
             },
             dl_library="PT",
             model_wrapper="D2FrcnnDetector",
         ),
+        "layout/d2_model_0829999_layout_inf_only.ts": ModelProfile(
+            name="layout/d2_model_0829999_layout_inf_only.ts",
+            description="Detectron2 layout detection model trained on Publaynet. Torchscript export",
+            config="dd/d2/layout/CASCADE_RCNN_R_50_FPN_GN_TS.yaml",
+            size=[274974842],
+            tp_model=False,
+            hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_publaynet_inference_only",
+            hf_model_name="d2_model_0829999_layout_inf_only.ts",
+            hf_config_file=["CASCADE_RCNN_R_50_FPN_GN_TS.yaml"],
+            categories={
+                "1": LayoutType.text,
+                "2": LayoutType.title,
+                "3": LayoutType.list,
+                "4": LayoutType.table,
+                "5": LayoutType.figure,
+            },
+            dl_library="PT",
+            model_wrapper="D2FrcnnTracingDetector",
+        ),
         "cell/d2_model-1800000-cell.pkl": ModelProfile(
             name="cell/d2_model-1800000-cell.pkl",
             description="Detectron2 cell detection inference only model trained on Pubtabnet",
             config="dd/d2/cell/CASCADE_RCNN_R_50_FPN_GN.yaml",
             size=[274519039],
             tp_model=False,
             hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_c_inference_only",
@@ -259,14 +278,27 @@
             hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_c_inference_only",
             hf_model_name="d2_model_1849999_cell_inf_only.pt",
             hf_config_file=["Base-RCNN-FPN.yaml", "CASCADE_RCNN_R_50_FPN_GN.yaml"],
             categories={"1": LayoutType.cell},
             dl_library="PT",
             model_wrapper="D2FrcnnDetector",
         ),
+        "cell/d2_model_1849999_cell_inf_only.ts": ModelProfile(
+            name="cell/d2_model_1849999_cell_inf_only.ts",
+            description="Detectron2 cell detection inference only model trained on Pubtabnet. Torchscript export",
+            config="dd/d2/cell/CASCADE_RCNN_R_50_FPN_GN_TS.yaml",
+            size=[274898682],
+            tp_model=False,
+            hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_c_inference_only",
+            hf_model_name="d2_model_1849999_cell_inf_only.ts",
+            hf_config_file=["CASCADE_RCNN_R_50_FPN_GN_TS.yaml"],
+            categories={"1": LayoutType.cell},
+            dl_library="PT",
+            model_wrapper="D2FrcnnTracingDetector",
+        ),
         "cell/d2_model_1849999_cell.pth": ModelProfile(
             name="cell/d2_model_1849999_cell.pth",
             description="Detectron2 cell detection inference only model trained on Pubtabnet",
             config="dd/d2/cell/CASCADE_RCNN_R_50_FPN_GN.yaml",
             size=[548279023],
             tp_model=False,
             hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_c_inference_only",
@@ -311,14 +343,27 @@
             hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_rc_inference_only",
             hf_model_name="d2_model_1639999_item_inf_only.pt",
             hf_config_file=["Base-RCNN-FPN.yaml", "CASCADE_RCNN_R_50_FPN_GN.yaml"],
             categories={"1": LayoutType.row, "2": LayoutType.column},
             dl_library="PT",
             model_wrapper="D2FrcnnDetector",
         ),
+        "item/d2_model_1639999_item_inf_only.ts": ModelProfile(
+            name="item/d2_model_1639999_item_inf_only.ts",
+            description="Detectron2 cell detection inference only model trained on Pubtabnet. Torchscript export",
+            config="dd/d2/item/CASCADE_RCNN_R_50_FPN_GN_TS.yaml",
+            size=[274910970],
+            tp_model=False,
+            hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_rc_inference_only",
+            hf_model_name="d2_model_1639999_item_inf_only.ts",
+            hf_config_file=["CASCADE_RCNN_R_50_FPN_GN_TS.yaml"],
+            categories={"1": LayoutType.row, "2": LayoutType.column},
+            dl_library="PT",
+            model_wrapper="D2FrcnnTracingDetector",
+        ),
         "microsoft/layoutlm-base-uncased/pytorch_model.bin": ModelProfile(
             name="microsoft/layoutlm-base-uncased/pytorch_model.bin",
             description="LayoutLM is a simple but effective pre-training method of text and layout for document image"
             " understanding and information extraction tasks, such as form understanding and receipt"
             " understanding. LayoutLM archived the SOTA results on multiple datasets. This model does not"
             "contain any head and has to be fine tuned on a downstream task. This is model has been trained "
             "on 11M documents for 2 epochs.  Configuration: 12-layer, 768-hidden, 12-heads, 113M parameters",
```

### Comparing `deepdoctection-0.25/deepdoctection/extern/pdftext.py` & `deepdoctection-0.26/deepdoctection/extern/pdftext.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/pt/__init__.py` & `deepdoctection-0.26/deepdoctection/extern/tp/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Init file for pytorch compatibility package
+Init file for code from Tensorpack's FRCNN example
 """
```

### Comparing `deepdoctection-0.25/deepdoctection/extern/pt/ptutils.py` & `deepdoctection-0.26/deepdoctection/extern/pt/ptutils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tessocr.py` & `deepdoctection-0.26/deepdoctection/extern/tessocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/texocr.py` & `deepdoctection-0.26/deepdoctection/extern/texocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/__init__.py` & `deepdoctection-0.26/tests/datapoint/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,11 +10,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-"""
-Init file for code from Tensorpack's FRCNN example
-"""
```

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tfutils.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tfutils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tpcompat.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tpcompat.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/common.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/config/config.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/config/config.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/predict.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/predict.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/preproc.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/preproc.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py` & `deepdoctection-0.26/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/extern/tpdetect.py` & `deepdoctection-0.26/deepdoctection/extern/tpdetect.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/mapper/__init__.py` & `deepdoctection-0.26/deepdoctection/mapper/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,32 +14,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Contains everything that is related to transformation between datapoints
 """
-from typing import Callable, Optional
+from typing import Callable
 
-from ..datapoint.image import Image
-from ..utils.file_utils import detectron2_available, pytorch_available, transformers_available
+from ..utils.file_utils import pytorch_available, transformers_available
 from .cats import *
 from .cocostruct import *
 from .maputils import *
 from .match import *
 from .misc import *
 from .pascalstruct import *
 from .prodigystruct import *
 from .pubstruct import *
 from .tpstruct import *
 from .xfundstruct import *
 
-if detectron2_available() and pytorch_available():
-    from .d2struct import *
-
 if pytorch_available() and transformers_available():
     from .hfstruct import *
     from .laylmstruct import *
 
+if pytorch_available():
+    from .d2struct import *
 
 # Mapper
 Mapper = Callable[[Image], Optional[Image]]
```

### Comparing `deepdoctection-0.25/deepdoctection/mapper/cats.py` & `deepdoctection-0.26/deepdoctection/mapper/cats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/mapper/cocostruct.py` & `deepdoctection-0.26/deepdoctection/mapper/cocostruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     categories: Dict[str, str],
     load_image: bool,
     filter_empty_image: bool,
     fake_score: bool,
     coarse_mapping: Optional[Mapping[int, int]] = None,
     coarse_sub_cat_name: Optional[ObjectTypes] = None,
 ) -> Optional[Image]:
-
     """
     Map a dataset in coco format that has been serialized to image format. This serialized input requirements hold
     when a coco style sheet is loaded via `SerializerCoco.load`.
 
     :param dp: a datapoint in serialized coco format.
     :param categories: A dict of categories, e.g. `DatasetCategories.get_categories`
     :param load_image: If 'True' it will load image to attr: Image.image
```

### Comparing `deepdoctection-0.25/deepdoctection/mapper/d2struct.py` & `deepdoctection-0.26/deepdoctection/mapper/d2struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,26 @@
 
 
 import os.path
 from typing import Dict, List, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import torch
-from detectron2.layers import batched_nms
-from detectron2.structures import BoxMode
 
 from ..datapoint.annotation import ImageAnnotation
 from ..datapoint.image import Image
+from ..extern.pt.nms import batched_nms
 from ..mapper.maputils import curry
 from ..utils.detection_types import JsonDict
-from ..utils.file_utils import wandb_available
+from ..utils.file_utils import detectron2_available, wandb_available
 from ..utils.settings import ObjectTypes, TypeOrStr, get_type
 
+if detectron2_available():
+    from detectron2.structures import BoxMode
+
 if wandb_available():
     from wandb import Classes
     from wandb import Image as Wbimage
 
 
 @curry
 def image_to_d2_frcnn_training(
```

### Comparing `deepdoctection-0.25/deepdoctection/mapper/hfstruct.py` & `deepdoctection-0.26/deepdoctection/mapper/hfstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/mapper/laylmstruct.py` & `deepdoctection-0.26/deepdoctection/mapper/laylmstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/mapper/maputils.py` & `deepdoctection-0.26/deepdoctection/mapper/maputils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/mapper/match.py` & `deepdoctection-0.26/deepdoctection/mapper/match.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/mapper/misc.py` & `deepdoctection-0.26/deepdoctection/mapper/misc.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/mapper/pascalstruct.py` & `deepdoctection-0.26/deepdoctection/mapper/pascalstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/mapper/prodigystruct.py` & `deepdoctection-0.26/deepdoctection/mapper/prodigystruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/mapper/pubstruct.py` & `deepdoctection-0.26/deepdoctection/mapper/pubstruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 from ..utils.utils import is_file_extension
 from .maputils import MappingContextManager, curry, maybe_get_fake_score
 
 __all__ = ["pub_to_image"]
 
 
 def _convert_boxes(dp: JsonDict, height: int) -> JsonDict:
-
     if "bbox" in dp:
         table_box_3 = height - dp["bbox"][1]
         dp["bbox"][1] = height - dp["bbox"][3]
         dp["bbox"][3] = table_box_3
 
     for cell in dp["html"]["cells"]:
         if "bbox" in cell:
@@ -50,37 +49,34 @@
             cell["bbox"][1] = height - cell["bbox"][3]
             cell["bbox"][3] = cell_box_3
 
     return dp
 
 
 def _get_table_annotation(dp: JsonDict, category_id: str) -> ImageAnnotation:
-
     ulx, uly, lrx, lry = list(map(float, dp["bbox"]))
     bbox = BoundingBox(absolute_coords=True, ulx=ulx, uly=uly, lrx=lrx, lry=lry)
     annotation = ImageAnnotation(category_name=LayoutType.table, bounding_box=bbox, category_id=category_id)
     return annotation
 
 
 def _cell_token(html: Sequence[str]) -> List[List[int]]:
-
     index_rows = [i for i, tag in enumerate(html) if tag == "<tr>"]
     index_cells = [i for i, tag in enumerate(html) if tag in ("<td>", ">")]
     index_rows_tmp = [(index_rows[i], index_rows[i + 1]) for i in range(len(index_rows) - 1)]
     index_rows_tmp.append((index_rows[-1], index_cells[-1]))
     index_cells_tmp = [
         [index_cell for index_cell in index_cells if index_rows_tmp[i][0] < index_cell < index_rows_tmp[i][1]]
         for i in range(len(index_rows_tmp))
     ]
     index_cells_tmp[-1].append(index_cells[-1])
     return index_cells_tmp
 
 
 def _item_spans(html: Sequence[str], index_cells: Sequence[Sequence[int]], item: str) -> List[List[int]]:
-
     item_spans = [
         [
             int(html[index_cell - 1].replace(item + "=", "").replace('"', ""))
             if (item in html[index_cell - 1] and html[index_cell] == ">")
             else (
                 int(html[index_cell - 2].replace(item + "=", "").replace('"', ""))
                 if (item in html[index_cell - 2] and html[index_cell] == ">")
@@ -117,15 +113,14 @@
     number_of_cols = sum(col_spans[0])
     number_of_rows = len(col_spans)
     cell_ids = []
     i = 1
     for row in col_spans:
         cell_id_per_row = []
         for idx, k in enumerate(itertools.count(i)):
-
             if idx < len(row):
                 i += 1
                 cell_id_per_row.append(k)
             else:
                 break
         cell_ids.append(cell_id_per_row)
 
@@ -153,15 +148,14 @@
                     tiling[row_id + rs][col + cs] = cell_id
 
     np.array(tiling, dtype=np.int32)
     return tiling
 
 
 def _add_items(image: Image, item_type: str, categories_name_as_key: Dict[str, str], pubtables_like: bool) -> Image:
-
     item_number = CellType.row_number if item_type == LayoutType.row else CellType.column_number
     item_span = CellType.row_span if item_type == LayoutType.row else CellType.column_span
 
     summary_key = TableType.number_of_rows if item_type == LayoutType.row else TableType.number_of_columns
 
     number_of_items = 0
 
@@ -176,21 +170,21 @@
         cell_item = list(
             filter(
                 lambda x: x.get_sub_category(item_number).category_id == str(item_num), cells  # pylint: disable=W0640
             )
         )
         cell_item = list(filter(lambda x: x.get_sub_category(item_span).category_id == "1", cell_item))
         if cell_item:
-            ulx = min([cell.bounding_box.ulx for cell in cell_item if isinstance(cell.bounding_box, BoundingBox)])
+            ulx = min(cell.bounding_box.ulx for cell in cell_item if isinstance(cell.bounding_box, BoundingBox))
 
-            uly = min([cell.bounding_box.uly for cell in cell_item if isinstance(cell.bounding_box, BoundingBox)])
+            uly = min(cell.bounding_box.uly for cell in cell_item if isinstance(cell.bounding_box, BoundingBox))
 
-            lrx = max([cell.bounding_box.lrx for cell in cell_item if isinstance(cell.bounding_box, BoundingBox)])
+            lrx = max(cell.bounding_box.lrx for cell in cell_item if isinstance(cell.bounding_box, BoundingBox))
 
-            lry = max([cell.bounding_box.lry for cell in cell_item if isinstance(cell.bounding_box, BoundingBox)])
+            lry = max(cell.bounding_box.lry for cell in cell_item if isinstance(cell.bounding_box, BoundingBox))
 
             if pubtables_like:
                 tables = image.get_annotation(category_names=LayoutType.table)
                 if not tables:
                     raise ValueError("pubtables_like = True requires table")
                 table = tables[0]
 
@@ -224,15 +218,14 @@
             tmp_item_xy = table.bounding_box.uly + 1.0 if item_type == LayoutType.row else table.bounding_box.ulx + 1.0
         for idx, item in enumerate(item_type_anns):
             with MappingContextManager(
                 dp_name=image.file_name,
                 filter_level="bounding box",
                 image_annotation={"category_name": item.category_name, "annotation_id": item.annotation_id},
             ):
-
                 box = item.bounding_box
                 if box:
                     tmp_next_item_xy = 0.0
                     if idx != len(item_type_anns) - 1:
                         next_box = item_type_anns[idx + 1].bounding_box
                         if next_box:
                             tmp_next_item_xy = (
@@ -390,15 +383,14 @@
         col_spans = list(itertools.chain(*col_spans))  # type: ignore
         row_spans = list(itertools.chain(*row_spans))  # type: ignore
 
     if transforming_context.context_error:
         return None
 
     with MappingContextManager(str(idx)) as mapping_context:
-
         max_rs, max_cs = 0, 0
         if idx is None:
             raise ValueError("No valid datapoint external id")
 
         image = Image(file_name=os.path.split(dp["filename"])[1], location=dp["filename"], external_id=idx)
 
         if is_file_extension(dp["filename"], ".png"):
```

### Comparing `deepdoctection-0.25/deepdoctection/mapper/tpstruct.py` & `deepdoctection-0.26/deepdoctection/mapper/tpstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/mapper/xfundstruct.py` & `deepdoctection-0.26/deepdoctection/mapper/xfundstruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
     _, file_name = os.path.split(full_path)
     external_id = dp.get("uid")
     tag_to_id_mapping = ner_token_to_id_mapping[LayoutType.word][WordType.tag]
     token_class_to_id_mapping = ner_token_to_id_mapping[LayoutType.word][WordType.token_class]
     token_tag_to_id_mapping = ner_token_to_id_mapping[LayoutType.word][WordType.token_tag]
 
     with MappingContextManager(file_name) as mapping_context:
-
         image = Image(file_name=file_name, location=full_path, external_id=external_id)
 
         image.image = load_image_from_file(full_path)
 
         if not load_image:
             image.clear_image()
```

### Comparing `deepdoctection-0.25/deepdoctection/pipe/__init__.py` & `deepdoctection-0.26/deepdoctection/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/pipe/anngen.py` & `deepdoctection-0.26/deepdoctection/pipe/anngen.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/pipe/base.py` & `deepdoctection-0.26/deepdoctection/pipe/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/pipe/cell.py` & `deepdoctection-0.26/deepdoctection/pipe/cell.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/pipe/common.py` & `deepdoctection-0.26/deepdoctection/pipe/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,14 @@
             for idx, parent in enumerate(matched_parent_anns):
                 parent.dump_relationship(Relationships.child, matched_child_anns[idx].annotation_id)
 
     def clone(self) -> PipelineComponent:
         return self.__class__(self.parent_categories, self.child_categories, self.matching_rule, self.threshold)
 
     def get_meta_annotation(self) -> JsonDict:
-
         return dict(
             [
                 ("image_annotations", []),
                 ("sub_categories", {}),
                 ("relationships", {parent: {Relationships.child} for parent in self.parent_categories}),
                 ("summaries", []),
             ]
```

### Comparing `deepdoctection-0.25/deepdoctection/pipe/concurrency.py` & `deepdoctection-0.26/deepdoctection/pipe/concurrency.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,14 @@
     def __init__(
         self,
         pipeline_components: Sequence[Union[PipelineComponent, PageParsingService, ImageParsingService]],
         pre_proc_func: Optional[Callable[[Image], Image]] = None,
         post_proc_func: Optional[Callable[[Image], Image]] = None,
         max_datapoints: Optional[int] = None,
     ) -> None:
-
         """
         :param pipeline_components: list of identical pipeline component. Number of threads created is determined by
                                     `len`
         :param pre_proc_func: pass a function, that reads and returns an image. Will execute before entering the pipe
                               component
         :param post_proc_func: pass a function, that reads and returns an image. Will execute after entering the pipe
                                component
@@ -157,34 +156,34 @@
                 )
             all_results = list(itertools.chain(*[fut.result() for fut in futures]))
         return all_results
 
     @staticmethod
     def _thread_predict_on_queue(
         input_queue: QueueType,
-        component: PipelineComponent,
+        component: Union[PipelineComponent, PageParsingService, ImageParsingService],
         tqdm_bar: Optional[TqdmType] = None,
         pre_proc_func: Optional[Callable[[Image], Image]] = None,
         post_proc_func: Optional[Callable[[Image], Image]] = None,
     ) -> List[Image]:
-
         outputs = []
 
         with ExitStack() as stack:
             if tqdm_bar is None:
                 tqdm_bar = stack.enter_context(get_tqdm(total=input_queue.qsize()))
 
             while not input_queue.empty():
                 inp = input_queue.get_nowait()
                 if pre_proc_func is not None:
                     inp = pre_proc_func(inp)
                 out = component.pass_datapoint(inp)
-                if post_proc_func is not None:
+                if post_proc_func is not None and out is not None:
                     out = post_proc_func(out)
-                outputs.append(out)
+                if out is not None:
+                    outputs.append(out)
                 tqdm_bar.update(1)
         return outputs
 
     def _put_datapoints_to_queue(self, df: Union[DataFlow, List[Image]]) -> None:
         if isinstance(df, DataFlow):
             df.reset_state()
         for idx, dp in enumerate(df):
```

### Comparing `deepdoctection-0.25/deepdoctection/pipe/doctectionpipe.py` & `deepdoctection-0.26/deepdoctection/pipe/doctectionpipe.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/pipe/language.py` & `deepdoctection-0.26/deepdoctection/pipe/language.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/pipe/layout.py` & `deepdoctection-0.26/deepdoctection/pipe/layout.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/pipe/lm.py` & `deepdoctection-0.26/deepdoctection/pipe/lm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/pipe/order.py` & `deepdoctection-0.26/deepdoctection/pipe/order.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,15 +353,15 @@
         :return:
         """
         if not word_anns:
             return []
         # every list now non-empty
         word_anns_dict = {ann.annotation_id: ann for ann in word_anns}
         word_order_list = OrderGenerator.group_words_into_lines(word_anns, image_id)
-        number_rows = max([word[1] for word in word_order_list])
+        number_rows = max(word[1] for word in word_order_list)
         detection_result_list = []
         for row in range(1, number_rows + 1):
             ann_meta_per_row = [ann_meta for ann_meta in word_order_list if ann_meta[1] == row]
             ann_ids = [ann_meta[2] for ann_meta in ann_meta_per_row]
             anns_per_row = [word_anns_dict[ann_id] for ann_id in ann_ids]
             anns_per_row.sort(key=lambda x: x.image.get_embedding(image_id).ulx)  # type: ignore
```

### Comparing `deepdoctection-0.25/deepdoctection/pipe/refine.py` & `deepdoctection-0.26/deepdoctection/pipe/refine.py`

 * *Files 2% similar despite different names*

```diff
@@ -456,18 +456,18 @@
                             cells.pop(box_index)
                         no_context_error = not annotation_context.context_error
                     if no_context_error:
                         for cell in cells:
                             cell.deactivate()
 
             cells = table.image.get_annotation(category_names=self._cell_names)
-            number_of_rows = max([int(cell.get_sub_category(CellType.row_number).category_id) for cell in cells])
-            number_of_cols = max([int(cell.get_sub_category(CellType.column_number).category_id) for cell in cells])
-            max_row_span = max([int(cell.get_sub_category(CellType.row_span).category_id) for cell in cells])
-            max_col_span = max([int(cell.get_sub_category(CellType.column_span).category_id) for cell in cells])
+            number_of_rows = max(int(cell.get_sub_category(CellType.row_number).category_id) for cell in cells)
+            number_of_cols = max(int(cell.get_sub_category(CellType.column_number).category_id) for cell in cells)
+            max_row_span = max(int(cell.get_sub_category(CellType.row_span).category_id) for cell in cells)
+            max_col_span = max(int(cell.get_sub_category(CellType.column_span).category_id) for cell in cells)
             # TODO: the summaries should be sub categories of the underlying ann
             if TableType.number_of_rows in table.sub_categories:
                 table.remove_sub_category(TableType.number_of_rows)
             if TableType.number_of_columns in table.sub_categories:
                 table.remove_sub_category(TableType.number_of_columns)
             if TableType.max_row_span in table.sub_categories:
                 table.remove_sub_category(TableType.max_row_span)
```

### Comparing `deepdoctection-0.25/deepdoctection/pipe/registry.py` & `deepdoctection-0.26/deepdoctection/pipe/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/pipe/segment.py` & `deepdoctection-0.26/deepdoctection/pipe/segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,25 +467,23 @@
     raw_table_segments = []
     with MappingContextManager(dp_name=dp.file_name) as segment_mapping_context:
         for idx, cell in enumerate(cells):
             cell_positions_rows = cell_index_rows == idx
             rows_of_cell = [rows[k] for k in row_index[cell_positions_rows]]
             rs = np.count_nonzero(cell_index_rows == idx)
             if len(rows_of_cell):
-                row_number = min([int(row.get_sub_category(CellType.row_number).category_id) for row in rows_of_cell])
+                row_number = min(int(row.get_sub_category(CellType.row_number).category_id) for row in rows_of_cell)
             else:
                 row_number = 0
 
             cell_positions_cols = cell_index_cols == idx
             cols_of_cell = [columns[k] for k in col_index[cell_positions_cols]]
             cs = np.count_nonzero(cell_index_cols == idx)
             if len(cols_of_cell):
-                col_number = min(
-                    [int(col.get_sub_category(CellType.column_number).category_id) for col in cols_of_cell]
-                )
+                col_number = min(int(col.get_sub_category(CellType.column_number).category_id) for col in cols_of_cell)
             else:
                 col_number = 0
 
             raw_table_segments.append(
                 SegmentationResult(
                     annotation_id=cell.annotation_id,
                     row_num=row_number,
@@ -608,35 +606,33 @@
     raw_table_segments = []
 
     with MappingContextManager(dp_name=dp.file_name) as segment_mapping_context:
         for idx, cell in enumerate(spanning_cells):
             cell_positions_rows = cell_index_rows == idx
             rows_of_cell = [rows[k] for k in row_index[cell_positions_rows]]
             rs = (
-                max([int(row.get_sub_category(CellType.row_number).category_id) for row in rows_of_cell])
-                - min([int(row.get_sub_category(CellType.row_number).category_id) for row in rows_of_cell])
+                max(int(row.get_sub_category(CellType.row_number).category_id) for row in rows_of_cell)
+                - min(int(row.get_sub_category(CellType.row_number).category_id) for row in rows_of_cell)
                 + 1
             )
             if len(rows_of_cell):
-                row_number = min([int(row.get_sub_category(CellType.row_number).category_id) for row in rows_of_cell])
+                row_number = min(int(row.get_sub_category(CellType.row_number).category_id) for row in rows_of_cell)
             else:
                 row_number = 0
 
             cell_positions_cols = cell_index_cols == idx
             cols_of_cell = [columns[k] for k in col_index[cell_positions_cols]]
             cs = (
-                max([int(col.get_sub_category(CellType.column_number).category_id) for col in cols_of_cell])
-                - min([int(col.get_sub_category(CellType.column_number).category_id) for col in cols_of_cell])
+                max(int(col.get_sub_category(CellType.column_number).category_id) for col in cols_of_cell)
+                - min(int(col.get_sub_category(CellType.column_number).category_id) for col in cols_of_cell)
                 + 1
             )
 
             if len(cols_of_cell):
-                col_number = min(
-                    [int(col.get_sub_category(CellType.column_number).category_id) for col in cols_of_cell]
-                )
+                col_number = min(int(col.get_sub_category(CellType.column_number).category_id) for col in cols_of_cell)
             else:
                 col_number = 0
 
             raw_table_segments.append(
                 SegmentationResult(
                     annotation_id=cell.annotation_id,
                     row_num=row_number,
@@ -778,18 +774,18 @@
                 )
                 self.dp_manager.set_category_annotation(
                     CellType.column_span, segment_result.cs, CellType.column_span, segment_result.annotation_id
                 )
 
             if table.image:
                 cells = table.image.get_annotation(category_names=self._cell_names)
-                number_of_rows = max([int(cell.get_sub_category(CellType.row_number).category_id) for cell in cells])
-                number_of_cols = max([int(cell.get_sub_category(CellType.column_number).category_id) for cell in cells])
-                max_row_span = max([int(cell.get_sub_category(CellType.row_span).category_id) for cell in cells])
-                max_col_span = max([int(cell.get_sub_category(CellType.column_span).category_id) for cell in cells])
+                number_of_rows = max(int(cell.get_sub_category(CellType.row_number).category_id) for cell in cells)
+                number_of_cols = max(int(cell.get_sub_category(CellType.column_number).category_id) for cell in cells)
+                max_row_span = max(int(cell.get_sub_category(CellType.row_span).category_id) for cell in cells)
+                max_col_span = max(int(cell.get_sub_category(CellType.column_span).category_id) for cell in cells)
                 # TODO: the summaries should be sub categories of the underlying ann
                 self.dp_manager.set_summary_annotation(
                     TableType.number_of_rows,
                     TableType.number_of_rows,
                     number_of_rows,
                     annotation_id=table.annotation_id,
                 )
@@ -1018,18 +1014,18 @@
                 for cell_position in cells_to_deactivate:
                     cell_ann_id = cell_rn_cn_to_ann_id[cell_position]
                     self.dp_manager.deactivate_annotation(cell_ann_id)
 
             cells = []
             if table.image:
                 cells = table.image.get_annotation(category_names=self._cell_names)
-            number_of_rows = max([int(cell.get_sub_category(CellType.row_number).category_id) for cell in cells])
-            number_of_cols = max([int(cell.get_sub_category(CellType.column_number).category_id) for cell in cells])
-            max_row_span = max([int(cell.get_sub_category(CellType.row_span).category_id) for cell in cells])
-            max_col_span = max([int(cell.get_sub_category(CellType.column_span).category_id) for cell in cells])
+            number_of_rows = max(int(cell.get_sub_category(CellType.row_number).category_id) for cell in cells)
+            number_of_cols = max(int(cell.get_sub_category(CellType.column_number).category_id) for cell in cells)
+            max_row_span = max(int(cell.get_sub_category(CellType.row_span).category_id) for cell in cells)
+            max_col_span = max(int(cell.get_sub_category(CellType.column_span).category_id) for cell in cells)
             # TODO: the summaries should be sub categories of the underlying ann
             self.dp_manager.set_summary_annotation(
                 TableType.number_of_rows, TableType.number_of_rows, number_of_rows, annotation_id=table.annotation_id
             )
             self.dp_manager.set_summary_annotation(
                 TableType.number_of_columns,
                 TableType.number_of_columns,
```

### Comparing `deepdoctection-0.25/deepdoctection/pipe/text.py` & `deepdoctection-0.26/deepdoctection/pipe/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,27 +95,27 @@
                 self.predictor, TesseractOcrDetector
             ), "Only TesseractOcrDetector supports multiple languages"
 
         self.run_time_ocr_language_selection = run_time_ocr_language_selection
         self.skip_if_text_extracted = skip_if_text_extracted
         if self.skip_if_text_extracted and isinstance(self.predictor, TextRecognizer):
             raise ValueError(
-                "skip_if_text_extracted=True and TextRecognizer in TextExtractionService is not " "compatible"
+                "skip_if_text_extracted=True and TextRecognizer in TextExtractionService is not compatible"
             )
 
     def serve(self, dp: Image) -> None:
         maybe_batched_text_rois = self.get_text_rois(dp)
         for text_roi in maybe_batched_text_rois:
             ann_id = None
             if isinstance(text_roi, ImageAnnotation):
                 ann_id = text_roi.annotation_id
             predictor_input = self.get_predictor_input(text_roi)
             if predictor_input is None:
                 raise ValueError("predictor_input cannot be None")
-            if predictor_input in [b""]:
+            if isinstance(predictor_input, int):
                 pass
             else:
                 width, height = None, None
                 if self.run_time_ocr_language_selection:
                     self.predictor.set_language(dp.summary.get_sub_category(PageType.language).value)  # type: ignore
                 detect_result_list = self.predictor.predict(predictor_input)  # type: ignore
                 if isinstance(self.predictor, PdfMiner):
@@ -156,15 +156,15 @@
             if self.predictor.accepts_batch:
                 return [dp.get_annotation(category_names=self.extract_from_category)]
             return dp.get_annotation(category_names=self.extract_from_category)
         return [dp]
 
     def get_predictor_input(
         self, text_roi: Union[Image, ImageAnnotation, List[ImageAnnotation]]
-    ) -> Optional[Union[bytes, ImageType, List[Tuple[str, ImageType]]]]:
+    ) -> Optional[Union[bytes, ImageType, List[Tuple[str, ImageType]], int]]:
         """
         Return raw input for a given `text_roi`. This can be a numpy array or pdf bytes and depends on the chosen
         predictor.
 
         :param text_roi: `Image` or `ImageAnnotation`
         :return: pdf bytes or numpy array
         """
@@ -181,15 +181,15 @@
             return text_roi.image
         if isinstance(text_roi, list):
             assert all(roi.image is not None for roi in text_roi)
             assert all(roi.image.image is not None for roi in text_roi)  # type: ignore
             return [(roi.annotation_id, roi.image.image) for roi in text_roi]  # type: ignore
         if isinstance(self.predictor, PdfMiner) and text_roi.pdf_bytes is not None:
             return text_roi.pdf_bytes
-        return b""
+        return 1
 
     def get_meta_annotation(self) -> JsonDict:
         if self.extract_from_category:
             sub_cat_dict = {category: {WordType.characters} for category in self.extract_from_category}
         else:
             if not isinstance(self.predictor, (ObjectDetector, PdfMiner)):
                 raise TypeError(
```

### Comparing `deepdoctection-0.25/deepdoctection/pipe/transform.py` & `deepdoctection-0.26/deepdoctection/pipe/transform.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/train/__init__.py` & `deepdoctection-0.26/deepdoctection/train/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/train/d2_frcnn_train.py` & `deepdoctection-0.26/deepdoctection/train/d2_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/train/hf_detr_train.py` & `deepdoctection-0.26/deepdoctection/train/hf_detr_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/train/hf_layoutlm_train.py` & `deepdoctection-0.26/deepdoctection/train/hf_layoutlm_train.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,15 @@
         raise ValueError("Dataset type not supported for training")
 
     config_cls, model_cls, model_wrapper_cls, tokenizer_fast = _get_model_class_and_tokenizer(
         path_config_json, dataset_type, use_xlm_tokenizer
     )
     image_to_raw_layoutlm_kwargs = {"dataset_type": dataset_type, "use_token_tag": use_token_tag}
     if segment_positions:
-        image_to_raw_layoutlm_kwargs["segment_positions"] = segment_positions
+        image_to_raw_layoutlm_kwargs["segment_positions"] = segment_positions  # type: ignore
     image_to_raw_layoutlm_kwargs.update(model_wrapper_cls.default_kwargs_for_input_mapping())
     dataset = DatasetAdapter(
         dataset_train,
         True,
         image_to_raw_layoutlm_features(**image_to_raw_layoutlm_kwargs),
         use_token_tag,
         **build_train_dict,
```

### Comparing `deepdoctection-0.25/deepdoctection/train/tp_frcnn_train.py` & `deepdoctection-0.26/deepdoctection/train/tp_frcnn_train.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                     "Datapoint have images as np arrays stored and they will be loaded into memory. "
                     "To avoid OOM set 'load_image'=False in dataflow build config. This will load "
                     "images when needed and reduce memory costs!!!",
                     "warn",
                 )
             summarizer.dump(dp["gt_labels"])
             datapoints.append(dp)
-            status_bar.update()  # type: ignore
+            status_bar.update()
     summarizer.print_summary_histogram(dd_logic=False)
     num_datapoints = len(datapoints)
     logger.info("Total #images for training: %i", num_datapoints)
     df = DataFromList(datapoints, shuffle=True)
     buffer_size = min(num_datapoints - 1, 200)
 
     load_augment_anchors = LoadAugmentAddAnchors(cfg)  # can't use dec: curry as pickling will fail in mp
```

### Comparing `deepdoctection-0.25/deepdoctection/utils/__init__.py` & `deepdoctection-0.26/deepdoctection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/utils/concurrency.py` & `deepdoctection-0.26/deepdoctection/utils/concurrency.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         """Stop the thread"""
         self._stop_evt.set()
 
     def stopped(self) -> bool:
         """
         :param bool: whether the thread is stopped or not
         """
-        return self._stop_evt.isSet()
+        return self._stop_evt.is_set()
 
     def queue_put_stoppable(self, q: QueueType, obj: Any) -> None:
         """Put obj to queue, but will give up when the thread is stopped"""
         while not self.stopped():
             try:
                 q.put(obj, timeout=5)
                 break
@@ -101,20 +101,19 @@
         import prctl  # type: ignore #pylint: disable=C0415  # pip install python-prctl
     except ImportError:
         if _warn:
             log_once(
                 '"import prctl" failed! Install python-prctl so that processes can be cleaned with guarantee.', "warn"
             )
         return
-    else:
-        assert hasattr(
-            prctl, "set_pdeathsig"
-        ), "prctl.set_pdeathsig does not exist! Note that you need to install 'python-prctl' instead of 'prctl'."
-        # is SIGHUP a good choice?
-        prctl.set_pdeathsig(signal.SIGHUP)
+    assert hasattr(
+        prctl, "set_pdeathsig"
+    ), "prctl.set_pdeathsig does not exist! Note that you need to install 'python-prctl' instead of 'prctl'."
+    # is SIGHUP a good choice?
+    prctl.set_pdeathsig(signal.SIGHUP)
 
 
 # taken from https://github.com/tensorpack/dataflow/blob/master/dataflow/utils/concurrency.py
 
 
 @no_type_check
 def start_proc_mask_signal(proc):
```

### Comparing `deepdoctection-0.25/deepdoctection/utils/context.py` & `deepdoctection-0.26/deepdoctection/utils/context.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/utils/detection_types.py` & `deepdoctection-0.26/deepdoctection/utils/detection_types.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/utils/develop.py` & `deepdoctection-0.26/deepdoctection/utils/develop.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/utils/file_utils.py` & `deepdoctection-0.26/deepdoctection/utils/file_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     return bool(_LXML_AVAILABLE)
 
 
 def get_lxml_requirement() -> Requirement:
     """
     Returns lxml requirement
     """
-    return "lxml", lxml_available(), _TRANSFORMERS_ERR_MSG
+    return "lxml", lxml_available(), _LXML_ERR_MSG
 
 
 # apted
 _APTED_AVAILABLE = importlib.util.find_spec("apted") is not None
 _APTED_ERR_MSG = "APTED must be installed: pip install apted"
 
 
@@ -288,15 +288,15 @@
 
 class TesseractNotFound(BaseException):
     """
     Exception class for Tesseract being not found
     """
 
 
-def get_tesseract_version() -> Union[int, version.Version, version.LegacyVersion]:
+def get_tesseract_version() -> Union[int, version.Version]:
     """
     Returns Version object of the Tesseract version. We need at least Tesseract 3.05
     """
     try:
         output = subprocess.check_output(
             [_TESS_PATH, "--version"],
             stderr=subprocess.STDOUT,
@@ -348,15 +348,15 @@
 
 class PopplerNotFound(BaseException):
     """
     Exception class for Poppler being not found
     """
 
 
-def get_poppler_version() -> Union[int, version.Version, version.LegacyVersion]:
+def get_poppler_version() -> Union[int, version.Version]:
     """
     Returns Version object of the Poppler version. We need at least Tesseract 3.05
     """
 
     if pdf_to_ppm_available():
         command = "pdftoppm"
     elif pdf_to_cairo_available():
```

### Comparing `deepdoctection-0.25/deepdoctection/utils/fs.py` & `deepdoctection-0.26/deepdoctection/utils/fs.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/utils/identifier.py` & `deepdoctection-0.26/deepdoctection/utils/identifier.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/utils/logger.py` & `deepdoctection-0.26/deepdoctection/utils/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     def dir_nonempty(directory: str) -> int:
         return os.path.isdir(directory) and len([x for x in os.listdir(directory) if x[0] != "."])
 
     if dir_nonempty(dir_name):
         if not action:
             logger.warning("Log directory %s exists! Use 'd' to delete it. ", dir_name)
             logger.warning(
-                "If you're resuming from a previous run, you can choose to keep it." "Press any other key to exit. "
+                "If you're resuming from a previous run, you can choose to keep it. Press any other key to exit. "
             )
         while not action:
             action = input("Select Action: k (keep) / d (delete) / q (quit):").lower().strip()
         act = action
         if act == "b":
             backup_name = dir_name + _get_time_str()
             shutil.move(dir_name, backup_name)
@@ -221,15 +221,15 @@
     'script_name' is the name of the main python file currently running.
 
     :param action: an action of ["k","d","q"] to be performed (see also func: set_logger_dir)
     :param name: Optional suffix of file name.
     """
 
     mod = sys.modules["__main__"]
-    basename = str(os.path.basename(mod.__file__))  # type: ignore
+    basename = str(os.path.basename(mod.__file__))  # type: ignore  # pylint: disable=E1101
     auto_dir_name = os.path.join("train_log", basename[: basename.rfind(".")])
     if name:
         auto_dir_name += "_%s" % name if os.name == "nt" else ":%s" % name  # pylint: disable=C0209
     set_logger_dir(auto_dir_name, action=action)
 
 
 def get_logger_dir() -> Optional[str]:
```

### Comparing `deepdoctection-0.25/deepdoctection/utils/metacfg.py` & `deepdoctection-0.26/deepdoctection/utils/metacfg.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/utils/pdf_utils.py` & `deepdoctection-0.26/deepdoctection/utils/pdf_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from errno import ENOENT
 from io import BytesIO
 from shutil import copyfile
 from typing import Generator, List, Optional, Tuple
 
 from cv2 import IMREAD_COLOR, imread
 from numpy import uint8
-from PyPDF2 import PdfFileReader, PdfFileWriter, errors
+from PyPDF2 import PdfReader, PdfWriter, errors
 
 from .context import save_tmp_file, timeout_manager
 from .detection_types import ImageType, Pathlike
 from .file_utils import PopplerNotFound, pdf_to_cairo_available, pdf_to_ppm_available, qpdf_available
 from .logger import logger
 from .utils import FileExtensionError, is_file_extension
 
@@ -66,15 +66,15 @@
         if not response:
             return True
     else:
         logger.info("qpdf is not installed. If the document must be decrypted please ensure that it is installed")
     return False
 
 
-def get_pdf_file_reader(path: Pathlike) -> PdfFileReader:
+def get_pdf_file_reader(path: Pathlike) -> PdfReader:
     """
     Creates a file reader object from a pdf document. Will try to decrypt the document if it is
     encrypted. (See `decrypt_pdf_document` to understand what is meant with "decrypt").
 
     :param path: A path to a pdf document
     :return: A file reader object from which you can iterate through the document.
     """
@@ -84,35 +84,35 @@
     file_name = os.path.split(path)[1]
     if not is_file_extension(file_name, ".pdf"):
         raise FileExtensionError(f"must be a pdf file: {file_name}")
 
     with open(path, "rb") as file:
         qpdf_called = False
         try:
-            input_pdf_as_bytes = PdfFileReader(file)
+            input_pdf_as_bytes = PdfReader(file)
         except (errors.PdfReadError, AttributeError):
             _ = decrypt_pdf_document(path)
             qpdf_called = True
 
         if not qpdf_called:
-            if input_pdf_as_bytes.isEncrypted:
+            if input_pdf_as_bytes.is_encrypted:
                 is_decrypted = decrypt_pdf_document(path)
                 if not is_decrypted:
                     logger.error("pdf document %s cannot be decrypted and therefore cannot be processed further.", path)
                     sys.exit()
 
-    file_reader = PdfFileReader(open(path, "rb"))  # pylint: disable=R1732
+    file_reader = PdfReader(open(path, "rb"))  # pylint: disable=R1732
     return file_reader
 
 
-def get_pdf_file_writer() -> PdfFileWriter:
+def get_pdf_file_writer() -> PdfWriter:
     """
-    `PdfFileWriter` instance
+    `PdfWriter` instance
     """
-    return PdfFileWriter()
+    return PdfWriter()
 
 
 class PDFStreamer:
     """
     A class for streaming pdf documents as bytes objects. Build as a generator, it is possible to load the document
     iteratively into memory. Uses py2pdf FileReader and FileWriter.
 
@@ -127,36 +127,35 @@
     """
 
     def __init__(self, path: Pathlike) -> None:
         """
         :param path: to a pdf.
         """
         self.file_reader = get_pdf_file_reader(path)
-        self.file_writer = PdfFileWriter()
+        self.file_writer = PdfWriter()
 
     def __len__(self) -> int:
-        return self.file_reader.getNumPages()
+        return len(self.file_reader.pages)
 
     def __iter__(self) -> Generator[Tuple[bytes, int], None, None]:
         for k in range(len(self)):
             buffer = BytesIO()
-            writer = PdfFileWriter()
-            writer.addPage(self.file_reader.getPage(k))
+            writer = get_pdf_file_writer()
+            writer.add_page(self.file_reader.pages[k])
             writer.write(buffer)
             yield buffer.getvalue(), k
 
 
 # The following functions are modified versions from the Python poppler wrapper
 # https://github.com/Belval/pdf2image/blob/master/pdf2image/pdf2image.py
 
 
 def _input_to_cli_str(
     input_file_name: Pathlike, output_file_name: Pathlike, dpi: int, size: Optional[Tuple[int, int]] = None
 ) -> List[str]:
-
     cmd_args: List[str] = []
 
     if pdf_to_ppm_available():
         command = "pdftoppm"
     elif pdf_to_cairo_available():
         command = "pdftocairo"
     else:
```

### Comparing `deepdoctection-0.25/deepdoctection/utils/settings.py` & `deepdoctection-0.26/deepdoctection/utils/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         """
         for member in cls.__members__.values():
             if member.value == value:
                 return member
         raise ValueError(f"value {value} does not have corresponding member")
 
 
-TypeOrStr = Union[ObjectTypes, str]
+TypeOrStr = Union[ObjectTypes, str]  # pylint: disable=C0103
 
 object_types_registry = catalogue.create("deepdoctection", "settings", entry_points=True)
 
 
 # pylint: disable=invalid-name
 @object_types_registry.register("DefaultType")
 class DefaultType(ObjectTypes):
```

### Comparing `deepdoctection-0.25/deepdoctection/utils/systools.py` & `deepdoctection-0.26/deepdoctection/utils/systools.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/utils/tqdm.py` & `deepdoctection-0.26/deepdoctection/utils/tqdm.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,23 +32,23 @@
     **kwargs: Optional[Union[str, int, float]]
 ) -> Dict[str, Union[str, float, bool, int, None]]:
     """
     Return default arguments to be used with tqdm.
     :param kwargs: extra arguments to be used.
     """
 
-    return dict(
-        total=kwargs.get("total"),
-        leave=True,
-        smoothing=0.5,
-        dynamic_ncols=True,
-        ascii=True,
-        bar_format="{l_bar}{bar}|{n_fmt}/{total_fmt}[{elapsed}<{remaining},{rate_noinv_fmt}]",
-        mininterval=5,
-    )
+    return {
+        "total": kwargs.get("total"),
+        "leave": True,
+        "smoothing": 0.5,
+        "dynamic_ncols": True,
+        "ascii": True,
+        "bar_format": "{l_bar}{bar}|{n_fmt}/{total_fmt}[{elapsed}<{remaining},{rate_noinv_fmt}]",
+        "mininterval": 5,
+    }
 
 
 def get_tqdm(total: Optional[Union[int, float]] = None, **kwargs: Union[str, int, float]) -> TqdmType:
     """
     Get tqdm progress bar with some default options to have consistent style.
 
     :param total:  The number of expected iterations.
```

### Comparing `deepdoctection-0.25/deepdoctection/utils/transform.py` & `deepdoctection-0.26/deepdoctection/utils/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     def __init__(
         self,
         h: Union[int, float],
         w: Union[int, float],
         new_h: Union[int, float],
         new_w: Union[int, float],
-        interp: str,
+        interp: Union[str, int],
     ):
         """
         :param h: height
         :param w: width
         :param new_h: target height
         :param new_w: target width
         :param interp: cv2 interpolation method like cv2.INTER_NEAREST, cv2.INTER_LINEAR,
@@ -75,15 +75,15 @@
         self.w = w
         self.new_h = new_h
         self.new_w = new_w
         self.interp = interp
 
     def apply_image(self, img: ImageType) -> ImageType:
         assert img.shape[:2] == (self.h, self.w)
-        ret = cv2.resize(img, (self.new_w, self.new_h), interpolation=self.interp)
+        ret = cv2.resize(img, (self.new_w, self.new_h), interpolation=self.interp)  # type: ignore
         if img.ndim == 3 and ret.ndim == 2:
             ret = ret[:, :, np.newaxis]
         return ret
 
     def apply_coords(self, coords: npt.NDArray[float32]) -> npt.NDArray[float32]:
         """Transformation that should be applied to coordinates"""
         coords[:, 0] = coords[:, 0] * (self.new_w * 1.0 / self.w)
@@ -93,15 +93,15 @@
 
 class InferenceResize:
     """
     Try resizing the shortest edge to a certain number while avoiding the longest edge to exceed max_size. This is
     the inference version of `extern.tp.frcnn.common.CustomResize` .
     """
 
-    def __init__(self, short_edge_length: int, max_size: int, interp: str = cv2.INTER_LINEAR) -> None:
+    def __init__(self, short_edge_length: int, max_size: int, interp: int = cv2.INTER_LINEAR) -> None:
         """
         :param short_edge_length: a [min, max] interval from which to sample the shortest edge length.
         :param max_size: maximum allowed longest edge length.
         """
         self.short_edge_length = short_edge_length
         self.max_size = max_size
         self.interp = interp
@@ -146,15 +146,15 @@
 
     :param image: image as np.array
     :param top: Top pixel value to pad
     :param right: Right pixel value to pad
     :param bottom: Bottom pixel value to pad
     :param left: Left pixel value to pad
     """
-    return np.pad(image, ((left, right), (top, bottom), (0, 0)), "constant", constant_values=(255))
+    return np.pad(image, ((left, right), (top, bottom), (0, 0)), "constant", constant_values=255)
 
 
 class PadTransform(BaseTransform):
     """
     A transform for padding images left/right/top/bottom-wise.
     """
```

### Comparing `deepdoctection-0.25/deepdoctection/utils/utils.py` & `deepdoctection-0.26/deepdoctection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/deepdoctection/utils/viz.py` & `deepdoctection-0.26/deepdoctection/utils/viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 <https://github.com/tensorpack/tensorpack/blob/master/tensorpack/utils/viz.py>
 
 and
 
 <https://github.com/facebookresearch/detectron2/blob/main/detectron2/utils/colormap.py>
 """
 import sys
-from typing import Callable, List, Optional, Tuple
+from typing import Callable, List, Optional, Tuple, no_type_check
 
 import cv2
 import numpy as np
 import numpy.typing as npt
 from numpy import float32
 
 from .detection_types import ImageType
@@ -285,14 +285,15 @@
             font = cv2.FONT_HERSHEY_SIMPLEX
             ((_, text_h), _) = cv2.getTextSize(category, font, font_scale, 2)
             y_0 = y_0 - int(10 * text_h)
 
     return np_image
 
 
+@no_type_check
 def interactive_imshow(
     img: ImageType,
     lclick_cb: Optional[Callable[[npt.NDArray[float32], int, int], None]] = None,
     rclick_cb: Optional[Callable[[npt.NDArray[float32], int, int], None]] = None,
     **kwargs: str,
 ) -> None:
     """
@@ -307,28 +308,28 @@
                           * q: destroy the current window
                           * x: execute ``sys.exit()``
                           * s: save image to "out.png"
     """
     name = "q, x: quit / s: save"
     cv2.imshow(name, img)
 
-    def mouse_cb(event, x, y, *args):  # type: ignore
+    def mouse_cb(event, x, y, *args):
         if event == cv2.EVENT_LBUTTONUP and lclick_cb is not None:
             lclick_cb(img.astype(dtype=float32), x, y)
         elif event == cv2.EVENT_RBUTTONUP and rclick_cb is not None:
             rclick_cb(img.astype(dtype=float32), x, y)
 
     cv2.setMouseCallback(name, mouse_cb)
     key = cv2.waitKey(-1)
     while key >= 128:
         key = cv2.waitKey(-1)
     key = chr(key & 0xFF)
     cb_name = "key_cb_" + key
     if cb_name in kwargs:
-        kwargs[cb_name](img)  # type: ignore
+        kwargs[cb_name](img)
     elif key == "q":
         cv2.destroyWindow(name)
     elif key == "x":
         sys.exit()
     elif key == "s":
         cv2.imwrite("out.png", img)
     elif key in ["+", "="]:
```

### Comparing `deepdoctection-0.25/deepdoctection.egg-info/PKG-INFO` & `deepdoctection-0.26/deepdoctection.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepdoctection
-Version: 0.25
+Version: 0.26
 Summary: Repository for Document AI
 Home-page: https://github.com/deepdoctection/deepdoctection
 Author: Dr. Janis Meyer
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -52,21 +52,25 @@
  - OCR with support of [**Tesseract**](https://github.com/tesseract-ocr/tesseract), [**DocTr**](https://github.com/mindee/doctr)
    (Tensorflow and PyTorch implementations available) and a wrapper to an API for a commercial solution, 
  - Text mining for native PDFs with  [**pdfplumber**](https://github.com/jsvine/pdfplumber), 
  - Language detection with [**fastText**](https://github.com/facebookresearch/fastText),
  - Deskewing and rotating images with [**jdeskew**](https://github.com/phamquiluan/jdeskew). 
  - Document and token classification with all LayoutLM models provided by the Transformer library. 
    (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!).
-   Table detection and table structure recognition with 
-   [**table-transformer**](https://github.com/microsoft/table-transformer). You can try a pipeline using 
-   [**this script**](https://github.com/deepdoctection/deepdoctection/discussions/116).  
- - [**new!**] There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE)
+ - Table detection and table structure recognition with 
+   [**table-transformer**](https://github.com/microsoft/table-transformer). 
+ - There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE)
    and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v2_on_custom_token_classification.ipynb) 
    to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3.
-   
+ - Comprehensive configuration of **analyzer** like choosing different models, output parsing, OCR selection.
+   Check this [notebook](https://github.com/deepdoctection/notebooks/blob/main/Analyzer_Configuration.ipynb) or the 
+   [docs](https://deepdoctection.readthedocs.io/en/latest/tutorials/analyzer_configuration_notebook/) for more infos.
+ - [**new**] Document layout analysis and table recognition now runs with Torchscript (CPU) as well and Detectron2 is 
+   not required anymore for basic inference. 
+
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself. 
      
 Have a look at the [**introduction notebook**](https://github.com/deepdoctection/notebooks/blob/main/Get_Started.ipynb) in the 
 [notebook repo](https://github.com/deepdoctection/notebooks) for an easy start.
 
@@ -125,15 +129,15 @@
 HTML(page.tables[0].html)
 ```
 
 ![table](./docs/tutorials/_imgs/dd_rm_table.png)
 
 
 ```
-print(page.get_text())
+print(page.text)
 ```
 
 ![table](./docs/tutorials/_imgs/dd_rm_text.png)
  
 
 ## Documentation
 
@@ -149,33 +153,58 @@
 ![requirements](./docs/tutorials/_imgs/requirements_deepdoctection.png)
 
 Everything in the overview listed below the **deep**doctection layer are necessary requirements and have to be installed 
 separately. 
 
 - Linux or macOS. (Windows is not supported but there is a [Dockerfile](./docker/pytorch-cpu-jupyter/Dockerfile) available)
 - Python >= 3.8
-- PyTorch >= 1.8 **or** Tensorflow >= 2.9 and CUDA. If you want to run the models provided by Tensorpack a GPU is
+- 1.8 <= PyTorch < 2.0 **or** Tensorflow >= 2.9 and CUDA. If you want to run the models provided by Tensorpack a GPU is
   required. You can run on PyTorch with a CPU only.
 - **deep**doctection uses Python wrappers for [Poppler](https://poppler.freedesktop.org/) to convert PDF documents into 
 images. 
 - With respect to the Deep Learning framework, you must decide between [Tensorflow](https://www.tensorflow.org/install?hl=en)
   and [PyTorch](https://pytorch.org/get-started/locally/).
 - [Tesseract](https://github.com/tesseract-ocr/tesseract) OCR engine will be used through a Python wrapper. The core 
   engine has to be installed separately.
 
+The following overview shows the availability of the models in conjunction with the DL framework.
+
+| Task                                          | PyTorch | Torchscript    |  Tensorflow  |
+|-----------------------------------------------|:-------:|----------------|:------------:|
+| Layout detection via Detectron2/Tensorpack    |    ✅    | ✅ (CPU only)   | ✅ (GPU only) |
+| Table recognition via Detectron2/Tensorpack   |    ✅    | ✅ (CPU only)   | ✅ (GPU only) |
+| Table transformer via Transformers            |    ✅    | ❌              |      ❌       |
+| DocTr                                         |    ✅    | ❌              |      ✅       |
+| LayoutLM (v1, v2, v3, XLM) via Transformers   |    ✅    | ❌              | ❌            |
+
 
 
 ## Installation
 
-We recommend using a virtual environment. You can install the package via pip or from source. Bug fixes or enhancements
-will be deployed to PyPi every 4 to 6 weeks.
+We recommend using a virtual environment. You can install the package via pip or from source. 
 
 ### Install with pip from PyPi
 
-Depending on which Deep Learning library you have available, use the following installation option:
+#### Minimal installation 
+
+If you want to get started with a minimal setting (e.g. running the **deep**doctection analyzer with 
+default configuration or trying the 'Get started notebook'), install **deep**doctection with
+
+```
+pip install deepdoctection
+```
+
+If you want to use the Tensorflow framework, please install Tensorpack separately. Detectron2 will not be installed 
+and layout models/ table recognition models will run with Torchscript on a CPU.
+
+#### Full installation
+
+The following installation will give you ALL models available within the Deep Learning framework as well as all models
+that are independent of Tensorflow/PyTorch. Please note, that the dependencies are very complex. We try hard to keep 
+the requirements up to date though.
 
 For **Tensorflow**, run
 
 ```
 pip install deepdoctection[tf]
 ```
 
@@ -230,15 +259,16 @@
 
 We thank all libraries that provide high quality code and pre-trained models. Without, it would have been impossible 
 to develop this framework.
 
 ## Problems
 
 We try hard to eliminate bugs. We also know that the code is not free of issues. We welcome all issues relevant to this
-repo and try to address them as quickly as possible.
+repo and try to address them as quickly as possible. Bug fixes or enhancements will be deployed in a new release every 4 
+to 6 weeks.
 
 ## If you like **deep**doctection ...
  
  ...you can easily support the project by making it more visible. Leaving a star or a recommendation will help. 
 
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deepdoctection-0.25/deepdoctection.egg-info/SOURCES.txt` & `deepdoctection-0.26/deepdoctection.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 deepdoctection/extern/hflayoutlm.py
 deepdoctection/extern/model.py
 deepdoctection/extern/pdftext.py
 deepdoctection/extern/tessocr.py
 deepdoctection/extern/texocr.py
 deepdoctection/extern/tpdetect.py
 deepdoctection/extern/pt/__init__.py
+deepdoctection/extern/pt/nms.py
 deepdoctection/extern/pt/ptutils.py
 deepdoctection/extern/tp/__init__.py
 deepdoctection/extern/tp/tfutils.py
 deepdoctection/extern/tp/tpcompat.py
 deepdoctection/extern/tp/tpfrcnn/__init__.py
 deepdoctection/extern/tp/tpfrcnn/common.py
 deepdoctection/extern/tp/tpfrcnn/predict.py
```

### Comparing `deepdoctection-0.25/deepdoctection.egg-info/requires.txt` & `deepdoctection-0.26/deepdoctection.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,155 +1,132 @@
-apted==1.0.3
 catalogue==2.0.7
-distance==0.1.3
 huggingface_hub>=0.12.0
 importlib-metadata>=4.11.2
 jsonlines==3.0.0
-lxml>=4.9.1
 mock==4.0.3
 networkx>=2.7.1
-numpy<1.24,>=1.21
+numpy>=1.21
 opencv-python==4.5.4.60
-packaging<22.0,>=20.0
-pycocotools>=2.0.2
-pypdf2<2.10.1,>=1.27.5
+packaging>=20.0
+pypdf2
 pyyaml==6.0
 pyzmq>=16
-rapidfuzz<3.0,>=1.6.0
 termcolor>=1.1
 tabulate>=0.7.7
 tqdm==4.64.0
+
+[dev]
+click
+black==23.7.0
+isort
+pylint==2.17.4
+mypy==1.4.1
+wandb
 types-PyYAML
 types-termcolor==1.1.3
 types-tabulate
 types-tqdm
 lxml-stubs
 
-[dev]
-click==8.0.4
-black==22.3.0
-isort
-pylint==2.13.4
-mypy==0.942
-wandb
-
 [docs]
 tensorpack
 boto3
 transformers
 pdfplumber>=0.7.1
 lxml>=4.9.1
 lxml-stubs
-pycocotools>=2.0.2
 jdeskew
 jinja2==3.0.3
 mkdocs-material
 mkdocstrings-python
 griffe==0.25.0
 
 [hf]
-apted==1.0.3
 catalogue==2.0.7
-distance==0.1.3
 huggingface_hub>=0.12.0
 importlib-metadata>=4.11.2
 jsonlines==3.0.0
-lxml>=4.9.1
 mock==4.0.3
 networkx>=2.7.1
-numpy<1.24,>=1.21
+numpy>=1.21
 opencv-python==4.5.4.60
-packaging<22.0,>=20.0
-pycocotools>=2.0.2
-pypdf2<2.10.1,>=1.27.5
+packaging>=20.0
+pypdf2
 pyyaml==6.0
 pyzmq>=16
-rapidfuzz<3.0,>=1.6.0
 termcolor>=1.1
 tabulate>=0.7.7
 tqdm==4.64.0
-types-PyYAML
-types-termcolor==1.1.3
-types-tabulate
-types-tqdm
-lxml-stubs
 timm
 transformers
 python-doctr==0.6.0
+rapidfuzz<3.0,>=1.6.0
 boto3
 pdfplumber>=0.7.1
 fasttext
 jdeskew
+apted==1.0.3
+distance==0.1.3
+lxml>=4.9.1
 
 [pt]
-apted==1.0.3
 catalogue==2.0.7
-distance==0.1.3
 huggingface_hub>=0.12.0
 importlib-metadata>=4.11.2
 jsonlines==3.0.0
-lxml>=4.9.1
 mock==4.0.3
 networkx>=2.7.1
-numpy<1.24,>=1.21
+numpy>=1.21
 opencv-python==4.5.4.60
-packaging<22.0,>=20.0
-pycocotools>=2.0.2
-pypdf2<2.10.1,>=1.27.5
+packaging>=20.0
+pypdf2
 pyyaml==6.0
 pyzmq>=16
-rapidfuzz<3.0,>=1.6.0
 termcolor>=1.1
 tabulate>=0.7.7
 tqdm==4.64.0
-types-PyYAML
-types-termcolor==1.1.3
-types-tabulate
-types-tqdm
-lxml-stubs
 timm
 transformers
 python-doctr==0.6.0
+rapidfuzz<3.0,>=1.6.0
 boto3
 pdfplumber>=0.7.1
 fasttext
 jdeskew
+apted==1.0.3
+distance==0.1.3
+lxml>=4.9.1
 
 [test]
 pytest
 pytest-cov
 
 [tf]
-apted==1.0.3
 catalogue==2.0.7
-distance==0.1.3
 huggingface_hub>=0.12.0
 importlib-metadata>=4.11.2
 jsonlines==3.0.0
-lxml>=4.9.1
 mock==4.0.3
 networkx>=2.7.1
-numpy<1.24,>=1.21
+numpy>=1.21
 opencv-python==4.5.4.60
-packaging<22.0,>=20.0
-pycocotools>=2.0.2
-pypdf2<2.10.1,>=1.27.5
+packaging>=20.0
+pypdf2
 pyyaml==6.0
 pyzmq>=16
-rapidfuzz<3.0,>=1.6.0
 termcolor>=1.1
 tabulate>=0.7.7
 tqdm==4.64.0
-types-PyYAML
-types-termcolor==1.1.3
-types-tabulate
-types-tqdm
-lxml-stubs
 tensorpack
 protobuf==3.20.1
 tensorflow-addons>=0.17.1
 tf2onnx>=1.9.2
 python-doctr==0.6.0
+rapidfuzz<3.0,>=1.6.0
+pycocotools>=2.0.2
 boto3
 pdfplumber>=0.7.1
 fasttext
 jdeskew
+apted==1.0.3
+distance==0.1.3
+lxml>=4.9.1
```

### Comparing `deepdoctection-0.25/setup.cfg` & `deepdoctection-0.26/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -14,28 +14,27 @@
 	W0401, # wildcard-import
 	W0614, # unused-wildcard-import
 	R0401, # cyclic import
 	W0511, # fixme
 	E1120, # no-value-for-parameter (because it does not work properly with the ubiquitous curry decorator
 	E1205, # logging-too-many-args
 extension-pkg-whitelist = cv2
-load-plugins = pylint_strict_informational
 
 [pylint.TYPECHECK]
 generated-members = torch.*
 ignored-modules = torch, transformers, detectron2, boto3
 
 [pylint.FORMAT]
 max-module-lines = 2500
 max-line-length = 120
 good-names = x,y,k,n,dp,df,el,ex,cx,cy,w,h,l,i,rs,cs,p6,H1,H2,H3,B1,B2,B3,B1_proposal,B2_proposal,GroupNorm,c2,c3,c4,c5,G,q
 
 [pylint.DESIGN]
 max-args = 16
-max-branches = 27
+max-branches = 33
 max-attributes = 18
 max-locals = 44
 max-returns = 8
 max-statements = 100
 max-public-methods = 30
 min-public-methods = 1
 max-nested-blocks = 8
```

### Comparing `deepdoctection-0.25/setup.py` & `deepdoctection-0.26/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,19 @@
     "distance==0.1.3",
     "huggingface_hub>=0.12.0",
     "importlib-metadata>=4.11.2",
     "jsonlines==3.0.0",
     "lxml>=4.9.1",
     "mock==4.0.3",
     "networkx>=2.7.1",
-    "numpy>=1.21,<1.24",
+    "numpy>=1.21",
     "opencv-python==4.5.4.60",
-    "packaging>=20.0,<22.0",
+    "packaging>=20.0",
     "pycocotools>=2.0.2",
-    "pypdf2>=1.27.5,<2.10.1",
+    "pypdf2",
     "python-prctl",
     "pyyaml==6.0",
     "pyzmq>=16",
     "rapidfuzz>=1.6.0,<3.0",  # we need this requirement for Doctr as long they have not fixed #1186 for v.0.6.0
     "termcolor>=1.1",
     "tabulate>=0.7.7",
     "tqdm==4.64.0",
@@ -80,19 +80,19 @@
     "boto3",
     "pdfplumber>=0.7.1",
     "tensorflow-addons>=0.17.1",
     "tf2onnx>=1.9.2",
     "python-doctr==0.6.0",
     "fasttext",
     # dev dependencies
-    "click==8.0.4",  # version will not break black
-    "black==22.3.0",
+    "click",  # version will not break black
+    "black==23.7.0",
     "isort",
-    "pylint==2.13.4",
-    "mypy==0.942",
+    "pylint==2.17.4",
+    "mypy==1.4.1",
     # docs
     "jinja2==3.0.3",
     "mkdocs-material",
     "mkdocstrings-python",
     "griffe==0.25.0",
     # test
     "pytest",
@@ -108,50 +108,50 @@
 
 def deps_list(*pkgs: str):
     return [deps[pkg] for pkg in pkgs]
 
 
 # pypi dependencies without considering DL models specific dependencies
 dist_deps = deps_list(
-    "apted",
     "catalogue",
-    "distance",
     "huggingface_hub",
     "importlib-metadata",
     "jsonlines",
-    "lxml",
     "mock",
     "networkx",
     "numpy",
     "opencv-python",
     "packaging",
-    "pycocotools",
     "pypdf2",
     "pyyaml",
     "pyzmq",
-    "rapidfuzz",
     "termcolor",
     "tabulate",
     "tqdm",
-    "types-PyYAML",
-    "types-termcolor",
-    "types-tabulate",
-    "types-tqdm",
-    "lxml-stubs",
 )
 
 
 # remaining dependencies to use models that neither require TF nor PyTorch
-additional_deps = deps_list("boto3", "pdfplumber", "fasttext", "jdeskew")
+additional_deps = deps_list(
+    "boto3",
+    "pdfplumber",
+    "fasttext",
+    "jdeskew",
+    "apted",
+    "distance",
+    "lxml",
+)
 
-# Tensorflow dependencies
-tf_deps = deps_list("tensorpack", "protobuf", "tensorflow-addons", "tf2onnx", "python-doctr")
+# Tensorflow dependencies. We also add pycocotools as they wouldn't have been added otherwise
+tf_deps = deps_list(
+    "tensorpack", "protobuf", "tensorflow-addons", "tf2onnx", "python-doctr", "rapidfuzz", "pycocotools"
+)
 
 # PyTorch dependencies
-pt_deps = deps_list("timm", "transformers", "python-doctr")
+pt_deps = deps_list("timm", "transformers", "python-doctr", "rapidfuzz")
 source_pt_deps = pt_deps + deps_list("detectron2 @ git+https://github.com/facebookresearch/detectron2.git")
 
 # Putting all together
 tf_deps = dist_deps + tf_deps + additional_deps
 pt_deps = dist_deps + pt_deps + additional_deps
 source_pt_deps = dist_deps + source_pt_deps + additional_deps
 
@@ -163,28 +163,39 @@
 docs_deps = deps_list(
     "tensorpack",
     "boto3",
     "transformers",
     "pdfplumber",
     "lxml",
     "lxml-stubs",
-    "pycocotools",
     "jdeskew",
     "jinja2",
     "mkdocs-material",
     "mkdocstrings-python",
     "griffe",
 )
 
 
 # test dependencies
 test_deps = deps_list("pytest", "pytest-cov")
 
 # dev dependencies
-dev_deps = deps_list("click", "black", "isort", "pylint", "mypy", "wandb")
+dev_deps = deps_list(
+    "click",
+    "black",
+    "isort",
+    "pylint",
+    "mypy",
+    "wandb",
+    "types-PyYAML",
+    "types-termcolor",
+    "types-tabulate",
+    "types-tqdm",
+    "lxml-stubs",
+)
 
 # TODO: add function that lists correct not pre-installed third party libs in package, such that requirement errors
 #  can be printed with correct version dependencies.
 # when uploading to pypi first comment all source extra dependencies so that there are no dependencies to dataflow
 
 EXTRA_DEPS = {
     "tf": tf_deps,
```

### Comparing `deepdoctection-0.25/tests/__init__.py` & `deepdoctection-0.26/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/analyzer/__init__.py` & `deepdoctection-0.26/tests/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/conftest.py` & `deepdoctection-0.26/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     TestType,
     get_layoutlm_features,
     get_layoutlm_input,
     get_sequence_class_result,
     get_token_class_result,
 )
 from .mapper.data import DatapointImage
+from .test_utils import get_test_path
 
 
 def get_image_results() -> DatapointImage:
     """
     DatapointImage
     """
     return DatapointImage()
@@ -76,23 +77,23 @@
 
 
 @fixture(name="path_to_tp_frcnn_yaml")
 def fixture_path_to_tp_frcnn_yaml() -> Path:
     """
     path to tp frcnn yaml file
     """
-    return get_package_path() / "configs/tp/layout/conf_frcnn_layout.yaml"
+    return get_test_path() / "configs/tp/conf_frcnn_layout.yaml"
 
 
 @fixture(name="path_to_d2_frcnn_yaml")
 def fixture_path_to_d2_frcnn_yaml() -> Path:
     """
     path to d2 frcnn yaml file
     """
-    return get_package_path() / "configs/d2/layout/CASCADE_RCNN_R_50_FPN_GN.yaml"
+    return get_test_path() / "configs/d2/CASCADE_RCNN_R_50_FPN_GN.yaml"
 
 
 @fixture(name="categories")
 def fixture_categories() -> Dict[str, str]:
     """
     Categories as Dict
     """
@@ -250,17 +251,17 @@
 @fixture(name="col_sub_cats")
 def fixture_col_sub_cats() -> List[CategoryAnnotation]:
     """fixture col_sub_cats"""
     return deepcopy(Annotations().get_col_sub_cats())
 
 
 @fixture(name="cell_sub_cats")
-def fixture_cell_sub_cats() -> List[
-    Tuple[CategoryAnnotation, CategoryAnnotation, CategoryAnnotation, CategoryAnnotation]
-]:
+def fixture_cell_sub_cats() -> (
+    List[Tuple[CategoryAnnotation, CategoryAnnotation, CategoryAnnotation, CategoryAnnotation]]
+):
     """fixture cell_sub_cats"""
     return deepcopy(Annotations().get_cell_sub_cats())
 
 
 @fixture(name="word_layout_annotations_for_ordering")
 def fixture_word_layout_annotations_for_ordering() -> List[ImageAnnotation]:
     """fixture word_layout_annotations_for_ordering"""
@@ -335,25 +336,25 @@
         cell.dump_sub_category(CellType.row_span, sub_cats[2])
         cell.dump_sub_category(CellType.column_span, sub_cats[3])
 
     return deepcopy(dp)
 
 
 @fixture(name="cell_sub_cats_when_table_fully_tiled")
-def fixture_cell_sub_cats_when_table_fully_tiled() -> List[
-    Tuple[CategoryAnnotation, CategoryAnnotation, CategoryAnnotation, CategoryAnnotation]
-]:
+def fixture_cell_sub_cats_when_table_fully_tiled() -> (
+    List[Tuple[CategoryAnnotation, CategoryAnnotation, CategoryAnnotation, CategoryAnnotation]]
+):
     """fixture cell_sub_cats_when_table_fully_tiled"""
     return deepcopy(Annotations().get_cell_sub_cats_when_table_fully_tiled())
 
 
 @fixture(name="summary_sub_cats_when_table_fully_tiled")
-def fixture_summary_sub_cats_when_table_fully_tiled() -> Tuple[
-    CategoryAnnotation, CategoryAnnotation, CategoryAnnotation, CategoryAnnotation
-]:
+def fixture_summary_sub_cats_when_table_fully_tiled() -> (
+    Tuple[CategoryAnnotation, CategoryAnnotation, CategoryAnnotation, CategoryAnnotation]
+):
     """fixture summary_sub_cats_when_table_fully_tiled"""
     return deepcopy(Annotations().get_summary_sub_cats_when_table_fully_tiled())
 
 
 @fixture(name="summary_htab_sub_cat")
 def fixture_summary_htab_sub_cat() -> ContainerAnnotation:
     """fixture summary_htab_sub_cat"""
```

### Comparing `deepdoctection-0.25/tests/data.py` & `deepdoctection-0.26/tests/data.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/dataflow/__init__.py` & `deepdoctection-0.26/tests/dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/dataflow/conftest.py` & `deepdoctection-0.26/tests/dataflow/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/dataflow/test_common.py` & `deepdoctection-0.26/tests/dataflow/test_common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/dataflow/test_custom.py` & `deepdoctection-0.26/tests/dataflow/test_custom.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/dataflow/test_custom_serialize.py` & `deepdoctection-0.26/tests/dataflow/test_custom_serialize.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/dataflow/test_parallel_map.py` & `deepdoctection-0.26/tests/dataflow/test_parallel_map.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/dataflow/test_stats.py` & `deepdoctection-0.26/tests/dataflow/test_stats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datapoint/__init__.py` & `deepdoctection-0.26/tests/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datapoint/conftest.py` & `deepdoctection-0.26/tests/datapoint/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datapoint/test_annotation.py` & `deepdoctection-0.26/tests/datapoint/test_annotation.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datapoint/test_box.py` & `deepdoctection-0.26/tests/datapoint/test_box.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datapoint/test_convert.py` & `deepdoctection-0.26/tests/datapoint/test_convert.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datapoint/test_image.py` & `deepdoctection-0.26/tests/datapoint/test_image.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datapoint/test_view.py` & `deepdoctection-0.26/tests/datapoint/test_view.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datasets/__init__.py` & `deepdoctection-0.26/tests/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datasets/instances/__init__.py` & `deepdoctection-0.26/tests/datasets/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datasets/instances/conftest.py` & `deepdoctection-0.26/tests/datasets/instances/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datasets/instances/test_doclaynet.py` & `deepdoctection-0.26/tests/datasets/instances/test_doclaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datasets/instances/test_fintabnet.py` & `deepdoctection-0.26/tests/datasets/instances/test_fintabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datasets/instances/test_funsd.py` & `deepdoctection-0.26/tests/datasets/instances/test_funsd.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datasets/instances/test_iiitar13k.py` & `deepdoctection-0.26/tests/datasets/instances/test_iiitar13k.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from pytest import mark
 
 from deepdoctection.datasets import IIITar13K
 
 from ...test_utils import collect_datapoint_from_dataflow, get_test_path
 
 
-@mark.basic
+@mark.additional
 def test_dataset_iiitar13k_returns_image() -> None:
     """
     test dataset iiitar13k returns image
     """
 
     # Arrange
     iiitar13k = IIITar13K()
```

### Comparing `deepdoctection-0.25/tests/datasets/instances/test_layouttest.py` & `deepdoctection-0.26/tests/datasets/instances/test_layouttest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datasets/instances/test_publaynet.py` & `deepdoctection-0.26/tests/datasets/instances/test_publaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datasets/instances/test_pubtables1m.py` & `deepdoctection-0.26/tests/datasets/instances/test_pubtables1m.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from pytest import mark
 
 from deepdoctection.datasets import Pubtables1MDet, Pubtables1MStruct
 
 from ...test_utils import collect_datapoint_from_dataflow, get_test_path
 
 
-@mark.basic
+@mark.additional
 def test_dataset_pubtables1m_det_returns_image() -> None:
     """
     test dataset pubtables1m_det return image
     """
 
     # Arrange
     pubtables = Pubtables1MDet()
@@ -41,15 +41,15 @@
     df = pubtables.dataflow.build()
 
     # Act
     df_list = collect_datapoint_from_dataflow(df)
     assert len(df_list) == 1
 
 
-@mark.basic
+@mark.additional
 def test_dataset_pubtables1m_struct_returns_image() -> None:
     """
     test dataset pubtables1m_struct return image
     """
 
     def get_pubtab1m_struct_test_path() -> Path:
         test_path = get_test_path() / "pubtable1m_struct"
```

### Comparing `deepdoctection-0.25/tests/datasets/instances/test_pubtabnet.py` & `deepdoctection-0.26/tests/datasets/instances/test_pubtabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datasets/instances/test_rvlcdip.py` & `deepdoctection-0.26/tests/datasets/instances/test_rvlcdip.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datasets/test_adapter.py` & `deepdoctection-0.26/tests/datasets/test_adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from ..test_utils import collect_datapoint_from_dataflow, get_test_path
 
 if pytorch_available() and detectron2_available():
     from deepdoctection.datasets.adapter import DatasetAdapter
     from deepdoctection.mapper.d2struct import image_to_d2_frcnn_training
 
 
-@mark.requires_pt
+@mark.pt_deps  # pt_deps because we need Detectron2 here
 @patch("deepdoctection.mapper.tpstruct.os.path.isfile", MagicMock(return_value=True))
 def test_adapter_with_cached_dataset() -> None:
     """
     test DatasetAdapter wraps a dd dataset into a torch dataset and yields datapoints correctly when the whole dataset
     is cached
     """
 
@@ -51,15 +51,15 @@
 
     # Act & Assert
     dataset_iter = iter(adapter)
     df_list = collect_datapoint_from_dataflow(dataset_iter, max_datapoints=4)
     assert len(df_list) == 4
 
 
-@mark.requires_pt
+@mark.pt_deps  # pt_deps because we need Detectron2 here
 @patch("deepdoctection.mapper.tpstruct.os.path.isfile", MagicMock(return_value=True))
 def test_adapter_with_uncached_dataset() -> None:
     """
     test DatasetAdapter wraps a dd dataset into a torch dataset and yields datapoints correctly when the dataset
     is not cached
     """
```

### Comparing `deepdoctection-0.25/tests/datasets/test_info.py` & `deepdoctection-0.26/tests/datasets/test_info.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/datasets/test_registry.py` & `deepdoctection-0.26/tests/datasets/test_registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/eval/__init__.py` & `deepdoctection-0.26/tests/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/eval/conftest.py` & `deepdoctection-0.26/tests/eval/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/eval/test_accmetric.py` & `deepdoctection-0.26/tests/eval/test_accmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/eval/test_cocometric.py` & `deepdoctection-0.26/tests/eval/test_cocometric.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         """
 
         dp_list = [get_image_results().image]
         self.dataflow_gt = DataFromList(dp_list)
         self.dataflow_pr = DataFromList(dp_list)
         self.categories = get_image_results().get_dataset_categories()
 
-    @mark.basic
+    @mark.additional
     def test_coco_metric_returns_correct_distance(self) -> None:
         """
         when testing datapoint against itself, evaluation returns full score except when some areas do not exist
         """
 
         self.setup()
 
@@ -61,15 +61,15 @@
             output_list.append(res["val"])
         output = np.asarray(output_list)  # type: ignore
 
         expected_output = np.asarray([1, 1, 1, 1, -1, -1, 1, 1, 1, 1, -1, -1])
 
         assert_allclose(output, expected_output, atol=1e-10)  # type: ignore
 
-    @mark.basic
+    @mark.additional
     def test_when_params_change_coco_metric_returns_correct_distance(self) -> None:
         """
         when parameters are changed then coco metric return correct distance
         """
 
         self.setup()
 
@@ -91,15 +91,15 @@
         expected_output = np.asarray([-1, 1, 1, -1, 1, -1, 1, 1, 1, -1, 1, -1])
 
         assert_allclose(output, expected_output, atol=1e-10)  # type: ignore
 
         # Clean-up
         CocoMetric._params = {}  # pylint: disable=W0212
 
-    @mark.basic
+    @mark.additional
     def test_when_f1_score_coco_metric_returns_correct_distance(self) -> None:
         """
         when f1_score = True is set then coco metric returns correct distance
         """
         self.setup()
 
         # Arrange
```

### Comparing `deepdoctection-0.25/tests/eval/test_eval.py` & `deepdoctection-0.26/tests/eval/test_eval.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,16 +69,15 @@
         )
         self._pipe_component = ImageLayoutService(self._layout_detector)
         self._pipe_component.predictor.predict = MagicMock(return_value=detection_results)  # type: ignore
         self._metric = CocoMetric
 
         self.evaluator = Evaluator(self._dataset, self._pipe_component, self._metric, 1)
 
-    @mark.requires_tf
-    @mark.full
+    @mark.tf_deps
     def test_evaluator_runs_and_returns_distance(self, setup_method) -> None:  #  type: ignore  # pylint: disable=W0613
         """
         Testing evaluator runs and returns metric distance
         """
 
         # Act
         out = self.evaluator.run()
```

### Comparing `deepdoctection-0.25/tests/eval/test_registry.py` & `deepdoctection-0.26/tests/eval/test_registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/eval/test_tedsmetric.py` & `deepdoctection-0.26/tests/eval/test_tedsmetric.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from deepdoctection.utils.file_utils import apted_available
 
 if apted_available():
     from deepdoctection.eval.tedsmetric import teds_metric
 
 
-@mark.basic
+@mark.additional
 def test_teds_metric_returns_correct_distance() -> None:
     """
     teds returns score of 1.0 when comparing identical html strings
     """
 
     html_str = "<table><tr><td></td><td></td><td></td></tr><tr><td></td><td></td><td></td></tr></table>"
     results, number_results = teds_metric([html_str], [html_str], False)
```

### Comparing `deepdoctection-0.25/tests/extern/conftest.py` & `deepdoctection-0.26/tests/extern/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/extern/data.py` & `deepdoctection-0.26/tests/extern/data.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/extern/test_deskew.py` & `deepdoctection-0.26/tests/extern/test_deskew.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 class TestJdeskewer:
     """
     Test Jdeskewer
     """
 
     @staticmethod
-    @mark.requires_tf_or_pt
+    @mark.additional
     def test_deskewer_transforms_image() -> None:
         """
         Detector deskews image and rotates it accordingly
         """
 
         # Arrange
         test_path_input_image = get_test_path() / "skewed_input.png"
```

### Comparing `deepdoctection-0.25/tests/extern/test_doctrocr.py` & `deepdoctection-0.26/tests/extern/test_doctrocr.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     """
     return Annotations().get_word_detect_results()
 
 
 def get_mock_text_line_results(  # type: ignore
     inputs: List[Tuple[str, ImageType]], predictor, device  # pylint: disable=W0613
 ) -> List[DetectionResult]:
-
     """
     Returns two DetectionResult
     """
 
     return [
         DetectionResult(score=0.1, text="Foo", uuid="cf234ec9-52cf-4710-94ce-288f0e055091"),
         DetectionResult(score=0.4, text="Bak", uuid="cf234ec9-52cf-4710-94ce-288f0e055092"),
@@ -55,15 +54,15 @@
 
 class TestDoctrTextlineDetector:
     """
     Test DoctrTextlineDetector
     """
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch("deepdoctection.extern.doctrocr.doctr_predict_text_lines", MagicMock(side_effect=get_mock_word_results))
     def test_pt_doctr_detector_predicts_image(np_image: ImageType) -> None:
         """
         Detector calls doctr_predict_text_lines. Only runs in pt environment
         """
 
         # Arrange
@@ -76,15 +75,15 @@
         # Act
         results = doctr.predict(np_image)
 
         # Assert
         assert len(results) == 2
 
     @staticmethod
-    @mark.requires_tf
+    @mark.tf_deps
     @patch("deepdoctection.extern.doctrocr.doctr_predict_text_lines", MagicMock(side_effect=get_mock_word_results))
     def test_tf_doctr_detector_predicts_image(np_image: ImageType) -> None:
         """
         Detector calls doctr_predict_text_lines. Only runs in tf environment
         """
 
         # Arrange
@@ -103,15 +102,15 @@
 
 class TestDoctrTextRecognizer:
     """
     Test DoctrTextRecognizer
     """
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch("deepdoctection.extern.doctrocr.doctr_predict_text", MagicMock(side_effect=get_mock_text_line_results))
     def test_doctr_pt_recognizer_predicts_text(text_lines: List[Tuple[str, ImageType]]) -> None:
         """
         Detector calls doctr_predict_text. Only runs in pt environment
         """
 
         # Arrange
@@ -123,15 +122,15 @@
         # Act
         results = doctr.predict(text_lines)
 
         # Assert
         assert len(results) == 2
 
     @staticmethod
-    @mark.requires_tf
+    @mark.tf_deps
     @patch("deepdoctection.extern.doctrocr.doctr_predict_text", MagicMock(side_effect=get_mock_text_line_results))
     def test_doctr_tf_recognizer_predicts_text(text_lines: List[Tuple[str, ImageType]]) -> None:
         """
         Detector calls doctr_predict_text. Only runs in tf environment
         """
 
         # Arrange
```

### Comparing `deepdoctection-0.25/tests/extern/test_fastlang.py` & `deepdoctection-0.26/tests/extern/test_fastlang.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 class TestFasttextLangDetector:
     """
     Test FasttextLangDetector
     """
 
     @staticmethod
-    @mark.requires_tf_or_pt
+    @mark.additional
     @patch("deepdoctection.extern.fastlang.load_model", MagicMock(return_value=MagicMock()))
     def test_fasttext_lang_detector_predicts_language() -> None:
         """
         Detector calls model.predict(text_string) and processes returned results correctly
         """
 
         # Arrange
```

### Comparing `deepdoctection-0.25/tests/extern/test_hfdetr.py` & `deepdoctection-0.26/tests/extern/test_hfdetr.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
 class TestHFDetrDerivedDetector:
     """
     Test HFDetrDerivedDetector
     """
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch("deepdoctection.extern.hfdetr.HFDetrDerivedDetector.set_model", MagicMock(return_value=MagicMock()))
     @patch("deepdoctection.extern.hfdetr.HFDetrDerivedDetector.set_pre_processor", MagicMock())
     @patch("deepdoctection.extern.hfdetr.PretrainedConfig.from_pretrained", MagicMock())
     def test_hf_detr_predicts_image(detr_categories: Dict[str, ObjectTypes], np_image: ImageType) -> None:
         """
         D2 FRCNN calls predict_image and post processes DetectionResult correctly, e.g. adding class names
         """
```

### Comparing `deepdoctection-0.25/tests/extern/test_hflayoutlm.py` & `deepdoctection-0.26/tests/extern/test_hflayoutlm.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 class TestHFLayoutLmTokenClassifier:
     """
     Test HFLayoutLmTokenClassifier
     """
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch(
         "deepdoctection.extern.hflayoutlm.get_pytorch_requirement", MagicMock(return_value=("torch", False, "DUMMY"))
     )
     @patch("deepdoctection.extern.hflayoutlm.PretrainedConfig.from_pretrained", MagicMock())
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMForTokenClassification.from_pretrained", MagicMock())
     def test_hf_layout_lm_does_not_build_when_pt_not_available() -> None:
         """
@@ -89,15 +89,15 @@
         """
 
         # Arrange, Act & Assert
         with raises(ImportError):
             HFLayoutLmTokenClassifier("path/to/json", "path/to/model", ["foo"], ["B", "I", "O"])
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch("deepdoctection.extern.hflayoutlm.PretrainedConfig.from_pretrained", MagicMock())
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMForTokenClassification.from_pretrained", MagicMock())
     def test_categories_are_constructed_properly() -> None:
         """
         HFLayoutLmTokenClassifier creates a full category set depending on semantics, tagging or by passing the
         set of categories directly
         """
@@ -122,15 +122,15 @@
         # Act
         model = HFLayoutLmTokenClassifier("path/to/json", "path/to/model", categories=categories_explicit)
 
         # Assert
         assert model.categories == categories_explicit
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMForTokenClassification.from_pretrained", MagicMock())
     @patch("deepdoctection.extern.hflayoutlm.PretrainedConfig.from_pretrained", MagicMock())
     @patch("deepdoctection.extern.hflayoutlm.predict_token_classes", MagicMock(side_effect=get_token_class_results))
     def test_hf_layout_lm_predicts_token(
         layoutlm_input_for_predictor: JsonDict,
         categories_semantics: List[str],
         categories_bio: List[str],
@@ -169,15 +169,15 @@
 
 class TestHFLayoutLmv2TokenClassifier:
     """
     Test HFLayoutLmv2TokenClassifier
     """
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch(
         "deepdoctection.extern.hflayoutlm.get_pytorch_requirement", MagicMock(return_value=("torch", False, "DUMMY"))
     )
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv2Config.from_pretrained", MagicMock())
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv2ForTokenClassification.from_pretrained", MagicMock())
     def test_hf_layout_lm_does_not_build_when_pt_not_available() -> None:
         """
@@ -185,15 +185,15 @@
         """
 
         # Arrange, Act & Assert
         with raises(ImportError):
             HFLayoutLmv2TokenClassifier("path/to/json", "path/to/model", ["foo"], ["B", "I", "O"])
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv2Config.from_pretrained", MagicMock())
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv2ForTokenClassification.from_pretrained", MagicMock())
     def test_categories_are_constructed_properly() -> None:
         """
         HFLayoutLmv2TokenClassifier creates a full category set depending on semantics, tagging or by passing the
         set of categories directly
         """
@@ -218,15 +218,15 @@
         # Act
         model = HFLayoutLmv2TokenClassifier("path/to/json", "path/to/model", categories=categories_explicit)
 
         # Assert
         assert model.categories == categories_explicit
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv2ForTokenClassification.from_pretrained", MagicMock())
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv2Config.from_pretrained", MagicMock())
     @patch("deepdoctection.extern.hflayoutlm.predict_token_classes", MagicMock(side_effect=get_token_class_results))
     def test_hf_layout_lm_predicts_token(
         layoutlm_v2_input: JsonDict,
         categories_semantics: List[str],
         categories_bio: List[str],
@@ -266,15 +266,15 @@
 
 class TestHFLayoutLmv3TokenClassifier:
     """
     Test HFLayoutLmv3TokenClassifier
     """
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch(
         "deepdoctection.extern.hflayoutlm.get_pytorch_requirement", MagicMock(return_value=("torch", False, "DUMMY"))
     )
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv3Config.from_pretrained", MagicMock())
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv3ForTokenClassification.from_pretrained", MagicMock())
     def test_hf_layout_lm_does_not_build_when_pt_not_available() -> None:
         """
@@ -282,15 +282,15 @@
         """
 
         # Arrange, Act & Assert
         with raises(ImportError):
             HFLayoutLmv3TokenClassifier("path/to/json", "path/to/model", ["foo"], ["B", "I", "O"])
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv3Config.from_pretrained", MagicMock())
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv3ForTokenClassification.from_pretrained", MagicMock())
     def test_categories_are_constructed_properly() -> None:
         """
         HFLayoutLmv3TokenClassifier creates a full category set depending on semantics, tagging or by passing the
         set of categories directly
         """
@@ -315,15 +315,15 @@
         # Act
         model = HFLayoutLmv3TokenClassifier("path/to/json", "path/to/model", categories=categories_explicit)
 
         # Assert
         assert model.categories == categories_explicit
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv3ForTokenClassification.from_pretrained", MagicMock())
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv3Config.from_pretrained", MagicMock())
     @patch("deepdoctection.extern.hflayoutlm.predict_token_classes", MagicMock(side_effect=get_token_class_results))
     def test_hf_layout_lm_predicts_token(
         layoutlm_v2_input: JsonDict,
         categories_semantics: List[str],
         categories_bio: List[str],
@@ -363,15 +363,15 @@
 
 class TestHFLayoutLmSequenceClassifier:
     """
     Test HFLayoutLmSequenceClassifier
     """
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMForSequenceClassification.from_pretrained", MagicMock())
     @patch("deepdoctection.extern.hflayoutlm.PretrainedConfig.from_pretrained", MagicMock())
     @patch(
         "deepdoctection.extern.hflayoutlm.predict_sequence_classes", MagicMock(side_effect=get_sequence_class_result)
     )
     def test_hf_layout_lm_predicts_sequence_class(
         layoutlm_input_for_predictor: JsonDict,
@@ -406,15 +406,15 @@
 
 class TestHFLayoutLmv2SequenceClassifier:
     """
     Test HFLayoutLmv2SequenceClassifier
     """
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv2ForSequenceClassification.from_pretrained", MagicMock())
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv2Config.from_pretrained", MagicMock())
     @patch(
         "deepdoctection.extern.hflayoutlm.predict_sequence_classes", MagicMock(side_effect=get_sequence_class_result)
     )
     def test_hf_layout_lm_v2_predicts_sequence_class(
         layoutlm_v2_input: JsonDict,
@@ -450,15 +450,15 @@
 
 class TestHFLayoutLmv3SequenceClassifier:
     """
     Test HFLayoutLmv3SequenceClassifier
     """
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv3ForSequenceClassification.from_pretrained", MagicMock())
     @patch("deepdoctection.extern.hflayoutlm.LayoutLMv3Config.from_pretrained", MagicMock())
     @patch(
         "deepdoctection.extern.hflayoutlm.predict_sequence_classes", MagicMock(side_effect=get_sequence_class_result)
     )
     def test_hf_layout_lm_v3_predicts_sequence_class(
         layoutlm_v2_input: JsonDict,
```

### Comparing `deepdoctection-0.25/tests/extern/test_pdftext.py` & `deepdoctection-0.26/tests/extern/test_pdftext.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 class TestPdfPlumberTextDetector:
     """
     Test PdfPlumberTextDetector
     """
 
     @staticmethod
-    @mark.requires_tf_or_pt
+    @mark.additional
     def test_pdf_plumber_detector_predicts_image(pdf_bytes: bytes) -> None:
         """
         PdfPlumber returns words from pdf_bytes correctly
         """
 
         # Arrange
         pdf_text_predictor = PdfPlumberTextDetector()
@@ -43,15 +43,15 @@
 
         # Assert
         assert len(detect_results_list) == 109
         assert detect_results_list[0].text == "A"
         assert detect_results_list[1].text == "Simple"
 
     @staticmethod
-    @mark.requires_tf_or_pt
+    @mark.additional
     def test_pdf_plumber_detector_returns_width_height(pdf_bytes: bytes, pdf_bytes_page_2: bytes) -> None:
         """
         PdfPlumber returns pdf width and height correctly
         """
 
         # Arrange
         pdf_text_predictor = PdfPlumberTextDetector()
```

### Comparing `deepdoctection-0.25/tests/extern/test_tessocr.py` & `deepdoctection-0.26/tests/extern/test_tessocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/extern/test_texocr.py` & `deepdoctection-0.26/tests/extern/test_texocr.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,17 +29,16 @@
 
 class TestTextractOcrDetector:
     """
     Test TextractOcrDetector
     """
 
     @staticmethod
-    @mark.requires_pt_or_tf
-    @patch("deepdoctection.extern.texocr.get_aws_requirement", MagicMock(return_value=("boto3", True, "")))
-    @patch("deepdoctection.extern.texocr.get_boto3_requirement", MagicMock(return_value=("aws", True, "")))
+    @mark.additional
+    @patch("deepdoctection.extern.texocr.get_boto3_requirement", MagicMock(return_value=("boto3", True, "")))
     @patch("deepdoctection.extern.texocr.boto3", MagicMock())
     def test_textract_ocr_predicts_image(np_image: ImageType, textract_response: JsonDict) -> None:
         """
         Detector calls predict_text and returns only detected word blocks
         """
 
         # Arrange
```

### Comparing `deepdoctection-0.25/tests/extern/test_tpdetect.py` & `deepdoctection-0.26/tests/extern/test_tpdetect.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,41 +67,41 @@
 
 class TestTPFrcnnDetector:
     """
     Test TPFrcnnDetector constructor
     """
 
     @staticmethod
-    @mark.requires_tf
+    @mark.tf_deps
     @patch("deepdoctection.extern.tp.tpcompat.get_num_gpu", MagicMock(side_effect=set_num_gpu_to_zero))
     def test_tp_frcnn_does_not_build_when_no_gpu(
         path_to_tp_frcnn_yaml: str, categories: Dict[str, ObjectTypes]
     ) -> None:
         """
         TP FRCNN needs one GPU for predicting. Construction fails, when no GPU is found
         """
         # Arrange, Act & Assert
         with raises(AssertionError):
             TPFrcnnDetector(path_yaml=path_to_tp_frcnn_yaml, path_weights="", categories=categories)
 
     @staticmethod
-    @mark.requires_tf
+    @mark.tf_deps
     @patch("deepdoctection.extern.tp.tpcompat.get_num_gpu", MagicMock(side_effect=set_num_gpu_to_one))
     def test_tp_frcnn_returns_fpn_model(path_to_tp_frcnn_yaml: str, categories: Dict[str, ObjectTypes]) -> None:
         """
         TP FRCNN builds RestNetFPN model is construction is successful.
         """
         # Arrange, Act
         frcnn = TPFrcnnDetector(path_yaml=path_to_tp_frcnn_yaml, path_weights="", categories=categories)
 
         # Assert
         assert isinstance(frcnn._model, ResNetFPNModel)  # pylint: disable=W0212
 
     @staticmethod
-    @mark.requires_tf
+    @mark.tf_deps
     @patch("deepdoctection.extern.tp.tpcompat.get_num_gpu", MagicMock(side_effect=set_num_gpu_to_one))
     @patch("deepdoctection.extern.tp.tpcompat.TensorpackPredictor._build_config", MagicMock())
     @patch("deepdoctection.extern.tp.tpcompat.TensorpackPredictor.get_predictor", MagicMock())
     @patch("deepdoctection.extern.tpdetect.tp_predict_image", MagicMock(side_effect=get_mock_detection_results))
     def test_tp_frcnn_predicts_image(
         path_to_tp_frcnn_yaml: str, categories: Dict[str, ObjectTypes], np_image: ImageType
     ) -> None:
```

### Comparing `deepdoctection-0.25/tests/mapper/__init__.py` & `deepdoctection-0.26/tests/pipe/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# File: __init__.py
+# File: xxx.py
 
 # Copyright 2021 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `deepdoctection-0.25/tests/mapper/conftest.py` & `deepdoctection-0.26/tests/mapper/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/mapper/data.py` & `deepdoctection-0.26/tests/mapper/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -778,111 +778,127 @@
         """
         category_name or category_id
         """
         if as_index:
             return "1"
         return self.categories["1"]
 
-    def get_first_ann_sub_category_header_name(self) -> ObjectTypes:  # pylint: disable=R0201
+    @staticmethod
+    def get_first_ann_sub_category_header_name() -> ObjectTypes:
         """
         category_name of sub category
         """
         return CellType.body
 
     def get_last_ann_category_name(self) -> str:
         """
         category_name
         """
         return self.categories["1"]
 
-    def get_last_ann_sub_category_header_name(self) -> ObjectTypes:  # pylint: disable=R0201
+    @staticmethod
+    def get_last_ann_sub_category_header_name() -> ObjectTypes:
         """
         category_name of sub category
         """
         return CellType.header
 
-    def get_last_ann_sub_category_row_number_id(self) -> str:  # pylint: disable=R0201
+    @staticmethod
+    def get_last_ann_sub_category_row_number_id() -> str:
         """
         row number
         """
         return "1"
 
-    def get_last_ann_sub_category_col_number_id(self) -> str:  # pylint: disable=R0201
+    @staticmethod
+    def get_last_ann_sub_category_col_number_id() -> str:
         """
         col number
         """
         return "1"
 
-    def get_last_ann_sub_category_row_span_id(self) -> str:  # pylint: disable=R0201
+    @staticmethod
+    def get_last_ann_sub_category_row_span_id() -> str:
         """
         row span
         """
         return "1"
 
-    def get_last_ann_sub_category_col_span_id(self) -> str:  # pylint: disable=R0201
+    @staticmethod
+    def get_last_ann_sub_category_col_span_id() -> str:
         """
         col span
         """
         return "1"
 
-    def get_first_ann_sub_category_row_number_id(self) -> str:  # pylint: disable=R0201
+    @staticmethod
+    def get_first_ann_sub_category_row_number_id() -> str:
         """
         row number
         """
         return "14"
 
-    def get_first_ann_sub_category_col_number_id(self) -> str:  # pylint: disable=R0201
+    @staticmethod
+    def get_first_ann_sub_category_col_number_id() -> str:
         """
         col number
         """
         return "9"
 
-    def get_first_ann_sub_category_row_span_id(self) -> str:  # pylint: disable=R0201
+    @staticmethod
+    def get_first_ann_sub_category_row_span_id() -> str:
         """
         row span
         """
         return "1"
 
-    def get_first_ann_sub_category_col_span_id(self) -> str:  # pylint: disable=R0201
+    @staticmethod
+    def get_first_ann_sub_category_col_span_id() -> str:
         """
         col span
         """
         return "1"
 
-    def get_summary_ann_sub_category_rows_id(self) -> str:  # pylint: disable=R0201
+    @staticmethod
+    def get_summary_ann_sub_category_rows_id() -> str:
         """
         number rows
         """
         return "14"
 
-    def get_summary_ann_sub_category_col_id(self) -> str:  # pylint: disable=R0201
+    @staticmethod
+    def get_summary_ann_sub_category_col_id() -> str:
         """
         number cols
         """
         return "9"
 
-    def get_summary_ann_sub_category_row_span_id(self) -> str:  # pylint: disable=R0201
+    @staticmethod
+    def get_summary_ann_sub_category_row_span_id() -> str:
         """
         max row span
         """
         return "1"
 
-    def get_summary_ann_sub_category_col_span_id(self) -> str:  # pylint: disable=R0201
+    @staticmethod
+    def get_summary_ann_sub_category_col_span_id() -> str:
         """
         max col span
         """
         return "5"
 
-    def get_number_of_heads(self) -> int:  # pylint: disable=R0201
+    @staticmethod
+    def get_number_of_heads() -> int:
         """
         number of head cells
         """
         return 10
 
-    def get_number_of_bodies(self) -> int:  # pylint: disable=R0201
+    @staticmethod
+    def get_number_of_bodies() -> int:
         """
         number of body cells
         """
         return 108
 
     def get_html(self) -> str:
         """
```

### Comparing `deepdoctection-0.25/tests/mapper/test_cats.py` & `deepdoctection-0.26/tests/mapper/test_cats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/mapper/test_cocostruct.py` & `deepdoctection-0.26/tests/mapper/test_cocostruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/mapper/test_d2struct.py` & `deepdoctection-0.26/tests/mapper/test_d2struct.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 from .data import DatapointImage
 
 if detectron2_available():
     from deepdoctection.mapper.d2struct import image_to_d2_frcnn_training
 
 
-@mark.requires_pt
+@mark.pt_deps
 @patch("deepdoctection.mapper.d2struct.os.path.isfile", MagicMock(return_value=True))
 def test_image_to_d2_frcnn_training(datapoint_image: Image, image_results: DatapointImage) -> None:
     """
     testing image_to_d2_frcnn_training is mapping correctly
     """
 
     # Act
```

### Comparing `deepdoctection-0.25/tests/mapper/test_hfstruct.py` & `deepdoctection-0.26/tests/mapper/test_hfstruct.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from .data import DatapointImage
 
 if transformers_available():
     from deepdoctection.mapper.hfstruct import image_to_hf_detr_training
 
 
-@mark.requires_pt
+@mark.pt_deps
 @patch("deepdoctection.mapper.hfstruct.os.path.isfile", MagicMock(return_value=True))
 def test_image_to_hf_detr_training(datapoint_image: Image, image_results: DatapointImage) -> None:
     """
     testing image_to_hf_detr_training is mapping correctly
     """
 
     # Act
```

### Comparing `deepdoctection-0.25/tests/mapper/test_iiitar13k.py` & `deepdoctection-0.26/tests/mapper/test_iiitar13k.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 @patch("deepdoctection.mapper.pascalstruct.load_image_from_file", MagicMock())
 def test_pascal_voc_dict_to_image(
     datapoint_iiitar13kjson: JsonDict,
     iiitar13k_categories_name_as_keys: Dict[str, str],
     iiitar13k_category_names_mapping: Dict[str, str],
     iiitar13k_results: IIITar13KJson,
 ) -> None:
-
     """
     testing iiitar13k_to_image is mapping correctly
     """
 
     # Act
     iiitar13k_to_image_mapper = pascal_voc_dict_to_image(
         iiitar13k_categories_name_as_keys, False, False, False, iiitar13k_category_names_mapping
```

### Comparing `deepdoctection-0.25/tests/mapper/test_laylmstruct.py` & `deepdoctection-0.26/tests/mapper/test_laylmstruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     assert raw_features["ann_ids"] == raw_layoutlm_features["ann_ids"]
     assert raw_features["words"] == raw_layoutlm_features["words"]
     assert raw_features["bbox"] == raw_layoutlm_features["bbox"]
     assert raw_features["dataset_type"] == raw_layoutlm_features["dataset_type"]
     assert "labels" not in raw_features
 
 
-@mark.requires_pt
+@mark.pt_deps
 def test_raw_features_to_layoutlm_features(
     dp_image_with_layout_and_word_annotations: Image, layoutlm_features: JsonDict
 ) -> None:
     """
     testing image_to_layoutlm_features is mapping correctly
     """
```

### Comparing `deepdoctection-0.25/tests/mapper/test_misc.py` & `deepdoctection-0.26/tests/mapper/test_misc.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/mapper/test_prodigystruct.py` & `deepdoctection-0.26/tests/mapper/test_prodigystruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/mapper/test_pubstruct.py` & `deepdoctection-0.26/tests/mapper/test_pubstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/mapper/test_tpstruct.py` & `deepdoctection-0.26/tests/mapper/test_tpstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/mapper/test_utils.py` & `deepdoctection-0.26/tests/mapper/test_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/mapper/test_xfundstruct.py` & `deepdoctection-0.26/tests/mapper/test_xfundstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/pipe/__init__.py` & `deepdoctection-0.26/tests/train/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/pipe/test_anngen.py` & `deepdoctection-0.26/tests/pipe/test_anngen.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/pipe/test_cell.py` & `deepdoctection-0.26/tests/pipe/test_cell.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/pipe/test_common.py` & `deepdoctection-0.26/tests/pipe/test_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
         self._nms_pairs = [["row", "column"]]
         self._thresholds = [0.01]
         self._categories = ["row", "column"]
 
         self.nms_service = AnnotationNmsService(self._nms_pairs, self._thresholds)
 
-    @mark.requires_pt
+    @mark.pt_deps
     def test_integration_pipeline_component(self, dp_image_fully_segmented_unrelated_words: Image) -> None:
         """
         test annotation nms service suppresses the annotations within groups
         """
 
         dp = dp_image_fully_segmented_unrelated_words
```

### Comparing `deepdoctection-0.25/tests/pipe/test_language.py` & `deepdoctection-0.26/tests/pipe/test_language.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/pipe/test_layout.py` & `deepdoctection-0.26/tests/pipe/test_layout.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/pipe/test_lm.py` & `deepdoctection-0.26/tests/pipe/test_lm.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 class TestLMTokenClassifierService:
     """
     Test LMTokenClassifierService
     """
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     def test_pass_datapoint_2(
         dp_image_with_layout_and_word_annotations: Image,
         token_class_result: List[TokenClassResult],
     ) -> None:
         """
         Testing pass_datapoint with fast tokenizer
         """
@@ -86,15 +86,15 @@
 
 class TestLMSequenceClassifierService:
     """
     Test LMSequenceClassifierService
     """
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     def test_pass_datapoint(
         dp_image_with_layout_and_word_annotations: Image,
         sequence_class_result: SequenceClassResult,
     ) -> None:
         """
         Testing pass_datapoint
         """
```

### Comparing `deepdoctection-0.25/tests/pipe/test_order.py` & `deepdoctection-0.26/tests/pipe/test_order.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/pipe/test_refine.py` & `deepdoctection-0.26/tests/pipe/test_refine.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,16 +295,16 @@
         col_numbers = {cell.get_sub_category(CellType.column_number).category_id for cell in cells}
         row_spans = {cell.get_sub_category(CellType.row_span).category_id for cell in cells}
         col_spans = {cell.get_sub_category(CellType.column_span).category_id for cell in cells}
 
         assert len(cells) == 4
         assert row_numbers == {"1", "2"}
         assert col_numbers == {"1", "2"}
-        assert row_spans == {"1", "1", "1", "1"}
-        assert col_spans == {"1", "1", "1", "1"}
+        assert row_spans == {"1"}
+        assert col_spans == {"1"}
         assert summaries_table == ["2", "2", "1", "1"]
         assert isinstance(summary_html, ContainerAnnotation)
         assert summary_html.value == [
             "<table>",
             "<tr>",
             "<td>",
             "2c1458bf-6b21-327a-9632-21373da468bb",
```

### Comparing `deepdoctection-0.25/tests/pipe/test_registry.py` & `deepdoctection-0.26/tests/pipe/test_registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/pipe/test_segment.py` & `deepdoctection-0.26/tests/pipe/test_segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,14 +330,15 @@
             self._ioa_threshold_cols,
             self._tile_table_with_items,
             self._remove_iou_threshold_rows,
             self._remove_iou_threshold_cols,
             self.cell_class_id,
         )
 
+    @mark.basic
     def test_pass_datapoint(self, dp_image_tab_cell_item: Image) -> None:
         """test pass_datapoint"""
 
         # Arrange
         dp = dp_image_tab_cell_item
         cells = dp.get_annotation(category_names=LayoutType.cell)
         table = dp.get_annotation(category_names=LayoutType.table)[0]
```

### Comparing `deepdoctection-0.25/tests/pipe/test_text.py` & `deepdoctection-0.26/tests/pipe/test_text.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/pipe/test_transform.py` & `deepdoctection-0.26/tests/pipe/test_transform.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/test_utils.py` & `deepdoctection-0.26/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     :param df: A Dataflow
     :param max_datapoints: The maximum number of datapoints to yield from
     :return: A list of datapoints of df
     """
 
     output: List[Any] = []
     if hasattr(df, "reset_state"):
-        df.reset_state()  # type: ignore
+        df.reset_state()
 
     for idx, dp in enumerate(df):
         if max_datapoints is not None:
             if idx >= max_datapoints:
                 break
 
         output.append(dp)
```

### Comparing `deepdoctection-0.25/tests/train/__init__.py` & `deepdoctection-0.26/tests_d2/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # -*- coding: utf-8 -*-
-# File: xxx.py
+# File: __init__.py
 
 # Copyright 2021 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+"""
+Cannot place these tests under the general test folder as this will result in a python segmentation error
+"""
```

### Comparing `deepdoctection-0.25/tests/train/conftest.py` & `deepdoctection-0.26/tests/train/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/train/test_d2_frcnn_train.py` & `deepdoctection-0.26/tests/train/test_d2_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.25/tests/train/test_tp_frcnn_train.py` & `deepdoctection-0.26/tests/train/test_tp_frcnn_train.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from ..test_utils import collect_datapoint_from_dataflow, set_num_gpu_to_one
 
 if tf_available() and tensorpack_available():
     from deepdoctection.extern.tp.tpfrcnn.config.config import model_frcnn_config
     from deepdoctection.train.tp_frcnn_train import get_train_dataflow, train_faster_rcnn
 
 
-@mark.requires_tf
+@mark.tf_deps
 @patch("deepdoctection.mapper.tpstruct.os.path.isfile", MagicMock(return_value=True))
 @patch("deepdoctection.train.tp_frcnn_train.set_mp_spawn")
 def test_get_train_dataflow(
     set_mp_spawn: Any, test_dataset: DatasetBase, path_to_tp_frcnn_yaml: str  # pylint: disable=W0613
 ) -> None:
     """
     test get train dataflow
@@ -58,15 +58,15 @@
     dp = df_list[0]
     assert "image" in dp
     assert dp["image"].ndim == 3
     assert "gt_boxes" in dp
     assert "gt_labels" in dp
 
 
-@mark.requires_tf
+@mark.tf_deps
 @patch("deepdoctection.mapper.tpstruct.os.path.isfile", MagicMock(return_value=True))
 @patch("deepdoctection.extern.tp.tpcompat.get_num_gpu", MagicMock(side_effect=set_num_gpu_to_one))
 @patch("deepdoctection.extern.tp.tpfrcnn.config.config.get_num_gpu", MagicMock(side_effect=set_num_gpu_to_one))
 @patch("deepdoctection.train.tp_frcnn_train.ModelSaver")
 @patch("deepdoctection.train.tp_frcnn_train.PeriodicCallback")
 @patch("tensorpack.utils.logger.set_logger_dir")
 @patch("deepdoctection.train.tp_frcnn_train.launch_train_with_config")
```

### Comparing `deepdoctection-0.25/tests_d2/__init__.py` & `deepdoctection-0.26/deepdoctection/extern/pt/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,9 +12,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Cannot place these tests under the general test folder as this will result in a python segmentation error
+Init file for pytorch compatibility package
 """
+
+from .ptutils import *
+
+if pytorch_available():
+    from .nms import *
```

### Comparing `deepdoctection-0.25/tests_d2/conftest.py` & `deepdoctection-0.26/tests_d2/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,25 +22,25 @@
 from typing import Dict
 from pathlib import Path
 
 import numpy as np
 
 from pytest import fixture
 
-from deepdoctection.utils.systools import get_package_path
 from deepdoctection.utils.settings import LayoutType, ObjectTypes
 from deepdoctection.utils.detection_types import ImageType
 
+from tests.test_utils import get_test_path
 
 @fixture(name="path_to_d2_frcnn_yaml")
 def fixture_path_to_d2_frcnn_yaml() -> Path:
     """
     path to d2 frcnn yaml file
     """
-    return get_package_path() / "configs/d2/layout/CASCADE_RCNN_R_50_FPN_GN.yaml"
+    return get_test_path() / "configs/d2/CASCADE_RCNN_R_50_FPN_GN.yaml"
 
 
 @fixture(name="categories")
 def fixture_categories() -> Dict[str, ObjectTypes]:
     """
     Categories as Dict
     """
```

### Comparing `deepdoctection-0.25/tests_d2/test_d2detect.py` & `deepdoctection-0.26/tests_d2/test_d2detect.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
 from deepdoctection.utils.file_utils import pytorch_available, detectron2_available
 
 from deepdoctection.extern.d2detect import D2FrcnnDetector
 from deepdoctection.utils.detection_types import ImageType
 from deepdoctection.utils.settings import ObjectTypes
 
+
+
 if pytorch_available():
     import torch
 
 if detectron2_available():
     from detectron2.structures import Instances, Boxes
 
 
@@ -55,28 +57,28 @@
 
 class TestD2FrcnnDetector:
     """
     Test D2FrcnnDetector
     """
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch("deepdoctection.utils.file_utils.detectron2_available",MagicMock(return_value=False))
     def test_d2_does_not_build_when_d2_not_available(path_to_d2_frcnn_yaml: str,
                                                      categories: Dict[str,ObjectTypes]) -> None:
         """
         D2 FRCNN does only build when detectron2 is properly installed
         """
 
         # Arrange, Act & Assert
         with raises(ImportError):
             D2FrcnnDetector(path_yaml=path_to_d2_frcnn_yaml,path_weights="",categories=categories)
 
     @staticmethod
-    @mark.requires_pt
+    @mark.pt_deps
     @patch("deepdoctection.extern.d2detect.D2FrcnnDetector.set_model", MagicMock(return_value=MagicMock))
     @patch("deepdoctection.extern.d2detect.D2FrcnnDetector._instantiate_d2_predictor", MagicMock())
     def test_d2_frcnn_predicts_image(path_to_d2_frcnn_yaml: str, categories: Dict[str,ObjectTypes],
                                      np_image: ImageType)-> None:
         """
         D2 FRCNN calls predict_image and post processes DetectionResult correctly, e.g. adding class names
         """
```

