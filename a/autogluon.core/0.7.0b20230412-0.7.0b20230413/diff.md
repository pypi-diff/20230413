# Comparing `tmp/autogluon.core-0.7.0b20230412.tar.gz` & `tmp/autogluon.core-0.7.0b20230413.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-0.7.0b20230412.tar", last modified: Wed Apr 12 09:03:53 2023, max compression
+gzip compressed data, was "autogluon.core-0.7.0b20230413.tar", last modified: Thu Apr 13 09:04:13 2023, max compression
```

## Comparing `autogluon.core-0.7.0b20230412.tar` & `autogluon.core-0.7.0b20230413.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.961276 autogluon.core-0.7.0b20230412/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-12 09:03:53.961276 autogluon.core-0.7.0b20230412/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:03:53.961276 autogluon.core-0.7.0b20230412/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.949276 autogluon.core-0.7.0b20230412/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.953276 autogluon.core-0.7.0b20230412/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.953276 autogluon.core-0.7.0b20230412/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.953276 autogluon.core-0.7.0b20230412/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.953276 autogluon.core-0.7.0b20230412/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.953276 autogluon.core-0.7.0b20230412/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.953276 autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27098 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.953276 autogluon.core-0.7.0b20230412/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.953276 autogluon.core-0.7.0b20230412/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)    23243 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.957276 autogluon.core-0.7.0b20230412/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.957276 autogluon.core-0.7.0b20230412/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    91851 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.957276 autogluon.core-0.7.0b20230412/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.957276 autogluon.core-0.7.0b20230412/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57864 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    39103 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.957276 autogluon.core-0.7.0b20230412/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.957276 autogluon.core-0.7.0b20230412/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.957276 autogluon.core-0.7.0b20230412/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14276 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.957276 autogluon.core-0.7.0b20230412/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.957276 autogluon.core-0.7.0b20230412/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/searcher/searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.957276 autogluon.core-0.7.0b20230412/src/autogluon/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.957276 autogluon.core-0.7.0b20230412/src/autogluon/core/task/base/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/task/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/task/base/base_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.957276 autogluon.core-0.7.0b20230412/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   169377 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.961276 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.961276 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.961276 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-12 09:03:35.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 09:03:53.000000 autogluon.core-0.7.0b20230412/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:03:53.953276 autogluon.core-0.7.0b20230412/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-12 09:03:53.000000 autogluon.core-0.7.0b20230412/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-12 09:03:53.000000 autogluon.core-0.7.0b20230412/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:03:53.000000 autogluon.core-0.7.0b20230412/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 09:03:53.000000 autogluon.core-0.7.0b20230412/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-12 09:03:53.000000 autogluon.core-0.7.0b20230412/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 09:03:53.000000 autogluon.core-0.7.0b20230412/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:03:53.000000 autogluon.core-0.7.0b20230412/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.449202 autogluon.core-0.7.0b20230413/
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-13 09:04:13.449202 autogluon.core-0.7.0b20230413/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 09:04:13.449202 autogluon.core-0.7.0b20230413/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.437202 autogluon.core-0.7.0b20230413/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.441202 autogluon.core-0.7.0b20230413/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.441202 autogluon.core-0.7.0b20230413/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.441202 autogluon.core-0.7.0b20230413/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.441202 autogluon.core-0.7.0b20230413/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.441202 autogluon.core-0.7.0b20230413/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.441202 autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27098 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.445202 autogluon.core-0.7.0b20230413/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.445202 autogluon.core-0.7.0b20230413/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)    23243 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.445202 autogluon.core-0.7.0b20230413/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.445202 autogluon.core-0.7.0b20230413/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91851 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.445202 autogluon.core-0.7.0b20230413/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.445202 autogluon.core-0.7.0b20230413/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57864 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40136 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.445202 autogluon.core-0.7.0b20230413/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.445202 autogluon.core-0.7.0b20230413/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.445202 autogluon.core-0.7.0b20230413/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14276 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.445202 autogluon.core-0.7.0b20230413/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.445202 autogluon.core-0.7.0b20230413/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/searcher/searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.445202 autogluon.core-0.7.0b20230413/src/autogluon/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.445202 autogluon.core-0.7.0b20230413/src/autogluon/core/task/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/task/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/task/base/base_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.449202 autogluon.core-0.7.0b20230413/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169377 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.449202 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.449202 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.449202 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-13 09:03:58.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 09:04:13.000000 autogluon.core-0.7.0b20230413/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:13.441202 autogluon.core-0.7.0b20230413/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-13 09:04:13.000000 autogluon.core-0.7.0b20230413/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-13 09:04:13.000000 autogluon.core-0.7.0b20230413/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:04:13.000000 autogluon.core-0.7.0b20230413/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 09:04:13.000000 autogluon.core-0.7.0b20230413/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-13 09:04:13.000000 autogluon.core-0.7.0b20230413/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 09:04:13.000000 autogluon.core-0.7.0b20230413/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:04:13.000000 autogluon.core-0.7.0b20230413/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-0.7.0b20230412/PKG-INFO` & `autogluon.core-0.7.0b20230413/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.7.0b20230412
+Version: 0.7.0b20230413
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.7.0b20230412/setup.py` & `autogluon.core-0.7.0b20230413/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/_setup_utils.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/_setup_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/augmentation/distill_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/calibrate/conformity_score.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/constants.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/data/cleaner.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/data/cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/data/label_cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/dataset.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/executors.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/executors.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/ray_hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/ray_tune_scheduler_factory.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/ray_tune_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/hpo/space_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/metrics/__init__.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/models/_utils.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/models/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/models/abstract/_tags.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,16 +351,20 @@
     X_pseudo: Union[str, pd.DataFrame],
     y_pseudo: Union[str, pd.DataFrame],
     fold_ctx: Dict[str, Any],
     time_limit_fold: float,
     save_bag_folds: bool, 
     resources: Dict[str, Any],
     kwargs_fold: Dict[str, Any],
+    head_node_id: str,
     model_sync_path: Optional[str] = None
 ):
+    import ray  # ray must be present
+    node_id = ray.get_runtime_context().get_node_id()
+    is_head_node = node_id == head_node_id
     logger.log(10, 'ray worker training')
     time_start_fold = time.time()
     fold, folds_finished, folds_left, \
         folds_to_fit, is_last_fold, \
         model_name_suffix = FoldFittingStrategy._get_fold_properties(fold_ctx)
     train_index, val_index = fold
     fold_model = copy.deepcopy(model_base)
@@ -388,15 +392,15 @@
     fold_model.fit(X=X_fold, y=y_fold, X_val=X_val_fold, y_val=y_val_fold,
                    time_limit=time_limit_fold, **resources, **kwargs_fold)
     time_train_end_fold = time.time()
     fold_model.fit_time = time_train_end_fold - time_start_fold
     fold_model, pred_proba = _ray_predict_oof(fold_model, X_val_fold, y_val_fold,
                                               time_train_end_fold, resources['num_cpus'], save_bag_folds)
     save_path = fold_model.save()
-    if model_sync_path is not None:
+    if model_sync_path is not None and not is_head_node:
         model_sync_path = model_sync_path + f"{fold_model.name}/"  # s3 path hence need "/" as the saperator
         bucket, prefix = s3_path_to_bucket_prefix(model_sync_path)
         upload_s3_folder(
             bucket=bucket,
             prefix=prefix,
             folder_to_upload=save_path,
             verbose=False
@@ -511,24 +515,36 @@
             log_to_driver=False
         )
 
     def after_all_folds_scheduled(self):
         if not self.ray.is_initialized():
             ray_init_args = self._get_ray_init_args()
             self.ray.init(**ray_init_args)
+        head_node_id = self.ray.get_runtime_context().get_node_id()
         job_refs = []
         job_fold_map = {}
         # prepare shared data
         X, y, X_pseudo, y_pseudo = self._prepare_data()
         model_base_ref = self.ray.put(self.model_base)
         time_limit_fold = self._get_fold_time_limit()
         # spread the task
         for job in self.jobs:
             fold_ctx = job
-            ref = self._fit(model_base_ref, X, y, X_pseudo, y_pseudo, time_limit_fold, fold_ctx, self.resources, self.model_base_kwargs)
+            ref = self._fit(
+                model_base_ref=model_base_ref,
+                X_ref=X,
+                y_ref=y,
+                X_pseudo_ref=X_pseudo,
+                y_pseudo_ref=y_pseudo,
+                time_limit_fold=time_limit_fold,
+                fold_ctx=fold_ctx,
+                resources=self.resources,
+                head_node_id=head_node_id,
+                kwargs=self.model_base_kwargs
+            )
             job_fold_map[ref] = fold_ctx
             job_refs.append(ref)
 
         # update ensemble whenever a model return
         unfinished = job_refs
         while unfinished:
             finished, unfinished = self.ray.wait(unfinished, num_returns=1)
@@ -541,14 +557,23 @@
                 self._update_bagged_ensemble(fold_model=fold_model,
                                              pred_proba=pred_proba,
                                              time_start_fit=time_start_fit,
                                              time_end_fit=time_end_fit,
                                              predict_time=predict_time,
                                              predict_1_time=predict_1_time,
                                              fold_ctx=fold_ctx)
+                model_sync_path = None
+                if self.model_sync_path is not None:
+                    model_sync_path: str = self.model_sync_path + fold_model
+                    if not model_sync_path.endswith("/"):
+                        model_sync_path += "/"
+                self.sync_model_artifact(
+                    local_path=os.path.join(self.bagged_ensemble_model.path + fold_model),
+                    model_sync_path=model_sync_path
+                )
             except TimeLimitExceeded:
                 # Terminate all ray tasks because a fold failed
                 self.terminate_all_unfinished_tasks(unfinished)
                 raise TimeLimitExceeded
             # NotEnoughMemoryError is an autogluon custom error,
             # it predict memory usage before hand
             # MemoryError is the actual python memory error if the process failed
@@ -564,28 +589,37 @@
                 self.terminate_all_unfinished_tasks(unfinished)
                 raise NotEnoughMemoryError
             except Exception as e:
                 processed_exception = self._parse_ray_error(e)
                 # Terminate all ray tasks because a fold failed
                 self.terminate_all_unfinished_tasks(unfinished)
                 raise processed_exception
-        self.sync_model_artifact(
-            local_path=self.bagged_ensemble_model.path,
-            model_sync_path=self.model_sync_path
-        )
         self.fit_time = 0
         if self.time_start_fit and self.time_end_fit:
             self.fit_time = self.time_end_fit - self.time_start_fit
         self.bagged_ensemble_model._add_parallel_child_times(fit_time=self.fit_time, predict_time=self.predict_time, predict_1_time=self.predict_1_time)
 
     def terminate_all_unfinished_tasks(self, unfinished_tasks):
         for task in unfinished_tasks:
             self.ray.cancel(task, force=True)
 
-    def _fit(self, model_base_ref, X_ref, y_ref, X_pseudo_ref, y_pseudo_ref, time_limit_fold, fold_ctx, resources, kwargs):
+    def _fit(
+        self,
+        *,
+        model_base_ref,
+        X_ref,
+        y_ref,
+        X_pseudo_ref,
+        y_pseudo_ref,
+        time_limit_fold,
+        fold_ctx,
+        resources,
+        head_node_id,
+        kwargs
+    ):
         fold, folds_finished, folds_left, \
             folds_to_fit, is_last_fold, \
             model_name_suffix = self._get_fold_properties(fold_ctx)
         logger.debug(f'Folding resources per job {resources}')
         train_index, val_index = fold
         fold_ctx_ref = self.ray.put(fold_ctx)
         save_bag_folds = self.bagged_ensemble_model.params.get('save_bag_folds', True)
@@ -607,14 +641,15 @@
                 X_pseudo=X_pseudo_ref,
                 y_pseudo=y_pseudo_ref,
                 fold_ctx=fold_ctx_ref,
                 time_limit_fold=time_limit_fold,
                 save_bag_folds=save_bag_folds,
                 resources=resources,
                 kwargs_fold=kwargs_fold,
+                head_node_id=head_node_id,
                 model_sync_path=self.model_sync_path
             )
 
     def _update_bagged_ensemble(self, fold_model, pred_proba, time_start_fit,
                                 time_end_fit, predict_time, predict_1_time, fold_ctx):
         _, val_index = fold_ctx['fold']
         self.models.append(fold_model)
```

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/ray/resources_calculator.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/searcher/local_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/searcher/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/space.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/task/base/base_task.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/task/base/base_task.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/trainer/utils.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/utils/decorators.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/utils/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/utils/files.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/utils/miscs.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/utils/miscs.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/utils/plots.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/utils/plots.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/utils/time.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/utils/utils.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon/core/utils/version_utils.py` & `autogluon.core-0.7.0b20230413/src/autogluon/core/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-0.7.0b20230413/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.7.0b20230412
+Version: 0.7.0b20230413
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.7.0b20230412/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-0.7.0b20230413/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

