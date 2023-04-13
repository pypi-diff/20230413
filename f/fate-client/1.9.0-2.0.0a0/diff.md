# Comparing `tmp/fate_client-1.9.0.tar.gz` & `tmp/fate-client-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fate_client-1.9.0.tar", max compression
+gzip compressed data, was "fate-client-2.0.0a0.tar", last modified: Fri Feb  3 09:28:23 2023, max compression
```

## Comparing `fate_client-1.9.0.tar` & `fate-client-2.0.0a0.tar`

### file list

```diff
@@ -1,210 +1,85 @@
--rw-r--r--   0        0        0       14 2022-09-02 08:09:40.729534 fate_client-1.9.0/README.rst
--rwxr-xr-x   0        0        0      616 2022-09-02 08:09:32.525486 fate_client-1.9.0/flow_client/__init__.py
--rw-r--r--   0        0        0     7142 2022-09-02 08:09:32.525486 fate_client-1.9.0/flow_client/flow.py
--rw-r--r--   0        0        0      616 2022-09-02 08:09:32.525486 fate_client-1.9.0/flow_client/flow_cli/__init__.py
--rw-r--r--   0        0        0      616 2022-09-02 08:09:32.525486 fate_client-1.9.0/flow_client/flow_cli/commands/__init__.py
--rw-r--r--   0        0        0     1956 2022-09-02 08:09:32.525486 fate_client-1.9.0/flow_client/flow_cli/commands/checkpoint.py
--rw-r--r--   0        0        0    11538 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/component.py
--rw-r--r--   0        0        0     5063 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/data.py
--rw-r--r--   0        0        0    10950 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/job.py
--rw-r--r--   0        0        0     2153 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/key.py
--rw-r--r--   0        0        0    17583 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/model.py
--rw-r--r--   0        0        0     2272 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/privilege.py
--rw-r--r--   0        0        0     2094 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/provider.py
--rw-r--r--   0        0        0     1182 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/queue.py
--rw-r--r--   0        0        0     1750 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/resource.py
--rw-r--r--   0        0        0     1482 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/server.py
--rw-r--r--   0        0        0     1273 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/service.py
--rw-r--r--   0        0        0     6001 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/table.py
--rw-r--r--   0        0        0     3699 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/tag.py
--rw-r--r--   0        0        0     1886 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/task.py
--rw-r--r--   0        0        0     2044 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/template.py
--rw-r--r--   0        0        0     2811 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/test.py
--rw-r--r--   0        0        0     8924 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/commands/tracking.py
--rw-r--r--   0        0        0      616 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/utils/__init__.py
--rw-r--r--   0        0        0     6594 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/utils/cli_args.py
--rw-r--r--   0        0        0     7929 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/utils/cli_utils.py
--rw-r--r--   0        0        0     1522 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/flow_cli/utils/detect_utils.py
--rw-r--r--   0        0        0       65 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_client/settings.yaml
--rw-r--r--   0        0        0      616 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/__init__.py
--rw-r--r--   0        0        0     1252 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/__init__.py
--rw-r--r--   0        0        0     1160 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/api/__init__.py
--rw-r--r--   0        0        0     1520 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/api/base.py
--rw-r--r--   0        0        0     1510 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/api/checkpoint.py
--rw-r--r--   0        0        0     5994 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/api/component.py
--rw-r--r--   0        0        0     3669 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/api/data.py
--rw-r--r--   0        0        0     4908 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/api/job.py
--rw-r--r--   0        0        0     6695 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/api/model.py
--rw-r--r--   0        0        0     1629 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/api/privilege.py
--rw-r--r--   0        0        0      763 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/api/queue.py
--rw-r--r--   0        0        0     1283 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/api/table.py
--rw-r--r--   0        0        0     1697 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/api/tag.py
--rw-r--r--   0        0        0     1144 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/api/task.py
--rw-r--r--   0        0        0     3698 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/api/test.py
--rw-r--r--   0        0        0     2036 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/api/version.py
--rw-r--r--   0        0        0     4394 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/client/base.py
--rw-r--r--   0        0        0     5047 2022-09-02 08:09:32.529487 fate_client-1.9.0/flow_sdk/utils.py
--rw-r--r--   0        0        0      321 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/__init__.py
--rw-r--r--   0        0        0     1188 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/backend/__init__.py
--rw-r--r--   0        0        0     3836 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/backend/_operation.py
--rw-r--r--   0        0        0     3562 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/backend/config.py
--rw-r--r--   0        0        0    32578 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/backend/pipeline.py
--rw-r--r--   0        0        0     2750 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/backend/task_info.py
--rw-r--r--   0        0        0     3218 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/__init__.py
--rw-r--r--   0        0        0     1375 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/cache_loader.py
--rw-r--r--   0        0        0     1355 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/column_expand.py
--rw-r--r--   0        0        0     7979 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/component_base.py
--rw-r--r--   0        0        0     1346 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/data_statistics.py
--rw-r--r--   0        0        0     1345 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/data_transform.py
--rw-r--r--   0        0        0     1415 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/dataio.py
--rw-r--r--   0        0        0     1317 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/evaluation.py
--rw-r--r--   0        0        0     1365 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/feature_imputation.py
--rw-r--r--   0        0        0     1358 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/feldman_verifiable_sum.py
--rw-r--r--   0        0        0     1351 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/hetero_data_split.py
--rw-r--r--   0        0        0     1460 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/hetero_fast_secureboost.py
--rw-r--r--   0        0        0     1362 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/hetero_feature_binning.py
--rw-r--r--   0        0        0     1356 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/hetero_feature_selection.py
--rw-r--r--   0        0        0     2852 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/hetero_ftl.py
--rw-r--r--   0        0        0     1358 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/hetero_kmeans.py
--rw-r--r--   0        0        0     1321 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/hetero_linr.py
--rw-r--r--   0        0        0     1343 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/hetero_lr.py
--rw-r--r--   0        0        0     5645 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/hetero_nn.py
--rw-r--r--   0        0        0     1301 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/hetero_pearson.py
--rw-r--r--   0        0        0     1331 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/hetero_poisson.py
--rw-r--r--   0        0        0     1358 2022-09-02 08:09:32.529487 fate_client-1.9.0/pipeline/component/hetero_secureboost.py
--rw-r--r--   0        0        0     1352 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/hetero_sshe_linr.py
--rw-r--r--   0        0        0     1340 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/hetero_sshe_lr.py
--rw-r--r--   0        0        0     1345 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/homo_data_split.py
--rw-r--r--   0        0        0     1371 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/homo_feature_binning.py
--rw-r--r--   0        0        0     1333 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/homo_lr.py
--rw-r--r--   0        0        0     2801 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/homo_nn.py
--rw-r--r--   0        0        0     1330 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/homo_onehot.py
--rw-r--r--   0        0        0     1349 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/homo_secureboost.py
--rw-r--r--   0        0        0     1340 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/intersection.py
--rw-r--r--   0        0        0     1367 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/label_transform.py
--rw-r--r--   0        0        0     1345 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/local_baseline.py
--rw-r--r--   0        0        0     1372 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/model_loader.py
--rw-r--r--   0        0        0        0 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/__init__.py
--rw-r--r--   0        0        0        0 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/__init__.py
--rw-r--r--   0        0        0      266 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/fate_torch/__init__.py
--rw-r--r--   0        0        0     3417 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/fate_torch/base.py
--rw-r--r--   0        0        0     1377 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/fate_torch/import_hook.py
--rw-r--r--   0        0        0     5980 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/fate_torch/init.py
--rw-r--r--   0        0        0    56623 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/fate_torch/nn.py
--rw-r--r--   0        0        0     3354 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/fate_torch/operation.py
--rw-r--r--   0        0        0     6620 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/fate_torch/optim.py
--rw-r--r--   0        0        0     3642 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/fate_torch/serialization.py
--rw-r--r--   0        0        0        0 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/fate_torch/torch_modules_extract/__init__.py
--rw-r--r--   0        0        0     3420 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/fate_torch/torch_modules_extract/extract_pytorch_modules.py
--rw-r--r--   0        0        0     1970 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/fate_torch/torch_modules_extract/extract_pytorch_optim.py
--rw-r--r--   0        0        0        0 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/keras/__init__.py
--rw-r--r--   0        0        0     2276 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/keras/model_builder.py
--rw-r--r--   0        0        0        0 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/pytorch/__init__.py
--rw-r--r--   0        0        0     1062 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/pytorch/model_builder.py
--rw-r--r--   0        0        0        0 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/tf/__init__.py
--rw-r--r--   0        0        0      918 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/backend/tf/model_builder.py
--rw-r--r--   0        0        0        0 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/models/__init__.py
--rw-r--r--   0        0        0     2861 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/nn/models/sequantial.py
--rw-r--r--   0        0        0     1326 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/one_hot_encoder.py
--rw-r--r--   0        0        0     1299 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/psi.py
--rw-r--r--   0        0        0     1133 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/reader.py
--rw-r--r--   0        0        0     1232 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/sample_weight.py
--rw-r--r--   0        0        0     1317 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/sampler.py
--rw-r--r--   0        0        0     1291 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/scale.py
--rw-r--r--   0        0        0     1310 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/scorecard.py
--rw-r--r--   0        0        0     1400 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/secure_information_retrieval.py
--rw-r--r--   0        0        0     1294 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/component/union.py
--rw-r--r--   0        0        0       90 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/config.yaml
--rw-r--r--   0        0        0     4017 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/constant.py
--rw-r--r--   0        0        0        0 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/demo/__init__.py
--rw-r--r--   0        0        0     5265 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/demo/pipeline-mini-demo.py
--rw-r--r--   0        0        0     2213 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/demo/pipeline-upload-spark.py
--rw-r--r--   0        0        0     1950 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/demo/pipeline-upload.py
--rw-r--r--   0        0        0      273 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/interface/__init__.py
--rw-r--r--   0        0        0      895 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/interface/cache.py
--rw-r--r--   0        0        0     1479 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/interface/data.py
--rw-r--r--   0        0        0     1914 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/interface/input.py
--rw-r--r--   0        0        0     1050 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/interface/model.py
--rw-r--r--   0        0        0     3257 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/interface/output.py
--rw-r--r--   0        0        0     3741 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/__init__.py
--rw-r--r--   0        0        0     6130 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/base_param.py
--rw-r--r--   0        0        0    35081 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/boosting_param.py
--rw-r--r--   0        0        0      948 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/cache_loader_param.py
--rw-r--r--   0        0        0     3567 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/callback_param.py
--rw-r--r--   0        0        0     3321 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/column_expand_param.py
--rw-r--r--   0        0        0     8281 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/consts.py
--rw-r--r--   0        0        0     3251 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/cross_validation_param.py
--rw-r--r--   0        0        0     4515 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/data_split_param.py
--rw-r--r--   0        0        0     8515 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/data_transform_param.py
--rw-r--r--   0        0        0     8289 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/dataio_param.py
--rw-r--r--   0        0        0     1481 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/encrypt_param.py
--rw-r--r--   0        0        0     1896 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/encrypted_mode_calculation_param.py
--rw-r--r--   0        0        0     6055 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/evaluation_param.py
--rw-r--r--   0        0        0    14541 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/feature_binning_param.py
--rw-r--r--   0        0        0     3811 2022-09-02 08:09:32.533486 fate_client-1.9.0/pipeline/param/feature_imputation_param.py
--rw-r--r--   0        0        0    22714 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/feature_selection_param.py
--rw-r--r--   0        0        0     2173 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/feldman_verifiable_sum_param.py
--rw-r--r--   0        0        0     7810 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/ftl_param.py
--rw-r--r--   0        0        0     9639 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/glm_param.py
--rw-r--r--   0        0        0     2211 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/hetero_kmeans_param.py
--rw-r--r--   0        0        0    11317 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/hetero_nn_param.py
--rw-r--r--   0        0        0     8024 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/hetero_sshe_linr_param.py
--rw-r--r--   0        0        0     8434 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/hetero_sshe_lr_param.py
--rw-r--r--   0        0        0     7003 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/homo_nn_param.py
--rw-r--r--   0        0        0     1307 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/homo_onehot_encoder_param.py
--rw-r--r--   0        0        0     2742 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/init_model_param.py
--rw-r--r--   0        0        0    25007 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/intersect_param.py
--rw-r--r--   0        0        0     2780 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/label_transform_param.py
--rw-r--r--   0        0        0     7207 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/linear_regression_param.py
--rw-r--r--   0        0        0     2219 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/local_baseline_param.py
--rw-r--r--   0        0        0    13063 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/logistic_regression_param.py
--rw-r--r--   0        0        0     1523 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/model_loader_param.py
--rw-r--r--   0        0        0     1456 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/one_vs_rest_param.py
--rw-r--r--   0        0        0     1819 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/onehot_encoder_param.py
--rw-r--r--   0        0        0     1633 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/onehot_encoder_with_alignment_param.py
--rw-r--r--   0        0        0     2979 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/pearson_param.py
--rw-r--r--   0        0        0     7753 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/poisson_regression_param.py
--rw-r--r--   0        0        0     1391 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/predict_param.py
--rw-r--r--   0        0        0     1480 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/psi_param.py
--rw-r--r--   0        0        0      742 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/reader_param.py
--rw-r--r--   0        0        0     2735 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/sample_param.py
--rw-r--r--   0        0        0     2737 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/sample_weight_param.py
--rw-r--r--   0        0        0     5074 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/scale_param.py
--rw-r--r--   0        0        0     3804 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/scorecard_param.py
--rw-r--r--   0        0        0     1371 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/secure_add_example_param.py
--rw-r--r--   0        0        0     4318 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/sir_param.py
--rw-r--r--   0        0        0     1814 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/sqn_param.py
--rw-r--r--   0        0        0     5750 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/statistics_param.py
--rw-r--r--   0        0        0     3512 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/stepwise_param.py
--rw-r--r--   0        0        0     2285 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/param/union_param.py
--rw-r--r--   0        0        0        0 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/parser/__init__.py
--rw-r--r--   0        0        0     5142 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/pipeline_cli.py
--rw-r--r--   0        0        0        0 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/runtime/__init__.py
--rw-r--r--   0        0        0     5453 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/runtime/entity.py
--rw-r--r--   0        0        0      616 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/__init__.py
--rw-r--r--   0        0        0      890 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_component.py
--rw-r--r--   0        0        0      731 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_evaluation.py
--rw-r--r--   0        0        0      851 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_hetero_linr.py
--rw-r--r--   0        0        0      847 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_hetero_lr.py
--rw-r--r--   0        0        0      757 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_hetero_nn.py
--rw-r--r--   0        0        0      790 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_hetero_pearson.py
--rw-r--r--   0        0        0      849 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_hetero_poisson.py
--rw-r--r--   0        0        0      783 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_hetero_secureboost.py
--rw-r--r--   0        0        0      739 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_homo_lr.py
--rw-r--r--   0        0        0      739 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_homo_nn.py
--rw-r--r--   0        0        0      775 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_homo_secureboost.py
--rw-r--r--   0        0        0      739 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_intersection.py
--rw-r--r--   0        0        0      783 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_local_baseline.py
--rw-r--r--   0        0        0      747 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_one_hot_encoder.py
--rw-r--r--   0        0        0      785 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_sampler.py
--rw-r--r--   0        0        0      725 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_scale.py
--rw-r--r--   0        0        0      711 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_union.py
--rw-r--r--   0        0        0     1860 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/test/test_upload.py
--rw-r--r--   0        0        0        0 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/utils/invoker/__init__.py
--rw-r--r--   0        0        0    18841 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/utils/invoker/job_submitter.py
--rw-r--r--   0        0        0     2213 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/utils/logger.py
--rw-r--r--   0        0        0     3127 2022-09-02 08:09:32.537487 fate_client-1.9.0/pipeline/utils/tools.py
--rw-r--r--   0        0        0     1362 2022-09-02 08:09:41.325539 fate_client-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     1715 2022-09-02 08:09:42.702515 fate_client-1.9.0/setup.py
--rw-r--r--   0        0        0     1419 2022-09-02 08:09:42.703001 fate_client-1.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.808302 fate-client-2.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-02-03 09:28:23.808302 fate-client-2.0.0a0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.804303 fate-client-2.0.0a0/fate_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.804303 fate-client-2.0.0a0/fate_client/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.804303 fate-client-2.0.0a0/fate_client/pipeline/component_define/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/component_define/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.804303 fate-client-2.0.0a0/fate_client/pipeline/component_define/fate/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/component_define/fate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/component_define/fate/evaluation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/component_define/fate/feature_scale.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/component_define/fate/hetero_lr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/component_define/fate/intersection.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/component_define/fate/reader.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.804303 fate-client-2.0.0a0/fate_client/pipeline/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/components/component_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.804303 fate-client-2.0.0a0/fate_client/pipeline/components/fate/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/components/fate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/components/fate/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/components/fate/feature_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/components/fate/intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/components/fate/lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/components/fate/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.804303 fate-client-2.0.0a0/fate_client/pipeline/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/conf/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/conf/job_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/conf/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.808302 fate-client-2.0.0a0/fate_client/pipeline/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/entity/component_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/entity/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/entity/dag_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/entity/model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/entity/model_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/entity/runtime_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/entity/task_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/entity/task_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.808302 fate-client-2.0.0a0/fate_client/pipeline/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/executor/task_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.808302 fate-client-2.0.0a0/fate_client/pipeline/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/interface/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.808302 fate-client-2.0.0a0/fate_client/pipeline/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/manager/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/manager/metric_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/manager/model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/manager/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/manager/status_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/manager/task_conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/pipeline_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/pipeline_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.808302 fate-client-2.0.0a0/fate_client/pipeline/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/scheduler/component_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27212 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/scheduler/dag_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/scheduler/runtime_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.808302 fate-client-2.0.0a0/fate_client/pipeline/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.808302 fate-client-2.0.0a0/fate_client/pipeline/utils/fateflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/utils/fateflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/utils/fateflow/fate_flow_job_invoker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/utils/fateflow/flow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/utils/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.808302 fate-client-2.0.0a0/fate_client/pipeline/utils/standalone/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/utils/standalone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/utils/standalone/id_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/utils/standalone/job_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/fate_client/pipeline/utils/uri_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:28:23.804303 fate-client-2.0.0a0/fate_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-02-03 09:28:23.000000 fate-client-2.0.0a0/fate_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-02-03 09:28:23.000000 fate-client-2.0.0a0/fate_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 09:28:23.000000 fate-client-2.0.0a0/fate_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-03 09:28:23.000000 fate-client-2.0.0a0/fate_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-03 09:28:23.000000 fate-client-2.0.0a0/fate_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-03 09:28:23.000000 fate-client-2.0.0a0/fate_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 09:28:23.808302 fate-client-2.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-02-03 09:28:22.000000 fate-client-2.0.0a0/setup.py
```

### Comparing `fate_client-1.9.0/flow_client/__init__.py` & `fate-client-2.0.0a0/fate_client/pipeline/component_define/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
```

### Comparing `fate_client-1.9.0/flow_client/flow_cli/__init__.py` & `fate-client-2.0.0a0/fate_client/pipeline/component_define/fate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
```

### Comparing `fate_client-1.9.0/flow_client/flow_cli/commands/__init__.py` & `fate-client-2.0.0a0/fate_client/pipeline/conf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
```

### Comparing `fate_client-1.9.0/flow_client/flow_cli/utils/__init__.py` & `fate-client-2.0.0a0/fate_client/pipeline/scheduler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
```

### Comparing `fate_client-1.9.0/flow_sdk/__init__.py` & `fate-client-2.0.0a0/fate_client/pipeline/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
```

### Comparing `fate_client-1.9.0/flow_sdk/client/api/queue.py` & `fate-client-2.0.0a0/fate_client/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,9 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-from flow_sdk.client.api.base import BaseFlowAPI
-
 
-class Queue(BaseFlowAPI):
-    def clean(self):
-        return self._post(url='job/clean/queue')
+__version__ = "2.0.0-alpha"
```

### Comparing `fate_client-1.9.0/pipeline/component/column_expand.py` & `fate-client-2.0.0a0/fate_client/pipeline/components/fate/evaluation.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-
-from pipeline.param.column_expand_param import ColumnExpandParam
-from pipeline.component.component_base import FateComponent
-from pipeline.interface import Input
-from pipeline.interface import Output
-from pipeline.utils.logger import LOGGER
-
-
-class ColumnExpand(FateComponent, ColumnExpandParam):
-    def __init__(self, **kwargs):
-        FateComponent.__init__(self, **kwargs)
-
-        #print (self.name)
-        LOGGER.debug(f"{self.name} component created")
-        new_kwargs = self.erase_component_base_param(**kwargs)
-
-        ColumnExpandParam.__init__(self, **new_kwargs)
-
-        self.input = Input(self.name)
-        self.output = Output(self.name, data_type='single', has_model=True)
-        self._module_name = "ColumnExpand"
+from typing import List
+from ...conf.types import PlaceHolder
+from ..component_base import Component
+from ...interface import ArtifactChannel
+
+
+class Evaluation(Component):
+    yaml_define_path = "./component_define/fate/evaluation.yaml"
+
+    def __init__(self,
+                 name: str,
+                 runtime_roles: List[str] = None,
+                 input_data: ArtifactChannel = PlaceHolder(),
+                 eval_type: str = PlaceHolder(),
+                 ):
+        inputs = locals()
+        self._process_init_inputs(inputs)
+        super(Evaluation, self).__init__()
+        self.name = name
+        self.runtime_roles = runtime_roles
+        self.input_data = input_data
+        self.eval_type = eval_type
```

### Comparing `fate_client-1.9.0/pipeline/component/data_transform.py` & `fate-client-2.0.0a0/fate_client/pipeline/components/fate/intersection.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-
-from pipeline.param.data_transform_param import DataTransformParam
-from pipeline.component.component_base import FateComponent
-from pipeline.interface import Input
-from pipeline.interface import Output
-from pipeline.utils.logger import LOGGER
-
-
-class DataTransform(FateComponent, DataTransformParam):
-    def __init__(self, **kwargs):
-        FateComponent.__init__(self, **kwargs)
-
-        #print (self.name)
-        LOGGER.debug(f"{self.name} component created")
-        new_kwargs = self.erase_component_base_param(**kwargs)
-
-        DataTransformParam.__init__(self, **new_kwargs)
-
-        self.input = Input(self.name)
-        self.output = Output(self.name, data_type='single')
-        self._module_name = "DataTransform"
+from typing import List
+from ...conf.types import PlaceHolder
+from ..component_base import Component
+from ...interface import ArtifactChannel
+
+
+class Intersection(Component):
+    yaml_define_path = "./component_define/fate/intersection.yaml"
+
+    def __init__(self,
+                 name: str,
+                 runtime_roles: List[str] = None,
+                 input_data: ArtifactChannel = PlaceHolder(),
+                 method: str = PlaceHolder(),
+                 ):
+        inputs = locals()
+        self._process_init_inputs(inputs)
+        super(Intersection, self).__init__()
+        self.name = name
+        self.runtime_roles = runtime_roles
+        self.input_data = input_data
+        self.method = method
```

### Comparing `fate_client-1.9.0/pipeline/component/feature_imputation.py` & `fate-client-2.0.0a0/fate_client/pipeline/components/fate/feature_scale.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,29 +8,33 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-
-from pipeline.param.feature_imputation_param import FeatureImputationParam
-from pipeline.component.component_base import FateComponent
-from pipeline.interface import Input
-from pipeline.interface import Output
-from pipeline.utils.logger import LOGGER
-
-
-class FeatureImputation(FateComponent, FeatureImputationParam):
-    def __init__(self, **kwargs):
-        FateComponent.__init__(self, **kwargs)
-
-        #print (self.name)
-        LOGGER.debug(f"{self.name} component created")
-
-        new_kwargs = self.erase_component_base_param(**kwargs)
-
-        FeatureImputationParam.__init__(self, **new_kwargs)
-        self.input = Input(self.name)
-        self.output = Output(self.name, has_model=True)
-        self._module_name = "FeatureImputation"
+from typing import List
+from ...conf.types import PlaceHolder
+from ..component_base import Component
+from ...interface import ArtifactChannel
+
+
+class FeatureScale(Component):
+    yaml_define_path = "./component_define/fate/feature_scale.yaml"
+
+    def __init__(self,
+                 name: str,
+                 runtime_roles: List[str] = None,
+                 method: str = PlaceHolder(),
+                 train_data: ArtifactChannel = PlaceHolder(),
+                 test_data: ArtifactChannel = PlaceHolder(),
+                 input_model: ArtifactChannel = PlaceHolder()
+                 ):
+        inputs = locals()
+        self._process_init_inputs(inputs)
+        super(FeatureScale, self).__init__()
+        self.name = name
+        self.runtime_roles = runtime_roles
+        self.method = method
+        self.train_data = train_data
+        self.test_data = test_data
+        self.input_model = input_model
```

### Comparing `fate_client-1.9.0/pipeline/component/nn/backend/tf/model_builder.py` & `fate-client-2.0.0a0/fate_client/pipeline/entity/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,21 +8,16 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-from collections import OrderedDict
-
-
-def build_model(model_type="sequential"):
-    if model_type != "sequential":
-        raise ValueError("Only support sequential model now")
-
-    return SequentialModel()
+from .dag import DAG
+from .task_info import FateFlowTaskInfo, StandaloneTaskInfo
 
 
-class SequentialModel(object):
-    def __init__(self):
-        self.__layers = OrderedDict()
+__all__ = [
+    "DAG",
+    "FateFlowTaskInfo",
+    "StandaloneTaskInfo"
+]
```

### Comparing `fate_client-1.9.0/pipeline/interface/cache.py` & `fate-client-2.0.0a0/fate_client/pipeline/interface/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,19 +8,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-
+from .channel import ArtifactChannel
 
-class Cache(object):
-    def __init__(self, cache=None):
-        self._cache = cache
 
-    def __getattr__(self, cache_key):
-        if cache_key == "cache":
-            return self._cache
-        else:
-            raise ValueError("cache key {} not support".format(cache_key))
+__all__ = ["ArtifactChannel"]
```

### Comparing `fate_client-1.9.0/pipeline/interface/data.py` & `fate-client-2.0.0a0/fate_client/pipeline/scheduler/component_stage.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,37 +8,53 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-from pipeline.backend.config import VERSION
-
-
-class Data(object):
-    def __init__(self, data=None, train_data=None, validate_data=None, test_data=None, predict_input=None):
-        self._data = data
-        self._train_data = train_data
-        self._validate_data = validate_data
-        self._test_data = test_data
-        self._predict_input = predict_input
-
-    def __getattr__(self, data_key):
-        if data_key == "train_data":
-            return self._train_data
-
-        elif data_key == "validate_data":
-            return self._validate_data
-
-        elif data_key == "test_data":
-            return self._test_data
+from typing import Dict
+from ..entity.component_structures import ArtifactSpec
 
-        elif data_key == "data":
-            return self._data
 
-        elif data_key == "predict_input":
-            return self._predict_input
+class ComponentStageSchedule(object):
+    @classmethod
+    def get_stage(cls, input_artifacts: Dict[str, ArtifactSpec]):
+        """
+        stage in [train, predict, default]
+        possible:
+            train_data, validate_data: stage = train
+            test_data: stage = predict
+            data: stage = default
+            train_data & input_model: stage = train
+            test_data & input_model: stage = train
+        """
+        stage = set()
+        data_type = 0
+        for input_key, artifact in input_artifacts.items():
+            if input_key == "train_data":
+                data_type |= 1
+            elif input_key == "validate_data":
+                data_type |= 2
+            elif input_key == "test_data":
+                data_type |= 4
+            else:
+                data_type |= 8
+
+            if not artifact.stages:
+                continue
+
+            stage_list = artifact.stages
+            if len(stage_list) == 1:
+                stage.add(stage_list[0])
+
+        if len(stage):
+            return list(stage)[0]
+
+        """the following is warm_start"""
+        if data_type & 1:
+            return "train"
+        if data_type & 4:
+            return "predict"
 
-        else:
-            raise ValueError("data key {} not support".format(data_key))
+        """the following is component which only has data key"""
+        return "default"
```

### Comparing `fate_client-1.9.0/pipeline/interface/model.py` & `fate-client-2.0.0a0/fate_client/pipeline/conf/job_configuration.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,22 +8,28 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
+class JobConf(object):
+    def __init__(self):
+        self._conf = dict()
+
+    def set(self, k, v):
+        self._conf[k] = v
+
+    def set_all(self, **kwargs):
+        self._conf.update(kwargs)
+
+    def update(self, conf: dict):
+        for k, v in conf.items():
+            if k not in self._conf:
+                self._conf[k] = v
+
+    def dict(self):
+        return self._conf
 
 
-class Model(object):
-    def __init__(self, model=None, isometric_model=None):
-        self._model = model
-        self._isometric_model = isometric_model
-
-    def __getattr__(self, model_key):
-        if model_key == "model":
-            return self.model
-        elif model_key == "isometric_model":
-            return self._isometric_model
-        else:
-            raise ValueError("model key {} not support".format(model_key))
+class TaskConf(JobConf):
+    ...
```

### Comparing `fate_client-1.9.0/pipeline/param/cache_loader_param.py` & `fate-client-2.0.0a0/fate_client/pipeline/executor/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,20 +8,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-
+from .task_executor import StandaloneExecutor
+from .task_executor import FateFlowExecutor
 
-class CacheLoaderParam:
-    def __init__(self, cache_key=None, job_id=None, component_name=None, cache_name=None):
-        super().__init__()
-        self.cache_key = cache_key
-        self.job_id = job_id
-        self.component_name = component_name
-        self.cache_name = cache_name
 
-    def check(self):
-        return True
+__all__ = [
+    "StandaloneExecutor",
+    "FateFlowExecutor"
+]
```

### Comparing `fate_client-1.9.0/pipeline/param/reader_param.py` & `fate-client-2.0.0a0/fate_client/pipeline/utils/fateflow/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,16 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-
-
-class ReaderParam:
-    def __init__(self, table=None):
-        self.table = table
-
-    def check(self):
-        return True
```

### Comparing `fate_client-1.9.0/pipeline/test/__init__.py` & `fate-client-2.0.0a0/fate_client/pipeline/utils/standalone/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
```

### Comparing `fate_client-1.9.0/pipeline/test/test_evaluation.py` & `fate-client-2.0.0a0/fate_client/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,16 +8,21 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
+import click
+from fate_client.pipeline.pipeline_cli import pipeline_group
+
 
+@click.group()
+def cli():
+    pass
 
-from pipeline.component.evaluation import Evaluation
 
+cli.add_command(pipeline_group)
 
-a = Evaluation(name="evaluation_0")
 
-print(a.output.data)
+if __name__ == '__main__':
+    cli()
```

### Comparing `fate_client-1.9.0/pipeline/test/test_hetero_linr.py` & `fate-client-2.0.0a0/fate_client/pipeline/components/fate/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,18 +8,12 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-
-
-from pipeline.component.hetero_linr import HeteroLinR
-
-
-a = HeteroLinR(name="hetero_linr_0", early_stop="weight_diff",
-               stepwise_param={"max_step": 3, "need_stepwise": True})
-
-print(a.output.data)
-print(a.output.model)
+from .evaluation import Evaluation
+from .feature_scale import FeatureScale
+from .lr import HeteroLR
+from .reader import Reader
+from .intersection import Intersection
```

### Comparing `fate_client-1.9.0/pipeline/test/test_homo_lr.py` & `fate-client-2.0.0a0/fate_client/pipeline/components/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,17 +8,12 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-
-
-from pipeline.component.homo_lr import HomoLR
-
-
-a = HomoLR(name="homo_lr_0")
+from .component_base import Component
 
-print(a.output.data)
-print(a.output.model)
+__all__ = ["Component",
+           "LR",
+           "DataInput"]
```

### Comparing `fate_client-1.9.0/pipeline/test/test_homo_nn.py` & `fate-client-2.0.0a0/fate_client/pipeline/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,17 +8,13 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-
-
-from pipeline.component.homo_nn import HomoNN
-
-
-a = HomoNN(name="homo_nn_0")
+from .pipeline import FateFlowPipeline, StandalonePipeline
 
-print(a.output.data)
-print(a.output.model)
+__all__ = [
+    "FateFlowPipeline",
+    "StandalonePipeline"
+]
```

