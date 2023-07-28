# Comparing `tmp/truss-0.5.1.tar.gz` & `tmp/truss-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.5.1.tar", max compression
+gzip compressed data, was "truss-0.5.2.tar", max compression
```

## Comparing `truss-0.5.1.tar` & `truss-0.5.2.tar`

### file list

```diff
@@ -1,217 +1,217 @@
--rw-r--r--   0        0        0     5483 2023-07-26 21:14:15.359366 truss-0.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2418 2023-07-26 21:14:15.363366 truss-0.5.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2023-07-26 21:14:15.363366 truss-0.5.1/LICENSE
--rw-r--r--   0        0        0     3415 2023-07-26 21:14:15.363366 truss-0.5.1/README.md
--rw-r--r--   0        0        0      933 2023-07-26 21:14:15.363366 truss-0.5.1/context_builder.Dockerfile
--rw-r--r--   0        0        0     2546 2023-07-26 21:14:15.435366 truss-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      330 2023-07-26 21:14:15.435366 truss-0.5.1/truss/__init__.py
--rw-r--r--   0        0        0      252 2023-07-26 21:14:15.435366 truss-0.5.1/truss/blob/blob_backend.py
--rw-r--r--   0        0        0      733 2023-07-26 21:14:15.435366 truss-0.5.1/truss/blob/blob_backend_registry.py
--rw-r--r--   0        0        0      648 2023-07-26 21:14:15.435366 truss-0.5.1/truss/blob/http_public_blob_backend.py
--rw-r--r--   0        0        0    13068 2023-07-26 21:14:15.439365 truss-0.5.1/truss/build.py
--rw-r--r--   0        0        0    11021 2023-07-26 21:14:15.439365 truss-0.5.1/truss/cli.py
--rw-r--r--   0        0        0     2873 2023-07-26 21:14:15.439365 truss-0.5.1/truss/constants.py
--rw-r--r--   0        0        0      338 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/image_builder/cache_warmer.py
--rw-r--r--   0        0        0     1294 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0     7028 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     4684 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/image_builder/training_image_builder.py
--rw-r--r--   0        0        0     1893 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     2120 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/local_loader/docker_build_emulator.py
--rw-r--r--   0        0        0     1823 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     2239 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/local_loader/train_local.py
--rw-r--r--   0        0        0     1072 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/local_loader/truss_file_syncer.py
--rw-r--r--   0        0        0     5801 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2023-07-26 21:14:15.439365 truss-0.5.1/truss/decorators.py
--rw-r--r--   0        0        0     3641 2023-07-26 21:14:15.439365 truss-0.5.1/truss/docker.py
--rw-r--r--   0        0        0     3759 2023-07-26 21:14:15.439365 truss-0.5.1/truss/environment_inference/requirements_inference.py
--rw-r--r--   0        0        0      643 2023-07-26 21:14:15.439365 truss-0.5.1/truss/errors.py
--rw-r--r--   0        0        0      824 2023-07-26 21:14:15.439365 truss-0.5.1/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2023-07-26 21:14:15.439365 truss-0.5.1/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     2713 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_framework.py
--rw-r--r--   0        0        0     1687 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/__init__.py
--rw-r--r--   0        0        0     1895 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/huggingface_transformer.py
--rw-r--r--   0        0        0      918 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/keras.py
--rw-r--r--   0        0        0     1230 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/lightgbm.py
--rw-r--r--   0        0        0     2403 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/mlflow.py
--rw-r--r--   0        0        0     2441 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/pytorch.py
--rw-r--r--   0        0        0     1225 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/sklearn.py
--rw-r--r--   0        0        0     1027 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/xgboost.py
--rw-r--r--   0        0        0     5425 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_inference.py
--rw-r--r--   0        0        0      510 2023-07-26 21:14:15.439365 truss-0.5.1/truss/notebook.py
--rw-r--r--   0        0        0    15420 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      139 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/constants.py
--rw-r--r--   0        0        0      774 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2378 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/hash.py
--rw-r--r--   0        0        0     2930 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/local_truss_patch_applier.py
--rw-r--r--   0        0        0      468 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/signature.py
--rw-r--r--   0        0        0     3075 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/truss_dir_patch_applier.py
--rw-r--r--   0        0        0      937 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/types.py
--rw-r--r--   0        0        0      237 2023-07-26 21:14:15.439365 truss-0.5.1/truss/pytest.ini
--rw-r--r--   0        0        0      705 2023-07-26 21:14:15.439365 truss-0.5.1/truss/readme_generator.py
--rw-r--r--   0        0        0      176 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/__init__.py
--rw-r--r--   0        0        0     4919 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/api.py
--rw-r--r--   0        0        0      752 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/auth.py
--rw-r--r--   0        0        0     3616 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/core.py
--rw-r--r--   0        0        0      943 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/error.py
--rw-r--r--   0        0        0     4639 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/remote.py
--rw-r--r--   0        0        0     1156 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/service.py
--rw-r--r--   0        0        0     2001 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/utils/tar.py
--rw-r--r--   0        0        0      985 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/utils/transfer.py
--rw-r--r--   0        0        0     1407 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/remote_cli.py
--rw-r--r--   0        0        0     4219 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/remote_factory.py
--rw-r--r--   0        0        0     5970 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/truss_remote.py
--rw-r--r--   0        0        0     2482 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/__init__.py
--rw-r--r--   0        0        0     1967 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     3819 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     5103 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      955 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     6317 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     4026 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2652 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0      998 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/truss_patch/__init__.py
--rw-r--r--   0        0        0     1842 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
--rw-r--r--   0        0        0     7386 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
--rw-r--r--   0        0        0      551 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
--rw-r--r--   0        0        0      208 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/truss_patch/system_packages.py
--rw-r--r--   0        0        0     5930 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     2319 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/server.py
--rw-r--r--   0        0        0      144 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       48 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0      534 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0      460 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/custom/train/train.py
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/huggingface_transformer/model/__init__.py
--rw-r--r--   0        0        0     1827 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/huggingface_transformer/model/model.py
--rw-r--r--   0        0        0       47 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/huggingface_transformer/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/keras/model/__init__.py
--rw-r--r--   0        0        0      728 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/keras/model/model.py
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/lightgbm/model/__init__.py
--rw-r--r--   0        0        0     1251 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/lightgbm/model/model.py
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/mlflow/model/__init__.py
--rw-r--r--   0        0        0      751 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/mlflow/model/model.py
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/pipeline/model/__init__.py
--rw-r--r--   0        0        0      430 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/pipeline/model/model.py
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/pytorch/model/__init__.py
--rw-r--r--   0        0        0     1263 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/pytorch/model/model.py
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0     2433 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     2382 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server/common/patches/whisper/patch.py
--rw-r--r--   0        0        0     1450 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server/common/patches.py
--rw-r--r--   0        0        0      593 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server/common/retry.py
--rw-r--r--   0        0        0     2340 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server/common/termination_handler_middleware.py
--rw-r--r--   0        0        0    12328 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0      727 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0    11624 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      274 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0     3279 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/shared/logging.py
--rw-r--r--   0        0        0     1430 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0     3318 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/shared/serialization.py
--rw-r--r--   0        0        0     1863 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/shared/util.py
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/sklearn/model/__init__.py
--rw-r--r--   0        0        0     1221 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/sklearn/model/model.py
--rw-r--r--   0        0        0     3400 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/training/job.py
--rw-r--r--   0        0        0       12 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/training/requirements.txt
--rw-r--r--   0        0        0      491 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/training.Dockerfile.jinja
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/xgboost/model/__init__.py
--rw-r--r--   0        0        0     1453 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/xgboost/model/model.py
--rw-r--r--   0        0        0    30286 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0       93 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0     1394 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0      739 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/model_load_failure_test/config.yaml
--rw-r--r--   0        0        0      552 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/model_load_failure_test/model/model.py
--rw-r--r--   0        0        0     1267 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0     1550 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/server.Dockerfile
--rw-r--r--   0        0        0      669 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/server_conformance_test_truss/config.yaml
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/server_conformance_test_truss/model/__init__.py
--rw-r--r--   0        0        0      597 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/server_conformance_test_truss/model/model.py
--rw-r--r--   0        0        0      739 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_async_truss/config.yaml
--rw-r--r--   0        0        0      646 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_async_truss/model/model.py
--rw-r--r--   0        0        0       34 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_concurrency_truss/config.yaml
--rw-r--r--   0        0        0      547 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_concurrency_truss/model/model.py
--rw-r--r--   0        0        0      739 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_streaming_async_generator_truss/config.yaml
--rw-r--r--   0        0        0      521 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_streaming_async_generator_truss/model/model.py
--rw-r--r--   0        0        0      773 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_streaming_truss/config.yaml
--rw-r--r--   0        0        0      568 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_streaming_truss/model/model.py
--rw-r--r--   0        0        0      669 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0      534 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        6 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_truss/packages/test_package/test.py
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/__init__.py
--rw-r--r--   0        0        0    22226 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/conftest.py
--rw-r--r--   0        0        0     1255 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/contexts/image_builder/test_serving_image_builder.py
--rw-r--r--   0        0        0      783 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      968 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/environments_inference/test_requirements_inference.py
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/model_frameworks/__init__.py
--rw-r--r--   0        0        0     3293 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
--rw-r--r--   0        0        0     2789 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/model_frameworks/test_keras_framework.py
--rw-r--r--   0        0        0     2409 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/model_frameworks/test_lightgbm_framework.py
--rw-r--r--   0        0        0     1479 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/model_frameworks/test_pytorch_framework.py
--rw-r--r--   0        0        0     2427 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/model_frameworks/test_sklearn_framework.py
--rw-r--r--   0        0        0     2437 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/model_frameworks/test_xgboost_framework.py
--rw-r--r--   0        0        0    18726 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0      487 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      394 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0     1929 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/patch/test_truss_dir_patch_applier.py
--rw-r--r--   0        0        0      273 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0     2073 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/remote/baseten/test_api.py
--rw-r--r--   0        0        0      580 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/remote/baseten/test_auth.py
--rw-r--r--   0        0        0      835 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/remote/baseten/test_core.py
--rw-r--r--   0        0        0     4316 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/remote/test_remote_factory.py
--rw-r--r--   0        0        0     2394 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/remote/test_truss_remote.py
--rw-r--r--   0        0        0    10415 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/samples.py
--rw-r--r--   0        0        0      283 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     6081 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
--rw-r--r--   0        0        0      964 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
--rw-r--r--   0        0        0     7513 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0     8326 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/control/control/test_server_integration.py
--rw-r--r--   0        0        0     1560 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/core/server/common/test_truss_server.py
--rw-r--r--   0        0        0      821 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     2038 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/server/common/test_retry.py
--rw-r--r--   0        0        0     2605 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/server/common/test_termination_handler_middleware.py
--rw-r--r--   0        0        0     2252 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/server/test_model_wrapper.py
--rw-r--r--   0        0        0     1910 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/test_backward.py
--rw-r--r--   0        0        0     8260 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/test_build.py
--rw-r--r--   0        0        0     8657 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0    14982 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_control_truss_patching.py
--rw-r--r--   0        0        0      517 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_docker.py
--rw-r--r--   0        0        0    12242 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0      656 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_notebooks.py
--rw-r--r--   0        0        0     1483 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    30057 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0     1865 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_validation.py
--rw-r--r--   0        0        0     4974 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/util/test_path.py
--rw-r--r--   0        0        0    15256 2023-07-26 21:14:15.447366 truss-0.5.1/truss/truss_config.py
--rw-r--r--   0        0        0     2698 2023-07-26 21:14:15.447366 truss-0.5.1/truss/truss_gatherer.py
--rw-r--r--   0        0        0    41143 2023-07-26 21:14:15.447366 truss-0.5.1/truss/truss_handle.py
--rw-r--r--   0        0        0     5671 2023-07-26 21:14:15.447366 truss-0.5.1/truss/truss_spec.py
--rw-r--r--   0        0        0     2782 2023-07-26 21:14:15.447366 truss-0.5.1/truss/types.py
--rw-r--r--   0        0        0     3121 2023-07-26 21:14:15.447366 truss-0.5.1/truss/util/.truss_ignore
--rw-r--r--   0        0        0      379 2023-07-26 21:14:15.447366 truss-0.5.1/truss/util/data_structures.py
--rw-r--r--   0        0        0     2552 2023-07-26 21:14:15.447366 truss-0.5.1/truss/util/download.py
--rw-r--r--   0        0        0      553 2023-07-26 21:14:15.447366 truss-0.5.1/truss/util/gpu.py
--rw-r--r--   0        0        0      333 2023-07-26 21:14:15.447366 truss-0.5.1/truss/util/jinja.py
--rw-r--r--   0        0        0     6040 2023-07-26 21:14:15.447366 truss-0.5.1/truss/util/path.py
--rw-r--r--   0        0        0     2736 2023-07-26 21:14:15.447366 truss-0.5.1/truss/validation.py
--rw-r--r--   0        0        0     5343 1970-01-01 00:00:00.000000 truss-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     5483 2023-07-28 22:19:05.925630 truss-0.5.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2418 2023-07-28 22:19:05.925630 truss-0.5.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2023-07-28 22:19:05.925630 truss-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3518 2023-07-28 22:19:05.925630 truss-0.5.2/README.md
+-rw-r--r--   0        0        0      933 2023-07-28 22:19:05.925630 truss-0.5.2/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2546 2023-07-28 22:19:06.033645 truss-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-07-28 22:19:06.033645 truss-0.5.2/truss/__init__.py
+-rw-r--r--   0        0        0      252 2023-07-28 22:19:06.033645 truss-0.5.2/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2023-07-28 22:19:06.033645 truss-0.5.2/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2023-07-28 22:19:06.033645 truss-0.5.2/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0    13068 2023-07-28 22:19:06.033645 truss-0.5.2/truss/build.py
+-rw-r--r--   0        0        0    11216 2023-07-28 22:19:06.033645 truss-0.5.2/truss/cli.py
+-rw-r--r--   0        0        0     2873 2023-07-28 22:19:06.033645 truss-0.5.2/truss/constants.py
+-rw-r--r--   0        0        0      338 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/image_builder/cache_warmer.py
+-rw-r--r--   0        0        0     1294 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0     7028 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     4684 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/image_builder/training_image_builder.py
+-rw-r--r--   0        0        0     1893 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     2120 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/local_loader/docker_build_emulator.py
+-rw-r--r--   0        0        0     1823 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     2239 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/local_loader/train_local.py
+-rw-r--r--   0        0        0     1072 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/local_loader/truss_file_syncer.py
+-rw-r--r--   0        0        0     5801 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2023-07-28 22:19:06.033645 truss-0.5.2/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2023-07-28 22:19:06.033645 truss-0.5.2/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2023-07-28 22:19:06.033645 truss-0.5.2/truss/docker.py
+-rw-r--r--   0        0        0     3759 2023-07-28 22:19:06.033645 truss-0.5.2/truss/environment_inference/requirements_inference.py
+-rw-r--r--   0        0        0      643 2023-07-28 22:19:06.033645 truss-0.5.2/truss/errors.py
+-rw-r--r--   0        0        0      824 2023-07-28 22:19:06.033645 truss-0.5.2/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2023-07-28 22:19:06.033645 truss-0.5.2/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     2713 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_framework.py
+-rw-r--r--   0        0        0     1687 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     1895 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/huggingface_transformer.py
+-rw-r--r--   0        0        0      918 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/keras.py
+-rw-r--r--   0        0        0     1230 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/lightgbm.py
+-rw-r--r--   0        0        0     2403 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/mlflow.py
+-rw-r--r--   0        0        0     2441 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/pytorch.py
+-rw-r--r--   0        0        0     1225 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/sklearn.py
+-rw-r--r--   0        0        0     1027 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_frameworks/xgboost.py
+-rw-r--r--   0        0        0     5425 2023-07-28 22:19:06.033645 truss-0.5.2/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2023-07-28 22:19:06.033645 truss-0.5.2/truss/notebook.py
+-rw-r--r--   0        0        0    15420 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      139 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/constants.py
+-rw-r--r--   0        0        0      774 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2378 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/hash.py
+-rw-r--r--   0        0        0     2930 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/local_truss_patch_applier.py
+-rw-r--r--   0        0        0      468 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/signature.py
+-rw-r--r--   0        0        0     3075 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      937 2023-07-28 22:19:06.033645 truss-0.5.2/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2023-07-28 22:19:06.033645 truss-0.5.2/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2023-07-28 22:19:06.033645 truss-0.5.2/truss/readme_generator.py
+-rw-r--r--   0        0        0      176 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/__init__.py
+-rw-r--r--   0        0        0     4919 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/api.py
+-rw-r--r--   0        0        0      752 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/auth.py
+-rw-r--r--   0        0        0     3616 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/core.py
+-rw-r--r--   0        0        0      943 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/error.py
+-rw-r--r--   0        0        0     4741 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/remote.py
+-rw-r--r--   0        0        0     1156 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/service.py
+-rw-r--r--   0        0        0     2001 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/utils/tar.py
+-rw-r--r--   0        0        0      985 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/baseten/utils/transfer.py
+-rw-r--r--   0        0        0     1407 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/remote_cli.py
+-rw-r--r--   0        0        0     4219 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/remote_factory.py
+-rw-r--r--   0        0        0     5970 2023-07-28 22:19:06.033645 truss-0.5.2/truss/remote/truss_remote.py
+-rw-r--r--   0        0        0     2482 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/__init__.py
+-rw-r--r--   0        0        0     1967 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     3819 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     5103 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      955 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     6317 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     4026 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2652 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0      998 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/truss_patch/__init__.py
+-rw-r--r--   0        0        0     1842 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
+-rw-r--r--   0        0        0     7386 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
+-rw-r--r--   0        0        0      551 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
+-rw-r--r--   0        0        0      208 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/truss_patch/system_packages.py
+-rw-r--r--   0        0        0     5930 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     2319 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0      144 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       48 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0      534 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0      460 2023-07-28 22:19:06.033645 truss-0.5.2/truss/templates/custom/train/train.py
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/huggingface_transformer/model/__init__.py
+-rw-r--r--   0        0        0     1827 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/huggingface_transformer/model/model.py
+-rw-r--r--   0        0        0       47 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/huggingface_transformer/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/keras/model/__init__.py
+-rw-r--r--   0        0        0      728 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/keras/model/model.py
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/lightgbm/model/__init__.py
+-rw-r--r--   0        0        0     1251 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/lightgbm/model/model.py
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/mlflow/model/__init__.py
+-rw-r--r--   0        0        0      751 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/mlflow/model/model.py
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/pipeline/model/__init__.py
+-rw-r--r--   0        0        0      430 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/pipeline/model/model.py
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/pytorch/model/__init__.py
+-rw-r--r--   0        0        0     1263 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/pytorch/model/model.py
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0     2433 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     2382 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/common/patches/whisper/patch.py
+-rw-r--r--   0        0        0     1450 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/common/patches.py
+-rw-r--r--   0        0        0      593 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/common/retry.py
+-rw-r--r--   0        0        0     2340 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/common/termination_handler_middleware.py
+-rw-r--r--   0        0        0    12328 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0      727 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0    11624 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      274 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     3279 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/shared/logging.py
+-rw-r--r--   0        0        0     1430 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0     3318 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/shared/serialization.py
+-rw-r--r--   0        0        0     1863 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/shared/util.py
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/sklearn/model/__init__.py
+-rw-r--r--   0        0        0     1221 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/sklearn/model/model.py
+-rw-r--r--   0        0        0     3400 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/training/job.py
+-rw-r--r--   0        0        0       12 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/training/requirements.txt
+-rw-r--r--   0        0        0      491 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/training.Dockerfile.jinja
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/xgboost/model/__init__.py
+-rw-r--r--   0        0        0     1453 2023-07-28 22:19:06.037646 truss-0.5.2/truss/templates/xgboost/model/model.py
+-rw-r--r--   0        0        0    30286 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0       93 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0     1394 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0      739 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/model_load_failure_test/config.yaml
+-rw-r--r--   0        0        0      552 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/model_load_failure_test/model/model.py
+-rw-r--r--   0        0        0     1267 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0     1550 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/server.Dockerfile
+-rw-r--r--   0        0        0      669 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/server_conformance_test_truss/config.yaml
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/server_conformance_test_truss/model/__init__.py
+-rw-r--r--   0        0        0      597 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/server_conformance_test_truss/model/model.py
+-rw-r--r--   0        0        0      739 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_async_truss/config.yaml
+-rw-r--r--   0        0        0      646 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_async_truss/model/model.py
+-rw-r--r--   0        0        0       34 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_concurrency_truss/config.yaml
+-rw-r--r--   0        0        0      547 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_concurrency_truss/model/model.py
+-rw-r--r--   0        0        0      739 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_streaming_async_generator_truss/config.yaml
+-rw-r--r--   0        0        0      521 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_streaming_async_generator_truss/model/model.py
+-rw-r--r--   0        0        0      773 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_streaming_truss/config.yaml
+-rw-r--r--   0        0        0      568 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_streaming_truss/model/model.py
+-rw-r--r--   0        0        0      669 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0      534 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        6 2023-07-28 22:19:06.037646 truss-0.5.2/truss/test_data/test_truss/packages/test_package/test.py
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/tests/__init__.py
+-rw-r--r--   0        0        0    22226 2023-07-28 22:19:06.037646 truss-0.5.2/truss/tests/conftest.py
+-rw-r--r--   0        0        0     1255 2023-07-28 22:19:06.037646 truss-0.5.2/truss/tests/contexts/image_builder/test_serving_image_builder.py
+-rw-r--r--   0        0        0      783 2023-07-28 22:19:06.037646 truss-0.5.2/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2023-07-28 22:19:06.037646 truss-0.5.2/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      968 2023-07-28 22:19:06.037646 truss-0.5.2/truss/tests/environments_inference/test_requirements_inference.py
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.037646 truss-0.5.2/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0        0 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     3293 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
+-rw-r--r--   0        0        0     2789 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/model_frameworks/test_keras_framework.py
+-rw-r--r--   0        0        0     2409 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/model_frameworks/test_lightgbm_framework.py
+-rw-r--r--   0        0        0     1479 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/model_frameworks/test_pytorch_framework.py
+-rw-r--r--   0        0        0     2427 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/model_frameworks/test_sklearn_framework.py
+-rw-r--r--   0        0        0     2437 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/model_frameworks/test_xgboost_framework.py
+-rw-r--r--   0        0        0    18726 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0      487 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      394 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0     1929 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/patch/test_truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      273 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0     2073 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/remote/baseten/test_api.py
+-rw-r--r--   0        0        0      580 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/remote/baseten/test_auth.py
+-rw-r--r--   0        0        0      835 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/remote/baseten/test_core.py
+-rw-r--r--   0        0        0     4316 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/remote/test_remote_factory.py
+-rw-r--r--   0        0        0     2394 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/remote/test_truss_remote.py
+-rw-r--r--   0        0        0    10415 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/samples.py
+-rw-r--r--   0        0        0      283 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     6081 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
+-rw-r--r--   0        0        0      964 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
+-rw-r--r--   0        0        0     7513 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0     8326 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/control/control/test_server_integration.py
+-rw-r--r--   0        0        0     1560 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/core/server/common/test_truss_server.py
+-rw-r--r--   0        0        0      821 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2038 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/server/common/test_retry.py
+-rw-r--r--   0        0        0     2605 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/server/common/test_termination_handler_middleware.py
+-rw-r--r--   0        0        0     2252 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/templates/server/test_model_wrapper.py
+-rw-r--r--   0        0        0     1910 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_backward.py
+-rw-r--r--   0        0        0     8260 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_build.py
+-rw-r--r--   0        0        0     8657 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0    14982 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_control_truss_patching.py
+-rw-r--r--   0        0        0      517 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_docker.py
+-rw-r--r--   0        0        0    12242 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0      656 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1483 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    30057 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0     1865 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/test_validation.py
+-rw-r--r--   0        0        0     4974 2023-07-28 22:19:06.041646 truss-0.5.2/truss/tests/util/test_path.py
+-rw-r--r--   0        0        0    15256 2023-07-28 22:19:06.041646 truss-0.5.2/truss/truss_config.py
+-rw-r--r--   0        0        0     2698 2023-07-28 22:19:06.041646 truss-0.5.2/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    41143 2023-07-28 22:19:06.041646 truss-0.5.2/truss/truss_handle.py
+-rw-r--r--   0        0        0     5671 2023-07-28 22:19:06.041646 truss-0.5.2/truss/truss_spec.py
+-rw-r--r--   0        0        0     2782 2023-07-28 22:19:06.041646 truss-0.5.2/truss/types.py
+-rw-r--r--   0        0        0     3121 2023-07-28 22:19:06.041646 truss-0.5.2/truss/util/.truss_ignore
+-rw-r--r--   0        0        0      379 2023-07-28 22:19:06.041646 truss-0.5.2/truss/util/data_structures.py
+-rw-r--r--   0        0        0     2552 2023-07-28 22:19:06.041646 truss-0.5.2/truss/util/download.py
+-rw-r--r--   0        0        0      553 2023-07-28 22:19:06.041646 truss-0.5.2/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2023-07-28 22:19:06.041646 truss-0.5.2/truss/util/jinja.py
+-rw-r--r--   0        0        0     6040 2023-07-28 22:19:06.041646 truss-0.5.2/truss/util/path.py
+-rw-r--r--   0        0        0     2736 2023-07-28 22:19:06.041646 truss-0.5.2/truss/validation.py
+-rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 truss-0.5.2/PKG-INFO
```

### Comparing `truss-0.5.1/CODE_OF_CONDUCT.md` & `truss-0.5.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/CONTRIBUTING.md` & `truss-0.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/LICENSE` & `truss-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/README.md` & `truss-0.5.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -77,21 +77,23 @@
 requirements:
   - torch==2.0.1
   - transformers==4.30.0
 ```
 
 No other configuration needs to be changed.
 
-## Running
+## Deployment
 
-You can run a Truss server locally by:
+You can deploy a Truss to your [Baseten](https://baseten.co) account with:
 
 ```
 cd ./text-classification
-truss run-image
+truss push
 ```
 
+Truss will support other remotes soon, starting with AWS SageMaker.
+
 ## Truss contributors
 
 Truss is backed by Baseten and built in collaboration with ML engineers worldwide. Special thanks to [Stephan Auerhahn](https://github.com/palp) @ [stability.ai](https://stability.ai/) and [Daniel Sarfati](https://github.com/dsarfati) @ [Salad Technologies](https://salad.com/) for their contributions.
 
 We enthusiastically welcome contributions in accordance with our [contributors' guide](CONTRIBUTING.md) and [code of conduct](CODE_OF_CONDUCT.md).
```

### Comparing `truss-0.5.1/context_builder.Dockerfile` & `truss-0.5.2/context_builder.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/pyproject.toml` & `truss-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.5.1"
+version = "0.5.2"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = ["MLOps", "AI", "Model Serving", "Model Deployment", "Machine Learning"]
```

### Comparing `truss-0.5.1/truss/blob/blob_backend_registry.py` & `truss-0.5.2/truss/blob/blob_backend_registry.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/blob/http_public_blob_backend.py` & `truss-0.5.2/truss/blob/http_public_blob_backend.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/build.py` & `truss-0.5.2/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/cli.py` & `truss-0.5.2/truss/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,20 +296,29 @@
     "--publish",
     type=bool,
     is_flag=True,
     required=False,
     default=False,
     help="Publish truss as production deployment.",
 )
+@click.option(
+    "--trusted",
+    type=bool,
+    is_flag=True,
+    required=False,
+    default=False,
+    help="Trust truss with hosted secrets.",
+)
 @error_handling
 def push(
     target_directory: str,
     remote: str,
     model_name: str,
     publish: bool = False,
+    trusted: bool = False,
 ) -> None:
     """
     Pushes a truss to a TrussRemote.
 
     TARGET_DIRECTORY: A Truss directory. If none, use current directory.
 
     """
@@ -327,15 +336,15 @@
 
     # Write model name to config if it's not already there
     if model_name != tr.spec.config.model_name:
         tr.spec.config.model_name = model_name
         tr.spec.config.write_to_yaml_file(tr.spec.config_path, verbose=False)
 
     # TODO(Abu): This needs to be refactored to be more generic
-    _ = remote_provider.push(tr, model_name, publish=publish)  # type: ignore
+    _ = remote_provider.push(tr, model_name, publish=publish, trusted=trusted)  # type: ignore
 
     click.echo(f"Model {model_name} was successfully pushed.")
 
 
 @container.command()  # type: ignore
 @click.argument("target_directory", required=False)
 @error_handling
```

### Comparing `truss-0.5.1/truss/constants.py` & `truss-0.5.2/truss/constants.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/contexts/image_builder/image_builder.py` & `truss-0.5.2/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.5.2/truss/contexts/image_builder/serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/contexts/image_builder/training_image_builder.py` & `truss-0.5.2/truss/contexts/image_builder/training_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/contexts/image_builder/util.py` & `truss-0.5.2/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/contexts/local_loader/docker_build_emulator.py` & `truss-0.5.2/truss/contexts/local_loader/docker_build_emulator.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/contexts/local_loader/load_model_local.py` & `truss-0.5.2/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/contexts/local_loader/train_local.py` & `truss-0.5.2/truss/contexts/local_loader/train_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/contexts/local_loader/truss_file_syncer.py` & `truss-0.5.2/truss/contexts/local_loader/truss_file_syncer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.5.2/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/contexts/local_loader/utils.py` & `truss-0.5.2/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/docker.py` & `truss-0.5.2/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/environment_inference/requirements_inference.py` & `truss-0.5.2/truss/environment_inference/requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/errors.py` & `truss-0.5.2/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/local/local_config.py` & `truss-0.5.2/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/local/local_config_handler.py` & `truss-0.5.2/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/model_framework.py` & `truss-0.5.2/truss/model_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/model_frameworks/__init__.py` & `truss-0.5.2/truss/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/model_frameworks/huggingface_transformer.py` & `truss-0.5.2/truss/model_frameworks/huggingface_transformer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/model_frameworks/keras.py` & `truss-0.5.2/truss/model_frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/model_frameworks/lightgbm.py` & `truss-0.5.2/truss/model_frameworks/lightgbm.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/model_frameworks/mlflow.py` & `truss-0.5.2/truss/model_frameworks/mlflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/model_frameworks/pytorch.py` & `truss-0.5.2/truss/model_frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/model_frameworks/sklearn.py` & `truss-0.5.2/truss/model_frameworks/sklearn.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/model_frameworks/xgboost.py` & `truss-0.5.2/truss/model_frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/model_inference.py` & `truss-0.5.2/truss/model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/patch/calc_patch.py` & `truss-0.5.2/truss/patch/calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/patch/dir_signature.py` & `truss-0.5.2/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/patch/hash.py` & `truss-0.5.2/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/patch/local_truss_patch_applier.py` & `truss-0.5.2/truss/patch/local_truss_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/patch/truss_dir_patch_applier.py` & `truss-0.5.2/truss/patch/truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/patch/types.py` & `truss-0.5.2/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/readme_generator.py` & `truss-0.5.2/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/remote/baseten/api.py` & `truss-0.5.2/truss/remote/baseten/api.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/remote/baseten/auth.py` & `truss-0.5.2/truss/remote/baseten/auth.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/remote/baseten/core.py` & `truss-0.5.2/truss/remote/baseten/core.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/remote/baseten/error.py` & `truss-0.5.2/truss/remote/baseten/error.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/remote/baseten/remote.py` & `truss-0.5.2/truss/remote/baseten/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,21 @@
         super().__init__(remote_url, **kwargs)
         self._auth_service = AuthService(api_key=api_key)
         self._api = BasetenApi(f"{self._remote_url}/graphql/", self._auth_service)
 
     def authenticate(self):
         return self._auth_service.validate()
 
-    def push(self, truss_handle: TrussHandle, model_name: str, publish: bool = True):  # type: ignore
+    def push(  # type: ignore
+        self,
+        truss_handle: TrussHandle,
+        model_name: str,
+        publish: bool = True,
+        trusted: bool = False,
+    ):
         if model_name.isspace():
             raise ValueError("Model name cannot be empty")
 
         model_id = exists_model(self._api, model_name)
 
         gathered_truss = TrussHandle(truss_handle.gather())
         encoded_config_str = base64_encoded_json_str(
@@ -45,14 +51,15 @@
         model_id, model_version_id = create_truss_service(
             api=self._api,
             model_name=model_name,
             s3_key=s3_key,
             config=encoded_config_str,
             is_draft=not publish,
             model_id=model_id,
+            is_trusted=trusted,
         )
 
         return BasetenService(
             model_id=model_id,
             model_version_id=model_version_id,
             is_draft=not publish,
             api_key=self._auth_service.authenticate().value,
```

### Comparing `truss-0.5.1/truss/remote/baseten/service.py` & `truss-0.5.2/truss/remote/baseten/service.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/remote/baseten/utils/tar.py` & `truss-0.5.2/truss/remote/baseten/utils/tar.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/remote/baseten/utils/transfer.py` & `truss-0.5.2/truss/remote/baseten/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/remote/remote_cli.py` & `truss-0.5.2/truss/remote/remote_cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/remote/remote_factory.py` & `truss-0.5.2/truss/remote/remote_factory.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/remote/truss_remote.py` & `truss-0.5.2/truss/remote/truss_remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/README.md.jinja` & `truss-0.5.2/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/base.Dockerfile.jinja` & `truss-0.5.2/truss/templates/base.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/control/control/application.py` & `truss-0.5.2/truss/templates/control/control/application.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/control/control/endpoints.py` & `truss-0.5.2/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/control/control/helpers/errors.py` & `truss-0.5.2/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.5.2/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.5.2/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.5.2/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/control/control/helpers/truss_patch/__init__.py` & `truss-0.5.2/truss/templates/control/control/helpers/truss_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py` & `truss-0.5.2/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py` & `truss-0.5.2/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py` & `truss-0.5.2/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/control/control/helpers/types.py` & `truss-0.5.2/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/control/control/server.py` & `truss-0.5.2/truss/templates/control/control/server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/custom/model/model.py` & `truss-0.5.2/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/huggingface_transformer/model/model.py` & `truss-0.5.2/truss/templates/huggingface_transformer/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/keras/model/model.py` & `truss-0.5.2/truss/templates/keras/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/lightgbm/model/model.py` & `truss-0.5.2/truss/templates/lightgbm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/mlflow/model/model.py` & `truss-0.5.2/truss/templates/mlflow/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/pytorch/model/model.py` & `truss-0.5.2/truss/templates/pytorch/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/server/common/errors.py` & `truss-0.5.2/truss/templates/server/common/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/server/common/patches/whisper/patch.py` & `truss-0.5.2/truss/templates/server/common/patches/whisper/patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/server/common/patches.py` & `truss-0.5.2/truss/templates/server/common/patches.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/server/common/retry.py` & `truss-0.5.2/truss/templates/server/common/retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/server/common/termination_handler_middleware.py` & `truss-0.5.2/truss/templates/server/common/termination_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/server/common/truss_server.py` & `truss-0.5.2/truss/templates/server/common/truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/server/inference_server.py` & `truss-0.5.2/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/server/model_wrapper.py` & `truss-0.5.2/truss/templates/server/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/server.Dockerfile.jinja` & `truss-0.5.2/truss/templates/server.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/shared/logging.py` & `truss-0.5.2/truss/templates/shared/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/shared/secrets_resolver.py` & `truss-0.5.2/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/shared/serialization.py` & `truss-0.5.2/truss/templates/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/shared/util.py` & `truss-0.5.2/truss/templates/shared/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/sklearn/model/model.py` & `truss-0.5.2/truss/templates/sklearn/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/training/job.py` & `truss-0.5.2/truss/templates/training/job.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/templates/xgboost/model/model.py` & `truss-0.5.2/truss/templates/xgboost/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/auto-mpg.data` & `truss-0.5.2/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/happy.ipynb` & `truss-0.5.2/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/model_load_failure_test/config.yaml` & `truss-0.5.2/truss/test_data/model_load_failure_test/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/model_load_failure_test/model/model.py` & `truss-0.5.2/truss/test_data/model_load_failure_test/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/patch_ping_test_server/app.py` & `truss-0.5.2/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/pima-indians-diabetes.csv` & `truss-0.5.2/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/readme_int_example.md` & `truss-0.5.2/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/readme_no_example.md` & `truss-0.5.2/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/readme_str_example.md` & `truss-0.5.2/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/server.Dockerfile` & `truss-0.5.2/truss/test_data/server.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/server_conformance_test_truss/config.yaml` & `truss-0.5.2/truss/test_data/server_conformance_test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/server_conformance_test_truss/model/model.py` & `truss-0.5.2/truss/test_data/server_conformance_test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/test_async_truss/config.yaml` & `truss-0.5.2/truss/test_data/test_async_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/test_async_truss/model/model.py` & `truss-0.5.2/truss/test_data/test_async_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/test_concurrency_truss/model/model.py` & `truss-0.5.2/truss/test_data/test_concurrency_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/test_streaming_async_generator_truss/config.yaml` & `truss-0.5.2/truss/test_data/test_streaming_async_generator_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/test_streaming_async_generator_truss/model/model.py` & `truss-0.5.2/truss/test_data/test_streaming_async_generator_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/test_streaming_truss/config.yaml` & `truss-0.5.2/truss/test_data/test_streaming_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/test_streaming_truss/model/model.py` & `truss-0.5.2/truss/test_data/test_streaming_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/test_truss/config.yaml` & `truss-0.5.2/truss/test_data/test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/test_data/test_truss/model/model.py` & `truss-0.5.2/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/conftest.py` & `truss-0.5.2/truss/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/contexts/image_builder/test_serving_image_builder.py` & `truss-0.5.2/truss/tests/contexts/image_builder/test_serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.5.2/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.5.2/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/environments_inference/test_requirements_inference.py` & `truss-0.5.2/truss/tests/environments_inference/test_requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/local/test_local_config_handler.py` & `truss-0.5.2/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/model_frameworks/test_huggingface_transformer_framework.py` & `truss-0.5.2/truss/tests/model_frameworks/test_huggingface_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/model_frameworks/test_keras_framework.py` & `truss-0.5.2/truss/tests/model_frameworks/test_keras_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/model_frameworks/test_lightgbm_framework.py` & `truss-0.5.2/truss/tests/model_frameworks/test_lightgbm_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/model_frameworks/test_pytorch_framework.py` & `truss-0.5.2/truss/tests/model_frameworks/test_pytorch_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/model_frameworks/test_sklearn_framework.py` & `truss-0.5.2/truss/tests/model_frameworks/test_sklearn_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/model_frameworks/test_xgboost_framework.py` & `truss-0.5.2/truss/tests/model_frameworks/test_xgboost_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/patch/test_calc_patch.py` & `truss-0.5.2/truss/tests/patch/test_calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/patch/test_hash.py` & `truss-0.5.2/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/patch/test_truss_dir_patch_applier.py` & `truss-0.5.2/truss/tests/patch/test_truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/remote/baseten/test_api.py` & `truss-0.5.2/truss/tests/remote/baseten/test_api.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/remote/baseten/test_auth.py` & `truss-0.5.2/truss/tests/remote/baseten/test_auth.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/remote/baseten/test_core.py` & `truss-0.5.2/truss/tests/remote/baseten/test_core.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/remote/test_remote_factory.py` & `truss-0.5.2/truss/tests/remote/test_remote_factory.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/remote/test_truss_remote.py` & `truss-0.5.2/truss/tests/remote/test_truss_remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/samples.py` & `truss-0.5.2/truss/tests/samples.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py` & `truss-0.5.2/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py` & `truss-0.5.2/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/templates/control/control/test_server.py` & `truss-0.5.2/truss/tests/templates/control/control/test_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/templates/control/control/test_server_integration.py` & `truss-0.5.2/truss/tests/templates/control/control/test_server_integration.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/templates/core/server/common/test_truss_server.py` & `truss-0.5.2/truss/tests/templates/core/server/common/test_truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/templates/core/server/common/test_util.py` & `truss-0.5.2/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.5.2/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/templates/server/common/test_retry.py` & `truss-0.5.2/truss/tests/templates/server/common/test_retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/templates/server/common/test_termination_handler_middleware.py` & `truss-0.5.2/truss/tests/templates/server/common/test_termination_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/templates/server/test_model_wrapper.py` & `truss-0.5.2/truss/tests/templates/server/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/test_backward.py` & `truss-0.5.2/truss/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/test_build.py` & `truss-0.5.2/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/test_config.py` & `truss-0.5.2/truss/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/test_context_builder_image.py` & `truss-0.5.2/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/test_control_truss_patching.py` & `truss-0.5.2/truss/tests/test_control_truss_patching.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/test_docker.py` & `truss-0.5.2/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/test_model_inference.py` & `truss-0.5.2/truss/tests/test_model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/test_notebooks.py` & `truss-0.5.2/truss/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.5.2/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/test_truss_gatherer.py` & `truss-0.5.2/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/test_truss_handle.py` & `truss-0.5.2/truss/tests/test_truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/test_validation.py` & `truss-0.5.2/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/tests/util/test_path.py` & `truss-0.5.2/truss/tests/util/test_path.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/truss_config.py` & `truss-0.5.2/truss/truss_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/truss_gatherer.py` & `truss-0.5.2/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/truss_handle.py` & `truss-0.5.2/truss/truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/truss_spec.py` & `truss-0.5.2/truss/truss_spec.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/types.py` & `truss-0.5.2/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/util/.truss_ignore` & `truss-0.5.2/truss/util/.truss_ignore`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/util/download.py` & `truss-0.5.2/truss/util/download.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/util/gpu.py` & `truss-0.5.2/truss/util/gpu.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/util/path.py` & `truss-0.5.2/truss/util/path.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/truss/validation.py` & `truss-0.5.2/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.1/PKG-INFO` & `truss-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.5.1
+Version: 0.5.2
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.12
@@ -124,22 +124,24 @@
 requirements:
   - torch==2.0.1
   - transformers==4.30.0
 ```
 
 No other configuration needs to be changed.
 
-## Running
+## Deployment
 
-You can run a Truss server locally by:
+You can deploy a Truss to your [Baseten](https://baseten.co) account with:
 
 ```
 cd ./text-classification
-truss run-image
+truss push
 ```
 
+Truss will support other remotes soon, starting with AWS SageMaker.
+
 ## Truss contributors
 
 Truss is backed by Baseten and built in collaboration with ML engineers worldwide. Special thanks to [Stephan Auerhahn](https://github.com/palp) @ [stability.ai](https://stability.ai/) and [Daniel Sarfati](https://github.com/dsarfati) @ [Salad Technologies](https://salad.com/) for their contributions.
 
 We enthusiastically welcome contributions in accordance with our [contributors' guide](CONTRIBUTING.md) and [code of conduct](CODE_OF_CONDUCT.md).
```

