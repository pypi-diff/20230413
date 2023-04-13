# Comparing `tmp/ml-starter-0.0.15.tar.gz` & `tmp/ml-starter-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.15.tar", last modified: Wed Apr 12 19:50:26 2023, max compression
+gzip compressed data, was "ml-starter-0.0.16.tar", last modified: Thu Apr 13 03:26:31 2023, max compression
```

## Comparing `ml-starter-0.0.15.tar` & `ml-starter-0.0.16.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.129917 ml-starter-0.0.15/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 19:50:16.000000 ml-starter-0.0.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-12 19:50:26.129917 ml-starter-0.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-12 19:50:16.000000 ml-starter-0.0.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.113917 ml-starter-0.0.15/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/__version__.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.113917 ml-starter-0.0.15/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    21504 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.113917 ml-starter-0.0.15/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.117917 ml-starter-0.0.15/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.117917 ml-starter-0.0.15/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.117917 ml-starter-0.0.15/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.117917 ml-starter-0.0.15/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.117917 ml-starter-0.0.15/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/scripts/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/scripts/mp_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.121917 ml-starter-0.0.15/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17584 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.121917 ml-starter-0.0.15/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.121917 ml-starter-0.0.15/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.121917 ml-starter-0.0.15/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.121917 ml-starter-0.0.15/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.121917 ml-starter-0.0.15/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.125917 ml-starter-0.0.15/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/ddp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.125917 ml-starter-0.0.15/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/mixins/cpu_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.125917 ml-starter-0.0.15/ml/trainers/mixins/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/mixins/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/mixins/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/mixins/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/mixins/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/mixins/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/mixins/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.129917 ml-starter-0.0.15/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-12 19:50:16.000000 ml-starter-0.0.15/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:50:26.129917 ml-starter-0.0.15/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-12 19:50:26.000000 ml-starter-0.0.15/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-12 19:50:26.000000 ml-starter-0.0.15/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:50:26.000000 ml-starter-0.0.15/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 19:50:26.000000 ml-starter-0.0.15/ml_starter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 19:50:26.000000 ml-starter-0.0.15/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-12 19:50:26.000000 ml-starter-0.0.15/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-12 19:50:16.000000 ml-starter-0.0.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 19:50:16.000000 ml-starter-0.0.15/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 19:50:16.000000 ml-starter-0.0.15/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-12 19:50:26.129917 ml-starter-0.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-12 19:50:16.000000 ml-starter-0.0.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.114343 ml-starter-0.0.16/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 03:26:20.000000 ml-starter-0.0.16/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-13 03:26:31.114343 ml-starter-0.0.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-13 03:26:20.000000 ml-starter-0.0.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.098342 ml-starter-0.0.16/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/__version__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.098342 ml-starter-0.0.16/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21504 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.098342 ml-starter-0.0.16/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.098342 ml-starter-0.0.16/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.098342 ml-starter-0.0.16/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.102342 ml-starter-0.0.16/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.102342 ml-starter-0.0.16/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.102342 ml-starter-0.0.16/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/scripts/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/scripts/mp_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.102342 ml-starter-0.0.16/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17584 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.106342 ml-starter-0.0.16/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.106342 ml-starter-0.0.16/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.106342 ml-starter-0.0.16/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.106342 ml-starter-0.0.16/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.106342 ml-starter-0.0.16/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.106342 ml-starter-0.0.16/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/ddp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.110342 ml-starter-0.0.16/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/cpu_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.110342 ml-starter-0.0.16/ml/trainers/mixins/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.114343 ml-starter-0.0.16/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.114343 ml-starter-0.0.16/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-13 03:26:31.000000 ml-starter-0.0.16/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-13 03:26:31.000000 ml-starter-0.0.16/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 03:26:31.000000 ml-starter-0.0.16/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 03:26:31.000000 ml-starter-0.0.16/ml_starter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-13 03:26:31.000000 ml-starter-0.0.16/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-13 03:26:31.000000 ml-starter-0.0.16/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-13 03:26:20.000000 ml-starter-0.0.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-13 03:26:20.000000 ml-starter-0.0.16/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 03:26:20.000000 ml-starter-0.0.16/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 03:26:31.114343 ml-starter-0.0.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-13 03:26:20.000000 ml-starter-0.0.16/setup.py
```

### Comparing `ml-starter-0.0.15/PKG-INFO` & `ml-starter-0.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.15
+Version: 0.0.16
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.15/README.md` & `ml-starter-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/api.py` & `ml-starter-0.0.16/ml/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "as_numpy_array",
     "assert_no_nans",
     "AsyncEnvironmentWorker",
     "AsyncIterableDataset",
     "AsyncWorkerPool",
     "atomic_save",
     "AutoDevice",
+    "BaseDevice",
     "BaseEnvironmentWorker",
     "BaseLRScheduler",
     "BaseLRSchedulerConfig",
     "BaseModel",
     "BaseModelConfig",
     "BaseOptimizer",
     "BaseOptimizerConfig",
@@ -49,36 +50,39 @@
     "Environment",
     "format_timedelta",
     "from_args",
     "get_activation",
     "get_args",
     "get_cache_dir",
     "get_data_dir",
-    "get_eval_dir",
+    "get_dataset_split_for_phase",
+    "get_dataset_splits",
+    "get_eval_run_dir",
     "get_exp_name",
     "get_image_mask",
-    "get_log_dir",
     "get_master_addr",
     "get_master_port",
     "get_model_dir",
     "get_norm_1d",
     "get_norm_2d",
     "get_norm_3d",
     "get_norm_linear",
     "get_positional_embeddings",
     "get_random_port",
     "get_rank_optional",
     "get_rank",
+    "get_run_dir",
     "get_type_from_string",
     "get_worker_info",
     "get_world_size_optional",
     "get_world_size",
     "init_",
     "init_empty_weights",
     "InitializationType",
+    "is_debugging",
     "is_distributed",
     "is_master",
     "LearnedPositionalEmbeddings",
     "load_model_and_task",
     "Loss",
     "meta_to_empty_func",
     "MultiIterDataset",
@@ -99,14 +103,15 @@
     "ReinforcementLearningSlurmTrainer",
     "ReinforcementLearningSlurmTrainerConfig",
     "ReinforcementLearningTask",
     "ReinforcementLearningTaskConfig",
     "ReinforcementLearningTrainerConfig",
     "ReinforcementLearningVanillaTrainer",
     "RotaryEmbeddings",
+    "set_random_seed",
     "set_slurm_master_addr",
     "set_slurm_rank_and_world_size",
     "SinusoidalEmbeddings",
     "SlurmTrainer",
     "SlurmTrainerConfig",
     "stage_environment",
     "State",
@@ -134,18 +139,19 @@
 ]
 
 from ml.core.common_types import Batch, Loss, Output
 from ml.core.config import conf_field
 from ml.core.env import (
     get_cache_dir,
     get_data_dir,
-    get_eval_dir,
+    get_eval_run_dir,
     get_exp_name,
-    get_log_dir,
     get_model_dir,
+    get_run_dir,
+    is_debugging,
 )
 from ml.core.registry import (
     register_logger,
     register_lr_scheduler,
     register_model,
     register_optimizer,
     register_task,
@@ -193,14 +199,15 @@
 )
 from ml.tasks.losses.reduce import cast_reduce_type, reduce
 from ml.tasks.rl.base import ReinforcementLearningTask, ReinforcementLearningTaskConfig
 from ml.tasks.sl.base import SupervisedLearningTask, SupervisedLearningTaskConfig
 from ml.trainers.base import BaseTrainer, BaseTrainerConfig
 from ml.trainers.ddp import DDPTrainer
 from ml.trainers.mixins.device.auto import AutoDevice
+from ml.trainers.mixins.device.base import BaseDevice
 from ml.trainers.rl import (
     ReinforcementLearningDDPTrainer,
     ReinforcementLearningSlurmTrainer,
     ReinforcementLearningSlurmTrainerConfig,
     ReinforcementLearningTrainerConfig,
     ReinforcementLearningVanillaTrainer,
 )
@@ -215,15 +222,15 @@
 from ml.trainers.vanilla import VanillaTrainer, VanillaTrainerConfig
 from ml.utils.argparse import from_args, get_args, get_type_from_string
 from ml.utils.atomic import atomic_save, open_atomic
 from ml.utils.augmentation import get_image_mask
 from ml.utils.caching import cached_object
 from ml.utils.checks import assert_no_nans
 from ml.utils.colors import colorize
-from ml.utils.data import get_worker_info
+from ml.utils.data import get_dataset_split_for_phase, get_dataset_splits, get_worker_info
 from ml.utils.datetime import format_timedelta
 from ml.utils.distributed import (
     get_master_addr,
     get_master_port,
     get_random_port,
     get_rank,
     get_rank_optional,
@@ -232,10 +239,11 @@
     is_distributed,
     is_master,
 )
 from ml.utils.io import load_model_and_task
 from ml.utils.large_models import init_empty_weights, meta_to_empty_func
 from ml.utils.logging import configure_logging
 from ml.utils.numpy import as_cpu_tensor, as_numpy_array
+from ml.utils.random import set_random_seed
 from ml.utils.staging import stage_environment
 from ml.utils.timer import Timer, timeout
 from ml.utils.video import READERS as VIDEO_READERS, WRITERS as VIDEO_WRITERS
```

### Comparing `ml-starter-0.0.15/ml/core/config.py` & `ml-starter-0.0.16/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/core/env.py` & `ml-starter-0.0.16/ml/core/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,23 +99,23 @@
 Debugging = _BoolEnvVar("DEBUG")
 is_debugging = Debugging.get
 
 # Where to store miscellaneous cache artifacts.
 CacheDir = _PathEnvVar("CACHE_DIR", default=Path.home() / ".cache", suffix="model-artifacts")
 get_cache_dir = CacheDir.get
 
-# Where to store run log info.
-LogDir = _PathEnvVar("LOG_DIR")
-get_log_dir = LogDir.get
-set_log_dir = LogDir.set
+# Root directory for training runs.
+RunDir = _PathEnvVar("RUN_DIR")
+get_run_dir = RunDir.get
+set_run_dir = RunDir.set
 
-# Where to store eval results.
-EvalDir = _PathEnvVar("EVAL_DIR")
-get_eval_dir = EvalDir.get
-set_eval_dir = EvalDir.set
+# Root directory for evaluation runs.
+EvalRunDir = _PathEnvVar("EVAL_RUN_DIR")
+get_eval_run_dir = EvalRunDir.get
+set_eval_run_dir = EvalRunDir.set
 
 # The name of the experiment (set by the training script).
 ExpName = _StrEnvVar("EXPERIMENT_NAME", default="Experiment")
 get_exp_name = ExpName.get
 set_exp_name = ExpName.set
 
 # Base directory where various datasets are stored.
```

### Comparing `ml-starter-0.0.15/ml/core/registry.py` & `ml-starter-0.0.16/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/core/state.py` & `ml-starter-0.0.16/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/loggers/base.py` & `ml-starter-0.0.16/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/loggers/meter.py` & `ml-starter-0.0.16/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/loggers/multi.py` & `ml-starter-0.0.16/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/loggers/stdout.py` & `ml-starter-0.0.16/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/loggers/tensorboard.py` & `ml-starter-0.0.16/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/lr_schedulers/base.py` & `ml-starter-0.0.16/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.16/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.16/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/lr_schedulers/linear.py` & `ml-starter-0.0.16/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.16/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.16/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/models/activations.py` & `ml-starter-0.0.16/ml/models/activations.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,21 +5,29 @@
 ActivationType = Literal[
     "no_act",
     "relu",
     "relu6",
     "clamp6",
     "leaky_relu",
     "elu",
+    "celu",
     "selu",
     "sigmoid",
     "log_sigmoid",
+    "hard_sigomid",
     "tanh",
     "softsign",
     "softplus",
     "silu",
+    "mish",
+    "hard_swish",
+    "soft_shrink",
+    "hard_shrink",
+    "tanh_shrink",
+    "soft_sign",
 ]
 
 
 def cast_activation_type(s: str) -> ActivationType:
     args = get_args(ActivationType)
     assert s in args, f"Invalid activation type: '{s}' Valid options are {args}"
     return cast(ActivationType, s)
@@ -81,23 +89,39 @@
             return nn.ReLU6(inplace=inplace)
         case "clamp6":
             return Clamp6(inplace=inplace)
         case "leaky_relu":
             return nn.LeakyReLU(inplace=inplace)
         case "elu":
             return nn.ELU(inplace=inplace)
+        case "celu":
+            return nn.CELU(inplace=inplace)
         case "selu":
             return nn.SELU(inplace=inplace)
         case "sigmoid":
             return nn.Sigmoid()
         case "log_sigmoid":
             return nn.LogSigmoid()
+        case "hard_sigomid":
+            return nn.Hardsigmoid(inplace=inplace)
         case "tanh":
             return nn.Tanh()
         case "softsign":
             return nn.Softsign()
         case "softplus":
             return nn.Softplus()
         case "silu":
             return nn.SiLU()
+        case "mish":
+            return nn.Mish(inplace=inplace)
+        case "hard_swish":
+            return nn.Hardswish(inplace=inplace)
+        case "soft_shrink":
+            return nn.Softshrink()
+        case "hard_shrink":
+            return nn.Hardshrink()
+        case "tanh_shrink":
+            return nn.Tanhshrink()
+        case "soft_sign":
+            return nn.Softsign()
         case _:
             raise NotImplementedError(f"Activation function '{act}' is not implemented.")
```

### Comparing `ml-starter-0.0.15/ml/models/base.py` & `ml-starter-0.0.16/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/models/embeddings.py` & `ml-starter-0.0.16/ml/models/embeddings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from typing import Literal, cast, get_args, overload
 
 import torch
 from torch import Tensor, nn
 
 from ml.models.init import InitializationType, init_
 
-EmbeddingKind = Literal["learned", "sinusoidal", "rotary"]
+EmbeddingKind = Literal["identity", "learned", "sinusoidal", "rotary"]
 
 
 def cast_embedding_kind(k: str) -> EmbeddingKind:
     args = get_args(EmbeddingKind)
     assert k in args, f"Invalid initialization type: '{k}' Valid options are {args}"
     return cast(EmbeddingKind, k)
 
 
+class IdentityPositionalEmbeddings(nn.Module):
+    def forward(self, x: Tensor, offset: int = 0, times: Tensor | None = None) -> Tensor:
+        return x
+
+
 class LearnedPositionalEmbeddings(nn.Module):
     def __init__(
         self,
         max_tsz: int,
         embed_dim: int,
         weight_init: InitializationType = "normal",
         learnable: bool = True,
@@ -40,15 +45,15 @@
         self.embeddings = nn.Parameter(torch.empty(max_tsz, embed_dim), requires_grad=learnable)
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         init_(self.embeddings.data, None, self.weight_init)
 
     def forward(self, x: Tensor, offset: int = 0, times: Tensor | None = None) -> Tensor:
-        return x + self.embeddings[None, offset : offset + x.size(1)] if times is None else self.embeddings[times]
+        return x + (self.embeddings[None, offset : offset + x.size(1)] if times is None else self.embeddings[times])
 
 
 class SinusoidalEmbeddings(LearnedPositionalEmbeddings):
     def __init__(
         self,
         max_tsz: int,
         embed_dim: int,
@@ -122,24 +127,33 @@
         quarter_d = self.embed_dim // 4
         return torch.cat([-x[..., quarter_d:], x[..., :quarter_d]], dim=-1)
 
     def forward(self, x: Tensor, offset: int = 0, times: Tensor | None = None) -> Tensor:
         half_d = self.embed_dim // 2
         x_rope, x_pass = x[..., :half_d], x[..., half_d:]
         neg_half_x = self._neg_half(x_rope)
-        cos_part = x_rope * self.cos[None, offset : offset + x.shape[1]]
-        sin_part = neg_half_x * self.sin[None, offset : offset + x.shape[1]]
-        x_rope = cos_part + sin_part
+        cos_part = self.cos[None, offset : offset + x.shape[1]] if times is None else self.cos[times]
+        sin_part = self.sin[None, offset : offset + x.shape[1]] if times is None else self.sin[times]
+        x_rope = x_rope * cos_part + neg_half_x * sin_part
         return torch.cat((x_rope, x_pass), dim=-1)
 
 
 @overload
 def get_positional_embeddings(
     max_tsz: int,
     embed_dim: int,
+    kind: Literal["identity"],
+) -> IdentityPositionalEmbeddings:
+    ...
+
+
+@overload
+def get_positional_embeddings(
+    max_tsz: int,
+    embed_dim: int,
     kind: Literal["learned"],
     *,
     weight_init: InitializationType = "normal",
     learnable: bool = True,
 ) -> LearnedPositionalEmbeddings:
     ...
 
@@ -164,23 +178,36 @@
     *,
     learnable: bool = False,
     base: int = 10_000,
 ) -> RotaryEmbeddings:
     ...
 
 
+@overload
 def get_positional_embeddings(
     max_tsz: int,
     embed_dim: int,
     kind: EmbeddingKind,
     *,
     weight_init: InitializationType = "normal",
     learnable: bool = False,
     base: int = 10_000,
-) -> LearnedPositionalEmbeddings | SinusoidalEmbeddings | RotaryEmbeddings:
+) -> IdentityPositionalEmbeddings | LearnedPositionalEmbeddings | SinusoidalEmbeddings | RotaryEmbeddings:
+    ...
+
+
+def get_positional_embeddings(
+    max_tsz: int,
+    embed_dim: int,
+    kind: EmbeddingKind,
+    *,
+    weight_init: InitializationType = "normal",
+    learnable: bool = False,
+    base: int = 10_000,
+) -> nn.Module:
     """Defines the common module for adding positional embeddings.
 
     Args:
         max_tsz: The maximum sequence length.
         embed_dim: The embedding dimension.
         kind: The type of embedding to use.
         weight_init: The weight initialization for learned embeddings.
@@ -191,33 +218,36 @@
         The positional embeddings module.
 
     Raises:
         ValueError: If an invalid embedding kind is supplied.
     """
 
     match kind:
-        case "sinusoidal":
-            return SinusoidalEmbeddings(
+        case "identity":
+            return IdentityPositionalEmbeddings()
+
+        case "learned":
+            return LearnedPositionalEmbeddings(
                 max_tsz=max_tsz,
                 embed_dim=embed_dim,
+                weight_init=weight_init,
                 learnable=learnable,
-                base=base,
             )
 
-        case "rotary":
-            return RotaryEmbeddings(
+        case "sinusoidal":
+            return SinusoidalEmbeddings(
                 max_tsz=max_tsz,
                 embed_dim=embed_dim,
                 learnable=learnable,
                 base=base,
             )
 
-        case "learned":
-            return LearnedPositionalEmbeddings(
+        case "rotary":
+            return RotaryEmbeddings(
                 max_tsz=max_tsz,
                 embed_dim=embed_dim,
-                weight_init=weight_init,
                 learnable=learnable,
+                base=base,
             )
 
         case _:
             raise ValueError(f"Invalid embedding kind: {kind}")
```

### Comparing `ml-starter-0.0.15/ml/models/init.py` & `ml-starter-0.0.16/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/models/norms.py` & `ml-starter-0.0.16/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/optimizers/adam.py` & `ml-starter-0.0.16/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/optimizers/adamw.py` & `ml-starter-0.0.16/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/optimizers/adan.py` & `ml-starter-0.0.16/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/optimizers/base.py` & `ml-starter-0.0.16/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/optimizers/sgd.py` & `ml-starter-0.0.16/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/optimizers/shampoo.py` & `ml-starter-0.0.16/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/scripts/cli.py` & `ml-starter-0.0.16/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/scripts/compiler.py` & `ml-starter-0.0.16/ml/scripts/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/scripts/stage.py` & `ml-starter-0.0.16/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/scripts/train.py` & `ml-starter-0.0.16/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/base.py` & `ml-starter-0.0.16/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.16/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.16/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/datasets/collate.py` & `ml-starter-0.0.16/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.16/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.16/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.16/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.16/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.16/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/datasets/utils.py` & `ml-starter-0.0.16/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.16/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/environments/base.py` & `ml-starter-0.0.16/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/environments/utils.py` & `ml-starter-0.0.16/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/environments/worker.py` & `ml-starter-0.0.16/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/losses/reduce.py` & `ml-starter-0.0.16/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/rl/base.py` & `ml-starter-0.0.16/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/rl/replay.py` & `ml-starter-0.0.16/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/tasks/sl/base.py` & `ml-starter-0.0.16/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/base.py` & `ml-starter-0.0.16/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/ddp.py` & `ml-starter-0.0.16/ml/trainers/ddp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.16/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/mixins/device/auto.py` & `ml-starter-0.0.16/ml/trainers/mixins/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/mixins/device/base.py` & `ml-starter-0.0.16/ml/trainers/mixins/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/mixins/device/cpu.py` & `ml-starter-0.0.16/ml/trainers/mixins/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/mixins/device/gpu.py` & `ml-starter-0.0.16/ml/trainers/mixins/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/mixins/device/metal.py` & `ml-starter-0.0.16/ml/trainers/mixins/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.16/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.16/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.16/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.16/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.16/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/rl.py` & `ml-starter-0.0.16/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/sl.py` & `ml-starter-0.0.16/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/slurm.py` & `ml-starter-0.0.16/ml/trainers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/trainers/vanilla.py` & `ml-starter-0.0.16/ml/trainers/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/argparse.py` & `ml-starter-0.0.16/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/atomic.py` & `ml-starter-0.0.16/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/augmentation.py` & `ml-starter-0.0.16/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/caching.py` & `ml-starter-0.0.16/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/call_train.py` & `ml-starter-0.0.16/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/cli.py` & `ml-starter-0.0.16/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/colors.py` & `ml-starter-0.0.16/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/compiler.py` & `ml-starter-0.0.16/ml/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/datetime.py` & `ml-starter-0.0.16/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/distributed.py` & `ml-starter-0.0.16/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/io.py` & `ml-starter-0.0.16/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/large_models.py` & `ml-starter-0.0.16/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/logging.py` & `ml-starter-0.0.16/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/meter.py` & `ml-starter-0.0.16/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/staging.py` & `ml-starter-0.0.16/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/timer.py` & `ml-starter-0.0.16/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml/utils/video.py` & `ml-starter-0.0.16/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.16/ml_starter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.15
+Version: 0.0.16
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.15/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.16/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/pyproject.toml` & `ml-starter-0.0.16/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.15/setup.py` & `ml-starter-0.0.16/setup.py`

 * *Files identical despite different names*

