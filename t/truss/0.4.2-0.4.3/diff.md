# Comparing `tmp/truss-0.4.2.tar.gz` & `tmp/truss-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.4.2.tar", max compression
+gzip compressed data, was "truss-0.4.3.tar", max compression
```

## Comparing `truss-0.4.2.tar` & `truss-0.4.3.tar`

### file list

```diff
@@ -1,156 +1,156 @@
--rw-r--r--   0        0        0     5483 2023-04-12 20:02:08.670506 truss-0.4.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2576 2023-04-12 20:02:08.670506 truss-0.4.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2023-04-12 20:02:08.670506 truss-0.4.2/LICENSE
--rw-r--r--   0        0        0     5958 2023-04-12 20:02:08.670506 truss-0.4.2/README.md
--rw-r--r--   0        0        0     3316 2023-04-12 20:02:08.670506 truss-0.4.2/ROADMAP.md
--rw-r--r--   0        0        0      465 2023-04-12 20:02:08.670506 truss-0.4.2/context_builder.Dockerfile
--rw-r--r--   0        0        0     2205 2023-04-12 20:02:08.766507 truss-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      330 2023-04-12 20:02:08.766507 truss-0.4.2/truss/__init__.py
--rw-r--r--   0        0        0    13286 2023-04-12 20:02:08.766507 truss-0.4.2/truss/build.py
--rw-r--r--   0        0        0    10452 2023-04-12 20:02:08.766507 truss-0.4.2/truss/cli.py
--rw-r--r--   0        0        0     2700 2023-04-12 20:02:08.766507 truss-0.4.2/truss/constants.py
--rw-r--r--   0        0        0     1233 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0     5791 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     4507 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/image_builder/training_image_builder.py
--rw-r--r--   0        0        0     1976 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     1686 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     2239 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/local_loader/train_local.py
--rw-r--r--   0        0        0     5801 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2023-04-12 20:02:08.766507 truss-0.4.2/truss/decorators.py
--rw-r--r--   0        0        0     3641 2023-04-12 20:02:08.766507 truss-0.4.2/truss/docker.py
--rw-r--r--   0        0        0     3759 2023-04-12 20:02:08.766507 truss-0.4.2/truss/environment_inference/requirements_inference.py
--rw-r--r--   0        0        0      643 2023-04-12 20:02:08.766507 truss-0.4.2/truss/errors.py
--rw-r--r--   0        0        0      824 2023-04-12 20:02:08.766507 truss-0.4.2/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2023-04-12 20:02:08.766507 truss-0.4.2/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     2709 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_framework.py
--rw-r--r--   0        0        0     1687 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/__init__.py
--rw-r--r--   0        0        0     1895 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/huggingface_transformer.py
--rw-r--r--   0        0        0      918 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/keras.py
--rw-r--r--   0        0        0     1237 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/lightgbm.py
--rw-r--r--   0        0        0     2410 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/mlflow.py
--rw-r--r--   0        0        0     2441 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/pytorch.py
--rw-r--r--   0        0        0     1232 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/sklearn.py
--rw-r--r--   0        0        0     1027 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/xgboost.py
--rw-r--r--   0        0        0     6565 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_inference.py
--rw-r--r--   0        0        0      510 2023-04-12 20:02:08.766507 truss-0.4.2/truss/notebook.py
--rw-r--r--   0        0        0     9521 2023-04-12 20:02:08.766507 truss-0.4.2/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      774 2023-04-12 20:02:08.766507 truss-0.4.2/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2388 2023-04-12 20:02:08.766507 truss-0.4.2/truss/patch/hash.py
--rw-r--r--   0        0        0      468 2023-04-12 20:02:08.766507 truss-0.4.2/truss/patch/signature.py
--rw-r--r--   0        0        0      937 2023-04-12 20:02:08.766507 truss-0.4.2/truss/patch/types.py
--rw-r--r--   0        0        0      237 2023-04-12 20:02:08.766507 truss-0.4.2/truss/pytest.ini
--rw-r--r--   0        0        0      705 2023-04-12 20:02:08.766507 truss-0.4.2/truss/readme_generator.py
--rw-r--r--   0        0        0     2482 2023-04-12 20:02:08.766507 truss-0.4.2/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.766507 truss-0.4.2/truss/templates/__init__.py
--rw-r--r--   0        0        0     1375 2023-04-12 20:02:08.766507 truss-0.4.2/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     2190 2023-04-12 20:02:08.766507 truss-0.4.2/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     4083 2023-04-12 20:02:08.766507 truss-0.4.2/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2023-04-12 20:02:08.766507 truss-0.4.2/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      877 2023-04-12 20:02:08.766507 truss-0.4.2/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     5801 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     2596 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2399 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0     5389 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/control/control/helpers/patch_applier.py
--rw-r--r--   0        0        0     3070 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     1849 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/control/control/server.py
--rw-r--r--   0        0        0       82 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       48 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0      979 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0      460 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/custom/train/train.py
--rw-r--r--   0        0        0     2616 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/docs/README.md
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/huggingface_transformer/model/__init__.py
--rw-r--r--   0        0        0     2272 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/huggingface_transformer/model/model.py
--rw-r--r--   0        0        0       47 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/huggingface_transformer/requirements.txt
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/keras/model/__init__.py
--rw-r--r--   0        0        0     1173 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/keras/model/model.py
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/lightgbm/model/__init__.py
--rw-r--r--   0        0        0     1696 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/lightgbm/model/model.py
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/mlflow/model/__init__.py
--rw-r--r--   0        0        0     1196 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/mlflow/model/model.py
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/pipeline/model/__init__.py
--rw-r--r--   0        0        0      875 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/pipeline/model/model.py
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/pytorch/model/__init__.py
--rw-r--r--   0        0        0     1708 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/pytorch/model/model.py
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0      237 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     1352 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/common/logging.py
--rw-r--r--   0        0        0     3318 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/common/serialization.py
--rw-r--r--   0        0        0     5511 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0      416 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/common/util.py
--rw-r--r--   0        0        0      733 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0     4943 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      162 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0      855 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1430 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/sklearn/model/__init__.py
--rw-r--r--   0        0        0     1666 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/sklearn/model/model.py
--rw-r--r--   0        0        0     3400 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/training/job.py
--rw-r--r--   0        0        0       12 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/training/requirements.txt
--rw-r--r--   0        0        0      491 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/training.Dockerfile.jinja
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/xgboost/model/__init__.py
--rw-r--r--   0        0        0     1898 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/xgboost/model/model.py
--rw-r--r--   0        0        0    30286 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0      216 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0     1394 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0     1267 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0      669 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0     1006 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/__init__.py
--rw-r--r--   0        0        0    19167 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/conftest.py
--rw-r--r--   0        0        0      783 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      968 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/environments_inference/test_requirements_inference.py
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/model_frameworks/__init__.py
--rw-r--r--   0        0        0     3293 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
--rw-r--r--   0        0        0     2789 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/model_frameworks/test_keras_framework.py
--rw-r--r--   0        0        0     2409 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/model_frameworks/test_lightgbm_framework.py
--rw-r--r--   0        0        0     1479 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/model_frameworks/test_pytorch_framework.py
--rw-r--r--   0        0        0     2427 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/model_frameworks/test_sklearn_framework.py
--rw-r--r--   0        0        0     2437 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/model_frameworks/test_xgboost_framework.py
--rw-r--r--   0        0        0      487 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0     9348 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/patch/test_patch.py
--rw-r--r--   0        0        0      394 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0      273 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0    10415 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/samples.py
--rw-r--r--   0        0        0      283 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     1976 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/templates/control/control/helpers/test_patch_applier.py
--rw-r--r--   0        0        0     6937 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0      750 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     1910 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_backward.py
--rw-r--r--   0        0        0     8260 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_build.py
--rw-r--r--   0        0        0     2359 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0      517 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_docker.py
--rw-r--r--   0        0        0     2605 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0      656 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_notebooks.py
--rw-r--r--   0        0        0     1483 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    31557 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0      433 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_truss_util.py
--rw-r--r--   0        0        0     1865 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_validation.py
--rw-r--r--   0        0        0     9289 2023-04-12 20:02:08.774507 truss-0.4.2/truss/truss_config.py
--rw-r--r--   0        0        0     2841 2023-04-12 20:02:08.774507 truss-0.4.2/truss/truss_gatherer.py
--rw-r--r--   0        0        0    39722 2023-04-12 20:02:08.774507 truss-0.4.2/truss/truss_handle.py
--rw-r--r--   0        0        0     5195 2023-04-12 20:02:08.774507 truss-0.4.2/truss/truss_spec.py
--rw-r--r--   0        0        0     2124 2023-04-12 20:02:08.774507 truss-0.4.2/truss/types.py
--rw-r--r--   0        0        0     2350 2023-04-12 20:02:08.774507 truss-0.4.2/truss/utils.py
--rw-r--r--   0        0        0     2317 2023-04-12 20:02:08.774507 truss-0.4.2/truss/validation.py
--rw-r--r--   0        0        0     7297 1970-01-01 00:00:00.000000 truss-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     5483 2023-04-13 16:45:41.461156 truss-0.4.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2576 2023-04-13 16:45:41.461156 truss-0.4.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2023-04-13 16:45:41.461156 truss-0.4.3/LICENSE
+-rw-r--r--   0        0        0     5958 2023-04-13 16:45:41.461156 truss-0.4.3/README.md
+-rw-r--r--   0        0        0     3316 2023-04-13 16:45:41.461156 truss-0.4.3/ROADMAP.md
+-rw-r--r--   0        0        0      465 2023-04-13 16:45:41.461156 truss-0.4.3/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2205 2023-04-13 16:45:41.553157 truss-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-04-13 16:45:41.553157 truss-0.4.3/truss/__init__.py
+-rw-r--r--   0        0        0    13286 2023-04-13 16:45:41.553157 truss-0.4.3/truss/build.py
+-rw-r--r--   0        0        0    10452 2023-04-13 16:45:41.553157 truss-0.4.3/truss/cli.py
+-rw-r--r--   0        0        0     2700 2023-04-13 16:45:41.553157 truss-0.4.3/truss/constants.py
+-rw-r--r--   0        0        0     1233 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0     5791 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     4507 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/image_builder/training_image_builder.py
+-rw-r--r--   0        0        0     1976 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     1686 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     2239 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/local_loader/train_local.py
+-rw-r--r--   0        0        0     5801 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2023-04-13 16:45:41.553157 truss-0.4.3/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2023-04-13 16:45:41.553157 truss-0.4.3/truss/docker.py
+-rw-r--r--   0        0        0     3759 2023-04-13 16:45:41.553157 truss-0.4.3/truss/environment_inference/requirements_inference.py
+-rw-r--r--   0        0        0      643 2023-04-13 16:45:41.553157 truss-0.4.3/truss/errors.py
+-rw-r--r--   0        0        0      824 2023-04-13 16:45:41.553157 truss-0.4.3/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2023-04-13 16:45:41.553157 truss-0.4.3/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     2709 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_framework.py
+-rw-r--r--   0        0        0     1687 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     1895 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/huggingface_transformer.py
+-rw-r--r--   0        0        0      918 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/keras.py
+-rw-r--r--   0        0        0     1237 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/lightgbm.py
+-rw-r--r--   0        0        0     2410 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/mlflow.py
+-rw-r--r--   0        0        0     2441 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/pytorch.py
+-rw-r--r--   0        0        0     1232 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/sklearn.py
+-rw-r--r--   0        0        0     1027 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/xgboost.py
+-rw-r--r--   0        0        0     6565 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2023-04-13 16:45:41.553157 truss-0.4.3/truss/notebook.py
+-rw-r--r--   0        0        0    10874 2023-04-13 16:45:41.553157 truss-0.4.3/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      774 2023-04-13 16:45:41.553157 truss-0.4.3/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2388 2023-04-13 16:45:41.553157 truss-0.4.3/truss/patch/hash.py
+-rw-r--r--   0        0        0      468 2023-04-13 16:45:41.553157 truss-0.4.3/truss/patch/signature.py
+-rw-r--r--   0        0        0      937 2023-04-13 16:45:41.553157 truss-0.4.3/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2023-04-13 16:45:41.553157 truss-0.4.3/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2023-04-13 16:45:41.553157 truss-0.4.3/truss/readme_generator.py
+-rw-r--r--   0        0        0     2482 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/__init__.py
+-rw-r--r--   0        0        0     1375 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     2190 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     4083 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      877 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     5801 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     2596 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2399 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0     5389 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/helpers/patch_applier.py
+-rw-r--r--   0        0        0     3070 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     1849 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0       82 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       48 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0      979 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0      460 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/custom/train/train.py
+-rw-r--r--   0        0        0     2616 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/docs/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/huggingface_transformer/model/__init__.py
+-rw-r--r--   0        0        0     2272 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/huggingface_transformer/model/model.py
+-rw-r--r--   0        0        0       47 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/huggingface_transformer/requirements.txt
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/keras/model/__init__.py
+-rw-r--r--   0        0        0     1173 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/keras/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/lightgbm/model/__init__.py
+-rw-r--r--   0        0        0     1696 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/lightgbm/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/mlflow/model/__init__.py
+-rw-r--r--   0        0        0     1196 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/mlflow/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/pipeline/model/__init__.py
+-rw-r--r--   0        0        0      875 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/pipeline/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/pytorch/model/__init__.py
+-rw-r--r--   0        0        0     1708 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/pytorch/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0      237 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     1352 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/server/common/logging.py
+-rw-r--r--   0        0        0     3318 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/server/common/serialization.py
+-rw-r--r--   0        0        0     5511 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0      416 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/server/common/util.py
+-rw-r--r--   0        0        0      733 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0     4943 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      162 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0      855 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1430 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/sklearn/model/__init__.py
+-rw-r--r--   0        0        0     1666 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/sklearn/model/model.py
+-rw-r--r--   0        0        0     3400 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/training/job.py
+-rw-r--r--   0        0        0       12 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/training/requirements.txt
+-rw-r--r--   0        0        0      491 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/training.Dockerfile.jinja
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/xgboost/model/__init__.py
+-rw-r--r--   0        0        0     1898 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/xgboost/model/model.py
+-rw-r--r--   0        0        0    30286 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0      216 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0     1394 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0     1267 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0      669 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0     1006 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/__init__.py
+-rw-r--r--   0        0        0    19167 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/conftest.py
+-rw-r--r--   0        0        0      783 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      968 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/environments_inference/test_requirements_inference.py
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     3293 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
+-rw-r--r--   0        0        0     2789 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/model_frameworks/test_keras_framework.py
+-rw-r--r--   0        0        0     2409 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/model_frameworks/test_lightgbm_framework.py
+-rw-r--r--   0        0        0     1479 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/model_frameworks/test_pytorch_framework.py
+-rw-r--r--   0        0        0     2427 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/model_frameworks/test_sklearn_framework.py
+-rw-r--r--   0        0        0     2437 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/model_frameworks/test_xgboost_framework.py
+-rw-r--r--   0        0        0    10483 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0      487 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      394 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0      273 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0    10415 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/samples.py
+-rw-r--r--   0        0        0      283 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     1976 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/templates/control/control/helpers/test_patch_applier.py
+-rw-r--r--   0        0        0     6937 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0      750 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     1910 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_backward.py
+-rw-r--r--   0        0        0     8260 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_build.py
+-rw-r--r--   0        0        0     2359 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0      517 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_docker.py
+-rw-r--r--   0        0        0     2605 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0      656 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1483 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    31557 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0      433 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_truss_util.py
+-rw-r--r--   0        0        0     1865 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_validation.py
+-rw-r--r--   0        0        0     9289 2023-04-13 16:45:41.557157 truss-0.4.3/truss/truss_config.py
+-rw-r--r--   0        0        0     2841 2023-04-13 16:45:41.557157 truss-0.4.3/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    39722 2023-04-13 16:45:41.557157 truss-0.4.3/truss/truss_handle.py
+-rw-r--r--   0        0        0     5195 2023-04-13 16:45:41.557157 truss-0.4.3/truss/truss_spec.py
+-rw-r--r--   0        0        0     2124 2023-04-13 16:45:41.557157 truss-0.4.3/truss/types.py
+-rw-r--r--   0        0        0     2350 2023-04-13 16:45:41.557157 truss-0.4.3/truss/utils.py
+-rw-r--r--   0        0        0     2317 2023-04-13 16:45:41.557157 truss-0.4.3/truss/validation.py
+-rw-r--r--   0        0        0     7297 1970-01-01 00:00:00.000000 truss-0.4.3/PKG-INFO
```

### Comparing `truss-0.4.2/CODE_OF_CONDUCT.md` & `truss-0.4.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/CONTRIBUTING.md` & `truss-0.4.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/LICENSE` & `truss-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/README.md` & `truss-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/ROADMAP.md` & `truss-0.4.3/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/pyproject.toml` & `truss-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.4.2"
+version = "0.4.3"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = ["MLOps", "AI", "Model Serving", "Model Deployment", "Machine Learning"]
```

### Comparing `truss-0.4.2/truss/build.py` & `truss-0.4.3/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/cli.py` & `truss-0.4.3/truss/cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/constants.py` & `truss-0.4.3/truss/constants.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/contexts/image_builder/image_builder.py` & `truss-0.4.3/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.4.3/truss/contexts/image_builder/serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/contexts/image_builder/training_image_builder.py` & `truss-0.4.3/truss/contexts/image_builder/training_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/contexts/image_builder/util.py` & `truss-0.4.3/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/contexts/local_loader/load_model_local.py` & `truss-0.4.3/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/contexts/local_loader/train_local.py` & `truss-0.4.3/truss/contexts/local_loader/train_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.4.3/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/contexts/local_loader/utils.py` & `truss-0.4.3/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/docker.py` & `truss-0.4.3/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/environment_inference/requirements_inference.py` & `truss-0.4.3/truss/environment_inference/requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/errors.py` & `truss-0.4.3/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/local/local_config.py` & `truss-0.4.3/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/local/local_config_handler.py` & `truss-0.4.3/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/model_framework.py` & `truss-0.4.3/truss/model_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/model_frameworks/__init__.py` & `truss-0.4.3/truss/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/model_frameworks/huggingface_transformer.py` & `truss-0.4.3/truss/model_frameworks/huggingface_transformer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/model_frameworks/keras.py` & `truss-0.4.3/truss/model_frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/model_frameworks/lightgbm.py` & `truss-0.4.3/truss/model_frameworks/lightgbm.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/model_frameworks/mlflow.py` & `truss-0.4.3/truss/model_frameworks/mlflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/model_frameworks/pytorch.py` & `truss-0.4.3/truss/model_frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/model_frameworks/sklearn.py` & `truss-0.4.3/truss/model_frameworks/sklearn.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/model_frameworks/xgboost.py` & `truss-0.4.3/truss/model_frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/model_inference.py` & `truss-0.4.3/truss/model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/patch/calc_patch.py` & `truss-0.4.3/truss/patch/calc_patch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+import logging
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Set
 
 import pkg_resources
 import yaml
+from truss.constants import CONFIG_FILE
 from truss.patch.hash import file_content_hash_str
 from truss.patch.types import TrussSignature
 from truss.templates.control.control.helpers.types import (
     Action,
     ModelCodePatch,
     Patch,
     PatchType,
     PythonRequirementPatch,
     SystemPackagePatch,
 )
 from truss.truss_config import TrussConfig
 from truss.truss_spec import TrussSpec
 
+logger: logging.Logger = logging.getLogger(__name__)
 PYCACHE_IGNORE_PATTERNS = [
     "**/__pycache__/**/*",
     "**/__pycache__/**",
 ]
 
 
 def calc_truss_patch(
@@ -27,90 +30,102 @@
     previous_truss_signature: TrussSignature,
     ignore_patterns: Optional[List[str]] = None,
 ) -> Optional[List[Patch]]:
     """
     Calculate patch for a truss from a previous state.
 
     Returns: None if patch cannot be calculated, otherwise a list of patches.
-        Note that the none return value is pretty important, patch coverage
-        is limited and this usually indicates that the identified change cannot
-        be expressed with currently supported patches.
+        Note that the none return value is pretty important, patch coverage is
+        limited and this usually indicates that the identified change cannot be
+        expressed with currently supported patches.
+
+        Only standard and relevant truss paths are scanned for changes, rest
+        ignored. E.g. at the root level, only changes to config.yaml are
+        checked, any other changes are ignored.
     """
+
+    def _relative_to_root(path: Path) -> str:
+        return str(path.relative_to(truss_dir))
+
     if ignore_patterns is None:
         ignore_patterns = PYCACHE_IGNORE_PATTERNS
 
     changed_paths = _calc_changed_paths(
         truss_dir,
         previous_truss_signature.content_hashes_by_path,
         ignore_patterns,
     )
     # TODO(pankaj) Calculate model code patches only for now, add config changes
     # later.
+
     truss_spec = TrussSpec(truss_dir)
-    model_module_path = str(truss_spec.model_module_dir.relative_to(truss_dir))
-    training_module_path = str(truss_spec.training_module_dir.relative_to(truss_dir))
+    model_module_path = _relative_to_root(truss_spec.model_module_dir)
+    data_dir_path = _relative_to_root(truss_spec.data_dir)
+    bundled_packages_path = _relative_to_root(truss_spec.bundled_packages_dir)
+
+    def _under_unsupported_patch_dir(path: str) -> bool:
+        """
+        Checks if the given path is under one of the directories that don't
+        support patching. Note that if path `is` one of those directories that's
+        ok, because those empty directories can be ignored from patching point
+        of view.
+        """
+        return _strictly_under(path, [data_dir_path, bundled_packages_path])
 
     patches = []
     for path in changed_paths["removed"]:
         if path.startswith(model_module_path):
-            relative_to_model_module_path = str(
-                Path(path).relative_to(model_module_path)
-            )
             patches.append(
                 Patch(
                     type=PatchType.MODEL_CODE,
                     body=ModelCodePatch(
                         action=Action.REMOVE,
-                        path=relative_to_model_module_path,
+                        path=_relative_to(path, model_module_path),
                     ),
                 )
             )
-        elif path.startswith(training_module_path):
-            # Ignore training changes from patch
-            continue
-        else:
+        elif path == CONFIG_FILE:
+            # Don't support removal of config file
+            logger.info(f"Patching not supported for removing {path}")
+            return None
+        elif _under_unsupported_patch_dir(path):
+            logger.info(f"Patching not supported for removing {path}")
             return None
 
     for path in changed_paths["added"] + changed_paths["updated"]:
         if path.startswith(model_module_path):
             full_path = truss_dir / path
-            relative_to_model_module_path = str(
-                Path(path).relative_to(model_module_path)
-            )
 
             # TODO(pankaj) Add support for empty directories, skip them for now.
             if not full_path.is_file():
                 continue
 
-            with full_path.open() as file:
-                content = file.read()
             action = Action.ADD if path in changed_paths["added"] else Action.UPDATE
             patches.append(
                 Patch(
                     type=PatchType.MODEL_CODE,
                     body=ModelCodePatch(
                         action=action,
-                        path=relative_to_model_module_path,
-                        content=content,
+                        path=_relative_to(path, model_module_path),
+                        content=_file_content(full_path),
                     ),
                 )
             )
-        elif path.startswith(training_module_path):
-            # Ignore training changes from patch
-            continue
-        elif str(path) == "config.yaml":
-            new_config = TrussConfig.from_yaml(truss_dir / "config.yaml")
+        elif path == CONFIG_FILE:
+            new_config = TrussConfig.from_yaml(truss_dir / CONFIG_FILE)
             prev_config = TrussConfig.from_dict(
                 yaml.safe_load(previous_truss_signature.config)
             )
             config_patches = _calc_config_patches(prev_config, new_config)
             if config_patches is None:
+                logger.info(f"Unable to patch update to {path}")
                 return None
             patches.extend(config_patches)
-        else:
+        elif _under_unsupported_patch_dir(path):
+            logger.info(f"Patching not supported for updating {path}")
             return None
     return patches
 
 
 def _calc_changed_paths(
     root: Path,
     previous_root_path_content_hashes: Dict[str, str],
@@ -276,7 +291,27 @@
     return Patch(
         type=PatchType.SYSTEM_PACKAGE,
         body=SystemPackagePatch(
             action=action,
             package=package,
         ),
     )
+
+
+def _relative_to(path: str, relative_to_path: str):
+    return str(Path(path).relative_to(relative_to_path))
+
+
+def _strictly_under(path: str, parent_paths: List[str]) -> bool:
+    """
+    Checks if given path is under one of the given paths, but not the same as
+    them. Assumes that parent paths themselves are not under each other.
+    """
+    for dir_path in parent_paths:
+        if path.startswith(dir_path) and not path == dir_path:
+            return True
+    return False
+
+
+def _file_content(path: Path) -> str:
+    with path.open() as file:
+        return file.read()
```

### Comparing `truss-0.4.2/truss/patch/dir_signature.py` & `truss-0.4.3/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/patch/hash.py` & `truss-0.4.3/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/patch/types.py` & `truss-0.4.3/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/readme_generator.py` & `truss-0.4.3/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/README.md.jinja` & `truss-0.4.3/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/base.Dockerfile.jinja` & `truss-0.4.3/truss/templates/base.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/control/control/application.py` & `truss-0.4.3/truss/templates/control/control/application.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/control/control/endpoints.py` & `truss-0.4.3/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/control/control/helpers/errors.py` & `truss-0.4.3/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.4.3/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.4.3/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.4.3/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/control/control/helpers/patch_applier.py` & `truss-0.4.3/truss/templates/control/control/helpers/patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/control/control/helpers/types.py` & `truss-0.4.3/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/control/control/server.py` & `truss-0.4.3/truss/templates/control/control/server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/custom/model/model.py` & `truss-0.4.3/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/docs/README.md` & `truss-0.4.3/truss/templates/docs/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/huggingface_transformer/model/model.py` & `truss-0.4.3/truss/templates/huggingface_transformer/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/keras/model/model.py` & `truss-0.4.3/truss/templates/keras/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/lightgbm/model/model.py` & `truss-0.4.3/truss/templates/lightgbm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/mlflow/model/model.py` & `truss-0.4.3/truss/templates/mlflow/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/pipeline/model/model.py` & `truss-0.4.3/truss/templates/pipeline/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/pytorch/model/model.py` & `truss-0.4.3/truss/templates/pytorch/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/server/common/logging.py` & `truss-0.4.3/truss/templates/server/common/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/server/common/serialization.py` & `truss-0.4.3/truss/templates/server/common/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/server/common/truss_server.py` & `truss-0.4.3/truss/templates/server/common/truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/server/inference_server.py` & `truss-0.4.3/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/server/model_wrapper.py` & `truss-0.4.3/truss/templates/server/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/server.Dockerfile.jinja` & `truss-0.4.3/truss/templates/server.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/shared/secrets_resolver.py` & `truss-0.4.3/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/sklearn/model/model.py` & `truss-0.4.3/truss/templates/sklearn/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/training/job.py` & `truss-0.4.3/truss/templates/training/job.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/templates/xgboost/model/model.py` & `truss-0.4.3/truss/templates/xgboost/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/test_data/auto-mpg.data` & `truss-0.4.3/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/test_data/happy.ipynb` & `truss-0.4.3/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/test_data/patch_ping_test_server/app.py` & `truss-0.4.3/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/test_data/pima-indians-diabetes.csv` & `truss-0.4.3/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/test_data/readme_int_example.md` & `truss-0.4.3/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/test_data/readme_no_example.md` & `truss-0.4.3/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/test_data/readme_str_example.md` & `truss-0.4.3/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/test_data/test_truss/config.yaml` & `truss-0.4.3/truss/test_data/test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/test_data/test_truss/model/model.py` & `truss-0.4.3/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/conftest.py` & `truss-0.4.3/truss/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.4.3/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.4.3/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/environments_inference/test_requirements_inference.py` & `truss-0.4.3/truss/tests/environments_inference/test_requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/local/test_local_config_handler.py` & `truss-0.4.3/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/model_frameworks/test_huggingface_transformer_framework.py` & `truss-0.4.3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/model_frameworks/test_keras_framework.py` & `truss-0.4.3/truss/tests/model_frameworks/test_keras_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/model_frameworks/test_lightgbm_framework.py` & `truss-0.4.3/truss/tests/model_frameworks/test_lightgbm_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/model_frameworks/test_pytorch_framework.py` & `truss-0.4.3/truss/tests/model_frameworks/test_pytorch_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/model_frameworks/test_sklearn_framework.py` & `truss-0.4.3/truss/tests/model_frameworks/test_sklearn_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/model_frameworks/test_xgboost_framework.py` & `truss-0.4.3/truss/tests/model_frameworks/test_xgboost_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/patch/test_hash.py` & `truss-0.4.3/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/patch/test_patch.py` & `truss-0.4.3/truss/tests/patch/test_calc_patch.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,32 +12,41 @@
     SystemPackagePatch,
 )
 from truss.truss_config import TrussConfig
 
 
 def test_calc_truss_patch_unsupported(custom_model_truss_dir: Path):
     prev_sign = calc_truss_signature(custom_model_truss_dir)
-    (custom_model_truss_dir / "dummy").touch()
+
+    # Unsupported directory should result in no patches
+    (custom_model_truss_dir / "data").touch()
+    patches = calc_truss_patch(custom_model_truss_dir, prev_sign)
+    assert len(patches) == 0
+
+    # Changes under unsupported directory should return None to reflect
+    # inability to calculate patch.
+    (custom_model_truss_dir / "data" / "dummy").touch()
     patches = calc_truss_patch(custom_model_truss_dir, prev_sign)
     assert patches is None
 
 
 def test_calc_truss_patch_add_file(custom_model_truss_dir: Path):
     prev_sign = calc_truss_signature(custom_model_truss_dir)
-    (custom_model_truss_dir / "model" / "dummy").touch()
+    with (custom_model_truss_dir / "model" / "dummy").open("w") as file:
+        file.write("content")
     patches = calc_truss_patch(custom_model_truss_dir, prev_sign)
 
     assert len(patches) == 1
     patch = patches[0]
     assert patch == Patch(
         type=PatchType.MODEL_CODE,
         body=ModelCodePatch(
             action=Action.ADD,
             path="dummy",
-            content="",
+            content="content",
         ),
     )
 
 
 def test_calc_truss_patch_add_under_new_directory(custom_model_truss_dir: Path):
     prev_sign = calc_truss_signature(custom_model_truss_dir)
     new_dir = custom_model_truss_dir / "model" / "dir"
@@ -106,14 +115,41 @@
     patches = calc_truss_patch(
         custom_model_truss_dir,
         prev_sign,
     )
     assert len(patches) == 0
 
 
+def test_calc_truss_ignore_changes_outside_patch_relevant_dirs(
+    custom_model_truss_dir: Path,
+):
+    prev_sign = calc_truss_signature(custom_model_truss_dir)
+    top_pycache_path = custom_model_truss_dir / "__pycache__"
+    top_pycache_path.mkdir()
+    (top_pycache_path / "README.md").touch()
+    git_dir = custom_model_truss_dir / ".git"
+    git_dir.mkdir()
+    (git_dir / "dummy").touch()
+
+    patches = calc_truss_patch(
+        custom_model_truss_dir,
+        prev_sign,
+    )
+    assert len(patches) == 0
+
+    # Removing should also be ignored
+    new_sign = calc_truss_signature(custom_model_truss_dir)
+    (git_dir / "dummy").unlink()
+    patches = calc_truss_patch(
+        custom_model_truss_dir,
+        new_sign,
+    )
+    assert len(patches) == 0
+
+
 def test_calc_config_patches_add_python_requirement(custom_model_truss_dir: Path):
     patches = _apply_config_change_and_calc_patches(
         custom_model_truss_dir,
         lambda config: config.requirements.append("requests==1.0.0"),
     )
     assert len(patches) == 1
     patch = patches[0]
```

### Comparing `truss-0.4.2/truss/tests/samples.py` & `truss-0.4.3/truss/tests/samples.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/templates/control/control/helpers/test_patch_applier.py` & `truss-0.4.3/truss/tests/templates/control/control/helpers/test_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/templates/control/control/test_server.py` & `truss-0.4.3/truss/tests/templates/control/control/test_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/templates/core/server/common/test_util.py` & `truss-0.4.3/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.4.3/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/test_backward.py` & `truss-0.4.3/truss/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/test_build.py` & `truss-0.4.3/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/test_config.py` & `truss-0.4.3/truss/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/test_context_builder_image.py` & `truss-0.4.3/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/test_docker.py` & `truss-0.4.3/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/test_model_inference.py` & `truss-0.4.3/truss/tests/test_model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/test_notebooks.py` & `truss-0.4.3/truss/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.4.3/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/test_truss_gatherer.py` & `truss-0.4.3/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/test_truss_handle.py` & `truss-0.4.3/truss/tests/test_truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/tests/test_validation.py` & `truss-0.4.3/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/truss_config.py` & `truss-0.4.3/truss/truss_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/truss_gatherer.py` & `truss-0.4.3/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/truss_handle.py` & `truss-0.4.3/truss/truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/truss_spec.py` & `truss-0.4.3/truss/truss_spec.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/types.py` & `truss-0.4.3/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/utils.py` & `truss-0.4.3/truss/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/truss/validation.py` & `truss-0.4.3/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.2/PKG-INFO` & `truss-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.4.2
+Version: 0.4.3
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.11
```

