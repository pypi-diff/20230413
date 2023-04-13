# Comparing `tmp/openfl-x-1.4.0.dev2.tar.gz` & `tmp/openfl-x-1.4.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfl-x-1.4.0.dev2.tar", last modified: Thu Apr 13 09:50:00 2023, max compression
+gzip compressed data, was "openfl-x-1.4.0.dev3.tar", last modified: Thu Apr 13 10:27:01 2023, max compression
```

## Comparing `openfl-x-1.4.0.dev2.tar` & `openfl-x-1.4.0.dev3.tar`

### file list

```diff
@@ -1,738 +1,738 @@
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.914839 openfl-x-1.4.0.dev2/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    11356 2023-04-12 07:59:56.000000 openfl-x-1.4.0.dev2/LICENSE
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    63100 2023-04-12 07:59:56.000000 openfl-x-1.4.0.dev2/LICENSE-3RD-PARTY
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      143 2023-04-12 07:59:56.000000 openfl-x-1.4.0.dev2/MANIFEST.in
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      566 2023-04-12 07:59:56.000000 openfl-x-1.4.0.dev2/NOTICE
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8396 2023-04-13 09:50:00.916479 openfl-x-1.4.0.dev2/PKG-INFO
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7321 2023-04-12 15:29:31.000000 openfl-x-1.4.0.dev2/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.625655 openfl-x-1.4.0.dev2/openfl/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      161 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      136 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/__version__.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.928935 openfl-x-1.4.0.dev2/openfl/component/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      766 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/__init__.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.939769 openfl-x-1.4.0.dev2/openfl/component/aggregator/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      178 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/aggregator/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    46450 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/aggregator/aggregator.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.989880 openfl-x-1.4.0.dev2/openfl/component/assigner/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      418 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/assigner/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1083 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/assigner/adaboost_assigner.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2651 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/assigner/assigner.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2872 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/assigner/custom_assigner.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3898 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/assigner/random_grouped_assigner.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3692 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/assigner/static_grouped_assigner.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      593 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/assigner/tasks.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.013000 openfl-x-1.4.0.dev2/openfl/component/ca/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      101 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/ca/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     9606 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/ca/ca.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.024985 openfl-x-1.4.0.dev2/openfl/component/collaborator/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      186 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/collaborator/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    25128 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/collaborator/collaborator.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.046400 openfl-x-1.4.0.dev2/openfl/component/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      171 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/director/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    11997 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/director/director.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7133 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/director/experiment.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.059798 openfl-x-1.4.0.dev2/openfl/component/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      104 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/envoy/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7445 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/envoy/envoy.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.082841 openfl-x-1.4.0.dev2/openfl/component/straggler_handling_functions/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      495 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/straggler_handling_functions/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1171 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/straggler_handling_functions/cutoff_time_based_straggler_handling.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      954 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/straggler_handling_functions/percentage_based_straggler_handling.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      490 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/component/straggler_handling_functions/straggler_handling_function.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.110231 openfl-x-1.4.0.dev2/openfl/cryptography/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      117 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/cryptography/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5002 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/cryptography/ca.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2656 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/cryptography/io.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2233 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/cryptography/participant.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.122769 openfl-x-1.4.0.dev2/openfl/databases/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      172 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/databases/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    10269 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/databases/tensor_db.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.158328 openfl-x-1.4.0.dev2/openfl/databases/utilities/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      279 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/databases/utilities/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4542 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/databases/utilities/dataframe.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.162718 openfl-x-1.4.0.dev2/openfl/federated/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      787 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/__init__.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.213152 openfl-x-1.4.0.dev2/openfl/federated/data/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      931 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/data/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3819 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/data/federated_data.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1563 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/data/loader.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1556 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/data/loader_fe.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1683 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/data/loader_fets_challenge.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3572 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/data/loader_generic.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3342 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/data/loader_keras.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3473 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/data/loader_pt.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3219 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/data/loader_tf.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.227960 openfl-x-1.4.0.dev2/openfl/federated/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      154 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/plan/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    23194 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/plan/plan.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.293790 openfl-x-1.4.0.dev2/openfl/federated/task/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      915 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/task/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4279 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/task/fl_model.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     6745 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/task/runner.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    11749 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/task/runner_fe.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    26843 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/task/runner_fets_challenge.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    17357 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/task/runner_generic.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    19206 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/task/runner_keras.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    25565 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/task/runner_pt.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    15427 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/task/runner_tf.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    15238 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/federated/task/task_runner.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.382677 openfl-x-1.4.0.dev2/openfl/interface/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      114 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/__init__.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.472619 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      981 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1756 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/adagrad_adaptive_aggregation.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1983 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/adam_adaptive_aggregation.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      765 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/aggregate_adaboost.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      486 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/aggregate_random_forest.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.489268 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/core/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      292 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/core/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3945 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/core/adaptive_aggregation.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2675 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/core/interface.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.498959 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/experimental/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      246 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/experimental/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2439 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/experimental/privileged_aggregation.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      965 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/fedcurv_weighted_average.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3330 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/geometric_median.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      239 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/identity.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1825 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/median.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2007 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/weighted_average.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1982 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/yogi_adaptive_aggregation.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     6716 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/aggregator.py
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)     6271 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/cli.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7212 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/cli_helper.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    14500 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/collaborator.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4644 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/director.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5788 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/envoy.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.520874 openfl-x-1.4.0.dev2/openfl/interface/interactive_api/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      113 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/interactive_api/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    28527 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/interactive_api/experiment.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2420 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/interactive_api/federation.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2883 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/interactive_api/shard_descriptor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3684 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/pki.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8243 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/plan.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1434 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/tutorial.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    18808 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/interface/workspace.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.536591 openfl-x-1.4.0.dev2/openfl/native/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      142 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/native/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7053 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/native/fastestimator.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    10633 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/native/native.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.600626 openfl-x-1.4.0.dev2/openfl/pipelines/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      745 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/pipelines/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    16028 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/pipelines/eden_pipeline.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      448 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl/pipelines/generic_pipeline.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5032 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/pipelines/kc_pipeline.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      499 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/pipelines/no_compression_pipeline.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4954 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/pipelines/pipeline.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2274 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/pipelines/random_shift_pipeline.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7230 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/pipelines/skc_pipeline.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     6937 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/pipelines/stc_pipeline.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    10229 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/pipelines/tensor_codec.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.555173 openfl-x-1.4.0.dev2/openfl/plugins/
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.626924 openfl-x-1.4.0.dev2/openfl/plugins/frameworks_adapters/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4086 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/plugins/frameworks_adapters/flax_adapter.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      993 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/plugins/frameworks_adapters/framework_adapter_interface.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      974 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/plugins/frameworks_adapters/generic_adapter.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4565 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/plugins/frameworks_adapters/keras_adapter.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     9325 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/plugins/frameworks_adapters/pytorch_adapter.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.644717 openfl-x-1.4.0.dev2/openfl/plugins/interface_serializer/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      726 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/plugins/interface_serializer/cloudpickle_serializer.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      705 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/plugins/interface_serializer/dill_serializer.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      529 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/plugins/interface_serializer/serializer_interface.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.665596 openfl-x-1.4.0.dev2/openfl/plugins/processing_units_monitor/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1131 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/plugins/processing_units_monitor/cuda_device_monitor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      557 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/plugins/processing_units_monitor/device_monitor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2250 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/plugins/processing_units_monitor/pynvml_monitor.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.717300 openfl-x-1.4.0.dev2/openfl/protocols/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      113 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/protocols/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    12851 2023-04-13 09:47:55.000000 openfl-x-1.4.0.dev2/openfl/protocols/aggregator_pb2.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    13310 2023-04-13 09:47:55.000000 openfl-x-1.4.0.dev2/openfl/protocols/aggregator_pb2_grpc.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7197 2023-04-13 09:47:55.000000 openfl-x-1.4.0.dev2/openfl/protocols/base_pb2.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      159 2023-04-13 09:47:55.000000 openfl-x-1.4.0.dev2/openfl/protocols/base_pb2_grpc.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    23316 2023-04-13 09:47:55.000000 openfl-x-1.4.0.dev2/openfl/protocols/director_pb2.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    23866 2023-04-13 09:47:55.000000 openfl-x-1.4.0.dev2/openfl/protocols/director_pb2_grpc.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3093 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/protocols/interceptors.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     9400 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/protocols/utils.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.721140 openfl-x-1.4.0.dev2/openfl/transport/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      328 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/transport/__init__.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.750663 openfl-x-1.4.0.dev2/openfl/transport/grpc/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      370 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/transport/grpc/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    12211 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/transport/grpc/aggregator_client.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    10107 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/transport/grpc/aggregator_server.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    12288 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/transport/grpc/director_client.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    14324 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/transport/grpc/director_server.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      254 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/transport/grpc/grpc_channel_options.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.789842 openfl-x-1.4.0.dev2/openfl/utilities/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      204 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      607 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/ca.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1447 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/checks.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      916 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/click_types.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.804889 openfl-x-1.4.0.dev2/openfl/utilities/data_splitters/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      750 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/data_splitters/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      529 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/data_splitters/data_splitter.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     9292 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/data_splitters/numpy.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.810307 openfl-x-1.4.0.dev2/openfl/utilities/fedcurv/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      122 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/fedcurv/__init__.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.819064 openfl-x-1.4.0.dev2/openfl/utilities/fedcurv/torch/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      165 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/fedcurv/torch/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5561 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/fedcurv/torch/fedcurv.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1001 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/logs.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.577423 openfl-x-1.4.0.dev2/openfl/utilities/optimizers/
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.831803 openfl-x-1.4.0.dev2/openfl/utilities/optimizers/keras/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      218 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/optimizers/keras/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2665 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/optimizers/keras/fedprox.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.853272 openfl-x-1.4.0.dev2/openfl/utilities/optimizers/numpy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      304 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/optimizers/numpy/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3188 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/optimizers/numpy/adagrad_optimizer.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5062 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/optimizers/numpy/adam_optimizer.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1259 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/optimizers/numpy/base_optimizer.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2405 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/optimizers/numpy/yogi_optimizer.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.865628 openfl-x-1.4.0.dev2/openfl/utilities/optimizers/torch/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      259 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/optimizers/torch/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     9309 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/optimizers/torch/fedprox.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      525 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/path_check.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      860 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/types.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8130 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/utils.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4201 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev2/openfl/utilities/workspace.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.649504 openfl-x-1.4.0.dev2/openfl-docker/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2332 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-docker/Dockerfile.base
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      692 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-docker/Dockerfile.workspace
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      137 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-docker/Makefile
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      327 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-docker/start_actor_in_container.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.682983 openfl-x-1.4.0.dev2/openfl-gramine/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1255 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-gramine/Dockerfile.gramine
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      782 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-gramine/Dockerfile.graminized.workspace
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    11312 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-gramine/MANUAL.md
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1307 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-gramine/Makefile
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2130 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-gramine/openfl.manifest.template
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       74 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-gramine/start_process.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.731342 openfl-x-1.4.0.dev2/openfl-tutorials/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4880 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/Federated_FastEstimator_FGSM_Tutorial.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    13000 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/Federated_FedProx_Keras_MNIST_Tutorial.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    16978 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/Federated_FedProx_PyTorch_MNIST_Tutorial.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8488 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/Federated_Keras_MNIST_Tutorial.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    12243 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/Federated_PyTorch_TinyImageNet.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    17984 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/Federated_PyTorch_UNET_Tutorial.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8601 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/Federated_Pytorch_MNIST_Tutorial.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    33580 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/Federated_Pytorch_MNIST_custom_aggregation_Tutorial.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      319 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.736771 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.748134 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3200 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.760337 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      178 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/director/start_director.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.776591 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4052 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/envoy/cifar10_shard_descriptor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      172 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/envoy/envoy_config_1.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      424 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/envoy/start_envoy.sh
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      184 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.782900 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    18740 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/workspace/FLAX_CIFAR10_CNN.ipynb
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.789023 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5303 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.801937 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      107 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       76 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/director/start_director.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.829424 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      303 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/envoy/envoy_config_one.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      303 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/envoy/envoy_config_two.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5975 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/envoy/landmark_shard_descriptor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       13 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/envoy/sd_requirements.txt
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/envoy/start_envoy.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.844273 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    16398 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/workspace/MXNet_landmarks.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3227 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/workspace/mxnet_adapter.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       18 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/workspace/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.849278 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3617 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.860311 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      113 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/director/director_config.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/director/start_director.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.887590 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     6028 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/envoy/dogs_cats_shard_descriptor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      358 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/envoy/envoy_config_one.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      358 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/envoy/envoy_config_two.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       26 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/envoy/sd_requirements.txt
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      126 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/envoy/start_envoy.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.898770 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    17160 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/workspace/PyTorch_DogsCats_ViT.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       55 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/workspace/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.908431 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2028 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.925096 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      109 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       86 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/director/start_director.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/director/start_director_with_tls.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.959943 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       14 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/.gitignore
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      208 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/envoy_config.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4700 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/histology_shard_descriptor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       40 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/requirements.txt
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      122 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/start_envoy.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      226 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/start_envoy_with_tls.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.965853 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    37702 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/workspace/pytorch_histology.ipynb
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.972269 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      795 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.990034 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      109 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/director/start_director.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/director/start_director_with_tls.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.032411 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       14 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/.gitignore
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      208 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/envoy_config.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5035 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/histology_shard_descriptor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      719 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/populate_envoys.sh
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       41 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/requirements.txt
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      122 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/start_envoy.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      226 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/start_envoy_with_tls.sh
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      259 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/start_envoys.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.043481 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)        5 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/workspace/.gitignore
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    15683 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/workspace/pytorch_histology.ipynb
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.049663 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3659 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.060331 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      100 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/director/start_director.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.082303 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      302 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/envoy/envoy_config.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       43 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/envoy/sd_requirements.txt
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      122 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/envoy/start_envoy.sh
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3209 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/envoy/superb_shard_descriptor.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.088100 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    12391 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/workspace/PyTorch_Huggingface_transformers_SUPERB.ipynb
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.093668 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2171 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.111826 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      168 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/director/start_director.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/director/start_director_with_tls.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.153821 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      364 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/envoy_config.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      234 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/envoy_config_no_gpu.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5318 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/kvasir_shard_descriptor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4356 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/kvasir_shard_descriptor_with_data_splitter.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       19 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/sd_requirements.txt
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      122 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/start_envoy.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      227 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/start_envoy_with_tls.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.167497 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    18206 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/workspace/PyTorch_Kvasir_UNet.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2723 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/workspace/layers.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.175550 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)     4502 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.187770 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      106 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/director/start_director.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.217863 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      299 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/envoy/envoy_config.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/envoy/envoy_config_no_gpu.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3152 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/envoy/mnist_shard_descriptor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       60 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/envoy/sd_requirements.txt
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      122 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/envoy/start_envoy.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.230608 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    21090 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/workspace/PyTorch_Lightning_GAN.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1228 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/workspace/plugin_for_multiple_optimizers.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.237013 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)     4172 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.254769 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      123 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/director/start_director.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/director/start_director_with_tls.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.286532 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      214 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/envoy/envoy_config.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     6107 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/envoy/mvtec_shard_descriptor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       20 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/envoy/sd_requirements.txt
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      122 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/envoy/start_envoy.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      225 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/envoy/start_envoy_with_tls.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.309273 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    36869 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/PatchSVDD_with_Director.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1532 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/data_transf.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4410 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/inspection.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3215 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/utils.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.314775 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2044 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.333377 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       90 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/director/start_director.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/director/start_director_with_tls.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.399445 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      213 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/envoy_config_one.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      213 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/envoy_config_two.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4473 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/market_shard_descriptor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/requirements.txt
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      110 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/start_envoy.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      225 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/start_envoy_with_tls.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.422644 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    18337 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/PyTorch_Market_Re-ID.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2972 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/losses.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       32 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/requirements.txt
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5445 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/tools.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3364 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/transforms.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.427371 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2561 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.436722 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      116 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/director/start_director.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.458742 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      221 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/envoy/envoy_config.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4348 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/envoy/medmnist_shard_descriptor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)        9 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/envoy/requirements.txt
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/envoy/start_envoy.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.464210 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    17604 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/workspace/Pytorch_MedMNIST_2D.ipynb
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.471293 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2613 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.482711 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      117 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/director/start_director.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.506711 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      225 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/envoy/envoy_config.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4449 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/envoy/medmnist_shard_descriptor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       99 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/envoy/requirements.txt
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/envoy/start_envoy.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.512445 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    22729 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/Pytorch_MedMNIST_3D.ipynb
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.545060 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       65 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    15829 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/batchnorm.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4449 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/comm.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3226 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/replicate.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1165 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/utils.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.555061 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2036 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.574297 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      119 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/director/start_director.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/director/start_director_with_tls.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.603691 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      217 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/envoy/envoy_config.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       13 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/envoy/requirements.txt
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      121 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/envoy/start_envoy.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      226 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/envoy/start_envoy_with_tls.sh
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4228 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/envoy/tinyimagenet_shard_descriptor.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.621252 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     9509 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/workspace/non-federated_case.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    14573 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/workspace/pytorch_tinyimagenet.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/workspace/requirements.txt
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      268 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.627166 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2433 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.638059 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      112 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/director/start_director.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.661844 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3073 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/envoy/cifar10_shard_descriptor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      173 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/envoy/envoy_config_one.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      173 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/envoy/envoy_config_two.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/envoy/start_envoy.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.667539 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    11077 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/workspace/Tensorflow_CIFAR.ipynb
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.673980 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2059 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.693320 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      112 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/director/start_director.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/director/start_director_with_tls.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.723413 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      169 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/envoy/envoy_config_one.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      169 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/envoy/envoy_config_two.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3245 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/envoy/mnist_shard_descriptor.py
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/envoy/start_envoy.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      237 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/envoy/start_envoy_with_tls.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.729286 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    15046 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/workspace/Tensorflow_MNIST.ipynb
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.735669 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3325 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.752210 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       86 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/director/start_director.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/director/start_director_with_tls.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.791280 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      258 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/envoy_config_one.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      255 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/envoy_config_three.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      260 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/envoy_config_two.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       56 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/sd_requirements.txt
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4811 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/shard_descriptor.py
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      109 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/start_envoy.sh
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      221 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/start_envoy_with_tls.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.802974 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    14173 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/workspace/Tensorflow_Word_Prediction.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       32 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/workspace/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.808819 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1429 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.821596 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      221 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/director/director_config.yaml
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/director/start_director.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.847192 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      178 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/envoy/envoy_config_1.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2661 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/envoy/regression_shard_descriptor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      118 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/envoy/requirements.txt
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/envoy/start_envoy.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.861833 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    15490 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/workspace/JAX_linear_regression.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      661 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/workspace/custom_adapter.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.868583 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1758 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.874400 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/director/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      145 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/director/director_config.yaml
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.890256 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/envoy/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      181 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/envoy/envoy_config.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1995 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/envoy/linreg_shard_descriptor.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       99 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/envoy/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.922011 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    14228 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/LinReg.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    23398 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/SingleNotebook.ipynb
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      661 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/custom_adapter.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      121 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/requirements.txt
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5372 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/start_federation.ipynb
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.934260 openfl-x-1.4.0.dev2/openfl-workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      114 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/__init__.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.963306 openfl-x-1.4.0.dev2/openfl-workspace/default/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      444 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/default/director.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1162 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/default/envoy_config.yaml
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.980798 openfl-x-1.4.0.dev2/openfl-workspace/default/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/default/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      217 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/default/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      950 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/default/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/default/requirements.txt
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      650 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/default/shard_descriptor.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:58.993928 openfl-x-1.4.0.dev2/openfl-workspace/fe_tf_adversarial_cifar/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_tf_adversarial_cifar/.workspace
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.016604 openfl-x-1.4.0.dev2/openfl-workspace/fe_tf_adversarial_cifar/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_tf_adversarial_cifar/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      217 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_tf_adversarial_cifar/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_tf_adversarial_cifar/plan/defaults
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1189 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_tf_adversarial_cifar/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       72 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_tf_adversarial_cifar/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.032687 openfl-x-1.4.0.dev2/openfl-workspace/fe_tf_adversarial_cifar/src/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      153 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_tf_adversarial_cifar/src/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4024 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_tf_adversarial_cifar/src/fe_fgsm.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3070 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_tf_adversarial_cifar/src/fecifar_inmemory.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.043905 openfl-x-1.4.0.dev2/openfl-workspace/fe_torch_adversarial_cifar/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_torch_adversarial_cifar/.workspace
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.059220 openfl-x-1.4.0.dev2/openfl-workspace/fe_torch_adversarial_cifar/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_torch_adversarial_cifar/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      217 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_torch_adversarial_cifar/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1189 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_torch_adversarial_cifar/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       72 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_torch_adversarial_cifar/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.076754 openfl-x-1.4.0.dev2/openfl-workspace/fe_torch_adversarial_cifar/src/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_torch_adversarial_cifar/src/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3870 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_torch_adversarial_cifar/src/fe_fgsm.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3141 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fe_torch_adversarial_cifar/src/fecifar_inmemory.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.415996 openfl-x-1.4.0.dev2/openfl-workspace/fets_challenge_seg_test/
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.097694 openfl-x-1.4.0.dev2/openfl-workspace/fets_challenge_seg_test/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      180 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fets_challenge_seg_test/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      213 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fets_challenge_seg_test/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fets_challenge_seg_test/plan/defaults
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3137 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/fets_challenge_seg_test/plan/plan.yaml
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.107953 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/.workspace
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.130985 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      218 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/plan/defaults
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1183 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       18 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.153285 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/src/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/src/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2733 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/src/keras_cnn.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3856 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/src/mnist_utils.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1329 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/src/tfmnist_inmemory.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.164487 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/.workspace
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.185741 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      218 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/plan/defaults
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1301 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       18 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.208216 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/src/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/src/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2733 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/src/keras_cnn.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3856 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/src/mnist_utils.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1329 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/src/tfmnist_inmemory.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.220396 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/.workspace
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.236536 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      218 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1255 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       18 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.259536 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/src/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      116 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/src/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     9181 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/src/dataloader_utils.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4994 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/src/nlp_dataloader.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2676 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/src/nlp_taskrunner.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.271610 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/.workspace
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.289093 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      218 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1255 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       22 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.312839 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/src/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      116 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/src/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8839 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/src/dataloader_utils.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4397 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/src/nlp_dataloader.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2676 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/src/nlp_taskrunner.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.327889 openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/.workspace
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2415 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.346486 openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      183 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      631 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/plan/defaults
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1234 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       26 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.370283 openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/src/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/src/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5148 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/src/brats_utils.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    11190 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/src/nii_reader.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8200 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/src/tf_2dunet.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1495 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/src/tfbrats_inmemory.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.393838 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/.workspace
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7175 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/README.md
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.413166 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      192 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      824 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/data.yaml
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.475664 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/defaults/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       81 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/defaults/aggregator.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      253 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/defaults/assigner.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      148 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/defaults/collaborator.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       49 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/defaults/compression_pipeline.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       38 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/defaults/data_loader.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/defaults/defaults
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      311 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/defaults/network.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       54 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/defaults/task_runner.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      396 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/defaults/tasks_fast_estimator.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      394 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/defaults/tasks_keras.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      395 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/defaults/tasks_tensorflow.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      305 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/defaults/tasks_torch.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2045 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       29 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/requirements.txt
--rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)     2112 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/split_directory.sh
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.498788 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/src/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/src/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    10500 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/src/dataloader.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5507 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/src/define_model.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7970 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/src/tf_3dunet_model.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3197 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/src/tf_brats_dataloader.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.508051 openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/.workspace
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.525714 openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      183 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      572 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/plan/defaults
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1627 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       45 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.544447 openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/src/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/src/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3913 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/src/tf_cnn.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4000 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/src/tfds_utils.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1071 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/src/tfhistology_inmemory.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.548631 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.562320 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      182 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      180 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1150 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      140 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.584526 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/src/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/src/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5556 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/src/histology_utils.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5555 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/src/pt_cnn.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1047 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/src/pthistology_inmemory.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       60 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/src/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.588800 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology_gramine_ready/
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.603223 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology_gramine_ready/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      182 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology_gramine_ready/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      180 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology_gramine_ready/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1150 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology_gramine_ready/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       97 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology_gramine_ready/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.622317 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology_gramine_ready/src/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology_gramine_ready/src/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5556 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology_gramine_ready/src/histology_utils.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5555 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology_gramine_ready/src/pt_cnn.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1047 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology_gramine_ready/src/pthistology_inmemory.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.631602 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/.workspace
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.653702 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      565 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/plan/defaults
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1270 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       48 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.675703 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/src/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      153 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/src/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3778 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/src/mnist_utils.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7223 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/src/pt_cnn.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1422 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/src/ptmnist_inmemory.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.688359 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/.workspace
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.707191 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      565 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/plan/defaults
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1468 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       48 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.726091 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/src/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      153 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/src/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3778 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/src/mnist_utils.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7223 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/src/pt_cnn.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1422 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/src/ptmnist_inmemory.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.735896 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/.workspace
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.755445 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      183 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      576 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/plan/defaults
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1567 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       53 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.775041 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/src/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      153 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/src/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5177 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/src/data_loader.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4819 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/src/fed_unet_runner.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2884 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/src/pt_unet_parts.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.784446 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/.workspace
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.802588 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/plan/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      183 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/plan/cols.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      576 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/plan/data.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/plan/defaults
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1567 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/plan/plan.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      119 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/requirements.txt
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.825789 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/src/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      153 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/src/__init__.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5177 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/src/data_loader.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4819 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/src/fed_unet_runner.py
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2884 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/src/pt_unet_parts.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.837691 openfl-x-1.4.0.dev2/openfl-workspace/workspace/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/workspace/.workspace
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/workspace/__init__.py
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.504293 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.913861 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/defaults/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       98 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/defaults/aggregator.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      253 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/defaults/assigner.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      148 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/defaults/collaborator.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       49 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/defaults/compression_pipeline.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       38 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/defaults/data_loader.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      310 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/defaults/network.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       54 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/defaults/task_runner.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      480 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/defaults/tasks_fast_estimator.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      394 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/defaults/tasks_keras.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      395 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/defaults/tasks_tensorflow.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      320 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/defaults/tasks_torch.yaml
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:57.505976 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/plans/
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:49:59.924577 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/plans/default/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      934 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/plans/default/base_plan_interactive_api.yaml
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1058 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/plans/default/plan.yaml
-drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 09:50:00.909639 openfl-x-1.4.0.dev2/openfl_x.egg-info/
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8396 2023-04-13 09:49:56.000000 openfl-x-1.4.0.dev2/openfl_x.egg-info/PKG-INFO
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    33690 2023-04-13 09:49:57.000000 openfl-x-1.4.0.dev2/openfl_x.egg-info/SOURCES.txt
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)        1 2023-04-13 09:49:56.000000 openfl-x-1.4.0.dev2/openfl_x.egg-info/dependency_links.txt
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       50 2023-04-13 09:49:56.000000 openfl-x-1.4.0.dev2/openfl_x.egg-info/entry_points.txt
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      229 2023-04-13 09:49:56.000000 openfl-x-1.4.0.dev2/openfl_x.egg-info/requires.txt
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       70 2023-04-13 09:49:56.000000 openfl-x-1.4.0.dev2/openfl_x.egg-info/top_level.txt
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      534 2023-04-13 09:50:00.920028 openfl-x-1.4.0.dev2/setup.cfg
--rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     6265 2023-04-13 09:49:39.000000 openfl-x-1.4.0.dev2/setup.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.505678 openfl-x-1.4.0.dev3/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    11356 2023-04-12 07:59:56.000000 openfl-x-1.4.0.dev3/LICENSE
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    63100 2023-04-12 07:59:56.000000 openfl-x-1.4.0.dev3/LICENSE-3RD-PARTY
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      143 2023-04-12 07:59:56.000000 openfl-x-1.4.0.dev3/MANIFEST.in
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      566 2023-04-12 07:59:56.000000 openfl-x-1.4.0.dev3/NOTICE
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8312 2023-04-13 10:27:01.507863 openfl-x-1.4.0.dev3/PKG-INFO
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7237 2023-04-13 10:06:24.000000 openfl-x-1.4.0.dev3/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.435573 openfl-x-1.4.0.dev3/openfl/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      161 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      136 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/__version__.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.714875 openfl-x-1.4.0.dev3/openfl/component/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      766 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/__init__.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.724152 openfl-x-1.4.0.dev3/openfl/component/aggregator/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      178 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/aggregator/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    46450 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/aggregator/aggregator.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.762161 openfl-x-1.4.0.dev3/openfl/component/assigner/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      418 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/assigner/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1083 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/assigner/adaboost_assigner.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2651 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/assigner/assigner.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2872 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/assigner/custom_assigner.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3898 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/assigner/random_grouped_assigner.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3692 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/assigner/static_grouped_assigner.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      593 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/assigner/tasks.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.771543 openfl-x-1.4.0.dev3/openfl/component/ca/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      101 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/ca/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     9606 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/ca/ca.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.780017 openfl-x-1.4.0.dev3/openfl/component/collaborator/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      186 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/collaborator/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    25128 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/collaborator/collaborator.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.791690 openfl-x-1.4.0.dev3/openfl/component/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      171 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/director/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    11997 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/director/director.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7133 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/director/experiment.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.799045 openfl-x-1.4.0.dev3/openfl/component/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      104 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/envoy/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7445 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/envoy/envoy.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.814557 openfl-x-1.4.0.dev3/openfl/component/straggler_handling_functions/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      495 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/straggler_handling_functions/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1171 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/straggler_handling_functions/cutoff_time_based_straggler_handling.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      954 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/straggler_handling_functions/percentage_based_straggler_handling.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      490 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/component/straggler_handling_functions/straggler_handling_function.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.830798 openfl-x-1.4.0.dev3/openfl/cryptography/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      117 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/cryptography/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5002 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/cryptography/ca.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2656 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/cryptography/io.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2233 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/cryptography/participant.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.839199 openfl-x-1.4.0.dev3/openfl/databases/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      172 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/databases/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    10269 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/databases/tensor_db.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.848241 openfl-x-1.4.0.dev3/openfl/databases/utilities/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      279 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/databases/utilities/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4542 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/databases/utilities/dataframe.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.851918 openfl-x-1.4.0.dev3/openfl/federated/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      787 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/__init__.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.896388 openfl-x-1.4.0.dev3/openfl/federated/data/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      931 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/data/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3819 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/data/federated_data.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1563 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/data/loader.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1556 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/data/loader_fe.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1683 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/data/loader_fets_challenge.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3572 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/data/loader_generic.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3342 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/data/loader_keras.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3473 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/data/loader_pt.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3219 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/data/loader_tf.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.906615 openfl-x-1.4.0.dev3/openfl/federated/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      154 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/plan/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    23194 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/plan/plan.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.960300 openfl-x-1.4.0.dev3/openfl/federated/task/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      915 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/task/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4279 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/task/fl_model.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     6745 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/task/runner.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    11749 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/task/runner_fe.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    26843 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/task/runner_fets_challenge.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    17357 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/task/runner_generic.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    19206 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/task/runner_keras.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    25565 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/task/runner_pt.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    15427 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/task/runner_tf.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    15238 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/federated/task/task_runner.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.028334 openfl-x-1.4.0.dev3/openfl/interface/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      114 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/__init__.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.099696 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      981 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1756 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/adagrad_adaptive_aggregation.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1983 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/adam_adaptive_aggregation.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      765 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/aggregate_adaboost.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      486 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/aggregate_random_forest.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.116447 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/core/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      292 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/core/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3945 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/core/adaptive_aggregation.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2675 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/core/interface.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.147662 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/experimental/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      246 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/experimental/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2439 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/experimental/privileged_aggregation.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      965 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/fedcurv_weighted_average.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3330 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/geometric_median.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      239 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/identity.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1825 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/median.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2007 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/weighted_average.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1982 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/yogi_adaptive_aggregation.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     6716 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/aggregator.py
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)     6271 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/cli.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7212 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/cli_helper.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    14500 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/collaborator.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4644 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/director.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5788 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/envoy.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.169586 openfl-x-1.4.0.dev3/openfl/interface/interactive_api/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      113 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/interactive_api/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    28527 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/interactive_api/experiment.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2420 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/interactive_api/federation.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2883 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/interactive_api/shard_descriptor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3684 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/pki.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8243 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/plan.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1434 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/tutorial.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    18808 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/interface/workspace.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.182574 openfl-x-1.4.0.dev3/openfl/native/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      142 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/native/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7053 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/native/fastestimator.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    10633 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/native/native.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.230137 openfl-x-1.4.0.dev3/openfl/pipelines/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      745 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/pipelines/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    16028 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/pipelines/eden_pipeline.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      448 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl/pipelines/generic_pipeline.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5032 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/pipelines/kc_pipeline.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      499 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/pipelines/no_compression_pipeline.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4954 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/pipelines/pipeline.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2274 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/pipelines/random_shift_pipeline.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7230 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/pipelines/skc_pipeline.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     6937 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/pipelines/stc_pipeline.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    10229 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/pipelines/tensor_codec.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.366539 openfl-x-1.4.0.dev3/openfl/plugins/
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.254456 openfl-x-1.4.0.dev3/openfl/plugins/frameworks_adapters/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4086 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/plugins/frameworks_adapters/flax_adapter.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      993 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/plugins/frameworks_adapters/framework_adapter_interface.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      974 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/plugins/frameworks_adapters/generic_adapter.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4565 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/plugins/frameworks_adapters/keras_adapter.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     9325 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/plugins/frameworks_adapters/pytorch_adapter.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.266599 openfl-x-1.4.0.dev3/openfl/plugins/interface_serializer/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      726 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/plugins/interface_serializer/cloudpickle_serializer.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      705 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/plugins/interface_serializer/dill_serializer.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      529 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/plugins/interface_serializer/serializer_interface.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.280340 openfl-x-1.4.0.dev3/openfl/plugins/processing_units_monitor/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1131 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/plugins/processing_units_monitor/cuda_device_monitor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      557 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/plugins/processing_units_monitor/device_monitor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2250 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/plugins/processing_units_monitor/pynvml_monitor.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.323858 openfl-x-1.4.0.dev3/openfl/protocols/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      113 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/protocols/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    12851 2023-04-13 10:24:27.000000 openfl-x-1.4.0.dev3/openfl/protocols/aggregator_pb2.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    13310 2023-04-13 10:24:27.000000 openfl-x-1.4.0.dev3/openfl/protocols/aggregator_pb2_grpc.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7197 2023-04-13 10:24:27.000000 openfl-x-1.4.0.dev3/openfl/protocols/base_pb2.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      159 2023-04-13 10:24:27.000000 openfl-x-1.4.0.dev3/openfl/protocols/base_pb2_grpc.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    23316 2023-04-13 10:24:27.000000 openfl-x-1.4.0.dev3/openfl/protocols/director_pb2.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    23866 2023-04-13 10:24:27.000000 openfl-x-1.4.0.dev3/openfl/protocols/director_pb2_grpc.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3093 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/protocols/interceptors.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     9400 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/protocols/utils.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.327523 openfl-x-1.4.0.dev3/openfl/transport/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      328 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/transport/__init__.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.356402 openfl-x-1.4.0.dev3/openfl/transport/grpc/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      370 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/transport/grpc/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    12211 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/transport/grpc/aggregator_client.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    10107 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/transport/grpc/aggregator_server.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    12288 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/transport/grpc/director_client.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    14324 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/transport/grpc/director_server.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      254 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/transport/grpc/grpc_channel_options.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.393356 openfl-x-1.4.0.dev3/openfl/utilities/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      204 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      607 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/ca.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1447 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/checks.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      916 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/click_types.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.407039 openfl-x-1.4.0.dev3/openfl/utilities/data_splitters/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      750 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/data_splitters/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      529 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/data_splitters/data_splitter.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     9292 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/data_splitters/numpy.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.411129 openfl-x-1.4.0.dev3/openfl/utilities/fedcurv/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      122 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/fedcurv/__init__.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.422838 openfl-x-1.4.0.dev3/openfl/utilities/fedcurv/torch/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      165 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/fedcurv/torch/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5561 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/fedcurv/torch/fedcurv.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1001 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/logs.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.384202 openfl-x-1.4.0.dev3/openfl/utilities/optimizers/
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.438572 openfl-x-1.4.0.dev3/openfl/utilities/optimizers/keras/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      218 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/optimizers/keras/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2665 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/optimizers/keras/fedprox.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.463619 openfl-x-1.4.0.dev3/openfl/utilities/optimizers/numpy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      304 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/optimizers/numpy/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3188 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/optimizers/numpy/adagrad_optimizer.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5062 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/optimizers/numpy/adam_optimizer.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1259 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/optimizers/numpy/base_optimizer.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2405 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/optimizers/numpy/yogi_optimizer.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.472976 openfl-x-1.4.0.dev3/openfl/utilities/optimizers/torch/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      259 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/optimizers/torch/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     9309 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/optimizers/torch/fedprox.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      525 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/path_check.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      860 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/types.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8130 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/utils.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4201 2023-04-12 08:00:01.000000 openfl-x-1.4.0.dev3/openfl/utilities/workspace.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.458893 openfl-x-1.4.0.dev3/openfl-docker/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2332 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-docker/Dockerfile.base
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      692 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-docker/Dockerfile.workspace
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      137 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-docker/Makefile
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      327 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-docker/start_actor_in_container.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.495544 openfl-x-1.4.0.dev3/openfl-gramine/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1255 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-gramine/Dockerfile.gramine
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      782 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-gramine/Dockerfile.graminized.workspace
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    11312 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-gramine/MANUAL.md
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1307 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-gramine/Makefile
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2130 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-gramine/openfl.manifest.template
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       74 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-gramine/start_process.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.548316 openfl-x-1.4.0.dev3/openfl-tutorials/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4880 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/Federated_FastEstimator_FGSM_Tutorial.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    13000 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/Federated_FedProx_Keras_MNIST_Tutorial.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    16978 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/Federated_FedProx_PyTorch_MNIST_Tutorial.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8488 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/Federated_Keras_MNIST_Tutorial.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    12243 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/Federated_PyTorch_TinyImageNet.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    17984 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/Federated_PyTorch_UNET_Tutorial.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8601 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/Federated_Pytorch_MNIST_Tutorial.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    33580 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/Federated_Pytorch_MNIST_custom_aggregation_Tutorial.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      319 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.553983 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.566668 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3200 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.578233 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      178 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/director/start_director.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.595112 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4052 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/envoy/cifar10_shard_descriptor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      172 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/envoy/envoy_config_1.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      424 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/envoy/start_envoy.sh
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      184 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.601672 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    18740 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/workspace/FLAX_CIFAR10_CNN.ipynb
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.607905 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5303 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.619084 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      107 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       76 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/director/start_director.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.651777 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      303 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/envoy/envoy_config_one.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      303 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/envoy/envoy_config_two.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5975 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/envoy/landmark_shard_descriptor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       13 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/envoy/sd_requirements.txt
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/envoy/start_envoy.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.667317 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    16398 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/workspace/MXNet_landmarks.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3227 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/workspace/mxnet_adapter.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       18 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/workspace/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.673387 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3617 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.683348 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      113 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/director/director_config.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/director/start_director.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.709479 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     6028 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/envoy/dogs_cats_shard_descriptor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      358 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/envoy/envoy_config_one.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      358 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/envoy/envoy_config_two.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       26 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/envoy/sd_requirements.txt
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      126 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/envoy/start_envoy.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.719371 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    17160 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/workspace/PyTorch_DogsCats_ViT.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       55 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/workspace/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.723900 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2028 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.739228 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      109 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       86 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/director/start_director.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/director/start_director_with_tls.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.781153 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       14 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/.gitignore
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      208 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/envoy_config.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4700 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/histology_shard_descriptor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       40 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/requirements.txt
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      122 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/start_envoy.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      226 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/start_envoy_with_tls.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.790875 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    37702 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/workspace/pytorch_histology.ipynb
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.797124 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      795 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.816104 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      109 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/director/start_director.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/director/start_director_with_tls.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.864187 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       14 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/.gitignore
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      208 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/envoy_config.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5035 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/histology_shard_descriptor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      719 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/populate_envoys.sh
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       41 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/requirements.txt
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      122 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/start_envoy.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      226 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/start_envoy_with_tls.sh
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      259 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/start_envoys.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.876403 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)        5 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/workspace/.gitignore
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    15683 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/workspace/pytorch_histology.ipynb
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.882532 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3659 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.893129 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      100 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/director/start_director.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.916917 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      302 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/envoy/envoy_config.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       43 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/envoy/sd_requirements.txt
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      122 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/envoy/start_envoy.sh
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3209 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/envoy/superb_shard_descriptor.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.924607 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    12391 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/workspace/PyTorch_Huggingface_transformers_SUPERB.ipynb
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.931172 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2171 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.948995 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      168 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/director/start_director.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/director/start_director_with_tls.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.993178 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      364 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/envoy_config.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      234 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/envoy_config_no_gpu.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5318 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/kvasir_shard_descriptor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4356 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/kvasir_shard_descriptor_with_data_splitter.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       19 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/sd_requirements.txt
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      122 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/start_envoy.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      227 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/start_envoy_with_tls.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.005389 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    18206 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/workspace/PyTorch_Kvasir_UNet.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2723 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/workspace/layers.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.011260 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)     4502 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.022790 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      106 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/director/start_director.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.055591 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      299 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/envoy/envoy_config.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/envoy/envoy_config_no_gpu.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3152 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/envoy/mnist_shard_descriptor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       60 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/envoy/sd_requirements.txt
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      122 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/envoy/start_envoy.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.066524 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    21090 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/workspace/PyTorch_Lightning_GAN.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1228 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/workspace/plugin_for_multiple_optimizers.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.072136 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)     4172 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.088119 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      123 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/director/start_director.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/director/start_director_with_tls.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.113893 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      214 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/envoy/envoy_config.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     6107 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/envoy/mvtec_shard_descriptor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       20 2023-04-12 07:59:58.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/envoy/sd_requirements.txt
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      122 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/envoy/start_envoy.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      225 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/envoy/start_envoy_with_tls.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.135213 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    36869 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/PatchSVDD_with_Director.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1532 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/data_transf.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4410 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/inspection.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3215 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/utils.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.141662 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2044 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.161804 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       90 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/director/start_director.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/director/start_director_with_tls.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.194111 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      213 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/envoy_config_one.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      213 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/envoy_config_two.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4473 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/market_shard_descriptor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/requirements.txt
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      110 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/start_envoy.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      225 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/start_envoy_with_tls.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.218640 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    18337 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/PyTorch_Market_Re-ID.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2972 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/losses.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       32 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/requirements.txt
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5445 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/tools.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3364 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/transforms.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.223919 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2561 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.234417 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      116 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/director/start_director.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.258951 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      221 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/envoy/envoy_config.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4348 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/envoy/medmnist_shard_descriptor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)        9 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/envoy/requirements.txt
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/envoy/start_envoy.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.265056 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    17604 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/workspace/Pytorch_MedMNIST_2D.ipynb
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.270233 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2613 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.280571 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      117 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/director/start_director.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.303023 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      225 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/envoy/envoy_config.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4449 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/envoy/medmnist_shard_descriptor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       99 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/envoy/requirements.txt
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/envoy/start_envoy.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.308856 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    22729 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/Pytorch_MedMNIST_3D.ipynb
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.348626 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       65 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    15829 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/batchnorm.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4449 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/comm.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3226 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/replicate.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1165 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/utils.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.353126 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2036 2023-04-13 10:26:59.355036 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.367168 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      119 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/director/start_director.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/director/start_director_with_tls.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.394541 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      217 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/envoy/envoy_config.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       13 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/envoy/requirements.txt
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      121 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/envoy/start_envoy.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      226 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/envoy/start_envoy_with_tls.sh
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4228 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/envoy/tinyimagenet_shard_descriptor.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.409426 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     9509 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/workspace/non-federated_case.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    14573 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/workspace/pytorch_tinyimagenet.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/workspace/requirements.txt
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      268 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.413838 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2433 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.423067 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      112 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/director/start_director.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.441622 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3073 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/envoy/cifar10_shard_descriptor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      173 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/envoy/envoy_config_one.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      173 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/envoy/envoy_config_two.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/envoy/start_envoy.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.446686 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    11077 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/workspace/Tensorflow_CIFAR.ipynb
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.452008 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2059 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.467922 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      112 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/director/start_director.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/director/start_director_with_tls.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.493641 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      169 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/envoy/envoy_config_one.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      169 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/envoy/envoy_config_two.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3245 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/envoy/mnist_shard_descriptor.py
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/envoy/start_envoy.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      237 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/envoy/start_envoy_with_tls.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.498247 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    15046 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/workspace/Tensorflow_MNIST.ipynb
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.502843 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3325 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.517729 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       86 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/director/start_director.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      135 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/director/start_director_with_tls.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.553339 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      258 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/envoy_config_one.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      255 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/envoy_config_three.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      260 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/envoy_config_two.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       56 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/sd_requirements.txt
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4811 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/shard_descriptor.py
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      109 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/start_envoy.sh
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      221 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/start_envoy_with_tls.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.563848 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    14173 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/workspace/Tensorflow_Word_Prediction.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       32 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/workspace/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.568065 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1429 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.577312 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      221 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/director/director_config.yaml
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)       75 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/director/start_director.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.596695 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      178 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/envoy/envoy_config_1.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2661 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/envoy/regression_shard_descriptor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      118 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/envoy/requirements.txt
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/envoy/start_envoy.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.610664 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    15490 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/workspace/JAX_linear_regression.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      661 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/workspace/custom_adapter.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.615328 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1758 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.620935 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/director/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      145 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/director/director_config.yaml
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.635074 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/envoy/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      181 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/envoy/envoy_config.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1995 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/envoy/linreg_shard_descriptor.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       99 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/envoy/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.671180 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    14228 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/LinReg.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    23398 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/SingleNotebook.ipynb
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      661 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/custom_adapter.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      121 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/requirements.txt
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5372 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/start_federation.ipynb
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.676495 openfl-x-1.4.0.dev3/openfl-workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      114 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/__init__.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.698007 openfl-x-1.4.0.dev3/openfl-workspace/default/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      444 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/default/director.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1162 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/default/envoy_config.yaml
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.715230 openfl-x-1.4.0.dev3/openfl-workspace/default/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/default/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      217 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/default/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      950 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/default/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/default/requirements.txt
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      650 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/default/shard_descriptor.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.727746 openfl-x-1.4.0.dev3/openfl-workspace/fe_tf_adversarial_cifar/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_tf_adversarial_cifar/.workspace
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.748644 openfl-x-1.4.0.dev3/openfl-workspace/fe_tf_adversarial_cifar/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_tf_adversarial_cifar/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      217 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_tf_adversarial_cifar/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_tf_adversarial_cifar/plan/defaults
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1189 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_tf_adversarial_cifar/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       72 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_tf_adversarial_cifar/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.765192 openfl-x-1.4.0.dev3/openfl-workspace/fe_tf_adversarial_cifar/src/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      153 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_tf_adversarial_cifar/src/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4024 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_tf_adversarial_cifar/src/fe_fgsm.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3070 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_tf_adversarial_cifar/src/fecifar_inmemory.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.774858 openfl-x-1.4.0.dev3/openfl-workspace/fe_torch_adversarial_cifar/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_torch_adversarial_cifar/.workspace
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.788328 openfl-x-1.4.0.dev3/openfl-workspace/fe_torch_adversarial_cifar/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_torch_adversarial_cifar/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      217 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_torch_adversarial_cifar/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1189 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_torch_adversarial_cifar/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       72 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_torch_adversarial_cifar/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.802143 openfl-x-1.4.0.dev3/openfl-workspace/fe_torch_adversarial_cifar/src/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_torch_adversarial_cifar/src/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3870 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_torch_adversarial_cifar/src/fe_fgsm.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3141 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fe_torch_adversarial_cifar/src/fecifar_inmemory.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.249257 openfl-x-1.4.0.dev3/openfl-workspace/fets_challenge_seg_test/
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.820921 openfl-x-1.4.0.dev3/openfl-workspace/fets_challenge_seg_test/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      180 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fets_challenge_seg_test/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      213 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fets_challenge_seg_test/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fets_challenge_seg_test/plan/defaults
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3137 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/fets_challenge_seg_test/plan/plan.yaml
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.832857 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/.workspace
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.853118 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      218 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/plan/defaults
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1183 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       18 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.871532 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/src/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/src/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2733 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/src/keras_cnn.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3856 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/src/mnist_utils.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1329 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/src/tfmnist_inmemory.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.881529 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/.workspace
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.901544 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      218 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/plan/defaults
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1301 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       18 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.920667 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/src/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/src/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2733 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/src/keras_cnn.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3856 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/src/mnist_utils.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1329 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/src/tfmnist_inmemory.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.931208 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/.workspace
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.946761 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      218 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1255 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       18 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.969047 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/src/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      116 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/src/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     9181 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/src/dataloader_utils.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4994 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/src/nlp_dataloader.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2676 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/src/nlp_taskrunner.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.979992 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/.workspace
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:59.997294 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      218 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1255 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       22 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.021394 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/src/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      116 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/src/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8839 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/src/dataloader_utils.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4397 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/src/nlp_dataloader.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2676 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/src/nlp_taskrunner.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.045930 openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/.workspace
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2415 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.072919 openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      183 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      631 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/plan/defaults
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1234 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       26 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.103005 openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/src/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/src/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5148 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/src/brats_utils.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    11190 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/src/nii_reader.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8200 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/src/tf_2dunet.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1495 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/src/tfbrats_inmemory.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.124261 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/.workspace
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7175 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/README.md
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.141199 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      192 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      824 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/data.yaml
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.233276 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/defaults/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       81 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/defaults/aggregator.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      253 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/defaults/assigner.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      148 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/defaults/collaborator.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       49 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/defaults/compression_pipeline.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       38 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/defaults/data_loader.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/defaults/defaults
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      311 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/defaults/network.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       54 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/defaults/task_runner.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      396 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/defaults/tasks_fast_estimator.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      394 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/defaults/tasks_keras.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      395 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/defaults/tasks_tensorflow.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      305 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/defaults/tasks_torch.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2045 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       29 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/requirements.txt
+-rwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)     2112 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/split_directory.sh
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.257539 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/src/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 07:59:59.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/src/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    10500 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/src/dataloader.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5507 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/src/define_model.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7970 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/src/tf_3dunet_model.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3197 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/src/tf_brats_dataloader.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.268519 openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/.workspace
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.302159 openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      183 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      572 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/plan/defaults
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1627 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       45 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.322908 openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/src/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/src/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3913 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/src/tf_cnn.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4000 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/src/tfds_utils.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1071 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/src/tfhistology_inmemory.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.329455 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.347027 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      182 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      180 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1150 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      140 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.373336 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/src/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/src/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5556 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/src/histology_utils.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5555 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/src/pt_cnn.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1047 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/src/pthistology_inmemory.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       60 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/src/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.379611 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology_gramine_ready/
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.396673 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology_gramine_ready/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      182 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology_gramine_ready/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      180 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology_gramine_ready/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1150 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology_gramine_ready/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       97 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology_gramine_ready/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.419604 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology_gramine_ready/src/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology_gramine_ready/src/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5556 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology_gramine_ready/src/histology_utils.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5555 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology_gramine_ready/src/pt_cnn.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1047 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology_gramine_ready/src/pthistology_inmemory.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.430507 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/.workspace
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.451526 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      565 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/plan/defaults
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1270 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       48 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.470256 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/src/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      153 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/src/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3778 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/src/mnist_utils.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7223 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/src/pt_cnn.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1422 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/src/ptmnist_inmemory.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.481513 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/.workspace
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.502666 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      185 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      565 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/plan/defaults
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1468 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       48 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.523636 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/src/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      153 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/src/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     3778 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/src/mnist_utils.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     7223 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/src/pt_cnn.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1422 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/src/ptmnist_inmemory.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.532680 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/.workspace
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.551168 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      183 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      576 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/plan/defaults
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1567 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       53 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.572001 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/src/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      153 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/src/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5177 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/src/data_loader.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4819 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/src/fed_unet_runner.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2884 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/src/pt_unet_parts.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.582295 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/.workspace
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.604721 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/plan/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      183 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/plan/cols.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      576 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/plan/data.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       31 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/plan/defaults
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1567 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/plan/plan.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      119 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/requirements.txt
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.631382 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/src/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      153 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/src/__init__.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     5177 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/src/data_loader.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     4819 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/src/fed_unet_runner.py
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     2884 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/src/pt_unet_parts.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.640106 openfl-x-1.4.0.dev3/openfl-workspace/workspace/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       28 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/workspace/.workspace
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      152 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/workspace/__init__.py
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.321615 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.699749 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/defaults/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       98 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/defaults/aggregator.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      253 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/defaults/assigner.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      148 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/defaults/collaborator.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       49 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/defaults/compression_pipeline.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       38 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/defaults/data_loader.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      310 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/defaults/network.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       54 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/defaults/task_runner.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      480 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/defaults/tasks_fast_estimator.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      394 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/defaults/tasks_keras.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      395 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/defaults/tasks_tensorflow.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      320 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/defaults/tasks_torch.yaml
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:26:58.323131 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/plans/
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:00.710633 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/plans/default/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      934 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/plans/default/base_plan_interactive_api.yaml
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     1058 2023-04-12 08:00:00.000000 openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/plans/default/plan.yaml
+drwxrwxr-x   0 lmancuso  (1001) lmancuso  (1001)        0 2023-04-13 10:27:01.500006 openfl-x-1.4.0.dev3/openfl_x.egg-info/
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     8312 2023-04-13 10:26:57.000000 openfl-x-1.4.0.dev3/openfl_x.egg-info/PKG-INFO
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)    33690 2023-04-13 10:26:58.000000 openfl-x-1.4.0.dev3/openfl_x.egg-info/SOURCES.txt
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)        1 2023-04-13 10:26:57.000000 openfl-x-1.4.0.dev3/openfl_x.egg-info/dependency_links.txt
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       50 2023-04-13 10:26:57.000000 openfl-x-1.4.0.dev3/openfl_x.egg-info/entry_points.txt
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      229 2023-04-13 10:26:57.000000 openfl-x-1.4.0.dev3/openfl_x.egg-info/requires.txt
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)       88 2023-04-13 10:26:57.000000 openfl-x-1.4.0.dev3/openfl_x.egg-info/top_level.txt
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)      534 2023-04-13 10:27:01.511746 openfl-x-1.4.0.dev3/setup.cfg
+-rw-rw-r--   0 lmancuso  (1001) lmancuso  (1001)     6294 2023-04-13 10:26:42.000000 openfl-x-1.4.0.dev3/setup.py
```

### Comparing `openfl-x-1.4.0.dev2/LICENSE` & `openfl-x-1.4.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/LICENSE-3RD-PARTY` & `openfl-x-1.4.0.dev3/LICENSE-3RD-PARTY`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/NOTICE` & `openfl-x-1.4.0.dev3/NOTICE`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/PKG-INFO` & `openfl-x-1.4.0.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfl-x
-Version: 1.4.0.dev2
+Version: 1.4.0.dev3
 Summary: Model-agnostic federated learning
 Home-page: https://github.com/alpha-unito/OpenFL-extended
 Author: Gianluca Mittone
 Project-URL: Source Code, https://github.com/alpha-unito/OpenFL-extended
 Classifier: Environment :: Console
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -31,19 +31,17 @@
 
 
 ## Installation
 
 It is highly recommended to create a **virtual environment** prior to installing OpenFL-x (with both [venv](https://docs.python.org/3/library/venv.html) or [conda](https://docs.conda.io/en/latest/)) to avoid compatibility issues with existing Python software already installed on the system.
 Furthermore, since OpenFL-x is an extended version of OpenFL, it integrates all the features of the base framework plus the federated bagging and boosting functionalities: it is then suggested to **not install both software in the same virtual environment** since this can lead to issues in the working of both software.
 
-To install OpenFL-x, clone this repository and run `pip install`:
+You can get the lates version of OpenFL-x from `pypi`:
 ```
-git clone https://github.com/alpha-unito/OpenFL-extended.git
-cd OpenFL-extended
-pip install .
+pip install openfl-x
 ```
 If this procedure completes successfully, you now have access to all the base features of OpenFL, plus the distributed bagging and boosting functionalities. Enjoy!
 
 
 
 ## Getting Started
```

### Comparing `openfl-x-1.4.0.dev2/README.md` & `openfl-x-1.4.0.dev3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,19 +5,17 @@
 
 
 ## Installation
 
 It is highly recommended to create a **virtual environment** prior to installing OpenFL-x (with both [venv](https://docs.python.org/3/library/venv.html) or [conda](https://docs.conda.io/en/latest/)) to avoid compatibility issues with existing Python software already installed on the system.
 Furthermore, since OpenFL-x is an extended version of OpenFL, it integrates all the features of the base framework plus the federated bagging and boosting functionalities: it is then suggested to **not install both software in the same virtual environment** since this can lead to issues in the working of both software.
 
-To install OpenFL-x, clone this repository and run `pip install`:
+You can get the lates version of OpenFL-x from `pypi`:
 ```
-git clone https://github.com/alpha-unito/OpenFL-extended.git
-cd OpenFL-extended
-pip install .
+pip install openfl-x
 ```
 If this procedure completes successfully, you now have access to all the base features of OpenFL, plus the distributed bagging and boosting functionalities. Enjoy!
 
 
 
 ## Getting Started
```

### Comparing `openfl-x-1.4.0.dev2/openfl/component/__init__.py` & `openfl-x-1.4.0.dev3/openfl/component/__init__.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/component/aggregator/aggregator.py` & `openfl-x-1.4.0.dev3/openfl/component/aggregator/aggregator.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/component/assigner/adaboost_assigner.py` & `openfl-x-1.4.0.dev3/openfl/component/assigner/adaboost_assigner.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/component/assigner/assigner.py` & `openfl-x-1.4.0.dev3/openfl/component/assigner/assigner.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/component/assigner/custom_assigner.py` & `openfl-x-1.4.0.dev3/openfl/component/assigner/custom_assigner.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/component/assigner/random_grouped_assigner.py` & `openfl-x-1.4.0.dev3/openfl/component/assigner/random_grouped_assigner.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/component/assigner/static_grouped_assigner.py` & `openfl-x-1.4.0.dev3/openfl/component/assigner/static_grouped_assigner.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/component/assigner/tasks.py` & `openfl-x-1.4.0.dev3/openfl/component/assigner/tasks.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/component/ca/ca.py` & `openfl-x-1.4.0.dev3/openfl/component/ca/ca.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/component/collaborator/collaborator.py` & `openfl-x-1.4.0.dev3/openfl/component/collaborator/collaborator.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/component/director/director.py` & `openfl-x-1.4.0.dev3/openfl/component/director/director.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/component/director/experiment.py` & `openfl-x-1.4.0.dev3/openfl/component/director/experiment.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/component/envoy/envoy.py` & `openfl-x-1.4.0.dev3/openfl/component/envoy/envoy.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/component/straggler_handling_functions/cutoff_time_based_straggler_handling.py` & `openfl-x-1.4.0.dev3/openfl/component/straggler_handling_functions/cutoff_time_based_straggler_handling.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/component/straggler_handling_functions/percentage_based_straggler_handling.py` & `openfl-x-1.4.0.dev3/openfl/component/straggler_handling_functions/percentage_based_straggler_handling.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/cryptography/ca.py` & `openfl-x-1.4.0.dev3/openfl/cryptography/ca.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/cryptography/io.py` & `openfl-x-1.4.0.dev3/openfl/cryptography/io.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/cryptography/participant.py` & `openfl-x-1.4.0.dev3/openfl/cryptography/participant.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/databases/tensor_db.py` & `openfl-x-1.4.0.dev3/openfl/databases/tensor_db.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/databases/utilities/dataframe.py` & `openfl-x-1.4.0.dev3/openfl/databases/utilities/dataframe.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/__init__.py` & `openfl-x-1.4.0.dev3/openfl/federated/__init__.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/data/__init__.py` & `openfl-x-1.4.0.dev3/openfl/federated/data/__init__.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/data/federated_data.py` & `openfl-x-1.4.0.dev3/openfl/federated/data/federated_data.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/data/loader.py` & `openfl-x-1.4.0.dev3/openfl/federated/data/loader.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/data/loader_fe.py` & `openfl-x-1.4.0.dev3/openfl/federated/data/loader_fe.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/data/loader_fets_challenge.py` & `openfl-x-1.4.0.dev3/openfl/federated/data/loader_fets_challenge.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/data/loader_generic.py` & `openfl-x-1.4.0.dev3/openfl/federated/data/loader_generic.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/data/loader_keras.py` & `openfl-x-1.4.0.dev3/openfl/federated/data/loader_keras.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/data/loader_pt.py` & `openfl-x-1.4.0.dev3/openfl/federated/data/loader_pt.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/data/loader_tf.py` & `openfl-x-1.4.0.dev3/openfl/federated/data/loader_tf.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/plan/plan.py` & `openfl-x-1.4.0.dev3/openfl/federated/plan/plan.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/task/__init__.py` & `openfl-x-1.4.0.dev3/openfl/federated/task/__init__.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/task/fl_model.py` & `openfl-x-1.4.0.dev3/openfl/federated/task/fl_model.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/task/runner.py` & `openfl-x-1.4.0.dev3/openfl/federated/task/runner.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/task/runner_fe.py` & `openfl-x-1.4.0.dev3/openfl/federated/task/runner_fe.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/task/runner_fets_challenge.py` & `openfl-x-1.4.0.dev3/openfl/federated/task/runner_fets_challenge.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/task/runner_generic.py` & `openfl-x-1.4.0.dev3/openfl/federated/task/runner_generic.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/task/runner_keras.py` & `openfl-x-1.4.0.dev3/openfl/federated/task/runner_keras.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/task/runner_pt.py` & `openfl-x-1.4.0.dev3/openfl/federated/task/runner_pt.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/task/runner_tf.py` & `openfl-x-1.4.0.dev3/openfl/federated/task/runner_tf.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/federated/task/task_runner.py` & `openfl-x-1.4.0.dev3/openfl/federated/task/task_runner.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/__init__.py` & `openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/adagrad_adaptive_aggregation.py` & `openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/adagrad_adaptive_aggregation.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/adam_adaptive_aggregation.py` & `openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/adam_adaptive_aggregation.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/aggregate_adaboost.py` & `openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/aggregate_adaboost.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/core/adaptive_aggregation.py` & `openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/core/adaptive_aggregation.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/core/interface.py` & `openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/core/interface.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/experimental/privileged_aggregation.py` & `openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/experimental/privileged_aggregation.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/fedcurv_weighted_average.py` & `openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/fedcurv_weighted_average.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/geometric_median.py` & `openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/geometric_median.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/median.py` & `openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/median.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/weighted_average.py` & `openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/weighted_average.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/aggregation_functions/yogi_adaptive_aggregation.py` & `openfl-x-1.4.0.dev3/openfl/interface/aggregation_functions/yogi_adaptive_aggregation.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/aggregator.py` & `openfl-x-1.4.0.dev3/openfl/interface/aggregator.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/cli.py` & `openfl-x-1.4.0.dev3/openfl/interface/cli.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/cli_helper.py` & `openfl-x-1.4.0.dev3/openfl/interface/cli_helper.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/collaborator.py` & `openfl-x-1.4.0.dev3/openfl/interface/collaborator.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/director.py` & `openfl-x-1.4.0.dev3/openfl/interface/director.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/envoy.py` & `openfl-x-1.4.0.dev3/openfl/interface/envoy.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/interactive_api/experiment.py` & `openfl-x-1.4.0.dev3/openfl/interface/interactive_api/experiment.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/interactive_api/federation.py` & `openfl-x-1.4.0.dev3/openfl/interface/interactive_api/federation.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/interactive_api/shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl/interface/interactive_api/shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/pki.py` & `openfl-x-1.4.0.dev3/openfl/interface/pki.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/plan.py` & `openfl-x-1.4.0.dev3/openfl/interface/plan.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/tutorial.py` & `openfl-x-1.4.0.dev3/openfl/interface/tutorial.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/interface/workspace.py` & `openfl-x-1.4.0.dev3/openfl/interface/workspace.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/native/fastestimator.py` & `openfl-x-1.4.0.dev3/openfl/native/fastestimator.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/native/native.py` & `openfl-x-1.4.0.dev3/openfl/native/native.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/pipelines/__init__.py` & `openfl-x-1.4.0.dev3/openfl/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/pipelines/eden_pipeline.py` & `openfl-x-1.4.0.dev3/openfl/pipelines/eden_pipeline.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/pipelines/kc_pipeline.py` & `openfl-x-1.4.0.dev3/openfl/pipelines/kc_pipeline.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/pipelines/pipeline.py` & `openfl-x-1.4.0.dev3/openfl/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/pipelines/random_shift_pipeline.py` & `openfl-x-1.4.0.dev3/openfl/pipelines/random_shift_pipeline.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/pipelines/skc_pipeline.py` & `openfl-x-1.4.0.dev3/openfl/pipelines/skc_pipeline.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/pipelines/stc_pipeline.py` & `openfl-x-1.4.0.dev3/openfl/pipelines/stc_pipeline.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/pipelines/tensor_codec.py` & `openfl-x-1.4.0.dev3/openfl/pipelines/tensor_codec.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/plugins/frameworks_adapters/flax_adapter.py` & `openfl-x-1.4.0.dev3/openfl/plugins/frameworks_adapters/flax_adapter.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/plugins/frameworks_adapters/framework_adapter_interface.py` & `openfl-x-1.4.0.dev3/openfl/plugins/frameworks_adapters/framework_adapter_interface.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/plugins/frameworks_adapters/generic_adapter.py` & `openfl-x-1.4.0.dev3/openfl/plugins/frameworks_adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/plugins/frameworks_adapters/keras_adapter.py` & `openfl-x-1.4.0.dev3/openfl/plugins/frameworks_adapters/keras_adapter.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/plugins/frameworks_adapters/pytorch_adapter.py` & `openfl-x-1.4.0.dev3/openfl/plugins/frameworks_adapters/pytorch_adapter.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/plugins/interface_serializer/cloudpickle_serializer.py` & `openfl-x-1.4.0.dev3/openfl/plugins/interface_serializer/cloudpickle_serializer.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/plugins/interface_serializer/dill_serializer.py` & `openfl-x-1.4.0.dev3/openfl/plugins/interface_serializer/dill_serializer.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/plugins/interface_serializer/serializer_interface.py` & `openfl-x-1.4.0.dev3/openfl/plugins/interface_serializer/serializer_interface.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/plugins/processing_units_monitor/cuda_device_monitor.py` & `openfl-x-1.4.0.dev3/openfl/plugins/processing_units_monitor/cuda_device_monitor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/plugins/processing_units_monitor/device_monitor.py` & `openfl-x-1.4.0.dev3/openfl/plugins/processing_units_monitor/device_monitor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/plugins/processing_units_monitor/pynvml_monitor.py` & `openfl-x-1.4.0.dev3/openfl/plugins/processing_units_monitor/pynvml_monitor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/protocols/aggregator_pb2.py` & `openfl-x-1.4.0.dev3/openfl/protocols/aggregator_pb2.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/protocols/aggregator_pb2_grpc.py` & `openfl-x-1.4.0.dev3/openfl/protocols/aggregator_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/protocols/base_pb2.py` & `openfl-x-1.4.0.dev3/openfl/protocols/base_pb2.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/protocols/director_pb2.py` & `openfl-x-1.4.0.dev3/openfl/protocols/director_pb2.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/protocols/director_pb2_grpc.py` & `openfl-x-1.4.0.dev3/openfl/protocols/director_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/protocols/interceptors.py` & `openfl-x-1.4.0.dev3/openfl/protocols/interceptors.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/protocols/utils.py` & `openfl-x-1.4.0.dev3/openfl/protocols/utils.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/transport/grpc/aggregator_client.py` & `openfl-x-1.4.0.dev3/openfl/transport/grpc/aggregator_client.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/transport/grpc/aggregator_server.py` & `openfl-x-1.4.0.dev3/openfl/transport/grpc/aggregator_server.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/transport/grpc/director_client.py` & `openfl-x-1.4.0.dev3/openfl/transport/grpc/director_client.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/transport/grpc/director_server.py` & `openfl-x-1.4.0.dev3/openfl/transport/grpc/director_server.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/ca.py` & `openfl-x-1.4.0.dev3/openfl/utilities/ca.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/checks.py` & `openfl-x-1.4.0.dev3/openfl/utilities/checks.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/click_types.py` & `openfl-x-1.4.0.dev3/openfl/utilities/click_types.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/data_splitters/__init__.py` & `openfl-x-1.4.0.dev3/openfl/utilities/data_splitters/__init__.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/data_splitters/data_splitter.py` & `openfl-x-1.4.0.dev3/openfl/utilities/data_splitters/data_splitter.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/data_splitters/numpy.py` & `openfl-x-1.4.0.dev3/openfl/utilities/data_splitters/numpy.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/fedcurv/torch/fedcurv.py` & `openfl-x-1.4.0.dev3/openfl/utilities/fedcurv/torch/fedcurv.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/logs.py` & `openfl-x-1.4.0.dev3/openfl/utilities/logs.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/optimizers/keras/fedprox.py` & `openfl-x-1.4.0.dev3/openfl/utilities/optimizers/keras/fedprox.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/optimizers/numpy/adagrad_optimizer.py` & `openfl-x-1.4.0.dev3/openfl/utilities/optimizers/numpy/adagrad_optimizer.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/optimizers/numpy/adam_optimizer.py` & `openfl-x-1.4.0.dev3/openfl/utilities/optimizers/numpy/adam_optimizer.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/optimizers/numpy/base_optimizer.py` & `openfl-x-1.4.0.dev3/openfl/utilities/optimizers/numpy/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/optimizers/numpy/yogi_optimizer.py` & `openfl-x-1.4.0.dev3/openfl/utilities/optimizers/numpy/yogi_optimizer.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/optimizers/torch/fedprox.py` & `openfl-x-1.4.0.dev3/openfl/utilities/optimizers/torch/fedprox.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/path_check.py` & `openfl-x-1.4.0.dev3/openfl/utilities/path_check.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/types.py` & `openfl-x-1.4.0.dev3/openfl/utilities/types.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/utils.py` & `openfl-x-1.4.0.dev3/openfl/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl/utilities/workspace.py` & `openfl-x-1.4.0.dev3/openfl/utilities/workspace.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-docker/Dockerfile.base` & `openfl-x-1.4.0.dev3/openfl-docker/Dockerfile.base`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-docker/Dockerfile.workspace` & `openfl-x-1.4.0.dev3/openfl-docker/Dockerfile.workspace`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-gramine/Dockerfile.gramine` & `openfl-x-1.4.0.dev3/openfl-gramine/Dockerfile.gramine`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-gramine/Dockerfile.graminized.workspace` & `openfl-x-1.4.0.dev3/openfl-gramine/Dockerfile.graminized.workspace`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-gramine/MANUAL.md` & `openfl-x-1.4.0.dev3/openfl-gramine/MANUAL.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-gramine/Makefile` & `openfl-x-1.4.0.dev3/openfl-gramine/Makefile`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-gramine/openfl.manifest.template` & `openfl-x-1.4.0.dev3/openfl-gramine/openfl.manifest.template`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/Federated_FastEstimator_FGSM_Tutorial.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/Federated_FastEstimator_FGSM_Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/Federated_FedProx_Keras_MNIST_Tutorial.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/Federated_FedProx_Keras_MNIST_Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/Federated_FedProx_PyTorch_MNIST_Tutorial.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/Federated_FedProx_PyTorch_MNIST_Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/Federated_Keras_MNIST_Tutorial.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/Federated_Keras_MNIST_Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/Federated_PyTorch_TinyImageNet.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/Federated_PyTorch_TinyImageNet.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/Federated_PyTorch_UNET_Tutorial.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/Federated_PyTorch_UNET_Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/Federated_Pytorch_MNIST_Tutorial.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/Federated_Pytorch_MNIST_Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/Federated_Pytorch_MNIST_custom_aggregation_Tutorial.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/Federated_Pytorch_MNIST_custom_aggregation_Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/envoy/cifar10_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/envoy/cifar10_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/workspace/FLAX_CIFAR10_CNN.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Flax_CNN_CIFAR/workspace/FLAX_CIFAR10_CNN.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/envoy/landmark_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/envoy/landmark_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/workspace/MXNet_landmarks.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/workspace/MXNet_landmarks.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/MXNet_landmarks/workspace/mxnet_adapter.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/MXNet_landmarks/workspace/mxnet_adapter.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/envoy/dogs_cats_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/envoy/dogs_cats_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/workspace/PyTorch_DogsCats_ViT.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_DogsCats_ViT/workspace/PyTorch_DogsCats_ViT.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/histology_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/envoy/histology_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology/workspace/pytorch_histology.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology/workspace/pytorch_histology.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/histology_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/histology_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/populate_envoys.sh` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/envoy/populate_envoys.sh`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/workspace/pytorch_histology.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Histology_FedCurv/workspace/pytorch_histology.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/envoy/superb_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/envoy/superb_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/workspace/PyTorch_Huggingface_transformers_SUPERB.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Huggingface_transformers_SUPERB/workspace/PyTorch_Huggingface_transformers_SUPERB.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/kvasir_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/kvasir_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/kvasir_shard_descriptor_with_data_splitter.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/envoy/kvasir_shard_descriptor_with_data_splitter.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/workspace/PyTorch_Kvasir_UNet.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/workspace/PyTorch_Kvasir_UNet.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/workspace/layers.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Kvasir_UNet/workspace/layers.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/envoy/mnist_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/envoy/mnist_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/workspace/PyTorch_Lightning_GAN.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/workspace/PyTorch_Lightning_GAN.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/workspace/plugin_for_multiple_optimizers.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Lightning_MNIST_GAN/workspace/plugin_for_multiple_optimizers.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/envoy/mvtec_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/envoy/mvtec_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/PatchSVDD_with_Director.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/PatchSVDD_with_Director.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/data_transf.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/data_transf.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/inspection.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/inspection.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/utils.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MVTec_PatchSVDD/workspace/utils.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/market_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/envoy/market_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/PyTorch_Market_Re-ID.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/PyTorch_Market_Re-ID.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/losses.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/losses.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/tools.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/tools.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/transforms.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_Market_Re-ID/workspace/transforms.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/envoy/medmnist_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/envoy/medmnist_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/workspace/Pytorch_MedMNIST_2D.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_2D/workspace/Pytorch_MedMNIST_2D.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/envoy/medmnist_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/envoy/medmnist_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/Pytorch_MedMNIST_3D.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/Pytorch_MedMNIST_3D.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/batchnorm.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/batchnorm.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/comm.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/comm.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/replicate.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/replicate.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/utils.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_MedMNIST_3D/workspace/wspace_utils/utils.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/envoy/tinyimagenet_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/envoy/tinyimagenet_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/workspace/non-federated_case.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/workspace/non-federated_case.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/workspace/pytorch_tinyimagenet.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/PyTorch_TinyImageNet/workspace/pytorch_tinyimagenet.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/envoy/cifar10_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/envoy/cifar10_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/workspace/Tensorflow_CIFAR.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_CIFAR_tfdata/workspace/Tensorflow_CIFAR.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/envoy/mnist_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/envoy/mnist_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_MNIST/workspace/Tensorflow_MNIST.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_MNIST/workspace/Tensorflow_MNIST.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/envoy/shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/workspace/Tensorflow_Word_Prediction.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/Tensorflow_Word_Prediction/workspace/Tensorflow_Word_Prediction.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/envoy/regression_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/envoy/regression_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/workspace/JAX_linear_regression.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/workspace/JAX_linear_regression.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/jax_linear_regression/workspace/custom_adapter.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/jax_linear_regression/workspace/custom_adapter.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/README.md` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/envoy/linreg_shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/envoy/linreg_shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/LinReg.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/LinReg.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/SingleNotebook.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/SingleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/custom_adapter.py` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/custom_adapter.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/start_federation.ipynb` & `openfl-x-1.4.0.dev3/openfl-tutorials/interactive_api/numpy_linear_regression/workspace/start_federation.ipynb`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/default/envoy_config.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/default/envoy_config.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/default/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/default/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/default/shard_descriptor.py` & `openfl-x-1.4.0.dev3/openfl-workspace/default/shard_descriptor.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/fe_tf_adversarial_cifar/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/fe_tf_adversarial_cifar/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/fe_tf_adversarial_cifar/src/fe_fgsm.py` & `openfl-x-1.4.0.dev3/openfl-workspace/fe_tf_adversarial_cifar/src/fe_fgsm.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/fe_tf_adversarial_cifar/src/fecifar_inmemory.py` & `openfl-x-1.4.0.dev3/openfl-workspace/fe_tf_adversarial_cifar/src/fecifar_inmemory.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/fe_torch_adversarial_cifar/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/fe_torch_adversarial_cifar/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/fe_torch_adversarial_cifar/src/fe_fgsm.py` & `openfl-x-1.4.0.dev3/openfl-workspace/fe_torch_adversarial_cifar/src/fe_fgsm.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/fe_torch_adversarial_cifar/src/fecifar_inmemory.py` & `openfl-x-1.4.0.dev3/openfl-workspace/fe_torch_adversarial_cifar/src/fecifar_inmemory.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/fets_challenge_seg_test/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/fets_challenge_seg_test/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/src/keras_cnn.py` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/src/keras_cnn.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/src/mnist_utils.py` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/src/mnist_utils.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_mnist/src/tfmnist_inmemory.py` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_mnist/src/tfmnist_inmemory.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/src/keras_cnn.py` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/src/keras_cnn.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/src/mnist_utils.py` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/src/mnist_utils.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_cnn_with_compression/src/tfmnist_inmemory.py` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_cnn_with_compression/src/tfmnist_inmemory.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/src/dataloader_utils.py` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/src/dataloader_utils.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/src/nlp_dataloader.py` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/src/nlp_dataloader.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp/src/nlp_taskrunner.py` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp/src/nlp_taskrunner.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/src/dataloader_utils.py` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/src/dataloader_utils.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/src/nlp_dataloader.py` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/src/nlp_dataloader.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/keras_nlp_gramine_ready/src/nlp_taskrunner.py` & `openfl-x-1.4.0.dev3/openfl-workspace/keras_nlp_gramine_ready/src/nlp_taskrunner.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/README.md` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/plan/data.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/plan/data.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/src/brats_utils.py` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/src/brats_utils.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/src/nii_reader.py` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/src/nii_reader.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/src/tf_2dunet.py` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/src/tf_2dunet.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_2dunet/src/tfbrats_inmemory.py` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_2dunet/src/tfbrats_inmemory.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/README.md` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/README.md`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/data.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/data.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/split_directory.sh` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/split_directory.sh`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/src/dataloader.py` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/src/dataloader.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/src/define_model.py` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/src/define_model.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/src/tf_3dunet_model.py` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/src/tf_3dunet_model.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_3dunet_brats/src/tf_brats_dataloader.py` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_3dunet_brats/src/tf_brats_dataloader.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/plan/data.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/plan/data.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/src/tf_cnn.py` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/src/tf_cnn.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/src/tfds_utils.py` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/src/tfds_utils.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/tf_cnn_histology/src/tfhistology_inmemory.py` & `openfl-x-1.4.0.dev3/openfl-workspace/tf_cnn_histology/src/tfhistology_inmemory.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/src/histology_utils.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/src/histology_utils.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/src/pt_cnn.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/src/pt_cnn.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology/src/pthistology_inmemory.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology/src/pthistology_inmemory.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology_gramine_ready/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology_gramine_ready/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology_gramine_ready/src/histology_utils.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology_gramine_ready/src/histology_utils.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology_gramine_ready/src/pt_cnn.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology_gramine_ready/src/pt_cnn.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_histology_gramine_ready/src/pthistology_inmemory.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_histology_gramine_ready/src/pthistology_inmemory.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/plan/data.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/plan/data.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/src/mnist_utils.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/src/mnist_utils.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/src/pt_cnn.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/src/pt_cnn.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist/src/ptmnist_inmemory.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist/src/ptmnist_inmemory.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/plan/data.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/plan/data.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/src/mnist_utils.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/src/mnist_utils.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/src/pt_cnn.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/src/pt_cnn.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_cnn_mnist_straggler_check/src/ptmnist_inmemory.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_cnn_mnist_straggler_check/src/ptmnist_inmemory.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/plan/data.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/plan/data.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/src/data_loader.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/src/data_loader.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/src/fed_unet_runner.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/src/fed_unet_runner.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir/src/pt_unet_parts.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir/src/pt_unet_parts.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/plan/data.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/plan/data.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/plan/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/plan/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/src/data_loader.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/src/data_loader.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/src/fed_unet_runner.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/src/fed_unet_runner.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/torch_unet_kvasir_gramine_ready/src/pt_unet_parts.py` & `openfl-x-1.4.0.dev3/openfl-workspace/torch_unet_kvasir_gramine_ready/src/pt_unet_parts.py`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/plans/default/base_plan_interactive_api.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/plans/default/base_plan_interactive_api.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl-workspace/workspace/plan/plans/default/plan.yaml` & `openfl-x-1.4.0.dev3/openfl-workspace/workspace/plan/plans/default/plan.yaml`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/openfl_x.egg-info/PKG-INFO` & `openfl-x-1.4.0.dev3/openfl_x.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfl-x
-Version: 1.4.0.dev2
+Version: 1.4.0.dev3
 Summary: Model-agnostic federated learning
 Home-page: https://github.com/alpha-unito/OpenFL-extended
 Author: Gianluca Mittone
 Project-URL: Source Code, https://github.com/alpha-unito/OpenFL-extended
 Classifier: Environment :: Console
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -31,19 +31,17 @@
 
 
 ## Installation
 
 It is highly recommended to create a **virtual environment** prior to installing OpenFL-x (with both [venv](https://docs.python.org/3/library/venv.html) or [conda](https://docs.conda.io/en/latest/)) to avoid compatibility issues with existing Python software already installed on the system.
 Furthermore, since OpenFL-x is an extended version of OpenFL, it integrates all the features of the base framework plus the federated bagging and boosting functionalities: it is then suggested to **not install both software in the same virtual environment** since this can lead to issues in the working of both software.
 
-To install OpenFL-x, clone this repository and run `pip install`:
+You can get the lates version of OpenFL-x from `pypi`:
 ```
-git clone https://github.com/alpha-unito/OpenFL-extended.git
-cd OpenFL-extended
-pip install .
+pip install openfl-x
 ```
 If this procedure completes successfully, you now have access to all the base features of OpenFL, plus the distributed bagging and boosting functionalities. Enjoy!
 
 
 
 ## Getting Started
```

### Comparing `openfl-x-1.4.0.dev2/openfl_x.egg-info/SOURCES.txt` & `openfl-x-1.4.0.dev3/openfl_x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/setup.cfg` & `openfl-x-1.4.0.dev3/setup.cfg`

 * *Files identical despite different names*

### Comparing `openfl-x-1.4.0.dev2/setup.py` & `openfl-x-1.4.0.dev3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openfl-x',
-    version='1.4.0.dev2',
+    version='1.4.0.dev3',
     author='Gianluca Mittone',
     description='Model-agnostic federated learning',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/alpha-unito/OpenFL-extended',
     packages=[
         'openfl',
@@ -120,14 +120,15 @@
         'openfl.utilities',
         'openfl.utilities.data_splitters',
         'openfl.utilities.fedcurv',
         'openfl.utilities.fedcurv.torch',
         'openfl.utilities.optimizers.keras',
         'openfl.utilities.optimizers.numpy',
         'openfl.utilities.optimizers.torch',
+        'boosting-examples',
         'openfl-docker',
         'openfl-gramine',
         'openfl-tutorials',
         'openfl-workspace',
     ],
     include_package_data=True,
     install_requires=[
```

