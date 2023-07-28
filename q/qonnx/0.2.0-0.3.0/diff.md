# Comparing `tmp/qonnx-0.2.0.tar.gz` & `tmp/qonnx-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qonnx-0.2.0.tar", last modified: Thu Feb 16 16:00:37 2023, max compression
+gzip compressed data, was "qonnx-0.3.0.tar", last modified: Fri Jul 28 22:20:35 2023, max compression
```

## Comparing `qonnx-0.2.0.tar` & `qonnx-0.3.0.tar`

### file list

```diff
@@ -1,198 +1,219 @@
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.096759 qonnx-0.2.0/
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.084759 qonnx-0.2.0/.github/
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.088759 qonnx-0.2.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     1492 2022-07-11 14:35:18.000000 qonnx-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      375 2022-07-11 14:35:18.000000 qonnx-0.2.0/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      984 2022-07-11 14:35:18.000000 qonnx-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.088759 qonnx-0.2.0/.github/workflows/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      288 2023-02-01 15:05:03.000000 qonnx-0.2.0/.github/workflows/docs.yml
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      580 2023-02-15 15:05:25.000000 qonnx-0.2.0/.github/workflows/pre-commit.yml
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      919 2023-02-16 15:22:12.000000 qonnx-0.2.0/.github/workflows/pypi-publish.yml
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      676 2023-02-15 15:05:25.000000 qonnx-0.2.0/.github/workflows/test.yml
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      949 2023-02-16 15:22:07.000000 qonnx-0.2.0/.github/workflows/testpypi-publish.yml
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2067 2023-02-15 15:05:25.000000 qonnx-0.2.0/.gitignore
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      287 2022-07-11 14:35:18.000000 qonnx-0.2.0/.isort.cfg
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      906 2023-02-15 15:05:25.000000 qonnx-0.2.0/.pre-commit-config.yaml
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      543 2023-02-15 17:45:14.000000 qonnx-0.2.0/.readthedocs.yaml
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      331 2023-02-15 16:57:27.000000 qonnx-0.2.0/AUTHORS.rst
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     1004 2023-02-15 15:05:25.000000 qonnx-0.2.0/CITATION.cff
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    11357 2022-07-11 14:35:18.000000 qonnx-0.2.0/LICENSE
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     8620 2023-02-16 16:00:37.096759 qonnx-0.2.0/PKG-INFO
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     8122 2023-02-16 14:20:57.000000 qonnx-0.2.0/README.md
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.088759 qonnx-0.2.0/docs/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     1153 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/Makefile
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.088759 qonnx-0.2.0/docs/_static/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)       18 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/_static/.gitignore
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.084759 qonnx-0.2.0/docs/_templates/
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.088759 qonnx-0.2.0/docs/_templates/apidoc/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      197 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/_templates/apidoc/module.rst_t
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     1079 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/_templates/apidoc/package.rst_t
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      229 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/_templates/apidoc/toc.rst_t
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)       41 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/authors.rst
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)       13 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/changelog.rst
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     9686 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/conf.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)       70 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/genindex.rst
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2618 2023-02-01 15:05:03.000000 qonnx-0.2.0/docs/index.rst
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)       63 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/license.rst
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     9207 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/overview.rst
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)   440130 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/qonnx-comparison.png
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.088759 qonnx-0.2.0/docs/qonnx-custom-ops/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     1856 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/qonnx-custom-ops/bipolar_quant_op.md
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     6195 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/qonnx-custom-ops/quant_op.md
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     3423 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/qonnx-custom-ops/trunc_op.md
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)       39 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/readme.rst
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      383 2023-02-01 15:05:03.000000 qonnx-0.2.0/docs/requirements.txt
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      777 2022-07-11 14:35:18.000000 qonnx-0.2.0/docs/tutorials.rst
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.088759 qonnx-0.2.0/notebooks/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    24026 2023-02-01 15:05:03.000000 qonnx-0.2.0/notebooks/0_how_to_work_with_onnx.ipynb
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     6670 2023-02-01 15:05:03.000000 qonnx-0.2.0/notebooks/1_custom_analysis_pass.ipynb
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    10754 2023-02-01 15:05:03.000000 qonnx-0.2.0/notebooks/2_custom_transformation_pass.ipynb
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    29044 2023-02-01 15:05:03.000000 qonnx-0.2.0/notebooks/3_custom_op.ipynb
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      403 2023-02-01 15:05:03.000000 qonnx-0.2.0/notebooks/README.md
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      311 2023-02-16 09:47:43.000000 qonnx-0.2.0/pyproject.toml
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     1678 2023-02-16 16:00:37.096759 qonnx-0.2.0/setup.cfg
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      772 2023-02-16 09:59:01.000000 qonnx-0.2.0/setup.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.084759 qonnx-0.2.0/src/
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.088759 qonnx-0.2.0/src/qonnx/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)        0 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/__init__.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.092759 qonnx-0.2.0/src/qonnx/analysis/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)        0 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/analysis/__init__.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     1831 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/analysis/base.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     9150 2022-12-12 09:14:09.000000 qonnx-0.2.0/src/qonnx/analysis/inference_cost.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4548 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/analysis/topology.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.092759 qonnx-0.2.0/src/qonnx/converters/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)       82 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/converters/__init__.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     9372 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/converters/keras.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.092759 qonnx-0.2.0/src/qonnx/converters/qkeras/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)        0 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/converters/qkeras/__init__.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     7626 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/converters/qkeras/onnx.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     5549 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/converters/qkeras/qlayers.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     3686 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/converters/qkeras/quantizers.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.092759 qonnx-0.2.0/src/qonnx/core/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)        0 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/core/__init__.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     1995 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/core/data_layout.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    10455 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/core/datatype.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2189 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/core/execute_custom_node.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    27095 2023-02-15 16:43:34.000000 qonnx-0.2.0/src/qonnx/core/modelwrapper.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     9864 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/core/onnx_exec.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.092759 qonnx-0.2.0/src/qonnx/custom_op/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)        0 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/custom_op/__init__.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     8732 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/custom_op/base.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.092759 qonnx-0.2.0/src/qonnx/custom_op/channels_last/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      322 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/custom_op/channels_last/__init__.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4844 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/custom_op/channels_last/base_wrapped_op.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4222 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/custom_op/channels_last/batch_normalization.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     6263 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/custom_op/channels_last/conv.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     5952 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/custom_op/channels_last/max_pool.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.092759 qonnx-0.2.0/src/qonnx/custom_op/general/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2539 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/custom_op/general/__init__.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     3895 2023-01-30 12:44:20.000000 qonnx-0.2.0/src/qonnx/custom_op/general/bipolar_quant.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2637 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/custom_op/general/debugmarker.py
--rwxrwxr-x   0 maltanar  (1000) maltanar  (1000)     4201 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/custom_op/general/genericpartition.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     9599 2023-02-01 15:05:03.000000 qonnx-0.2.0/src/qonnx/custom_op/general/im2col.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     5032 2023-02-01 15:05:03.000000 qonnx-0.2.0/src/qonnx/custom_op/general/maxpoolnhwc.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     7180 2023-01-30 12:44:43.000000 qonnx-0.2.0/src/qonnx/custom_op/general/multithreshold.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     9420 2023-02-01 15:05:03.000000 qonnx-0.2.0/src/qonnx/custom_op/general/quant.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     6078 2023-02-01 15:05:03.000000 qonnx-0.2.0/src/qonnx/custom_op/general/quantavgpool2d.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     3702 2023-01-30 12:43:08.000000 qonnx-0.2.0/src/qonnx/custom_op/general/trunc.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4904 2023-01-30 12:44:36.000000 qonnx-0.2.0/src/qonnx/custom_op/general/xnorpopcount.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2345 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/custom_op/registry.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.092759 qonnx-0.2.0/src/qonnx/data/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     1524 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/data/__init__.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.084759 qonnx-0.2.0/src/qonnx/data/onnx/
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.092759 qonnx-0.2.0/src/qonnx/data/onnx/mnist-conv/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)       86 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/data/onnx/mnist-conv/README.md
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    26454 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/data/onnx/mnist-conv/model.onnx
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.092759 qonnx-0.2.0/src/qonnx/data/onnx/mnist-conv/test_data_set_0/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     3149 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/data/onnx/mnist-conv/test_data_set_0/input_0.pb
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)       48 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/data/onnx/mnist-conv/test_data_set_0/output_0.pb
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.092759 qonnx-0.2.0/src/qonnx/transformation/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)        0 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/transformation/__init__.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     5238 2022-08-12 09:33:56.000000 qonnx-0.2.0/src/qonnx/transformation/base.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     5571 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/transformation/batchnorm_to_affine.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     7768 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/transformation/bipolar_to_xnor.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     9277 2022-08-12 09:14:08.000000 qonnx-0.2.0/src/qonnx/transformation/change_3d_tensors_to_4d.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     5079 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/transformation/change_datalayout.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    23422 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/transformation/channels_last.py
--rwxrwxr-x   0 maltanar  (1000) maltanar  (1000)     9268 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/transformation/create_generic_partitions.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2117 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/transformation/double_to_single_float.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4017 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/transformation/extend_partition.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     3702 2022-10-04 21:23:57.000000 qonnx-0.2.0/src/qonnx/transformation/extract_conv_bias.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4941 2023-02-15 15:05:21.000000 qonnx-0.2.0/src/qonnx/transformation/fold_constants.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     9545 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/transformation/gemm_to_matmul.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    12904 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/transformation/general.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     6072 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/transformation/infer_data_layouts.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     6165 2022-08-12 09:14:08.000000 qonnx-0.2.0/src/qonnx/transformation/infer_datatypes.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     3834 2022-08-12 09:14:08.000000 qonnx-0.2.0/src/qonnx/transformation/infer_shapes.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4163 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/transformation/insert_topk.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    11034 2022-09-28 08:42:49.000000 qonnx-0.2.0/src/qonnx/transformation/lower_convs_to_matmul.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4180 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/transformation/make_input_chanlast.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     6658 2023-02-01 15:05:03.000000 qonnx-0.2.0/src/qonnx/transformation/merge_onnx_models.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2593 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/transformation/quant_constant_folding.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     5932 2022-08-31 07:32:37.000000 qonnx-0.2.0/src/qonnx/transformation/rebalance_conv.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4069 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/transformation/remove.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.096759 qonnx-0.2.0/src/qonnx/util/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)        0 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/util/__init__.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    13500 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/util/basic.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2054 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/util/cleanup.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2311 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/util/config.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     1645 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/util/exec_qonnx.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4995 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/util/inference_cost.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     3085 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/util/onnx.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      247 2023-02-15 15:05:25.000000 qonnx-0.2.0/src/qonnx/util/random_reseed.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     1233 2022-07-11 14:35:18.000000 qonnx-0.2.0/src/qonnx/util/to_channels_last.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.088759 qonnx-0.2.0/src/qonnx.egg-info/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     8620 2023-02-16 16:00:37.000000 qonnx-0.2.0/src/qonnx.egg-info/PKG-INFO
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     5710 2023-02-16 16:00:37.000000 qonnx-0.2.0/src/qonnx.egg-info/SOURCES.txt
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)        1 2023-02-16 16:00:37.000000 qonnx-0.2.0/src/qonnx.egg-info/dependency_links.txt
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      284 2023-02-16 16:00:37.000000 qonnx-0.2.0/src/qonnx.egg-info/entry_points.txt
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)        1 2022-07-20 14:54:17.000000 qonnx-0.2.0/src/qonnx.egg-info/not-zip-safe
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      337 2023-02-16 16:00:37.000000 qonnx-0.2.0/src/qonnx.egg-info/requires.txt
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)        6 2023-02-16 16:00:37.000000 qonnx-0.2.0/src/qonnx.egg-info/top_level.txt
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.096759 qonnx-0.2.0/tests/
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.096759 qonnx-0.2.0/tests/analysis/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     3972 2023-02-01 15:05:03.000000 qonnx-0.2.0/tests/analysis/test_is_linear.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     6447 2023-02-01 15:05:03.000000 qonnx-0.2.0/tests/analysis/test_topology_checks.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)      282 2022-07-11 14:35:18.000000 qonnx-0.2.0/tests/conftest.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.096759 qonnx-0.2.0/tests/core/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4369 2023-02-01 15:05:03.000000 qonnx-0.2.0/tests/core/test_basic_onnx_exec.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     8237 2023-02-15 15:05:25.000000 qonnx-0.2.0/tests/core/test_custom_onnx_exec.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4620 2022-07-11 14:35:18.000000 qonnx-0.2.0/tests/core/test_datatypes.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     6007 2023-02-15 15:05:25.000000 qonnx-0.2.0/tests/core/test_mixed_onnx_exec.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     8824 2023-02-01 15:05:03.000000 qonnx-0.2.0/tests/core/test_modelwrapper.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.096759 qonnx-0.2.0/tests/custom_op/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     1981 2022-08-31 08:55:18.000000 qonnx-0.2.0/tests/custom_op/test_attr.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    43258 2023-02-01 15:05:03.000000 qonnx-0.2.0/tests/custom_op/test_im2col.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     9314 2023-02-15 15:05:25.000000 qonnx-0.2.0/tests/custom_op/test_multithreshold.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     3315 2023-02-01 15:05:03.000000 qonnx-0.2.0/tests/custom_op/test_xnorpopcountmatmul.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.096759 qonnx-0.2.0/tests/keras/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    26629 2023-02-16 10:19:05.000000 qonnx-0.2.0/tests/keras/test_keras_convert.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)       34 2022-07-11 14:35:18.000000 qonnx-0.2.0/tests/test_dummy.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.096759 qonnx-0.2.0/tests/transformation/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    12482 2023-02-01 15:05:03.000000 qonnx-0.2.0/tests/transformation/test_4d_conversion.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     5167 2023-02-01 15:05:03.000000 qonnx-0.2.0/tests/transformation/test_batchnorm_to_affine.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4973 2023-02-15 15:05:25.000000 qonnx-0.2.0/tests/transformation/test_change_datalayout.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    12537 2023-02-15 15:05:25.000000 qonnx-0.2.0/tests/transformation/test_channelslast.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    11713 2023-02-15 15:05:25.000000 qonnx-0.2.0/tests/transformation/test_conv_lowering.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)    10429 2023-02-01 15:05:03.000000 qonnx-0.2.0/tests/transformation/test_extend_partition.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     3110 2022-07-11 14:35:18.000000 qonnx-0.2.0/tests/transformation/test_fold_constants.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     8753 2023-02-15 16:43:34.000000 qonnx-0.2.0/tests/transformation/test_general_transformation.py
--rwxrwxr-x   0 maltanar  (1000) maltanar  (1000)     4695 2023-02-01 15:05:03.000000 qonnx-0.2.0/tests/transformation/test_generic_partitioning.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     3543 2023-02-15 15:05:25.000000 qonnx-0.2.0/tests/transformation/test_infer_data_layouts.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2875 2022-07-11 14:35:18.000000 qonnx-0.2.0/tests/transformation/test_infer_datatypes.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     3830 2022-07-11 14:35:18.000000 qonnx-0.2.0/tests/transformation/test_infer_shapes.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2221 2022-07-11 14:35:18.000000 qonnx-0.2.0/tests/transformation/test_make_input_chanlast.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     5845 2023-02-01 15:05:03.000000 qonnx-0.2.0/tests/transformation/test_merge_onnx_models.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2633 2023-01-30 12:43:56.000000 qonnx-0.2.0/tests/transformation/test_nodelocal_transform.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     1278 2022-07-11 14:35:18.000000 qonnx-0.2.0/tests/transformation/test_qonnx_cleanup.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4214 2022-08-31 07:32:37.000000 qonnx-0.2.0/tests/transformation/test_rebalance_conv.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     3788 2023-02-15 15:05:25.000000 qonnx-0.2.0/tests/transformation/test_remove_identity_ops.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4629 2022-07-11 14:35:18.000000 qonnx-0.2.0/tests/transformation/test_renaming.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4681 2023-02-01 15:05:03.000000 qonnx-0.2.0/tests/transformation/test_sort_graph.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2052 2023-02-01 15:05:03.000000 qonnx-0.2.0/tests/transformation/test_topk_insert.py
-drwxrwxr-x   0 maltanar  (1000) maltanar  (1000)        0 2023-02-16 16:00:37.096759 qonnx-0.2.0/tests/util/
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     4448 2022-07-11 14:35:18.000000 qonnx-0.2.0/tests/util/test_gen_finn_dt_tensor.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2606 2023-02-01 15:05:03.000000 qonnx-0.2.0/tests/util/test_matvec_range.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2588 2022-07-11 14:35:18.000000 qonnx-0.2.0/tests/util/test_padding.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     1927 2022-07-11 14:35:18.000000 qonnx-0.2.0/tests/util/test_shape_utils.py
--rw-rw-r--   0 maltanar  (1000) maltanar  (1000)     2010 2023-02-16 10:09:54.000000 qonnx-0.2.0/tox.ini
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.703931 qonnx-0.3.0/
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.558122 qonnx-0.3.0/.github/
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.580350 qonnx-0.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 yamanu     (501) staff       (20)     1492 2022-08-05 13:53:46.000000 qonnx-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 yamanu     (501) staff       (20)      375 2022-08-05 13:53:46.000000 qonnx-0.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 yamanu     (501) staff       (20)      984 2022-08-05 13:53:46.000000 qonnx-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.585500 qonnx-0.3.0/.github/workflows/
+-rw-r--r--   0 yamanu     (501) staff       (20)      288 2023-02-27 15:48:29.000000 qonnx-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 yamanu     (501) staff       (20)      580 2023-02-27 15:48:32.000000 qonnx-0.3.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 yamanu     (501) staff       (20)      919 2023-02-27 15:48:32.000000 qonnx-0.3.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 yamanu     (501) staff       (20)      684 2023-06-15 14:22:00.000000 qonnx-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0 yamanu     (501) staff       (20)      949 2023-02-27 15:48:32.000000 qonnx-0.3.0/.github/workflows/testpypi-publish.yml
+-rw-r--r--   0 yamanu     (501) staff       (20)     2067 2023-02-27 15:48:32.000000 qonnx-0.3.0/.gitignore
+-rw-r--r--   0 yamanu     (501) staff       (20)      287 2022-08-05 13:53:46.000000 qonnx-0.3.0/.isort.cfg
+-rw-r--r--   0 yamanu     (501) staff       (20)      906 2023-02-27 15:48:32.000000 qonnx-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 yamanu     (501) staff       (20)      543 2023-02-27 15:48:32.000000 qonnx-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 yamanu     (501) staff       (20)      331 2023-02-27 15:48:32.000000 qonnx-0.3.0/AUTHORS.rst
+-rw-r--r--   0 yamanu     (501) staff       (20)     1004 2023-02-27 15:48:32.000000 qonnx-0.3.0/CITATION.cff
+-rw-r--r--   0 yamanu     (501) staff       (20)    11357 2022-08-05 13:53:46.000000 qonnx-0.3.0/LICENSE
+-rw-r--r--   0 yamanu     (501) staff       (20)     9451 2023-07-28 22:20:35.704159 qonnx-0.3.0/PKG-INFO
+-rw-r--r--   0 yamanu     (501) staff       (20)     8955 2023-07-23 07:02:52.000000 qonnx-0.3.0/README.md
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.596884 qonnx-0.3.0/docs/
+-rw-r--r--   0 yamanu     (501) staff       (20)     1153 2022-08-05 13:53:46.000000 qonnx-0.3.0/docs/Makefile
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.597581 qonnx-0.3.0/docs/_static/
+-rw-r--r--   0 yamanu     (501) staff       (20)       18 2022-08-05 13:53:46.000000 qonnx-0.3.0/docs/_static/.gitignore
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.559690 qonnx-0.3.0/docs/_templates/
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.599299 qonnx-0.3.0/docs/_templates/apidoc/
+-rw-r--r--   0 yamanu     (501) staff       (20)      197 2022-08-05 13:53:46.000000 qonnx-0.3.0/docs/_templates/apidoc/module.rst_t
+-rw-r--r--   0 yamanu     (501) staff       (20)     1079 2022-08-05 13:53:46.000000 qonnx-0.3.0/docs/_templates/apidoc/package.rst_t
+-rw-r--r--   0 yamanu     (501) staff       (20)      229 2022-08-05 13:53:46.000000 qonnx-0.3.0/docs/_templates/apidoc/toc.rst_t
+-rw-r--r--   0 yamanu     (501) staff       (20)       41 2022-08-05 13:53:46.000000 qonnx-0.3.0/docs/authors.rst
+-rw-r--r--   0 yamanu     (501) staff       (20)       13 2022-08-05 13:53:46.000000 qonnx-0.3.0/docs/changelog.rst
+-rw-r--r--   0 yamanu     (501) staff       (20)     9686 2022-08-05 13:53:46.000000 qonnx-0.3.0/docs/conf.py
+-rw-r--r--   0 yamanu     (501) staff       (20)       70 2022-08-05 13:53:46.000000 qonnx-0.3.0/docs/genindex.rst
+-rw-r--r--   0 yamanu     (501) staff       (20)     2618 2023-02-27 15:48:29.000000 qonnx-0.3.0/docs/index.rst
+-rw-r--r--   0 yamanu     (501) staff       (20)       63 2022-08-05 13:53:46.000000 qonnx-0.3.0/docs/license.rst
+-rw-r--r--   0 yamanu     (501) staff       (20)     9207 2022-08-05 13:53:46.000000 qonnx-0.3.0/docs/overview.rst
+-rw-r--r--   0 yamanu     (501) staff       (20)   440130 2022-08-05 13:53:46.000000 qonnx-0.3.0/docs/qonnx-comparison.png
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.601315 qonnx-0.3.0/docs/qonnx-custom-ops/
+-rw-r--r--   0 yamanu     (501) staff       (20)     1856 2022-08-05 13:53:46.000000 qonnx-0.3.0/docs/qonnx-custom-ops/bipolar_quant_op.md
+-rw-r--r--   0 yamanu     (501) staff       (20)     6289 2023-07-23 07:02:52.000000 qonnx-0.3.0/docs/qonnx-custom-ops/quant_op.md
+-rw-r--r--   0 yamanu     (501) staff       (20)     3517 2023-07-23 07:02:52.000000 qonnx-0.3.0/docs/qonnx-custom-ops/trunc_op.md
+-rw-r--r--   0 yamanu     (501) staff       (20)       39 2022-08-05 13:53:46.000000 qonnx-0.3.0/docs/readme.rst
+-rw-r--r--   0 yamanu     (501) staff       (20)      383 2023-02-27 15:48:29.000000 qonnx-0.3.0/docs/requirements.txt
+-rw-r--r--   0 yamanu     (501) staff       (20)      777 2022-08-05 13:53:46.000000 qonnx-0.3.0/docs/tutorials.rst
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.605321 qonnx-0.3.0/notebooks/
+-rw-r--r--   0 yamanu     (501) staff       (20)    24026 2023-02-27 15:48:29.000000 qonnx-0.3.0/notebooks/0_how_to_work_with_onnx.ipynb
+-rw-r--r--   0 yamanu     (501) staff       (20)     6670 2023-02-27 15:48:29.000000 qonnx-0.3.0/notebooks/1_custom_analysis_pass.ipynb
+-rw-r--r--   0 yamanu     (501) staff       (20)    10754 2023-02-27 15:48:29.000000 qonnx-0.3.0/notebooks/2_custom_transformation_pass.ipynb
+-rw-r--r--   0 yamanu     (501) staff       (20)    29044 2023-02-27 15:48:29.000000 qonnx-0.3.0/notebooks/3_custom_op.ipynb
+-rw-r--r--   0 yamanu     (501) staff       (20)      403 2023-02-27 15:48:29.000000 qonnx-0.3.0/notebooks/README.md
+-rw-r--r--   0 yamanu     (501) staff       (20)      311 2022-08-05 13:53:46.000000 qonnx-0.3.0/pyproject.toml
+-rw-r--r--   0 yamanu     (501) staff       (20)     1850 2023-07-28 22:20:35.706189 qonnx-0.3.0/setup.cfg
+-rw-r--r--   0 yamanu     (501) staff       (20)      772 2023-02-27 15:48:32.000000 qonnx-0.3.0/setup.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.561563 qonnx-0.3.0/src/
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.605866 qonnx-0.3.0/src/qonnx/
+-rw-r--r--   0 yamanu     (501) staff       (20)        0 2023-02-27 15:48:32.000000 qonnx-0.3.0/src/qonnx/__init__.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.611560 qonnx-0.3.0/src/qonnx/analysis/
+-rw-r--r--   0 yamanu     (501) staff       (20)        0 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/analysis/__init__.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     1831 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/analysis/base.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     9150 2023-07-28 22:19:58.000000 qonnx-0.3.0/src/qonnx/analysis/inference_cost.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4548 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/analysis/topology.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.612790 qonnx-0.3.0/src/qonnx/converters/
+-rw-r--r--   0 yamanu     (501) staff       (20)       82 2023-02-27 15:48:32.000000 qonnx-0.3.0/src/qonnx/converters/__init__.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     9331 2023-05-12 09:16:32.000000 qonnx-0.3.0/src/qonnx/converters/keras.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.615428 qonnx-0.3.0/src/qonnx/converters/qkeras/
+-rw-r--r--   0 yamanu     (501) staff       (20)        0 2023-02-27 15:48:32.000000 qonnx-0.3.0/src/qonnx/converters/qkeras/__init__.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     7626 2023-02-27 15:48:32.000000 qonnx-0.3.0/src/qonnx/converters/qkeras/onnx.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     5549 2023-02-27 15:48:32.000000 qonnx-0.3.0/src/qonnx/converters/qkeras/qlayers.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     3686 2023-02-27 15:48:32.000000 qonnx-0.3.0/src/qonnx/converters/qkeras/quantizers.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.619320 qonnx-0.3.0/src/qonnx/core/
+-rw-r--r--   0 yamanu     (501) staff       (20)        0 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/core/__init__.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     1995 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/core/data_layout.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    11630 2023-05-03 16:10:56.000000 qonnx-0.3.0/src/qonnx/core/datatype.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2189 2023-02-27 15:48:32.000000 qonnx-0.3.0/src/qonnx/core/execute_custom_node.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    27467 2023-06-15 14:22:00.000000 qonnx-0.3.0/src/qonnx/core/modelwrapper.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    10302 2023-06-27 20:32:22.000000 qonnx-0.3.0/src/qonnx/core/onnx_exec.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.620966 qonnx-0.3.0/src/qonnx/custom_op/
+-rw-r--r--   0 yamanu     (501) staff       (20)        0 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/custom_op/__init__.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     8732 2023-02-27 15:48:32.000000 qonnx-0.3.0/src/qonnx/custom_op/base.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.624364 qonnx-0.3.0/src/qonnx/custom_op/channels_last/
+-rw-r--r--   0 yamanu     (501) staff       (20)      322 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/custom_op/channels_last/__init__.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4844 2023-02-27 15:48:32.000000 qonnx-0.3.0/src/qonnx/custom_op/channels_last/base_wrapped_op.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4222 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/custom_op/channels_last/batch_normalization.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     6263 2023-02-27 15:48:32.000000 qonnx-0.3.0/src/qonnx/custom_op/channels_last/conv.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     5952 2023-02-27 15:48:32.000000 qonnx-0.3.0/src/qonnx/custom_op/channels_last/max_pool.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.633234 qonnx-0.3.0/src/qonnx/custom_op/general/
+-rw-r--r--   0 yamanu     (501) staff       (20)     2539 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/custom_op/general/__init__.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     3895 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/custom_op/general/bipolar_quant.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2637 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/custom_op/general/debugmarker.py
+-rwxr-xr-x   0 yamanu     (501) staff       (20)     4201 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/custom_op/general/genericpartition.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     9599 2023-02-27 15:48:29.000000 qonnx-0.3.0/src/qonnx/custom_op/general/im2col.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     5215 2023-06-19 14:28:28.000000 qonnx-0.3.0/src/qonnx/custom_op/general/maxpoolnhwc.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     7180 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/custom_op/general/multithreshold.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    10762 2023-07-23 07:02:52.000000 qonnx-0.3.0/src/qonnx/custom_op/general/quant.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     6262 2023-06-19 14:28:28.000000 qonnx-0.3.0/src/qonnx/custom_op/general/quantavgpool2d.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     3702 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/custom_op/general/trunc.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4904 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/custom_op/general/xnorpopcount.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2539 2023-04-11 10:38:32.000000 qonnx-0.3.0/src/qonnx/custom_op/registry.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.633883 qonnx-0.3.0/src/qonnx/data/
+-rw-r--r--   0 yamanu     (501) staff       (20)     1524 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/data/__init__.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.565408 qonnx-0.3.0/src/qonnx/data/onnx/
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.634538 qonnx-0.3.0/src/qonnx/data/onnx/bsd300x3-espcn/
+-rw-r--r--   0 yamanu     (501) staff       (20)   273280 2023-05-12 09:16:32.000000 qonnx-0.3.0/src/qonnx/data/onnx/bsd300x3-espcn/model.onnx
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.637145 qonnx-0.3.0/src/qonnx/data/onnx/mnist-conv/
+-rw-r--r--   0 yamanu     (501) staff       (20)       86 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/data/onnx/mnist-conv/README.md
+-rw-r--r--   0 yamanu     (501) staff       (20)    26454 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/data/onnx/mnist-conv/model.onnx
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.638256 qonnx-0.3.0/src/qonnx/data/onnx/mnist-conv/test_data_set_0/
+-rw-r--r--   0 yamanu     (501) staff       (20)     3149 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/data/onnx/mnist-conv/test_data_set_0/input_0.pb
+-rw-r--r--   0 yamanu     (501) staff       (20)       48 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/data/onnx/mnist-conv/test_data_set_0/output_0.pb
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.655414 qonnx-0.3.0/src/qonnx/transformation/
+-rw-r--r--   0 yamanu     (501) staff       (20)        0 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/__init__.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     5238 2022-09-28 12:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/base.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     5571 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/batchnorm_to_affine.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     7768 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/bipolar_to_xnor.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     9277 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/change_3d_tensors_to_4d.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2966 2023-07-23 07:02:52.000000 qonnx-0.3.0/src/qonnx/transformation/change_batchsize.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     5079 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/change_datalayout.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    23422 2023-02-27 15:48:32.000000 qonnx-0.3.0/src/qonnx/transformation/channels_last.py
+-rwxr-xr-x   0 yamanu     (501) staff       (20)     9268 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/create_generic_partitions.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2117 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/double_to_single_float.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     3143 2023-07-23 07:02:52.000000 qonnx-0.3.0/src/qonnx/transformation/expose_intermediate.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4017 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/extend_partition.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     3702 2022-09-28 12:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/extract_conv_bias.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     5721 2023-07-23 07:02:52.000000 qonnx-0.3.0/src/qonnx/transformation/fold_constants.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     9545 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/gemm_to_matmul.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    14430 2023-07-23 07:02:52.000000 qonnx-0.3.0/src/qonnx/transformation/general.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     6072 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/infer_data_layouts.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     5904 2023-07-28 22:19:58.000000 qonnx-0.3.0/src/qonnx/transformation/infer_datatypes.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     3834 2023-07-18 11:14:19.000000 qonnx-0.3.0/src/qonnx/transformation/infer_shapes.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4163 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/insert_topk.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    11034 2022-09-28 12:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/lower_convs_to_matmul.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4180 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/make_input_chanlast.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     7218 2023-06-19 14:28:28.000000 qonnx-0.3.0/src/qonnx/transformation/merge_onnx_models.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    11035 2023-07-28 22:19:58.000000 qonnx-0.3.0/src/qonnx/transformation/pruning.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    10232 2023-07-23 07:02:52.000000 qonnx-0.3.0/src/qonnx/transformation/qcdq_to_qonnx.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     9384 2023-07-23 07:02:52.000000 qonnx-0.3.0/src/qonnx/transformation/qonnx_to_qcdq.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2593 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/quant_constant_folding.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     5932 2022-09-28 12:53:46.000000 qonnx-0.3.0/src/qonnx/transformation/rebalance_conv.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     5333 2023-07-23 07:02:52.000000 qonnx-0.3.0/src/qonnx/transformation/remove.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    10384 2023-05-12 09:16:32.000000 qonnx-0.3.0/src/qonnx/transformation/subpixel_to_deconv.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.662125 qonnx-0.3.0/src/qonnx/util/
+-rw-r--r--   0 yamanu     (501) staff       (20)        0 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/util/__init__.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    13552 2023-06-15 14:22:00.000000 qonnx-0.3.0/src/qonnx/util/basic.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2768 2023-07-28 22:19:58.000000 qonnx-0.3.0/src/qonnx/util/cleanup.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2311 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/util/config.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     3216 2023-07-23 07:02:52.000000 qonnx-0.3.0/src/qonnx/util/convert.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     8806 2023-07-23 07:02:52.000000 qonnx-0.3.0/src/qonnx/util/exec_qonnx.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     5099 2023-07-28 22:19:58.000000 qonnx-0.3.0/src/qonnx/util/inference_cost.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     3085 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/util/onnx.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2588 2023-07-28 22:19:58.000000 qonnx-0.3.0/src/qonnx/util/prune_stuck_channels.py
+-rw-r--r--   0 yamanu     (501) staff       (20)      247 2023-02-27 15:48:32.000000 qonnx-0.3.0/src/qonnx/util/random_reseed.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    14070 2023-07-28 22:19:58.000000 qonnx-0.3.0/src/qonnx/util/range_analysis.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     6310 2023-07-23 07:02:52.000000 qonnx-0.3.0/src/qonnx/util/test.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     1233 2022-08-05 13:53:46.000000 qonnx-0.3.0/src/qonnx/util/to_channels_last.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.609529 qonnx-0.3.0/src/qonnx.egg-info/
+-rw-r--r--   0 yamanu     (501) staff       (20)     9451 2023-07-28 22:20:35.000000 qonnx-0.3.0/src/qonnx.egg-info/PKG-INFO
+-rw-r--r--   0 yamanu     (501) staff       (20)     6522 2023-07-28 22:20:35.000000 qonnx-0.3.0/src/qonnx.egg-info/SOURCES.txt
+-rw-r--r--   0 yamanu     (501) staff       (20)        1 2023-07-28 22:20:35.000000 qonnx-0.3.0/src/qonnx.egg-info/dependency_links.txt
+-rw-r--r--   0 yamanu     (501) staff       (20)      437 2023-07-28 22:20:35.000000 qonnx-0.3.0/src/qonnx.egg-info/entry_points.txt
+-rw-r--r--   0 yamanu     (501) staff       (20)        1 2022-08-05 15:01:10.000000 qonnx-0.3.0/src/qonnx.egg-info/not-zip-safe
+-rw-r--r--   0 yamanu     (501) staff       (20)      351 2023-07-28 22:20:35.000000 qonnx-0.3.0/src/qonnx.egg-info/requires.txt
+-rw-r--r--   0 yamanu     (501) staff       (20)        6 2023-07-28 22:20:35.000000 qonnx-0.3.0/src/qonnx.egg-info/top_level.txt
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.663242 qonnx-0.3.0/tests/
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.666211 qonnx-0.3.0/tests/analysis/
+-rw-r--r--   0 yamanu     (501) staff       (20)     4858 2023-07-18 08:47:34.000000 qonnx-0.3.0/tests/analysis/test_inference_cost.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     3972 2023-02-27 15:48:29.000000 qonnx-0.3.0/tests/analysis/test_is_linear.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4415 2023-07-18 08:47:34.000000 qonnx-0.3.0/tests/analysis/test_range_analysis.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     6447 2023-02-27 15:48:29.000000 qonnx-0.3.0/tests/analysis/test_topology_checks.py
+-rw-r--r--   0 yamanu     (501) staff       (20)      282 2022-08-05 13:53:46.000000 qonnx-0.3.0/tests/conftest.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.668841 qonnx-0.3.0/tests/core/
+-rw-r--r--   0 yamanu     (501) staff       (20)     4369 2023-02-27 15:48:29.000000 qonnx-0.3.0/tests/core/test_basic_onnx_exec.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     8237 2023-02-27 15:48:32.000000 qonnx-0.3.0/tests/core/test_custom_onnx_exec.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4620 2022-08-05 13:53:46.000000 qonnx-0.3.0/tests/core/test_datatypes.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     6007 2023-02-27 15:48:32.000000 qonnx-0.3.0/tests/core/test_mixed_onnx_exec.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     8824 2023-02-27 15:48:29.000000 qonnx-0.3.0/tests/core/test_modelwrapper.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.671244 qonnx-0.3.0/tests/custom_op/
+-rw-r--r--   0 yamanu     (501) staff       (20)     1981 2022-09-28 12:53:46.000000 qonnx-0.3.0/tests/custom_op/test_attr.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    43258 2023-02-27 15:48:29.000000 qonnx-0.3.0/tests/custom_op/test_im2col.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     9314 2023-02-27 15:48:32.000000 qonnx-0.3.0/tests/custom_op/test_multithreshold.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     3315 2023-02-27 15:48:29.000000 qonnx-0.3.0/tests/custom_op/test_xnorpopcountmatmul.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.671685 qonnx-0.3.0/tests/keras/
+-rw-r--r--   0 yamanu     (501) staff       (20)    26655 2023-05-12 09:16:32.000000 qonnx-0.3.0/tests/keras/test_keras_convert.py
+-rw-r--r--   0 yamanu     (501) staff       (20)       34 2022-08-05 13:53:46.000000 qonnx-0.3.0/tests/test_dummy.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.696815 qonnx-0.3.0/tests/transformation/
+-rw-r--r--   0 yamanu     (501) staff       (20)    12482 2023-02-27 15:48:29.000000 qonnx-0.3.0/tests/transformation/test_4d_conversion.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     5189 2023-05-12 09:16:32.000000 qonnx-0.3.0/tests/transformation/test_batchnorm_to_affine.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2831 2023-07-23 07:02:52.000000 qonnx-0.3.0/tests/transformation/test_change_batchsize.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4973 2023-02-27 15:48:32.000000 qonnx-0.3.0/tests/transformation/test_change_datalayout.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    10810 2023-07-18 08:47:34.000000 qonnx-0.3.0/tests/transformation/test_channelslast.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    11713 2023-02-27 15:48:32.000000 qonnx-0.3.0/tests/transformation/test_conv_lowering.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2753 2023-07-23 07:02:52.000000 qonnx-0.3.0/tests/transformation/test_expose_intermediate.py
+-rw-r--r--   0 yamanu     (501) staff       (20)    10429 2023-02-27 15:48:29.000000 qonnx-0.3.0/tests/transformation/test_extend_partition.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     3110 2022-08-05 13:53:46.000000 qonnx-0.3.0/tests/transformation/test_fold_constants.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     8753 2023-02-27 15:48:32.000000 qonnx-0.3.0/tests/transformation/test_general_transformation.py
+-rwxr-xr-x   0 yamanu     (501) staff       (20)     4695 2023-02-27 15:48:29.000000 qonnx-0.3.0/tests/transformation/test_generic_partitioning.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     3543 2023-02-27 15:48:32.000000 qonnx-0.3.0/tests/transformation/test_infer_data_layouts.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4076 2023-06-15 14:22:01.000000 qonnx-0.3.0/tests/transformation/test_infer_datatypes.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     3830 2022-08-05 13:53:46.000000 qonnx-0.3.0/tests/transformation/test_infer_shapes.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2221 2022-08-05 13:53:46.000000 qonnx-0.3.0/tests/transformation/test_make_input_chanlast.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     6072 2023-06-19 14:28:28.000000 qonnx-0.3.0/tests/transformation/test_merge_onnx_models.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2633 2022-09-28 12:53:46.000000 qonnx-0.3.0/tests/transformation/test_nodelocal_transform.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     5502 2023-07-18 08:47:34.000000 qonnx-0.3.0/tests/transformation/test_pruning.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4378 2023-06-27 19:45:21.000000 qonnx-0.3.0/tests/transformation/test_qcdq_to_qonnx.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     1278 2022-08-05 13:53:46.000000 qonnx-0.3.0/tests/transformation/test_qonnx_cleanup.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4490 2023-07-23 07:02:52.000000 qonnx-0.3.0/tests/transformation/test_qonnx_to_qcdq.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4214 2022-09-28 12:53:46.000000 qonnx-0.3.0/tests/transformation/test_rebalance_conv.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     3788 2023-02-27 15:48:32.000000 qonnx-0.3.0/tests/transformation/test_remove_identity_ops.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2391 2023-07-23 07:02:52.000000 qonnx-0.3.0/tests/transformation/test_remove_unused.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4629 2022-08-05 13:53:46.000000 qonnx-0.3.0/tests/transformation/test_renaming.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     4681 2023-02-27 15:48:29.000000 qonnx-0.3.0/tests/transformation/test_sort_graph.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     5451 2023-05-12 09:16:32.000000 qonnx-0.3.0/tests/transformation/test_subpixel_to_deconv.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2052 2023-02-27 15:48:29.000000 qonnx-0.3.0/tests/transformation/test_topk_insert.py
+drwxr-xr-x   0 yamanu     (501) staff       (20)        0 2023-07-28 22:20:35.703268 qonnx-0.3.0/tests/util/
+-rw-r--r--   0 yamanu     (501) staff       (20)     4448 2022-08-05 13:53:46.000000 qonnx-0.3.0/tests/util/test_gen_finn_dt_tensor.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2606 2023-02-27 15:48:29.000000 qonnx-0.3.0/tests/util/test_matvec_range.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2588 2022-08-05 13:53:46.000000 qonnx-0.3.0/tests/util/test_padding.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     1927 2022-08-05 13:53:46.000000 qonnx-0.3.0/tests/util/test_shape_utils.py
+-rw-r--r--   0 yamanu     (501) staff       (20)     2010 2022-08-05 13:53:46.000000 qonnx-0.3.0/tox.ini
```

### Comparing `qonnx-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `qonnx-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `qonnx-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/.github/workflows/pre-commit.yml` & `qonnx-0.3.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/.github/workflows/pypi-publish.yml` & `qonnx-0.3.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/.github/workflows/test.yml` & `qonnx-0.3.0/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.8', '3.9']
+        python-version: ['3.8', '3.9', '3.10']
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `qonnx-0.2.0/.github/workflows/testpypi-publish.yml` & `qonnx-0.3.0/.github/workflows/testpypi-publish.yml`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/.gitignore` & `qonnx-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/.pre-commit-config.yaml` & `qonnx-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/.readthedocs.yaml` & `qonnx-0.3.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/CITATION.cff` & `qonnx-0.3.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/LICENSE` & `qonnx-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/PKG-INFO` & `qonnx-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,16 @@
-Metadata-Version: 2.1
-Name: qonnx
-Version: 0.2.0
-Summary: Frontend and utilities for QONNX
-Home-page: https://github.com/fastmachinelearning/qonnx
-License: Apache-2.0
-Project-URL: Documentation, https://pyscaffold.org/
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: notebooks
-Provides-Extra: qkeras
-Provides-Extra: testing
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 # QONNX: Arbitrary-Precision Quantized Neural Networks in ONNX
 
 [![ReadTheDocs](https://readthedocs.org/projects/qonnx/badge/?version=latest&style=plastic)](http://qonnx.readthedocs.io/)
 [![GitHub Discussions](https://img.shields.io/github/discussions/fastmachinelearning/qonnx)](https://github.com/fastmachinelearning/qonnx/discussions)
 ![Tests](https://github.com/fastmachinelearning/qonnx/actions/workflows/test.yml/badge.svg)
 ![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7622236.svg)](https://doi.org/10.5281/zenodo.7622236)
+[![PyPI version](https://badge.fury.io/py/qonnx.svg)](https://badge.fury.io/py/qonnx)
+[![Downloads](https://static.pepy.tech/personalized-badge/qonnx?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/qonnx)
 
 <img align="left" src="https://xilinx.github.io/finn/img/TFC_1W2A.onnx.png" alt="QONNX example" style="margin-right: 20px" width="200"/>
 
 
 QONNX (Quantized ONNX) introduces three new custom operators -- [`Quant`](docs/qonnx-custom-ops/quant_op.md), [`BipolarQuant`](docs/qonnx-custom-ops/bipolar_quant_op.md), and [`Trunc`](docs/qonnx-custom-ops/trunc_op.md) -- in order to represent arbitrary-precision uniform quantization in ONNX. This enables:
 * Representation of binary, ternary, 3-bit, 4-bit, 6-bit or any other quantization.
 * Quantization is an operator itself, and can be applied to any parameter or layer input.
@@ -87,51 +72,60 @@
 model = ModelWrapper("my-qonnx-model.onnx")
 idict = {"in0" : np.load("in0.npy), "in1" : np.load("in1.npy")}
 odict = execute_onnx(idict)
 ```
 
 ### Calculate inference cost for QONNX model
 
-Using the `qonnx-inference-cost` command line utility:
+Using the `qonnx-inference-cost` command line utility for the [CNV_2W2A example](https://github.com/fastmachinelearning/qonnx_model_zoo/tree/main/models/CIFAR10/Brevitas_FINN_CNV):
 
 `qonnx-inference-cost CNV_2W2A.onnx`
 
 Which will print a inference cost dictionary like the following:
 
 ```
 Inference cost for CNV_2W2A.onnx
 {
-  "discount_sparsity": true,    # discount MAC counts by layer sparsity (disregard zero-valued MACs)
+  "discount_sparsity": true,    # discount MAC counts by layer sparsity (disregard zero-valued MACs and params)
   # mem_o_X: number of layer outputs with datatype X
-  "mem_o_FLOAT32": 57600.0,     # number of FLOAT32 output elements
-  "mem_o_INT32": 85002.0,       # number of INT32 output elements
+  "mem_o_INT32": 142602.0,       # number of INT32 output elements
   # mem_o_X: number of layer parameters (weights) with datatype X
-  "mem_w_INT2": 1144512.0,      # number of INT2 parameters (weights)
+  "mem_w_INT2": 908033.0,      # number of INT2 parameters (weights)
   # op_mac_X_Y: number of MAC operations, datatype X by datatype Y
-  "op_mac_FLOAT32_INT2": 1555200.0, # number of float32 x int2 MACs
-  "op_mac_INT2_INT2": 57906176.0,   # number of int2 x int2 MACs
-  "total_bops": 331157504.0,        # total number of MACs normalized to bit-ops (BOPS)
+  # scaled integer datatypes have a tensor- or channelwise scale factor
+  "op_mac_SCALEDINT<8>_INT2": 1345500.0, # number of scaled int8 x int2 MACs
+  "op_mac_INT2_INT2": 35615771.0,   # number of int2 x int2 MACs
+  "total_bops": 163991084.0,        # total number of MACs normalized to bit-ops (BOPS)
   "total_mem_o_bits": 4563264.0,    # total number of bits for layer outputs
-  "total_mem_w_bits": 2289024.0,    # total number of bits for layer parameters
+  "total_mem_w_bits": 1816066.0,    # total number of bits for layer parameters
   "unsupported": "set()"
 }
 ```
 
 You can read more about the BOPS metric in [this paper](https://www.frontiersin.org/articles/10.3389/frai.2021.676564/full), Section 4.2 Bit Operations.
 
-### Development
+### Convert between different quantization representations
+
+Using the `qonnx-convert` command line utility you can convert from QONNX to QCDQ-style quantization:
+
+`qonnx-convert CNV_2W2A.onnx`
+
+This will convert `Quant` nodes to `QuantizeLinear -> Clip -> DequantizeLinear` nodes where possible.
+Please see the documentation of the `QuantToQCDQ` transformation to learn more about the limitations.
+
+## Development
 
 Install in editable mode in a venv:
 
 ```
 git clone https://github.com/fastmachinelearning/qonnx
 cd qonnx
 virtualenv -p python3.8 venv
 source venv/bin/activate
-pip install -e .[qkeras,testing]
+pip install -e .[qkeras,testing,docs]
 ```
 
 Run entire test suite, parallelized across CPU cores:
 ```
 pytest -n auto --verbose
 ```
 
@@ -181,9 +175,7 @@
   month        = {06},
   year         = 2022,
   publisher    = {Zenodo},
   doi          = {10.5281/zenodo.7622236},
   url          = {https://github.com/fastmachinelearning/qonnx}
 }
 ```
-
-
```

### Comparing `qonnx-0.2.0/README.md` & `qonnx-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,33 @@
+Metadata-Version: 2.1
+Name: qonnx
+Version: 0.3.0
+Summary: Frontend and utilities for QONNX
+Home-page: https://github.com/fastmachinelearning/qonnx
+License: Apache-2.0
+Project-URL: Documentation, https://pyscaffold.org/
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown; charset=UTF-8
+Provides-Extra: qkeras
+Provides-Extra: testing
+Provides-Extra: notebooks
+License-File: LICENSE
+License-File: AUTHORS.rst
+
 # QONNX: Arbitrary-Precision Quantized Neural Networks in ONNX
 
 [![ReadTheDocs](https://readthedocs.org/projects/qonnx/badge/?version=latest&style=plastic)](http://qonnx.readthedocs.io/)
 [![GitHub Discussions](https://img.shields.io/github/discussions/fastmachinelearning/qonnx)](https://github.com/fastmachinelearning/qonnx/discussions)
 ![Tests](https://github.com/fastmachinelearning/qonnx/actions/workflows/test.yml/badge.svg)
 ![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7622236.svg)](https://doi.org/10.5281/zenodo.7622236)
+[![PyPI version](https://badge.fury.io/py/qonnx.svg)](https://badge.fury.io/py/qonnx)
+[![Downloads](https://static.pepy.tech/personalized-badge/qonnx?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/qonnx)
 
 <img align="left" src="https://xilinx.github.io/finn/img/TFC_1W2A.onnx.png" alt="QONNX example" style="margin-right: 20px" width="200"/>
 
 
 QONNX (Quantized ONNX) introduces three new custom operators -- [`Quant`](docs/qonnx-custom-ops/quant_op.md), [`BipolarQuant`](docs/qonnx-custom-ops/bipolar_quant_op.md), and [`Trunc`](docs/qonnx-custom-ops/trunc_op.md) -- in order to represent arbitrary-precision uniform quantization in ONNX. This enables:
 * Representation of binary, ternary, 3-bit, 4-bit, 6-bit or any other quantization.
 * Quantization is an operator itself, and can be applied to any parameter or layer input.
@@ -70,51 +89,60 @@
 model = ModelWrapper("my-qonnx-model.onnx")
 idict = {"in0" : np.load("in0.npy), "in1" : np.load("in1.npy")}
 odict = execute_onnx(idict)
 ```
 
 ### Calculate inference cost for QONNX model
 
-Using the `qonnx-inference-cost` command line utility:
+Using the `qonnx-inference-cost` command line utility for the [CNV_2W2A example](https://github.com/fastmachinelearning/qonnx_model_zoo/tree/main/models/CIFAR10/Brevitas_FINN_CNV):
 
 `qonnx-inference-cost CNV_2W2A.onnx`
 
 Which will print a inference cost dictionary like the following:
 
 ```
 Inference cost for CNV_2W2A.onnx
 {
-  "discount_sparsity": true,    # discount MAC counts by layer sparsity (disregard zero-valued MACs)
+  "discount_sparsity": true,    # discount MAC counts by layer sparsity (disregard zero-valued MACs and params)
   # mem_o_X: number of layer outputs with datatype X
-  "mem_o_FLOAT32": 57600.0,     # number of FLOAT32 output elements
-  "mem_o_INT32": 85002.0,       # number of INT32 output elements
+  "mem_o_INT32": 142602.0,       # number of INT32 output elements
   # mem_o_X: number of layer parameters (weights) with datatype X
-  "mem_w_INT2": 1144512.0,      # number of INT2 parameters (weights)
+  "mem_w_INT2": 908033.0,      # number of INT2 parameters (weights)
   # op_mac_X_Y: number of MAC operations, datatype X by datatype Y
-  "op_mac_FLOAT32_INT2": 1555200.0, # number of float32 x int2 MACs
-  "op_mac_INT2_INT2": 57906176.0,   # number of int2 x int2 MACs
-  "total_bops": 331157504.0,        # total number of MACs normalized to bit-ops (BOPS)
+  # scaled integer datatypes have a tensor- or channelwise scale factor
+  "op_mac_SCALEDINT<8>_INT2": 1345500.0, # number of scaled int8 x int2 MACs
+  "op_mac_INT2_INT2": 35615771.0,   # number of int2 x int2 MACs
+  "total_bops": 163991084.0,        # total number of MACs normalized to bit-ops (BOPS)
   "total_mem_o_bits": 4563264.0,    # total number of bits for layer outputs
-  "total_mem_w_bits": 2289024.0,    # total number of bits for layer parameters
+  "total_mem_w_bits": 1816066.0,    # total number of bits for layer parameters
   "unsupported": "set()"
 }
 ```
 
 You can read more about the BOPS metric in [this paper](https://www.frontiersin.org/articles/10.3389/frai.2021.676564/full), Section 4.2 Bit Operations.
 
-### Development
+### Convert between different quantization representations
+
+Using the `qonnx-convert` command line utility you can convert from QONNX to QCDQ-style quantization:
+
+`qonnx-convert CNV_2W2A.onnx`
+
+This will convert `Quant` nodes to `QuantizeLinear -> Clip -> DequantizeLinear` nodes where possible.
+Please see the documentation of the `QuantToQCDQ` transformation to learn more about the limitations.
+
+## Development
 
 Install in editable mode in a venv:
 
 ```
 git clone https://github.com/fastmachinelearning/qonnx
 cd qonnx
 virtualenv -p python3.8 venv
 source venv/bin/activate
-pip install -e .[qkeras,testing]
+pip install -e .[qkeras,testing,docs]
 ```
 
 Run entire test suite, parallelized across CPU cores:
 ```
 pytest -n auto --verbose
 ```
```

### Comparing `qonnx-0.2.0/docs/Makefile` & `qonnx-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/docs/_templates/apidoc/package.rst_t` & `qonnx-0.3.0/docs/_templates/apidoc/package.rst_t`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/docs/conf.py` & `qonnx-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/docs/index.rst` & `qonnx-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/docs/overview.rst` & `qonnx-0.3.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/docs/qonnx-comparison.png` & `qonnx-0.3.0/docs/qonnx-comparison.png`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/docs/qonnx-custom-ops/bipolar_quant_op.md` & `qonnx-0.3.0/docs/qonnx-custom-ops/bipolar_quant_op.md`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/docs/qonnx-custom-ops/quant_op.md` & `qonnx-0.3.0/docs/qonnx-custom-ops/quant_op.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 <dl>
 <dt><tt>signed</tt> : int (default is 1)</dt>
 <dd>Defines if the quantization includes a signed bit. E.g. at 8b unsigned=[0, 255] vs signed=[-128, 127].</dd>
 <dt><tt>narrow</tt> : int (default is 0)</dt>
 <dd>Defines if the value range should be interpreted as narrow, when signed=1. E.g. at 8b regular=[-128, 127] vs narrow=[-127, 127].</dd>
 <dt><tt>rounding_mode</tt> : string (default is "ROUND")</dt>
-<dd>Defines how rounding should be applied during quantization. Currently available modes are: "ROUND", "CEIL" and "FLOOR". Here "ROUND" implies a round-to-even operation.</dd>
+<dd>Defines how rounding should be applied during quantization. Currently available modes are: "ROUND", "CEIL" and "FLOOR". Here "ROUND" implies a round-to-even operation. Lowercase variants for the rounding mode string are also supported: "round", "ceil", "floor".</dd>
 </dl>
 
 #### Inputs
 
 <dl>
 <dt><tt>X</tt> (differentiable) : tensor(float32)</dt>
 <dd>input tensor to quantize</dd>
```

### Comparing `qonnx-0.2.0/docs/qonnx-custom-ops/trunc_op.md` & `qonnx-0.3.0/docs/qonnx-custom-ops/trunc_op.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 This operator is not part of the ONNX standard and is not currently versioned.
 
 #### Attributes
 
 <dl>
 <dt><tt>rounding_mode</tt> : string (default is "FLOOR")</dt>
-<dd>Defines how rounding should be applied during truncation. Currently available modes are: "ROUND", "CEIL" and "FLOOR". Here "ROUND" implies a round-to-even operation.</dd>
+<dd>Defines how rounding should be applied during truncation. Currently available modes are: "ROUND", "CEIL" and "FLOOR". Here "ROUND" implies a round-to-even operation. Lowercase variants for the rounding mode string are also supported: "round", "ceil", "floor".</dd>
 </dl>
 
 #### Inputs
 
 <dl>
 <dt><tt>X</tt> (differentiable) : tensor(float32)</dt>
 <dd>input tensor to truncate</dd>
```

### Comparing `qonnx-0.2.0/docs/tutorials.rst` & `qonnx-0.3.0/docs/tutorials.rst`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/notebooks/0_how_to_work_with_onnx.ipynb` & `qonnx-0.3.0/notebooks/0_how_to_work_with_onnx.ipynb`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/notebooks/1_custom_analysis_pass.ipynb` & `qonnx-0.3.0/notebooks/1_custom_analysis_pass.ipynb`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/notebooks/2_custom_transformation_pass.ipynb` & `qonnx-0.3.0/notebooks/2_custom_transformation_pass.ipynb`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/notebooks/3_custom_op.ipynb` & `qonnx-0.3.0/notebooks/3_custom_op.ipynb`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/setup.cfg` & `qonnx-0.3.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -16,33 +16,34 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
-	clize==4.1.1
+	attrs>=22.2.0
+	clize>=5.0.1
 	protobuf==3.20.3
 	bitstring>=3.1.7
-	numpy==1.24.1
-	onnx==1.13.0
-	onnxruntime==1.11.1
-	sigtools==2.0.3
-	toposort==1.7.0
+	numpy>=1.24.1
+	onnx>=1.13.0
+	onnxruntime>=1.15.0
+	sigtools>=4.0.1
+	toposort>=1.7.0
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 qkeras = 
 	pyparsing
 	tf2onnx>=1.12.1
-	tensorflow==2.7.0
+	tensorflow==2.9.0
 	QKeras==0.9.0
 testing = 
 	setuptools
 	pytest
 	pytest-xdist
 	pytest-cov
 	pytest-randomly
@@ -52,14 +53,17 @@
 
 [options.entry_points]
 console_scripts = 
 	qonnx-cleanup = qonnx.util.cleanup:main
 	qonnx-exec = qonnx.util.exec_qonnx:main
 	qonnx-to-channels-last = qonnx.util.to_channels_last:main
 	qonnx-inference-cost = qonnx.util.inference_cost:main
+	qonnx-convert = qonnx.util.convert:main
+	qonnx-range-analysis = qonnx.util.range_analysis:main
+	qonnx-download-model = qonnx.util.test:qonnx_download_model
 pytest_randomly.random_seeder = 
 	qonnx = qonnx.util.random_reseed:reseed
 
 [tool:pytest]
 addopts = 
 	--cov qonnx --cov-report term-missing
 	--verbose
```

### Comparing `qonnx-0.2.0/setup.py` & `qonnx-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/analysis/base.py` & `qonnx-0.3.0/src/qonnx/analysis/base.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/analysis/inference_cost.py` & `qonnx-0.3.0/src/qonnx/analysis/inference_cost.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/analysis/topology.py` & `qonnx-0.3.0/src/qonnx/analysis/topology.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/converters/keras.py` & `qonnx-0.3.0/src/qonnx/converters/keras.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,16 +246,14 @@
     for q_op_type in qonnx_domain_ops:
         quant_nodes = onnx_model.get_nodes_by_op_type(q_op_type)
         q_node_outputs = [qn.output[0] for qn in quant_nodes]
         for tensor in onnx_model.graph.value_info:
             if tensor.name in q_node_outputs:
                 tensor.type.tensor_type.elem_type = 1
 
-    onnx_model.save(f"tmp_{name}.onnx")
-
     onnx_model = cleanup_model(onnx_model)
     onnx_model.model = add_value_info_for_constants(onnx_model.model)
 
     if output_path is not None:
         onnx_model.save(output_path)
 
     return onnx_model.model, external_storage
```

### Comparing `qonnx-0.2.0/src/qonnx/converters/qkeras/onnx.py` & `qonnx-0.3.0/src/qonnx/converters/qkeras/onnx.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/converters/qkeras/qlayers.py` & `qonnx-0.3.0/src/qonnx/converters/qkeras/qlayers.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/converters/qkeras/quantizers.py` & `qonnx-0.3.0/src/qonnx/converters/qkeras/quantizers.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/core/data_layout.py` & `qonnx-0.3.0/src/qonnx/core/data_layout.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/core/datatype.py` & `qonnx-0.3.0/src/qonnx/core/datatype.py`

 * *Files 4% similar despite different names*

```diff
@@ -303,14 +303,50 @@
     def to_numpy_dt(self):
         return np.float32
 
     def get_canonical_name(self):
         return "FIXED<%d,%d>" % (self.bitwidth(), self.int_bits())
 
 
+class ScaledIntType(IntType):
+    # scaled integer datatype, only intended for
+    # inference cost calculations, many of the
+    # member methods are not implemented
+    def __init__(self, bitwidth):
+        super().__init__(bitwidth=bitwidth, signed=True)
+
+    def min(self):
+        raise Exception("Undefined for ScaledIntType")
+
+    def max(self):
+        raise Exception("Undefined for ScaledIntType")
+
+    def allowed(self, value):
+        raise Exception("Undefined for ScaledIntType")
+
+    def is_integer(self):
+        return False
+
+    def is_fixed_point(self):
+        return False
+
+    def get_hls_datatype_str(self):
+        raise Exception("Undefined for ScaledIntType")
+
+    def to_numpy_dt(self):
+        return np.float32
+
+    def signed(self):
+        "Returns whether this DataType can represent negative numbers."
+        return True
+
+    def get_canonical_name(self):
+        return "SCALEDINT<%d>" % (self.bitwidth())
+
+
 def resolve_datatype(name):
     _special_types = {
         "BINARY": IntType(1, False),
         "BIPOLAR": BipolarType(),
         "TERNARY": TernaryType(),
         "FLOAT32": FloatType(),
     }
@@ -325,14 +361,20 @@
     elif name.startswith("FIXED"):
         name = name.replace("FIXED<", "")
         name = name.replace(">", "")
         nums = name.split(",")
         bitwidth = int(nums[0].strip())
         intwidth = int(nums[1].strip())
         return FixedPointType(bitwidth, intwidth)
+    elif name.startswith("SCALEDINT"):
+        name = name.replace("SCALEDINT<", "")
+        name = name.replace(">", "")
+        nums = name.split(",")
+        bitwidth = int(nums[0].strip())
+        return ScaledIntType(bitwidth)
     else:
         raise KeyError("Could not resolve DataType " + name)
 
 
 class DataTypeMeta(EnumMeta):
     def __getitem__(self, name):
         return resolve_datatype(name)
```

### Comparing `qonnx-0.2.0/src/qonnx/core/execute_custom_node.py` & `qonnx-0.3.0/src/qonnx/core/execute_custom_node.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/core/modelwrapper.py` & `qonnx-0.3.0/src/qonnx/core/modelwrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,20 +245,29 @@
                 return None
             else:
                 if fix_missing_init_shape:
                     self.set_tensor_shape(tensor_name, tensor_init.shape, dtype=tensor_init_dtype)
                 # use list return type to keep it consistent with ValueInfo case
                 return list(tensor_init.shape)
 
-    def set_tensor_shape(self, tensor_name, tensor_shape, dtype=TensorProto.FLOAT):
-        """Assigns shape in ValueInfoProto for tensor with given name."""
-        new_vi = oh.make_tensor_value_info(tensor_name, dtype, tensor_shape)
+    def set_tensor_shape(self, tensor_name, tensor_shape, dtype=None):
+        """Assigns shape in ValueInfoProto for tensor with given name. If override_dtype
+        is None, it will try to preserve the existing datatype, otherwise defaults to
+        single-precision float."""
         # call get_tensor_valueinfo to raise a warning for multiple ValueInfoProto cases
-        self.get_tensor_valueinfo(tensor_name)
-        # find what container tis tensor's ValueInfo lives in
+        old_vi = self.get_tensor_valueinfo(tensor_name)
+        # resolve dtype
+        if dtype is None:
+            # try to preserve old dtype
+            if old_vi is None:
+                dtype = TensorProto.FLOAT
+            else:
+                dtype = old_vi.type.tensor_type.elem_type
+        new_vi = oh.make_tensor_value_info(tensor_name, dtype, tensor_shape)
+        # find what container tHis tensor's ValueInfo lives in
         # if not found anywhere, we assume it's a new value_info
         target_container = self.graph.value_info
         if util.get_by_name(self.graph.input, tensor_name) is not None:
             target_container = self.graph.input
         if util.get_by_name(self.graph.output, tensor_name) is not None:
             target_container = self.graph.output
         # remove from target container and add new
```

### Comparing `qonnx-0.2.0/src/qonnx/core/onnx_exec.py` & `qonnx-0.3.0/src/qonnx/core/onnx_exec.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 import copy
 import numpy as np
 import onnx.helper as helper
 import onnxruntime as rt
+import warnings
 
 import qonnx.analysis.topology as ta
 import qonnx.core.execute_custom_node as ex_cu_node
 from qonnx.util.basic import (
     get_preferred_onnx_opset,
     get_sanitize_quant_tensors,
     is_finn_op,
@@ -60,14 +61,21 @@
         # input/outputs may get them reordered below
         # note: a node's input may (also) be a top-level input or output
         node_inputs = list(filter(lambda x: x.name in node.input, graph.input))
         node_inputs += list(filter(lambda x: x.name in node.input, graph.output))
         node_inputs += list(filter(lambda x: x.name in node.input, graph.value_info))
         node_outputs = list(filter(lambda x: x.name in node.output, graph.output))
         node_outputs += list(filter(lambda x: x.name in node.output, graph.value_info))
+        for attr in node.attribute:
+            if attr.type == 5:
+                subgraph = attr.g
+                for subgraph_node in subgraph.node:
+                    subgraph_node_inputs = list(filter(lambda x: x.name in subgraph_node.input, graph.value_info))
+                    new_inps = list(filter(lambda x: x not in node_inputs, subgraph_node_inputs))
+                    node_inputs += new_inps
         node_graph = helper.make_graph(
             nodes=[node],
             name="single-node-exec",
             inputs=node_inputs,
             outputs=node_outputs,
         )
         node_model = qonnx_make_model(node_graph)
@@ -86,18 +94,18 @@
             # retrieve the index of that name in node_outputs
             for i in range(len(node_outputs)):
                 if outp == node_outputs[i].name:
                     list_ind = i
 
             # use that index to index output_list
             if output_list[list_ind].shape != context[outp].shape:
-                raise Exception(
-                    """Output shapes disagree after node execution:
+                warnings.warn(
+                    """Output shapes disagree after node %s execution:
                     found %s vs expected %s"""
-                    % (str(output_list[list_ind].shape), str(context[outp].shape))
+                    % (str(node), str(output_list[list_ind].shape), str(context[outp].shape))
                 )
             context[outp] = output_list[list_ind]
 
 
 def execute_onnx(model, input_dict, return_full_exec_context=False, start_node=None, end_node=None):
     """Executes given ONNX ModelWrapper with given named inputs.
```

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/base.py` & `qonnx-0.3.0/src/qonnx/custom_op/base.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/channels_last/base_wrapped_op.py` & `qonnx-0.3.0/src/qonnx/custom_op/channels_last/base_wrapped_op.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/channels_last/batch_normalization.py` & `qonnx-0.3.0/src/qonnx/custom_op/channels_last/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/channels_last/conv.py` & `qonnx-0.3.0/src/qonnx/custom_op/channels_last/conv.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/channels_last/max_pool.py` & `qonnx-0.3.0/src/qonnx/custom_op/channels_last/max_pool.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/general/__init__.py` & `qonnx-0.3.0/src/qonnx/custom_op/general/__init__.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/general/bipolar_quant.py` & `qonnx-0.3.0/src/qonnx/custom_op/general/bipolar_quant.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/general/debugmarker.py` & `qonnx-0.3.0/src/qonnx/custom_op/general/debugmarker.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/general/genericpartition.py` & `qonnx-0.3.0/src/qonnx/custom_op/general/genericpartition.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/general/im2col.py` & `qonnx-0.3.0/src/qonnx/custom_op/general/im2col.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/general/maxpoolnhwc.py` & `qonnx-0.3.0/src/qonnx/custom_op/general/maxpoolnhwc.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,18 @@
         # execute as regular MaxPool
         orig_domain = node.domain
         node.domain = ""
         node.op_type = "MaxPool"
         inp_vi = helper.make_tensor_value_info(inp_name, TensorProto.FLOAT, inp.shape)
         out_vi = helper.make_tensor_value_info(out_name, TensorProto.FLOAT, dummy_out.shape)
         tmp_graph = helper.make_graph(nodes=[node], name="tmp_graph", inputs=[inp_vi], outputs=[out_vi])
-        tmp_model = qonnx_make_model(tmp_graph, producer_name="finn")
+        opset_version = self.onnx_opset_version
+        opset_imports = [helper.make_opsetid("", opset_version)]
+        onnx_kwargs = {"opset_imports": opset_imports}
+        tmp_model = qonnx_make_model(tmp_graph, producer_name="finn", **onnx_kwargs)
         tmp_model = ModelWrapper(tmp_model)
         new_ctx = {inp_name: inp}
         from qonnx.core.onnx_exec import execute_onnx
 
         ret = execute_onnx(tmp_model, new_ctx)
         # restore original node props
         node.domain = orig_domain
```

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/general/multithreshold.py` & `qonnx-0.3.0/src/qonnx/custom_op/general/multithreshold.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/general/quant.py` & `qonnx-0.3.0/src/qonnx/custom_op/general/quant.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import numpy as np
-import onnx.helper as helper
+from onnx import TensorProto, helper
 
 from qonnx.core.datatype import DataType
 from qonnx.custom_op.base import CustomOp
 
 
 def min_int(signed: bool, narrow_range: bool, bit_width: int) -> int:
     """Compute the minimum integer representable by a given number of bits.
@@ -130,22 +130,23 @@
 
     return out_tensor
 
 
 def resolve_rounding_mode(mode_string):
     """Resolve the rounding mode string of Quant and Trunc ops
     to the corresponding numpy functions."""
-    if mode_string == "ROUND":
+    normalized_mode_string = mode_string.upper()
+    if normalized_mode_string == "ROUND":
         return np.round
-    elif mode_string == "CEIL":
+    elif normalized_mode_string == "CEIL":
         return np.ceil
-    elif mode_string == "FLOOR":
+    elif normalized_mode_string == "FLOOR":
         return np.floor
     else:
-        raise ValueError(f"Could not resolve rounding mode called: {mode_string}")
+        raise ValueError(f"Could not resolve rounding mode called: {normalized_mode_string}")
 
 
 class Quant(CustomOp):
     """Generic quantization operation for QONNX. Takes four inputs:
     - input tensor to quantize
     - the scale
     - the zero-point
@@ -165,16 +166,40 @@
             "narrow": ("i", True, 1),
             # The rounding mode, which is used for the quant function
             # ToDo: This should be required (True) instead of optional (False)
             "rounding_mode": ("s", False, "ROUND"),
         }
 
     def make_shape_compatible_op(self, model):
-        node = self.onnx_node
-        return helper.make_node("Identity", [node.input[0]], [node.output[0]])
+        """Returns a standard ONNX op which is compatible with this CustomOp
+        for performing shape inference."""
+        return helper.make_node(
+            "Cast",
+            inputs=[self.onnx_node.input[0]],
+            outputs=[self.onnx_node.output[0]],
+            to=int(TensorProto.FLOAT),
+        )
+        # For Quant the output shape should be the same as the input shape.
+        # Get the output shape from the input
+        out_shape = model.get_tensor_shape(self.onnx_node.input[0])
+
+        # implement tensor with correct shape
+        values = np.random.randn(*out_shape).astype(np.float32)
+        return helper.make_node(
+            "Constant",
+            inputs=[],
+            outputs=[self.onnx_node.output[0]],
+            value=helper.make_tensor(
+                name="const_tensor",
+                data_type=TensorProto.FLOAT,
+                dims=values.shape,
+                vals=values.flatten().astype(float),
+            ),
+            name=self.onnx_node.name,
+        )
 
     def get_integer_datatype(self, model):
         signed = self.get_nodeattr("signed")
         bit_width = model.get_initializer(self.onnx_node.input[3])
         bit_width = int(bit_width)
         if bit_width == 1:
             if signed:
@@ -184,14 +209,20 @@
         else:
             if signed:
                 finn_dt = DataType["INT" + str(bit_width)]
             else:
                 finn_dt = DataType["UINT" + str(bit_width)]
         return finn_dt
 
+    def get_scaled_integer_datatype(self, model):
+        bit_width = model.get_initializer(self.onnx_node.input[3])
+        bit_width = int(bit_width)
+        finn_dt = DataType["SCALEDINT<%d>" % (bit_width)]
+        return finn_dt
+
     def get_output_dtype(self, model):
         node = self.onnx_node
         # scale, zero-point and bitwidth must be read from initializers
         scale = model.get_initializer(node.input[1])
         zeropt = model.get_initializer(node.input[2])
         bitwidth = model.get_initializer(node.input[3])
         assert scale is not None, "Found unspecified scale for Quant node: " + str(node)
@@ -205,16 +236,15 @@
         # determine the FINN DataType
         unit_scale = np.all(scale == 1.0)
         zero_zeropt = np.all(zeropt == 0.0)
         assert zero_zeropt, "Only zero_point=0 Quant nodes supported for now"
         if unit_scale and zero_zeropt:
             finn_dt = self.get_integer_datatype(model)
         else:
-            finn_dt = DataType["FLOAT32"]
-
+            finn_dt = self.get_scaled_integer_datatype(model)
         return finn_dt
 
     def infer_node_datatype(self, model):
         try:
             finn_dt = self.get_output_dtype(model)
         except AssertionError:
             finn_dt = DataType["FLOAT32"]
@@ -235,12 +265,14 @@
         # calculate output
         ret = quant(inp_tensor, scale, zeropt, bitwidth, signed, narrow, rounding_mode)
         # ensure output is ndarray (even if 0d)
         # since numpy silently flattens 0d arrays to scalars
         # more: https://github.com/numpy/numpy/issues/13105
         if not isinstance(ret, np.ndarray):
             ret = np.asarray(ret, dtype=np.float32)
+        if not ret.dtype == np.float32:
+            ret = ret.astype(np.float32)
         # set context according to output name
         context[node.output[0]] = ret
 
     def verify_node(self):
         pass
```

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/general/quantavgpool2d.py` & `qonnx-0.3.0/src/qonnx/custom_op/general/quantavgpool2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,15 +127,19 @@
         )
         graph_avgpool = helper.make_graph(
             nodes=[node_avgpool],
             name="single-avgpool-exec",
             inputs=[inp],
             outputs=[outp],
         )
-        model_avgpool = qonnx_make_model(graph_avgpool)
+
+        opset_version = self.onnx_opset_version
+        opset_imports = [helper.make_opsetid("", opset_version)]
+        onnx_kwargs = {"opset_imports": opset_imports}
+        model_avgpool = qonnx_make_model(graph_avgpool, **onnx_kwargs)
         idict = {node.input[0]: inp_values}
         sess = rt.InferenceSession(model_avgpool.SerializeToString())
         result_temp = sess.run(None, idict)
         # remove scaling introduced by average
         result_temp = result_temp[0] * (k * k)
         result = np.right_shift(result_temp.astype(int), self.get_shifts())
         if self.get_nodeattr("data_layout") == "NHWC":
```

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/general/trunc.py` & `qonnx-0.3.0/src/qonnx/custom_op/general/trunc.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/general/xnorpopcount.py` & `qonnx-0.3.0/src/qonnx/custom_op/general/xnorpopcount.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/custom_op/registry.py` & `qonnx-0.3.0/src/qonnx/custom_op/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,18 +27,21 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import importlib
 
 from qonnx.util.basic import get_preferred_onnx_opset
 
 
-def getCustomOp(node, onnx_opset_version=get_preferred_onnx_opset()):
+def getCustomOp(node, onnx_opset_version=get_preferred_onnx_opset(), brevitas_exception=True):
     "Return a QONNX CustomOp instance for the given ONNX node, if it exists."
     op_type = node.op_type
     domain = node.domain
+    if brevitas_exception:
+        # transparently resolve Brevitas domain ops to qonnx ones
+        domain = domain.replace("onnx.brevitas", "qonnx.custom_op.general")
     try:
         opset_module = importlib.import_module(domain)
         assert type(opset_module.custom_op) is dict, "custom_op dict not found in Python module %s" % domain
         inst_wrapper = opset_module.custom_op[op_type]
         inst = inst_wrapper(node, onnx_opset_version=onnx_opset_version)
         return inst
     except ModuleNotFoundError:
```

### Comparing `qonnx-0.2.0/src/qonnx/data/__init__.py` & `qonnx-0.3.0/src/qonnx/data/__init__.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/data/onnx/mnist-conv/model.onnx` & `qonnx-0.3.0/src/qonnx/data/onnx/mnist-conv/model.onnx`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/data/onnx/mnist-conv/test_data_set_0/input_0.pb` & `qonnx-0.3.0/src/qonnx/data/onnx/mnist-conv/test_data_set_0/input_0.pb`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/base.py` & `qonnx-0.3.0/src/qonnx/transformation/base.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/batchnorm_to_affine.py` & `qonnx-0.3.0/src/qonnx/transformation/batchnorm_to_affine.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/bipolar_to_xnor.py` & `qonnx-0.3.0/src/qonnx/transformation/bipolar_to_xnor.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/change_3d_tensors_to_4d.py` & `qonnx-0.3.0/src/qonnx/transformation/change_3d_tensors_to_4d.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/change_datalayout.py` & `qonnx-0.3.0/src/qonnx/transformation/change_datalayout.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/channels_last.py` & `qonnx-0.3.0/src/qonnx/transformation/channels_last.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/create_generic_partitions.py` & `qonnx-0.3.0/src/qonnx/transformation/create_generic_partitions.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/double_to_single_float.py` & `qonnx-0.3.0/src/qonnx/transformation/double_to_single_float.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/extend_partition.py` & `qonnx-0.3.0/src/qonnx/transformation/extend_partition.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/extract_conv_bias.py` & `qonnx-0.3.0/src/qonnx/transformation/extract_conv_bias.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/fold_constants.py` & `qonnx-0.3.0/src/qonnx/transformation/fold_constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,68 +37,82 @@
     can be eligible for const folding."""
 
     def __init__(self, match_filter_fxn):
         super().__init__()
         self.match_filter_fxn = match_filter_fxn
 
     def apply(self, model):
+        opset_version = model.model.opset_import[0].version
         graph = model.graph
         node_ind = 0
         graph_modified = False
         execution_context = model.make_empty_exec_context()
+        nodes_to_remove = []
         for n in graph.node:
             node_ind += 1
             node_inp_inits = list(map(lambda x: model.get_initializer(x), n.input))
             node_inp_dyn = list(filter(lambda x: x is None, node_inp_inits))
             node_out = n.output[0]
             is_all_constant_inputs = len(node_inp_dyn) == 0
             ishape = model.get_tensor_shape(n.input[0])
             is_const_shape = (n.op_type == "Shape") and (ishape is not None)
             eligible = self.match_filter_fxn(model, n)
             if (is_all_constant_inputs or is_const_shape) and eligible:
                 # this node has no dynamic inputs, only constant ones -- so we can
                 # do constant folding.
-                oxe.execute_node(n, execution_context, graph)
+                oxe.execute_node(n, execution_context, graph, opset_version=opset_version)
                 # use the execution result as an initializer
                 model.set_initializer(node_out, execution_context[node_out])
                 # remove old node
-                graph.node.remove(n)
+                nodes_to_remove.append(n)
                 graph_modified = True
+        for node in nodes_to_remove:
+            model.graph.node.remove(node)
         if graph_modified:
             model = model.transform(InferShapes())
         return (model, graph_modified)
 
 
 class FoldConstants(Transformation):
     """Replace the output of a node with const-only inputs with a precomputed
     result. Skip any op types given in exclude_op_types."""
 
     def __init__(self, exclude_op_types=["Quant", "BipolarQuant"]):
         super().__init__()
         self.exclude_op_types = exclude_op_types
 
     def apply(self, model):
-        graph = model.graph
+        opset_version = model.model.opset_import[0].version
         node_ind = 0
         graph_modified = False
         execution_context = model.make_empty_exec_context()
-        for n in graph.node:
+        nodes_to_remove = []
+        for n in model.graph.node:
             node_ind += 1
             node_inp_inits = list(map(lambda x: model.get_initializer(x), n.input))
             node_inp_dyn = list(filter(lambda x: x is None, node_inp_inits))
             node_out = n.output[0]
             is_all_constant_inputs = len(node_inp_dyn) == 0
-            ishape = model.get_tensor_shape(n.input[0])
-            is_const_shape = (n.op_type == "Shape") and (ishape is not None)
+            if len(n.input) > 0:
+                ishape = model.get_tensor_shape(n.input[0])
+                is_const_shape = (n.op_type == "Shape") and (ishape is not None)
+                is_no_input = False
+            else:
+                is_no_input = True
             exclude = n.op_type in self.exclude_op_types
-            if (is_all_constant_inputs or is_const_shape) and not exclude:
-                # this node has no dynamic inputs, only constant ones -- so we can
-                # do constant folding.
-                oxe.execute_node(n, execution_context, graph)
+            if (is_all_constant_inputs or is_const_shape or is_no_input) and not exclude:
+                # this node has no (dynamic) inputs, only constant ones -- so we can
+                # do constant folding. to ensure any missing ValueInfos from initializers
+                # are populated, we 'touch' the shape of all inputs first below.
+                for inp in n.input:
+                    model.get_tensor_shape(inp, fix_missing_init_shape=True)
+                oxe.execute_node(n, execution_context, model.graph, opset_version=opset_version)
                 # use the execution result as an initializer
                 model.set_initializer(node_out, execution_context[node_out])
                 # remove old node
-                graph.node.remove(n)
+                nodes_to_remove.append(n)
                 graph_modified = True
+        for node in nodes_to_remove:
+            model.graph.node.remove(node)
         if graph_modified:
             model = model.transform(InferShapes())
         return (model, graph_modified)
```

### Comparing `qonnx-0.2.0/src/qonnx/transformation/gemm_to_matmul.py` & `qonnx-0.3.0/src/qonnx/transformation/gemm_to_matmul.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/general.py` & `qonnx-0.3.0/src/qonnx/transformation/general.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,21 +23,52 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import json
+import numpy as np
 import warnings
+from onnx import mapping
 from toposort import toposort_flatten
 
 import qonnx.util.basic as util
 from qonnx.transformation.base import Transformation
 
 
+class MovePadAttributeToTensor(Transformation):
+    "Move padding info from attribute into input tensor for Pad nodes."
+
+    def apply(self, model):
+        run_again = False
+        pad_nodes = model.get_nodes_by_op_type("Pad")
+        for pad_node in pad_nodes:
+            pads = util.get_by_name(pad_node.attribute, "pads")
+            if pads is not None:
+                assert len(pad_node.input) == 1
+                pads_t = np.asarray(pads.ints)
+                new_pad_name = model.make_new_valueinfo_name()
+                model.set_initializer(new_pad_name, pads_t)
+                pad_node.input.append(new_pad_name)
+                pad_node.attribute.remove(pads)
+            padval = util.get_by_name(pad_node.attribute, "value")
+            if padval is not None:
+                # non-float types will need type correction here
+                input_vi = model.get_tensor_valueinfo(pad_node.input[0])
+                pad_dtype = mapping.TENSOR_TYPE_TO_NP_TYPE[input_vi.type.tensor_type.elem_type]
+                padval_t = np.asarray(padval.f, pad_dtype)
+                new_padval_name = model.make_new_valueinfo_name()
+                model.set_initializer(new_padval_name, padval_t)
+                pad_node.input.append(new_padval_name)
+                pad_node.attribute.remove(padval)
+
+        return (model, run_again)
+
+
 class RemoveUnusedTensors(Transformation):
     """Remove any unused tensors in the graph by removing any initializers,
     ValueInfo and tensor annotations associated with it. Unused tensors do not
     appear as any input/output for any graph nodes.
     """
 
     def apply(self, model):
@@ -271,30 +302,33 @@
         "Defaults" : {"kernel_size" : [3, ["Im2Col"]]},
         # set kernel_size = 7 for the particular node with name Im2Col_0
         "Im2Col_0" : {"kernel_size" : 7}
         }
 
     """
 
-    def __init__(self, config):
+    def __init__(self, config, node_filter=lambda x: True):
         super().__init__()
         self.config = config
+        self.node_filter = node_filter
 
     def apply(self, model):
         if isinstance(self.config, dict):
             model_config = self.config
         else:
             with open(self.config, "r") as f:
                 model_config = json.load(f)
 
         used_configurations = ["Defaults"]
         missing_configurations = []
 
         # Configure network
         for node_idx, node in enumerate(model.graph.node):
+            if not self.node_filter(node):
+                continue
             try:
                 node_config = model_config[node.name]
             except KeyError:
                 missing_configurations += [node.name]
                 node_config = {}
 
             from qonnx.custom_op.registry import getCustomOp
```

### Comparing `qonnx-0.2.0/src/qonnx/transformation/infer_data_layouts.py` & `qonnx-0.3.0/src/qonnx/transformation/infer_data_layouts.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/infer_datatypes.py` & `qonnx-0.3.0/src/qonnx/transformation/infer_datatypes.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,19 +23,38 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import qonnx.custom_op.registry as registry
-from qonnx.core.datatype import DataType
+from qonnx.core.datatype import DataType, ScaledIntType
 from qonnx.transformation.base import Transformation
 from qonnx.util.basic import get_by_name, is_finn_op
 
 
+def is_scaled_int(x):
+    # can treat both integer, fixed point and scaled int as scaled int
+    return x.is_integer() or x.is_fixed_point() or isinstance(x, ScaledIntType)
+
+
+def infer_mac_result_dtype(idtypes, possible_negation):
+    # will default to float32 unless specific cases detected
+    ret = DataType["FLOAT32"]
+    # result may be signed if:
+    # - any of the operands are signed
+    # - the operator itself may induce negation (like subtraction)
+    maybe_signed = possible_negation or any([x.signed() for x in idtypes])
+    if all([x.is_integer() for x in idtypes]):
+        ret = DataType["INT32"] if maybe_signed else DataType["UINT32"]
+    elif all([is_scaled_int(x) for x in idtypes]):
+        ret = DataType["SCALEDINT<32>"]
+    return ret
+
+
 def _infer_node_datatype(model, node):
     """Infer output datatype(s) for a particular node. Returns True if any
     changes were made."""
     dt_identity_optypes = [
         "Reshape",
         "Transpose",
         "Flatten",
@@ -50,15 +69,18 @@
         "GlobalMaxPool",
         "Scatter",
         "ScatterElements",
         "ScatterND",
         "Squeeze",
         "Unsqueeze",
         "Tile",
+        "Pad",
+        "Concat",
     ]
+    mac_like_optypes = ["MatMul", "Gemm", "Conv", "Add", "Sub", "Mul"]
     idtypes = list(map(lambda x: model.get_tensor_datatype(x), node.input))
     odtypes = list(map(lambda x: model.get_tensor_datatype(x), node.output))
     op_type = node.op_type
     if is_finn_op(node.domain):
         # handle DataType inference for CustomOp
         try:
             # lookup op_type in registry of CustomOps
@@ -67,48 +89,28 @@
         except KeyError:
             # exception if op_type is not supported
             raise Exception("Custom op_type %s is currently not supported." % op_type)
     else:
         if node.op_type == "Sign":
             # always produces bipolar outputs
             model.set_tensor_datatype(node.output[0], DataType["BIPOLAR"])
-        elif node.op_type in ["MatMul", "Conv"]:
-            if len(list(filter(lambda x: x == DataType["FLOAT32"], idtypes))) != 0:
-                # node has at least one float input, output is also float
-                model.set_tensor_datatype(node.output[0], DataType["FLOAT32"])
-            else:
-                # TODO compute minimum / maximum result to minimize bitwidth
-                # use (u)int32 accumulators for now
-                has_signed_inp = len(list(filter(lambda x: x.signed(), idtypes))) != 0
-                if has_signed_inp:
-                    odtype = DataType["INT32"]
-                else:
-                    odtype = DataType["UINT32"]
-                model.set_tensor_datatype(node.output[0], odtype)
+        elif node.op_type in mac_like_optypes:
+            possible_negation = node.op_type in ["Sub"]
+            odtype = infer_mac_result_dtype(idtypes, possible_negation=possible_negation)
+            model.set_tensor_datatype(node.output[0], odtype)
         elif node.op_type in ["Resize", "Upsample"]:
             mode = get_by_name(node.attribute, "mode").s
             if mode is None:
                 mode = "nearest"
             else:
                 mode = mode.decode("UTF-8")
             if mode == "nearest":
                 # set output dtype = input dtype
                 idtype = model.get_tensor_datatype(node.input[0])
                 model.set_tensor_datatype(node.output[0], idtype)
-        elif node.op_type in ["Add", "Sub"]:
-            if len(list(filter(lambda x: not (x.is_integer() or x.is_fixed_point()), idtypes))) != 0:
-                # node has at least one non-quantized input, output is also float
-                model.set_tensor_datatype(node.output[0], DataType["FLOAT32"])
-            else:
-                has_signed_inp = len(list(filter(lambda x: x.signed(), idtypes))) != 0
-                if has_signed_inp or (node.op_type == "Sub"):
-                    odtype = DataType["INT32"]
-                else:
-                    odtype = DataType["UINT32"]
-                model.set_tensor_datatype(node.output[0], odtype)
         elif node.op_type in dt_identity_optypes:
             # set output dtype = input dtype
             idtype = model.get_tensor_datatype(node.input[0])
             model.set_tensor_datatype(node.output[0], idtype)
         else:
             # unknown, assume node produces float32 outputs
             for o in node.output:
```

### Comparing `qonnx-0.2.0/src/qonnx/transformation/infer_shapes.py` & `qonnx-0.3.0/src/qonnx/transformation/infer_shapes.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/insert_topk.py` & `qonnx-0.3.0/src/qonnx/transformation/insert_topk.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/lower_convs_to_matmul.py` & `qonnx-0.3.0/src/qonnx/transformation/lower_convs_to_matmul.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/make_input_chanlast.py` & `qonnx-0.3.0/src/qonnx/transformation/make_input_chanlast.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/merge_onnx_models.py` & `qonnx-0.3.0/src/qonnx/transformation/merge_onnx_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,14 +59,22 @@
     def apply(self, model):
         graph_modified = False
         pre_model = self.pre_model
         post_model = copy.deepcopy(model)
         # to avoid mix-ups, start by giving all tensors random names
         pre_model = pre_model.transform(GiveRandomTensorNames())
         post_model = post_model.transform(GiveRandomTensorNames())
+        pre_model_opset = pre_model.model.opset_import[0].version
+        post_model_opset = post_model.model.opset_import[0].version
+        merged_model_opset = max(pre_model_opset, post_model_opset)
+        if pre_model_opset != post_model_opset:
+            warnings.warn(
+                "[MergeONNXModels] opsets for models to merge differ: %d vs %d, output model will use opset %d"
+                % (pre_model_opset, post_model_opset, merged_model_opset)
+            )
 
         # check for dynamic outputs of pre model
         dyn_outp = []
         for outp in pre_model.graph.output:
             init_val = pre_model.get_initializer(outp.name)
             if init_val is None:
                 dyn_outp.append(outp)
@@ -139,15 +147,17 @@
             nodes=node_new,
             name="fuse-graph",
             inputs=[inp],
             outputs=[outp],
             value_info=vi_new,
         )
 
-        new_model = qonnx_make_model(new_graph, producer_name="fuse_model")
+        new_model = qonnx_make_model(
+            new_graph, producer_name="fuse_model", opset_imports=[helper.make_opsetid("", merged_model_opset)]
+        )
         new_model = ModelWrapper(new_model)
 
         for i in init_new:
             new_model.graph.initializer.append(i)
         for qa in qa_new:
             new_model.graph.quantization_annotation.append(qa)
```

### Comparing `qonnx-0.2.0/src/qonnx/transformation/quant_constant_folding.py` & `qonnx-0.3.0/src/qonnx/transformation/quant_constant_folding.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/rebalance_conv.py` & `qonnx-0.3.0/src/qonnx/transformation/rebalance_conv.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/transformation/remove.py` & `qonnx-0.3.0/src/qonnx/transformation/remove.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,19 +25,42 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 import numpy as np
 
+from qonnx.core.modelwrapper import ModelWrapper
 from qonnx.transformation.base import Transformation
 from qonnx.transformation.infer_shapes import InferShapes
 from qonnx.util.basic import get_by_name
 
 
+class RemoveUnusedNodes(Transformation):
+    """Remove nodes which do not contribute to any top-level output in the graph,
+    either directly or indirectly."""
+
+    def apply(self, model: ModelWrapper):
+        run_again = False
+        graph_top_outputs = {x.name for x in model.graph.output}
+        for node in model.graph.node:
+            successors = model.find_direct_successors(node)
+            node_outputs = {x for x in node.output}
+            node_top_outputs = graph_top_outputs.intersection(node_outputs)
+            if (successors is None) and (len(node_top_outputs) == 0):
+                # found node with dangling output, remove
+                model.graph.node.remove(node)
+                run_again = True
+                # remove only one node at a time to avoid potential problems
+                # with protobuf container (model.graph.node)
+                break
+
+        return (model, run_again)
+
+
 def remove_node_and_rewire(model, node):
     producer = model.find_producer(node.input[0])
     if producer is not None:
         # wire output tensor to
         # output of producer node
         producer.output[0] = node.output[0]
     else:
@@ -79,14 +102,20 @@
                 A = model.get_initializer(n.input[1])
                 if A is not None and np.isclose(A, np.ones_like(A), atol=self.atol).all():
                     remove_node_and_rewire(model, n)
                     graph_modified = True
                     break
             elif n.op_type == "Pad" and not model.is_fork_node(n) and not model.is_join_node(n):
                 pads = get_by_name(n.attribute, "pads")
-                pads = np.asarray(pads.ints, dtype=np.int64)
-                if (pads == 0).all():
+                if pads is not None:
+                    # older versions of Pad op specify pads as attribute
+                    pads = np.asarray(pads.ints, dtype=np.int64)
+                else:
+                    # newer versions of Pad op specify pads as input
+                    pads = model.get_initializer(n.input[1])
+
+                if (pads is not None) and (pads == 0).all():
                     remove_node_and_rewire(model, n)
                     graph_modified = True
                     break
         model = model.transform(InferShapes())
         return (model, graph_modified)
```

### Comparing `qonnx-0.2.0/src/qonnx/util/basic.py` & `qonnx-0.3.0/src/qonnx/util/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     else:
         kwargs["opset_imports"] = opset_imports
     return make_model(graph_proto, **kwargs)
 
 
 def is_finn_op(op_type):
     "Return whether given op_type string is a QONNX or FINN custom op"
-    return op_type.startswith("finn") or op_type.startswith("qonnx.custom_op")
+    return op_type.startswith("finn") or op_type.startswith("qonnx.custom_op") or op_type.startswith("onnx.brevitas")
 
 
 def get_num_default_workers():
     """Return the number of workers for parallel transformations. Controllable
     via the NUM_DEFAULT_WORKERS environment variable. If the env.var. is
     undefined, the default value of 1 is returned.
     """
@@ -279,17 +279,17 @@
     (int_num * float_scale) / float_scale is not always equal to int_num.
     We use this function to ensure that the values that are supposed to be
     integers are indeed integers.
     """
 
     for tensor_name in node_tensors:
         dtype = model.get_tensor_datatype(tensor_name)
-        # floats don't need sanitization, skip to next
-        # introduces less quicker runtime
-        if dtype == DataType["FLOAT32"]:
+        # non-integers don't need sanitization, skip to next
+        # introduces less overhead and quicker runtime
+        if not dtype.is_integer():
             continue
         current_values = execution_context[tensor_name]
         updated_values = current_values
         has_to_be_rounded = False
         # TODO: vectorize with numpy
         for value in np.nditer(current_values):
             if not dtype.allowed(value):
```

### Comparing `qonnx-0.2.0/src/qonnx/util/config.py` & `qonnx-0.3.0/src/qonnx/util/config.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/util/inference_cost.py` & `qonnx-0.3.0/src/qonnx/util/inference_cost.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,37 +62,41 @@
         if k.startswith(filter_string):
             comps = k.split("_")
             dt = DataType[comps[2]]
             total_mem_bits += dt.bitwidth() * v
     return total_mem_bits
 
 
-def inference_cost(model_filename, *, output_json=None, output_onnx=None, preprocess=True, discount_sparsity=True):
-    """Print the inference cost estimate metric for given ONNX model.
+def inference_cost(
+    model_filename_or_wrapper, *, output_json=None, output_onnx=None, preprocess=True, discount_sparsity=True
+):
+    """Return the inference cost estimate metric for given ONNX model.
     Supports the Quant op for weight/activation quantization.
 
-    :param model_filename: Filename for ONNX model
+    :param model_filename_or_wrapper: Filename or ModelWrapper for ONNX model
     :param output_json: Optional JSON filename to save the inference cost dict
     :param output_onnx: Optional ONNX filename to save the final model after any
         preprocessing
     :param preprocess: If set, run preprocessing steps such as shape inference,
         datatype inference and constant folding. Strongly recommended.
     :param discount_sparsity: If set, will discount op cost of MAC ops with a
         constant zero weight, and the mem cost of constant zero weights.
     """
-    print("Inference cost for " + model_filename)
-    model = ModelWrapper(model_filename)
+    if isinstance(model_filename_or_wrapper, ModelWrapper):
+        model = model_filename_or_wrapper
+    else:
+        model = ModelWrapper(model_filename_or_wrapper)
     if preprocess:
         qnt_nodes = model.get_nodes_by_op_type("Quant")
         for qnt_node in qnt_nodes:
             qnt_node.domain = "qonnx.custom_op.general"
         model = model.transform(InferShapes())
         model = model.transform(GiveUniqueParameterTensors())
         model = model.transform(InferDataTypes())
-        model = model.transform(FoldConstants())
+        model = model.transform(FoldConstants(exclude_op_types=[]))
         model = model.transform(RemoveUnusedTensors())
         model = model.transform(RemoveStaticGraphInputs())
         model = model.transform(InferDataTypes())
     model = model.transform(GiveUniqueNodeNames())
     model = model.transform(GiveReadableTensorNames())
     if output_onnx is not None:
         model.save(output_onnx)
@@ -102,20 +106,21 @@
     mem_o_bits = compute_mem_bits(ret, "mem_o")
     ret["total_bops"] = bops
     ret["total_mem_w_bits"] = mem_w_bits
     ret["total_mem_o_bits"] = mem_o_bits
 
     if "unsupported" in ret:
         ret["unsupported"] = str(ret["unsupported"])
-    print(json.dumps(ret, sort_keys=True, indent=2))
 
     if output_json is not None:
         with open(output_json, "w") as f:
             json.dump(ret, f, sort_keys=True, indent=2)
 
+    return ret
+
 
 def main():
     clize.run(inference_cost)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `qonnx-0.2.0/src/qonnx/util/onnx.py` & `qonnx-0.3.0/src/qonnx/util/onnx.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx/util/to_channels_last.py` & `qonnx-0.3.0/src/qonnx/util/to_channels_last.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/src/qonnx.egg-info/PKG-INFO` & `qonnx-0.3.0/src/qonnx.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: qonnx
-Version: 0.2.0
+Version: 0.3.0
 Summary: Frontend and utilities for QONNX
 Home-page: https://github.com/fastmachinelearning/qonnx
 License: Apache-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: notebooks
 Provides-Extra: qkeras
 Provides-Extra: testing
+Provides-Extra: notebooks
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # QONNX: Arbitrary-Precision Quantized Neural Networks in ONNX
 
 [![ReadTheDocs](https://readthedocs.org/projects/qonnx/badge/?version=latest&style=plastic)](http://qonnx.readthedocs.io/)
 [![GitHub Discussions](https://img.shields.io/github/discussions/fastmachinelearning/qonnx)](https://github.com/fastmachinelearning/qonnx/discussions)
 ![Tests](https://github.com/fastmachinelearning/qonnx/actions/workflows/test.yml/badge.svg)
 ![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7622236.svg)](https://doi.org/10.5281/zenodo.7622236)
+[![PyPI version](https://badge.fury.io/py/qonnx.svg)](https://badge.fury.io/py/qonnx)
+[![Downloads](https://static.pepy.tech/personalized-badge/qonnx?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/qonnx)
 
 <img align="left" src="https://xilinx.github.io/finn/img/TFC_1W2A.onnx.png" alt="QONNX example" style="margin-right: 20px" width="200"/>
 
 
 QONNX (Quantized ONNX) introduces three new custom operators -- [`Quant`](docs/qonnx-custom-ops/quant_op.md), [`BipolarQuant`](docs/qonnx-custom-ops/bipolar_quant_op.md), and [`Trunc`](docs/qonnx-custom-ops/trunc_op.md) -- in order to represent arbitrary-precision uniform quantization in ONNX. This enables:
 * Representation of binary, ternary, 3-bit, 4-bit, 6-bit or any other quantization.
 * Quantization is an operator itself, and can be applied to any parameter or layer input.
@@ -87,51 +89,60 @@
 model = ModelWrapper("my-qonnx-model.onnx")
 idict = {"in0" : np.load("in0.npy), "in1" : np.load("in1.npy")}
 odict = execute_onnx(idict)
 ```
 
 ### Calculate inference cost for QONNX model
 
-Using the `qonnx-inference-cost` command line utility:
+Using the `qonnx-inference-cost` command line utility for the [CNV_2W2A example](https://github.com/fastmachinelearning/qonnx_model_zoo/tree/main/models/CIFAR10/Brevitas_FINN_CNV):
 
 `qonnx-inference-cost CNV_2W2A.onnx`
 
 Which will print a inference cost dictionary like the following:
 
 ```
 Inference cost for CNV_2W2A.onnx
 {
-  "discount_sparsity": true,    # discount MAC counts by layer sparsity (disregard zero-valued MACs)
+  "discount_sparsity": true,    # discount MAC counts by layer sparsity (disregard zero-valued MACs and params)
   # mem_o_X: number of layer outputs with datatype X
-  "mem_o_FLOAT32": 57600.0,     # number of FLOAT32 output elements
-  "mem_o_INT32": 85002.0,       # number of INT32 output elements
+  "mem_o_INT32": 142602.0,       # number of INT32 output elements
   # mem_o_X: number of layer parameters (weights) with datatype X
-  "mem_w_INT2": 1144512.0,      # number of INT2 parameters (weights)
+  "mem_w_INT2": 908033.0,      # number of INT2 parameters (weights)
   # op_mac_X_Y: number of MAC operations, datatype X by datatype Y
-  "op_mac_FLOAT32_INT2": 1555200.0, # number of float32 x int2 MACs
-  "op_mac_INT2_INT2": 57906176.0,   # number of int2 x int2 MACs
-  "total_bops": 331157504.0,        # total number of MACs normalized to bit-ops (BOPS)
+  # scaled integer datatypes have a tensor- or channelwise scale factor
+  "op_mac_SCALEDINT<8>_INT2": 1345500.0, # number of scaled int8 x int2 MACs
+  "op_mac_INT2_INT2": 35615771.0,   # number of int2 x int2 MACs
+  "total_bops": 163991084.0,        # total number of MACs normalized to bit-ops (BOPS)
   "total_mem_o_bits": 4563264.0,    # total number of bits for layer outputs
-  "total_mem_w_bits": 2289024.0,    # total number of bits for layer parameters
+  "total_mem_w_bits": 1816066.0,    # total number of bits for layer parameters
   "unsupported": "set()"
 }
 ```
 
 You can read more about the BOPS metric in [this paper](https://www.frontiersin.org/articles/10.3389/frai.2021.676564/full), Section 4.2 Bit Operations.
 
-### Development
+### Convert between different quantization representations
+
+Using the `qonnx-convert` command line utility you can convert from QONNX to QCDQ-style quantization:
+
+`qonnx-convert CNV_2W2A.onnx`
+
+This will convert `Quant` nodes to `QuantizeLinear -> Clip -> DequantizeLinear` nodes where possible.
+Please see the documentation of the `QuantToQCDQ` transformation to learn more about the limitations.
+
+## Development
 
 Install in editable mode in a venv:
 
 ```
 git clone https://github.com/fastmachinelearning/qonnx
 cd qonnx
 virtualenv -p python3.8 venv
 source venv/bin/activate
-pip install -e .[qkeras,testing]
+pip install -e .[qkeras,testing,docs]
 ```
 
 Run entire test suite, parallelized across CPU cores:
 ```
 pytest -n auto --verbose
 ```
 
@@ -181,9 +192,7 @@
   month        = {06},
   year         = 2022,
   publisher    = {Zenodo},
   doi          = {10.5281/zenodo.7622236},
   url          = {https://github.com/fastmachinelearning/qonnx}
 }
 ```
-
-
```

### Comparing `qonnx-0.2.0/src/qonnx.egg-info/SOURCES.txt` & `qonnx-0.3.0/src/qonnx.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -82,83 +82,103 @@
 src/qonnx/custom_op/general/maxpoolnhwc.py
 src/qonnx/custom_op/general/multithreshold.py
 src/qonnx/custom_op/general/quant.py
 src/qonnx/custom_op/general/quantavgpool2d.py
 src/qonnx/custom_op/general/trunc.py
 src/qonnx/custom_op/general/xnorpopcount.py
 src/qonnx/data/__init__.py
+src/qonnx/data/onnx/bsd300x3-espcn/model.onnx
 src/qonnx/data/onnx/mnist-conv/README.md
 src/qonnx/data/onnx/mnist-conv/model.onnx
 src/qonnx/data/onnx/mnist-conv/test_data_set_0/input_0.pb
 src/qonnx/data/onnx/mnist-conv/test_data_set_0/output_0.pb
 src/qonnx/transformation/__init__.py
 src/qonnx/transformation/base.py
 src/qonnx/transformation/batchnorm_to_affine.py
 src/qonnx/transformation/bipolar_to_xnor.py
 src/qonnx/transformation/change_3d_tensors_to_4d.py
+src/qonnx/transformation/change_batchsize.py
 src/qonnx/transformation/change_datalayout.py
 src/qonnx/transformation/channels_last.py
 src/qonnx/transformation/create_generic_partitions.py
 src/qonnx/transformation/double_to_single_float.py
+src/qonnx/transformation/expose_intermediate.py
 src/qonnx/transformation/extend_partition.py
 src/qonnx/transformation/extract_conv_bias.py
 src/qonnx/transformation/fold_constants.py
 src/qonnx/transformation/gemm_to_matmul.py
 src/qonnx/transformation/general.py
 src/qonnx/transformation/infer_data_layouts.py
 src/qonnx/transformation/infer_datatypes.py
 src/qonnx/transformation/infer_shapes.py
 src/qonnx/transformation/insert_topk.py
 src/qonnx/transformation/lower_convs_to_matmul.py
 src/qonnx/transformation/make_input_chanlast.py
 src/qonnx/transformation/merge_onnx_models.py
+src/qonnx/transformation/pruning.py
+src/qonnx/transformation/qcdq_to_qonnx.py
+src/qonnx/transformation/qonnx_to_qcdq.py
 src/qonnx/transformation/quant_constant_folding.py
 src/qonnx/transformation/rebalance_conv.py
 src/qonnx/transformation/remove.py
+src/qonnx/transformation/subpixel_to_deconv.py
 src/qonnx/util/__init__.py
 src/qonnx/util/basic.py
 src/qonnx/util/cleanup.py
 src/qonnx/util/config.py
+src/qonnx/util/convert.py
 src/qonnx/util/exec_qonnx.py
 src/qonnx/util/inference_cost.py
 src/qonnx/util/onnx.py
+src/qonnx/util/prune_stuck_channels.py
 src/qonnx/util/random_reseed.py
+src/qonnx/util/range_analysis.py
+src/qonnx/util/test.py
 src/qonnx/util/to_channels_last.py
 tests/conftest.py
 tests/test_dummy.py
+tests/analysis/test_inference_cost.py
 tests/analysis/test_is_linear.py
+tests/analysis/test_range_analysis.py
 tests/analysis/test_topology_checks.py
 tests/core/test_basic_onnx_exec.py
 tests/core/test_custom_onnx_exec.py
 tests/core/test_datatypes.py
 tests/core/test_mixed_onnx_exec.py
 tests/core/test_modelwrapper.py
 tests/custom_op/test_attr.py
 tests/custom_op/test_im2col.py
 tests/custom_op/test_multithreshold.py
 tests/custom_op/test_xnorpopcountmatmul.py
 tests/keras/test_keras_convert.py
 tests/transformation/test_4d_conversion.py
 tests/transformation/test_batchnorm_to_affine.py
+tests/transformation/test_change_batchsize.py
 tests/transformation/test_change_datalayout.py
 tests/transformation/test_channelslast.py
 tests/transformation/test_conv_lowering.py
+tests/transformation/test_expose_intermediate.py
 tests/transformation/test_extend_partition.py
 tests/transformation/test_fold_constants.py
 tests/transformation/test_general_transformation.py
 tests/transformation/test_generic_partitioning.py
 tests/transformation/test_infer_data_layouts.py
 tests/transformation/test_infer_datatypes.py
 tests/transformation/test_infer_shapes.py
 tests/transformation/test_make_input_chanlast.py
 tests/transformation/test_merge_onnx_models.py
 tests/transformation/test_nodelocal_transform.py
+tests/transformation/test_pruning.py
+tests/transformation/test_qcdq_to_qonnx.py
 tests/transformation/test_qonnx_cleanup.py
+tests/transformation/test_qonnx_to_qcdq.py
 tests/transformation/test_rebalance_conv.py
 tests/transformation/test_remove_identity_ops.py
+tests/transformation/test_remove_unused.py
 tests/transformation/test_renaming.py
 tests/transformation/test_sort_graph.py
+tests/transformation/test_subpixel_to_deconv.py
 tests/transformation/test_topk_insert.py
 tests/util/test_gen_finn_dt_tensor.py
 tests/util/test_matvec_range.py
 tests/util/test_padding.py
 tests/util/test_shape_utils.py
```

### Comparing `qonnx-0.2.0/tests/analysis/test_is_linear.py` & `qonnx-0.3.0/tests/analysis/test_is_linear.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/analysis/test_topology_checks.py` & `qonnx-0.3.0/tests/analysis/test_topology_checks.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/core/test_basic_onnx_exec.py` & `qonnx-0.3.0/tests/core/test_basic_onnx_exec.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/core/test_custom_onnx_exec.py` & `qonnx-0.3.0/tests/core/test_custom_onnx_exec.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/core/test_datatypes.py` & `qonnx-0.3.0/tests/core/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/core/test_mixed_onnx_exec.py` & `qonnx-0.3.0/tests/core/test_mixed_onnx_exec.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/core/test_modelwrapper.py` & `qonnx-0.3.0/tests/core/test_modelwrapper.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/custom_op/test_attr.py` & `qonnx-0.3.0/tests/custom_op/test_attr.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/custom_op/test_im2col.py` & `qonnx-0.3.0/tests/custom_op/test_im2col.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/custom_op/test_multithreshold.py` & `qonnx-0.3.0/tests/custom_op/test_multithreshold.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/custom_op/test_xnorpopcountmatmul.py` & `qonnx-0.3.0/tests/custom_op/test_xnorpopcountmatmul.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/keras/test_keras_convert.py` & `qonnx-0.3.0/tests/keras/test_keras_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     onnx_model = onnx_model.transform(InferShapes())
 
     idict = {onnx_model.graph.input[0].name: x_test}
     odict = oxe.execute_onnx(onnx_model, idict, True)
     y_qonnx = odict[onnx_model.graph.output[0].name]
 
     np.testing.assert_allclose(y_qkeras, y_qonnx, rtol=1e-5, atol=1e-5)
+    os.remove(model_path)
 
 
 # pairs of quantizers for kernel and bias
 kb_quantizers = [
     (quantized_bits(8, 4, 0, alpha=1), quantized_bits(8, 4, 0, alpha=1)),
     (quantized_bits(8, 4, 1, alpha=1), quantized_bits(8, 4, 1, alpha=1)),
     (quantized_bits(8, 8, 0, alpha=1), quantized_bits(8, 8, 0, alpha=1)),
```

### Comparing `qonnx-0.2.0/tests/transformation/test_4d_conversion.py` & `qonnx-0.3.0/tests/transformation/test_4d_conversion.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/transformation/test_batchnorm_to_affine.py` & `qonnx-0.3.0/tests/transformation/test_batchnorm_to_affine.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         pytest.skip("Couldn't download ONNX model, skipping")
     model = ModelWrapper(export_onnx_path)
     model = model.transform(InferShapes())
     model = model.transform(FoldConstants())
     iname = model.graph.input[0].name
     oname = model.graph.output[0].name
     ishape = model.get_tensor_shape(iname)
+    np.random.seed(0)
     rand_inp = gen_finn_dt_tensor(DataType["INT8"], ishape)
     input_dict = {iname: rand_inp}
     expected = oxe.execute_onnx(model, input_dict)[oname]
     new_model = model.transform(BatchNormToAffine())
     # check that there are no BN nodes left
     op_types = list(map(lambda x: x.op_type, new_model.graph.node))
     assert "BatchNormalization" not in op_types
```

### Comparing `qonnx-0.2.0/tests/transformation/test_change_datalayout.py` & `qonnx-0.3.0/tests/transformation/test_change_datalayout.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/transformation/test_channelslast.py` & `qonnx-0.3.0/tests/transformation/test_channelslast.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 
 import numpy as np
-import urllib.request
 
 import qonnx.core.onnx_exec as oxe
 from qonnx.core.modelwrapper import ModelWrapper
 from qonnx.custom_op import channels_last
 from qonnx.custom_op.channels_last.base_wrapped_op import to_channels_last_args
 from qonnx.custom_op.registry import getCustomOp
 from qonnx.transformation.channels_last import (
@@ -16,80 +15,34 @@
     RemoveConsecutiveChanFirstAndChanLastTrafos,
 )
 from qonnx.transformation.general import GiveUniqueNodeNames
 from qonnx.transformation.infer_shapes import InferShapes
 from qonnx.transformation.make_input_chanlast import MakeInputChannelsLast
 from qonnx.transformation.quant_constant_folding import FoldTransposeIntoQuantInit
 from qonnx.util.basic import is_finn_op
-from qonnx.util.cleanup import cleanup
+from qonnx.util.test import download_model, get_golden_in_and_output, test_model_details
 from qonnx.util.to_channels_last import to_channels_last
 
-model_details = {
+model_details_chanlast = {
     "FINN-CNV_W2A2": {
-        "url": (
-            "https://raw.githubusercontent.com/fastmachinelearning/"
-            "QONNX_model_zoo/main/models/CIFAR10/Brevitas_FINN_CNV/CNV_2W2A.onnx"
-        ),
-        "input_shape": (1, 3, 32, 32),
-        "input_range": (-1, +1),
         "layout_sensitive": True,
     },
     "FINN-TFC_W2A2": {
-        "url": (
-            "https://github.com/fastmachinelearning/QONNX_model_zoo/"
-            "raw/main/models/MNIST/Brevitas_FINN_TFC/TFC/TFC_2W2A.onnx"
-        ),
-        "input_shape": (1, 1, 28, 28),
-        "input_range": (-1, +1),
         "layout_sensitive": False,
     },
     "RadioML_VGG10": {
-        "url": (
-            "https://github.com/Xilinx/brevitas-radioml-challenge-21/raw/"
-            "9eef6a2417d6a0c078bfcc3a4dc95033739c5550/sandbox/notebooks/models/pretrained_VGG10_w8a8_20_export.onnx"
-        ),
-        "input_shape": (1, 2, 1024),
-        "input_range": (-1, +1),
         "layout_sensitive": True,
     },
     "Conv_bias_example": {
-        "url": "https://zenodo.org/record/7626922/files/super_resolution.onnx",
-        "input_shape": (1, 1, 28, 28),
-        "input_range": (-1, +1),
         "layout_sensitive": True,
     },
 }
-
-
-def download_model(test_model):
-    qonnx_url = model_details[test_model]["url"]
-    # download test data
-    dl_dir = "/tmp"
-    dl_file = dl_dir + f"/{test_model}.onnx"
-    urllib.request.urlretrieve(qonnx_url, dl_file)
-    # run cleanup with default settings
-    out_file = dl_dir + f"/{test_model}_clean.onnx"
-    cleanup(dl_file, out_file=out_file)
-    return out_file
-
-
-def get_golden_in_and_output(onnx_file, test_model):
-    rng = np.random.RandomState(42)
-    input_shape = model_details[test_model]["input_shape"]
-    (low, high) = model_details[test_model]["input_range"]
-    size = np.prod(np.asarray(input_shape))
-    input_tensor = rng.uniform(low=low, high=high, size=size)
-    input_tensor = input_tensor.astype(np.float32)
-    input_tensor = input_tensor.reshape(input_shape)
-    model = ModelWrapper(onnx_file)
-    input_dict = {model.graph.input[0].name: input_tensor}
-    golden_output_dict = oxe.execute_onnx(model, input_dict)
-    golden_result = golden_output_dict[model.graph.output[0].name]
-
-    return input_tensor, golden_result
+# inherit basics for matching testcases from test util
+model_details = {k: v for (k, v) in test_model_details.items() if k in model_details_chanlast.keys()}
+model_details = {**model_details, **model_details_chanlast}
 
 
 def analysis_testing_for_chanlast_domain(model):
     # Define for each ChannelsLast operation the number of minimum dimensions, it needs to have
     ChanLast_node_types_and_min_dim_input = {
         "Conv": 3,
         "MaxPool": 3,
@@ -144,16 +97,16 @@
     return result
 
 
 @pytest.mark.parametrize("make_input_channels_last", [True, False])
 @pytest.mark.parametrize("test_model", model_details.keys())
 def test_channelslast_conversion_end2end(test_model, make_input_channels_last):
     # Download an clean model
-    onnx_file = download_model(test_model)
-    input_tensor, golden_result = get_golden_in_and_output(onnx_file, test_model)
+    onnx_file = download_model(test_model, do_cleanup=True)
+    input_tensor, golden_result = get_golden_in_and_output(test_model)
 
     # Execute transformation
     qonnx_all_trafos = onnx_file.split(".onnx")[0] + "_all_nhwc_trafos_test.onnx"
     to_channels_last(onnx_file, make_input_channels_last=make_input_channels_last, out_file=qonnx_all_trafos)
 
     # Check output
     model = ModelWrapper(qonnx_all_trafos)
@@ -181,16 +134,16 @@
     if (not make_input_channels_last) and (model_details[test_model]["layout_sensitive"]):
         _ = model.analysis(analysis_first_node_is_transpose)
 
 
 @pytest.mark.parametrize("test_model", model_details.keys())
 def test_channelslast_conversion_step_by_step(test_model):
     # Download an clean model
-    onnx_file = download_model(test_model)
-    input_tensor, golden_result = get_golden_in_and_output(onnx_file, test_model)
+    onnx_file = download_model(test_model, do_cleanup=True)
+    input_tensor, golden_result = get_golden_in_and_output(test_model)
 
     # Execute transformation
     model = ModelWrapper(onnx_file)
     qonnx_all_trafos = onnx_file.split(".onnx")[0] + "_all_nhwc_trafos.onnx"
 
     # Run trafo
     model = model.transform(InsertChannelsLastDomainsAndTrafos())
```

### Comparing `qonnx-0.2.0/tests/transformation/test_conv_lowering.py` & `qonnx-0.3.0/tests/transformation/test_conv_lowering.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/transformation/test_extend_partition.py` & `qonnx-0.3.0/tests/transformation/test_extend_partition.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/transformation/test_fold_constants.py` & `qonnx-0.3.0/tests/transformation/test_fold_constants.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/transformation/test_general_transformation.py` & `qonnx-0.3.0/tests/transformation/test_general_transformation.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/transformation/test_generic_partitioning.py` & `qonnx-0.3.0/tests/transformation/test_generic_partitioning.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/transformation/test_infer_data_layouts.py` & `qonnx-0.3.0/tests/transformation/test_infer_data_layouts.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/transformation/test_infer_datatypes.py` & `qonnx-0.3.0/tests/transformation/test_nodelocal_transform.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020, Xilinx
+# Copyright (c) 2022, Xilinx
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -22,34 +22,36 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import numpy as np
+import onnx.helper as oh
 from pkgutil import get_data
 
-from qonnx.core.datatype import DataType
 from qonnx.core.modelwrapper import ModelWrapper
-from qonnx.transformation.fold_constants import FoldConstants
-from qonnx.transformation.general import GiveReadableTensorNames, GiveUniqueNodeNames
-from qonnx.transformation.infer_datatypes import InferDataTypes
-from qonnx.transformation.infer_shapes import InferShapes
+from qonnx.transformation.base import NodeLocalTransformation
+from qonnx.util.basic import get_by_name
 
 
-def test_infer_datatypes():
+class SumAndAnnotateConvWeights(NodeLocalTransformation):
+    def applyNodeLocal(self, node):
+        if node.op_type == "Conv":
+            # read conv weight tensor from model
+            W = self.ref_input_model.get_initializer(node.input[1])
+            sum = float(np.sum(W))
+            # add a dummy attribute for verification
+            attr_proto = oh.make_attribute("conv_w_sum", sum)
+            node.attribute.append(attr_proto)
+        return (node, False)
+
+
+def test_nodelocal_transform():
+    # load the onnx model
     raw_m = get_data("qonnx.data", "onnx/mnist-conv/model.onnx")
     model = ModelWrapper(raw_m)
-    model = model.transform(InferShapes())
-    model = model.transform(FoldConstants())
-    model = model.transform(GiveUniqueNodeNames())
-    model = model.transform(GiveReadableTensorNames())
-    # this model has no DataType info, so add some DataType annotation
-    # to make things a bit more exciting
-    model.set_tensor_datatype("global_in", DataType["UINT8"])
-    # Conv with int weights + inputs will have int output datatype
-    model.set_tensor_datatype("Conv_0_param0", DataType["INT4"])
-    model = model.transform(InferDataTypes())
-    assert model.get_tensor_datatype("global_in") == DataType["UINT8"]
-    assert model.get_tensor_datatype("Conv_0_out0") == DataType["INT32"]
-    assert model.get_tensor_datatype("Relu_0_out0") == DataType["FLOAT32"]
-    assert model.get_tensor_datatype("global_out") == DataType["FLOAT32"]
+    model = model.transform(SumAndAnnotateConvWeights())
+    for conv_node in model.get_nodes_by_op_type("Conv"):
+        wsum = float(np.sum(model.get_initializer(conv_node.input[1])))
+        assert get_by_name(conv_node.attribute, "conv_w_sum").f == wsum
```

### Comparing `qonnx-0.2.0/tests/transformation/test_infer_shapes.py` & `qonnx-0.3.0/tests/transformation/test_infer_shapes.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/transformation/test_make_input_chanlast.py` & `qonnx-0.3.0/tests/transformation/test_make_input_chanlast.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/transformation/test_merge_onnx_models.py` & `qonnx-0.3.0/tests/transformation/test_merge_onnx_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,15 +69,16 @@
         nodes=[mul_node, div_node],
         name="model2-graph",
         inputs=[inp],
         outputs=[outp],
         value_info=[a0, a1],
     )
 
-    model2 = qonnx_make_model(graph, producer_name="model2")
+    exp_opset_id = 13
+    model2 = qonnx_make_model(graph, producer_name="model2", opset_imports=[helper.make_opsetid("", exp_opset_id)])
     model2 = ModelWrapper(model2)
     # initialize model2
     a0_value = np.random.uniform(low=0, high=1, size=(1)).astype(np.float32)
     model2.set_initializer("a0", a0_value)
     a1_value = np.random.uniform(low=0.1, high=1, size=(1)).astype(np.float32)
     model2.set_initializer("a1", a1_value)
     # set a dummy sparsity annotation to check if it gets correctly transferred
@@ -118,7 +119,9 @@
         if n.op_type == "Div":
             tensor_name = n.input[1]
             set_sparsity = model_transformed.get_tensor_sparsity(tensor_name)
             assert sparsity == set_sparsity
 
     # check if finn datatype of graph.input[0] is still set to UINT8
     assert model_transformed.get_tensor_datatype("global_in") == DataType["UINT8"]
+    # check that the merged model uses the greater of the two input opsets
+    assert model_transformed.model.opset_import[0].version == exp_opset_id
```

### Comparing `qonnx-0.2.0/tests/transformation/test_qonnx_cleanup.py` & `qonnx-0.3.0/tests/transformation/test_qonnx_cleanup.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/transformation/test_rebalance_conv.py` & `qonnx-0.3.0/tests/transformation/test_rebalance_conv.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/transformation/test_remove_identity_ops.py` & `qonnx-0.3.0/tests/transformation/test_remove_identity_ops.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/transformation/test_renaming.py` & `qonnx-0.3.0/tests/transformation/test_renaming.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/transformation/test_sort_graph.py` & `qonnx-0.3.0/tests/transformation/test_sort_graph.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/transformation/test_topk_insert.py` & `qonnx-0.3.0/tests/transformation/test_topk_insert.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/util/test_gen_finn_dt_tensor.py` & `qonnx-0.3.0/tests/util/test_gen_finn_dt_tensor.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/util/test_matvec_range.py` & `qonnx-0.3.0/tests/util/test_matvec_range.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/util/test_padding.py` & `qonnx-0.3.0/tests/util/test_padding.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tests/util/test_shape_utils.py` & `qonnx-0.3.0/tests/util/test_shape_utils.py`

 * *Files identical despite different names*

### Comparing `qonnx-0.2.0/tox.ini` & `qonnx-0.3.0/tox.ini`

 * *Files identical despite different names*

