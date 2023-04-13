# Comparing `tmp/nemo-bo-0.1.8.tar.gz` & `tmp/nemo-bo-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemo-bo-0.1.8.tar", max compression
+gzip compressed data, was "nemo-bo-0.1.9.tar", max compression
```

## Comparing `nemo-bo-0.1.8.tar` & `nemo-bo-0.1.9.tar`

### file list

```diff
@@ -1,52 +1,99 @@
--rw-r--r--   0        0        0     1086 2022-06-14 14:34:55.937000 nemo-bo-0.1.8/LICENSE
--rw-r--r--   0        0        0       23 2022-06-14 16:14:55.553003 nemo-bo-0.1.8/nemo_bo/__init__.py
--rw-r--r--   0        0        0        0 2022-06-14 15:06:54.635282 nemo-bo-0.1.8/nemo_bo/acquisition_functions/__init__.py
--rw-r--r--   0        0        0     3184 2022-07-16 18:33:51.543810 nemo-bo-0.1.8/nemo_bo/acquisition_functions/base_acq_function.py
--rw-r--r--   0        0        0        0 2022-06-14 15:06:54.658218 nemo-bo-0.1.8/nemo_bo/acquisition_functions/expected_improvement/__init__.py
--rw-r--r--   0        0        0     2872 2022-08-28 06:30:22.481555 nemo-bo-0.1.8/nemo_bo/acquisition_functions/expected_improvement/ehvi.py
--rw-r--r--   0        0        0    23613 2022-08-28 06:30:22.492525 nemo-bo-0.1.8/nemo_bo/acquisition_functions/expected_improvement/expected_improvement.py
--rw-r--r--   0        0        0    24509 2022-08-28 06:30:22.502499 nemo-bo-0.1.8/nemo_bo/acquisition_functions/expected_improvement/expected_improvement_new_norm.py
--rw-r--r--   0        0        0    22934 2022-08-28 06:30:22.511476 nemo-bo-0.1.8/nemo_bo/acquisition_functions/expected_improvement/expected_improvement_old.py
--rw-r--r--   0        0        0        0 2022-06-14 15:06:54.616363 nemo-bo-0.1.8/nemo_bo/acquisition_functions/nsga_improvement/__init__.py
--rw-r--r--   0        0        0     6878 2022-06-20 15:44:38.767424 nemo-bo-0.1.8/nemo_bo/acquisition_functions/nsga_improvement/genetic.py
--rw-r--r--   0        0        0     8699 2022-08-28 06:30:22.523443 nemo-bo-0.1.8/nemo_bo/acquisition_functions/nsga_improvement/nsga2.py
--rw-r--r--   0        0        0    13736 2022-08-28 06:30:22.532418 nemo-bo-0.1.8/nemo_bo/acquisition_functions/nsga_improvement/nsga3.py
--rw-r--r--   0        0        0    16665 2022-08-28 06:30:22.542392 nemo-bo-0.1.8/nemo_bo/acquisition_functions/nsga_improvement/nsga_improvement.py
--rw-r--r--   0        0        0     3232 2022-08-28 06:30:22.551370 nemo-bo-0.1.8/nemo_bo/acquisition_functions/nsga_improvement/problem_wrapper.py
--rw-r--r--   0        0        0     1960 2022-08-28 06:30:22.560344 nemo-bo-0.1.8/nemo_bo/acquisition_functions/nsga_improvement/unsga3.py
--rw-r--r--   0        0        0    25539 2022-07-23 08:19:06.951222 nemo-bo-0.1.8/nemo_bo/datasets/Aldol_Condensation/Aldol_Condensation_STY_Cost.xlsx
--rw-r--r--   0        0        0    17738 2022-08-20 08:47:45.443827 nemo-bo-0.1.8/nemo_bo/datasets/Aldol_Condensation/Aldol_Condensation_Yield_Cost.xlsx
--rw-r--r--   0        0        0        0 2022-06-14 15:06:55.137935 nemo-bo-0.1.8/nemo_bo/models/__init__.py
--rw-r--r--   0        0        0        0 2022-06-14 15:06:55.123972 nemo-bo-0.1.8/nemo_bo/models/base/__init__.py
--rw-r--r--   0        0        0     3857 2022-06-21 16:39:21.262503 nemo-bo-0.1.8/nemo_bo/models/base/available_models.py
--rw-r--r--   0        0        0    43929 2022-08-28 06:30:22.571316 nemo-bo-0.1.8/nemo_bo/models/base/base_model.py
--rw-r--r--   0        0        0     2550 2022-06-29 14:12:13.338427 nemo-bo-0.1.8/nemo_bo/models/base/nn_save_checkpoint.py
--rw-r--r--   0        0        0    13693 2022-08-28 06:30:22.579293 nemo-bo-0.1.8/nemo_bo/models/gp.py
--rw-r--r--   0        0        0    13599 2022-08-28 06:30:22.594253 nemo-bo-0.1.8/nemo_bo/models/gp_gpytorch.py
--rw-r--r--   0        0        0    13147 2022-08-28 06:30:22.605225 nemo-bo-0.1.8/nemo_bo/models/ngb.py
--rw-r--r--   0        0        0    19477 2022-08-28 06:30:22.615198 nemo-bo-0.1.8/nemo_bo/models/nn_bayesian.py
--rw-r--r--   0        0        0    21322 2022-08-28 06:30:22.626168 nemo-bo-0.1.8/nemo_bo/models/nn_concrete.py
--rw-r--r--   0        0        0    17544 2022-08-28 06:30:22.640135 nemo-bo-0.1.8/nemo_bo/models/nn_ensemble.py
--rw-r--r--   0        0        0     9667 2022-08-28 06:30:22.678029 nemo-bo-0.1.8/nemo_bo/models/rf.py
--rw-r--r--   0        0        0    11929 2022-08-28 06:30:22.690995 nemo-bo-0.1.8/nemo_bo/models/xgb.py
--rw-r--r--   0        0        0        0 2022-06-14 15:06:55.169849 nemo-bo-0.1.8/nemo_bo/opt/__init__.py
--rw-r--r--   0        0        0     8169 2022-08-28 06:30:22.708948 nemo-bo-0.1.8/nemo_bo/opt/benchmark.py
--rw-r--r--   0        0        0    28524 2022-07-16 18:33:52.583573 nemo-bo-0.1.8/nemo_bo/opt/constraints.py
--rw-r--r--   0        0        0    28338 2022-07-02 12:12:47.034000 nemo-bo-0.1.8/nemo_bo/opt/constraints_original.py
--rw-r--r--   0        0        0    40998 2022-08-28 06:30:22.733885 nemo-bo-0.1.8/nemo_bo/opt/objectives.py
--rw-r--r--   0        0        0    33309 2022-08-28 06:30:22.752830 nemo-bo-0.1.8/nemo_bo/opt/optimisation.py
--rw-r--r--   0        0        0     4816 2022-06-16 17:34:41.807658 nemo-bo-0.1.8/nemo_bo/opt/random.py
--rw-r--r--   0        0        0    15330 2022-08-28 06:30:22.766311 nemo-bo-0.1.8/nemo_bo/opt/samplers.py
--rw-r--r--   0        0        0    34091 2022-08-28 06:30:22.789245 nemo-bo-0.1.8/nemo_bo/opt/utils_samplers/sampling.py
--rw-r--r--   0        0        0    39394 2022-08-28 06:30:22.802212 nemo-bo-0.1.8/nemo_bo/opt/variables.py
--rw-r--r--   0        0        0        0 2022-06-14 15:06:55.200765 nemo-bo-0.1.8/nemo_bo/utils/__init__.py
--rw-r--r--   0        0        0     8499 2022-08-28 06:30:22.814181 nemo-bo-0.1.8/nemo_bo/utils/data_proc.py
--rw-r--r--   0        0        0     7004 2022-06-19 16:40:37.958079 nemo-bo-0.1.8/nemo_bo/utils/extract_excel.py
--rw-r--r--   0        0        0     1856 2022-08-28 06:30:22.826147 nemo-bo-0.1.8/nemo_bo/utils/logger.py
--rw-r--r--   0        0        0     4435 2022-06-19 14:45:16.260837 nemo-bo-0.1.8/nemo_bo/utils/perf_metrics.py
--rw-r--r--   0        0        0    26521 2022-08-28 06:30:22.844099 nemo-bo-0.1.8/nemo_bo/utils/plotter.py
--rw-r--r--   0        0        0    11709 2022-06-19 16:40:38.170020 nemo-bo-0.1.8/nemo_bo/utils/transformations.py
--rw-r--r--   0        0        0     1550 2022-08-28 06:30:22.854072 nemo-bo-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      107 2022-06-14 16:00:33.986794 nemo-bo-0.1.8/README.md
--rw-r--r--   0        0        0     1682 2022-08-28 06:32:05.021462 nemo-bo-0.1.8/setup.py
--rw-r--r--   0        0        0     1900 2022-08-28 06:32:05.023456 nemo-bo-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1086 2022-06-14 14:34:55.937000 nemo-bo-0.1.9/LICENSE
+-rw-r--r--   0        0        0       23 2022-06-14 16:14:55.553003 nemo-bo-0.1.9/nemo_bo/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-14 15:06:54.635282 nemo-bo-0.1.9/nemo_bo/acquisition_functions/__init__.py
+-rw-r--r--   0        0        0      175 2022-09-11 17:14:39.217217 nemo-bo-0.1.9/nemo_bo/acquisition_functions/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3695 2022-09-11 17:14:39.311428 nemo-bo-0.1.9/nemo_bo/acquisition_functions/__pycache__/base_acq_function.cpython-39.pyc
+-rw-r--r--   0        0        0     3828 2022-09-26 15:13:00.387006 nemo-bo-0.1.9/nemo_bo/acquisition_functions/base_acq_function.py
+-rw-r--r--   0        0        0        0 2022-06-14 15:06:54.658218 nemo-bo-0.1.9/nemo_bo/acquisition_functions/expected_improvement/__init__.py
+-rw-r--r--   0        0        0      196 2022-09-11 17:14:39.221208 nemo-bo-0.1.9/nemo_bo/acquisition_functions/expected_improvement/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2658 2022-09-11 17:14:39.469005 nemo-bo-0.1.9/nemo_bo/acquisition_functions/expected_improvement/__pycache__/ehvi.cpython-39.pyc
+-rw-r--r--   0        0        0    22067 2022-09-11 17:14:39.279511 nemo-bo-0.1.9/nemo_bo/acquisition_functions/expected_improvement/__pycache__/expected_improvement.cpython-39.pyc
+-rw-r--r--   0        0        0     3246 2022-10-08 08:48:33.925846 nemo-bo-0.1.9/nemo_bo/acquisition_functions/expected_improvement/ehvi.py
+-rw-r--r--   0        0        0    41446 2022-10-08 08:48:34.866330 nemo-bo-0.1.9/nemo_bo/acquisition_functions/expected_improvement/expected_improvement.py
+-rw-r--r--   0        0        0        0 2022-09-16 12:28:11.975729 nemo-bo-0.1.9/nemo_bo/acquisition_functions/highest_uncertainty/__init__.py
+-rw-r--r--   0        0        0     5893 2022-10-08 08:48:33.919862 nemo-bo-0.1.9/nemo_bo/acquisition_functions/highest_uncertainty/highest_uncertainty.py
+-rw-r--r--   0        0        0        0 2022-06-14 15:06:54.616363 nemo-bo-0.1.9/nemo_bo/acquisition_functions/nsga_improvement/__init__.py
+-rw-r--r--   0        0        0     6926 2022-09-08 16:26:39.047014 nemo-bo-0.1.9/nemo_bo/acquisition_functions/nsga_improvement/genetic.py
+-rw-r--r--   0        0        0     8051 2022-09-08 16:26:39.278396 nemo-bo-0.1.9/nemo_bo/acquisition_functions/nsga_improvement/nsga2.py
+-rw-r--r--   0        0        0    13676 2022-09-08 16:26:39.624979 nemo-bo-0.1.9/nemo_bo/acquisition_functions/nsga_improvement/nsga3.py
+-rw-r--r--   0        0        0    11963 2022-10-08 08:48:27.819895 nemo-bo-0.1.9/nemo_bo/acquisition_functions/nsga_improvement/nsga_improvement.py
+-rw-r--r--   0        0        0     3530 2022-10-08 08:48:33.889942 nemo-bo-0.1.9/nemo_bo/acquisition_functions/nsga_improvement/problem_wrapper.py
+-rw-r--r--   0        0        0     1957 2022-10-08 08:48:27.842836 nemo-bo-0.1.9/nemo_bo/acquisition_functions/nsga_improvement/unsga3.py
+-rw-r--r--   0        0        0    17615 2022-09-11 16:11:31.190566 nemo-bo-0.1.9/nemo_bo/datasets/Aldol_Condensation/Aldol_Condensation_STY_Cost.xlsx
+-rw-r--r--   0        0        0    17695 2022-09-11 16:10:20.153188 nemo-bo-0.1.9/nemo_bo/datasets/Aldol_Condensation/Aldol_Condensation_Yield_Cost.xlsx
+-rw-r--r--   0        0        0        0 2022-06-14 15:06:55.137935 nemo-bo-0.1.9/nemo_bo/models/__init__.py
+-rw-r--r--   0        0        0      160 2022-09-11 17:11:58.242843 nemo-bo-0.1.9/nemo_bo/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    11272 2022-09-11 17:11:58.372498 nemo-bo-0.1.9/nemo_bo/models/__pycache__/gp.cpython-39.pyc
+-rw-r--r--   0        0        0    10985 2022-09-11 17:12:06.331580 nemo-bo-0.1.9/nemo_bo/models/__pycache__/ngb.cpython-39.pyc
+-rw-r--r--   0        0        0    17378 2022-09-11 17:12:09.425776 nemo-bo-0.1.9/nemo_bo/models/__pycache__/nn_bayesian.cpython-39.pyc
+-rw-r--r--   0        0        0    18027 2022-09-11 17:12:31.221353 nemo-bo-0.1.9/nemo_bo/models/__pycache__/nn_concrete.cpython-39.pyc
+-rw-r--r--   0        0        0    14704 2022-09-11 17:12:31.243293 nemo-bo-0.1.9/nemo_bo/models/__pycache__/nn_ensemble.cpython-39.pyc
+-rw-r--r--   0        0        0     8729 2022-09-11 17:12:31.250275 nemo-bo-0.1.9/nemo_bo/models/__pycache__/rf.cpython-39.pyc
+-rw-r--r--   0        0        0    10427 2022-09-11 17:12:31.533831 nemo-bo-0.1.9/nemo_bo/models/__pycache__/xgb.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2022-06-14 15:06:55.123972 nemo-bo-0.1.9/nemo_bo/models/base/__init__.py
+-rw-r--r--   0        0        0      165 2022-09-11 17:11:58.248828 nemo-bo-0.1.9/nemo_bo/models/base/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2572 2022-09-11 17:11:58.265780 nemo-bo-0.1.9/nemo_bo/models/base/__pycache__/available_models.cpython-39.pyc
+-rw-r--r--   0        0        0    30271 2022-09-11 17:11:58.298693 nemo-bo-0.1.9/nemo_bo/models/base/__pycache__/base_model.cpython-39.pyc
+-rw-r--r--   0        0        0     2717 2022-09-11 17:12:31.163538 nemo-bo-0.1.9/nemo_bo/models/base/__pycache__/nn_save_checkpoint.cpython-39.pyc
+-rw-r--r--   0        0        0     3908 2022-09-17 10:17:38.769225 nemo-bo-0.1.9/nemo_bo/models/base/available_models.py
+-rw-r--r--   0        0        0    43247 2022-10-08 08:48:34.820453 nemo-bo-0.1.9/nemo_bo/models/base/base_model.py
+-rw-r--r--   0        0        0     2585 2022-10-08 08:48:33.883959 nemo-bo-0.1.9/nemo_bo/models/base/nn_save_checkpoint.py
+-rw-r--r--   0        0        0    16805 2022-10-08 08:48:34.363675 nemo-bo-0.1.9/nemo_bo/models/gp.py
+-rw-r--r--   0        0        0    13977 2022-10-08 08:48:34.356693 nemo-bo-0.1.9/nemo_bo/models/gp_gpytorch.py
+-rw-r--r--   0        0        0    14433 2022-10-08 08:48:34.304832 nemo-bo-0.1.9/nemo_bo/models/ngb.py
+-rw-r--r--   0        0        0    21525 2022-10-08 08:48:34.545189 nemo-bo-0.1.9/nemo_bo/models/nn_bayesian.py
+-rw-r--r--   0        0        0    23040 2022-10-08 08:48:34.723714 nemo-bo-0.1.9/nemo_bo/models/nn_concrete.py
+-rw-r--r--   0        0        0    19307 2022-10-08 08:48:34.521253 nemo-bo-0.1.9/nemo_bo/models/nn_ensemble.py
+-rw-r--r--   0        0        0    10870 2022-09-17 08:20:57.813352 nemo-bo-0.1.9/nemo_bo/models/rf.py
+-rw-r--r--   0        0        0    13275 2022-10-08 08:48:34.659883 nemo-bo-0.1.9/nemo_bo/models/xgb.py
+-rw-r--r--   0        0        0        0 2022-06-14 15:06:55.169849 nemo-bo-0.1.9/nemo_bo/opt/__init__.py
+-rw-r--r--   0        0        0      157 2022-09-11 17:11:38.133292 nemo-bo-0.1.9/nemo_bo/opt/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    13907 2022-09-11 17:14:39.497926 nemo-bo-0.1.9/nemo_bo/opt/__pycache__/benchmark.cpython-39.pyc
+-rw-r--r--   0        0        0    22697 2022-09-11 17:14:39.335361 nemo-bo-0.1.9/nemo_bo/opt/__pycache__/constraints.cpython-39.pyc
+-rw-r--r--   0        0        0    36147 2022-09-11 17:11:38.277193 nemo-bo-0.1.9/nemo_bo/opt/__pycache__/objectives.cpython-39.pyc
+-rw-r--r--   0        0        0    24271 2022-09-11 17:14:39.486956 nemo-bo-0.1.9/nemo_bo/opt/__pycache__/optimisation.cpython-39.pyc
+-rw-r--r--   0        0        0    11873 2022-09-11 17:14:39.379244 nemo-bo-0.1.9/nemo_bo/opt/__pycache__/samplers.cpython-39.pyc
+-rw-r--r--   0        0        0    31680 2022-09-11 17:12:32.394523 nemo-bo-0.1.9/nemo_bo/opt/__pycache__/variables.cpython-39.pyc
+-rw-r--r--   0        0        0    27112 2022-10-08 08:48:35.048842 nemo-bo-0.1.9/nemo_bo/opt/benchmark.py
+-rw-r--r--   0        0        0    42030 2022-09-17 09:44:42.565067 nemo-bo-0.1.9/nemo_bo/opt/constraints.py
+-rw-r--r--   0        0        0    47002 2022-10-08 08:48:35.176500 nemo-bo-0.1.9/nemo_bo/opt/objectives.py
+-rw-r--r--   0        0        0    44116 2022-10-08 09:10:59.588094 nemo-bo-0.1.9/nemo_bo/opt/optimisation.py
+-rw-r--r--   0        0        0    15749 2022-10-08 08:48:34.931156 nemo-bo-0.1.9/nemo_bo/opt/samplers.py
+-rw-r--r--   0        0        0    27992 2022-09-11 17:14:39.396198 nemo-bo-0.1.9/nemo_bo/opt/utils_samplers/__pycache__/sampling.cpython-39.pyc
+-rw-r--r--   0        0        0    34483 2022-10-08 08:48:35.674170 nemo-bo-0.1.9/nemo_bo/opt/utils_samplers/sampling.py
+-rw-r--r--   0        0        0    39968 2022-10-08 08:48:35.588398 nemo-bo-0.1.9/nemo_bo/opt/variables.py
+-rw-r--r--   0        0        0     3106 2022-09-15 18:29:15.290229 nemo-bo-0.1.9/nemo_bo/tutorials/1. Setting up a single objective optimisation.ipynb
+-rw-r--r--   0        0        0     4451 2022-09-15 18:35:17.390899 nemo-bo-0.1.9/nemo_bo/tutorials/10. How to create a closed-loop optimisation using a pool-based sampler as the benchmark.ipynb
+-rw-r--r--   0        0        0     8504 2022-09-15 18:35:49.187538 nemo-bo-0.1.9/nemo_bo/tutorials/11. Setting up an optimisation with input constraints.ipynb
+-rw-r--r--   0        0        0     3009 2022-09-15 18:36:32.445584 nemo-bo-0.1.9/nemo_bo/tutorials/12. Generating samples without needing to perform an optimisation.ipynb
+-rw-r--r--   0        0        0     5875 2022-09-15 18:37:04.830242 nemo-bo-0.1.9/nemo_bo/tutorials/13. How to set up a manual optimisation.ipynb
+-rw-r--r--   0        0        0     4079 2022-10-08 09:11:55.619989 nemo-bo-0.1.9/nemo_bo/tutorials/14. How to resume an optimisation run.ipynb
+-rw-r--r--   0        0        0     5565 2022-09-15 18:38:04.169465 nemo-bo-0.1.9/nemo_bo/tutorials/15. How to use the BoTorch (quasi-) Monte-Carlo based acquisition functions in NEMO.ipynb
+-rw-r--r--   0        0        0     4906 2022-09-17 02:17:50.513560 nemo-bo-0.1.9/nemo_bo/tutorials/16. How to set up an optimisation that uses U-NSGA-III as the acquisition function.ipynb
+-rw-r--r--   0        0        0     5121 2022-09-15 18:38:52.158629 nemo-bo-0.1.9/nemo_bo/tutorials/17. Using the input template excel file template to import the variables and objectives data.ipynb
+-rw-r--r--   0        0        0     3800 2022-09-16 14:50:35.356911 nemo-bo-0.1.9/nemo_bo/tutorials/18. How to set up an optimisation that uses the highest uncertainty acquisition function.ipynb
+-rw-r--r--   0        0        0     4859 2022-09-15 18:29:59.736825 nemo-bo-0.1.9/nemo_bo/tutorials/2. How to select specific machine learning models types for the objectives.ipynb
+-rw-r--r--   0        0        0     5983 2022-09-15 18:30:24.022141 nemo-bo-0.1.9/nemo_bo/tutorials/3. How to use calculable objectives.ipynb
+-rw-r--r--   0        0        0     4753 2022-09-15 18:31:29.432963 nemo-bo-0.1.9/nemo_bo/tutorials/4. How to define transformers for variables and objectives.ipynb
+-rw-r--r--   0        0        0     4084 2022-09-15 18:32:01.490068 nemo-bo-0.1.9/nemo_bo/tutorials/5. using_categorical_variables_with_descriptors.ipynb
+-rw-r--r--   0        0        0     4023 2022-10-08 08:48:34.904229 nemo-bo-0.1.9/nemo_bo/tutorials/6. Utilising the machine learning model fitting in NEMO without Bayesian optimisation.ipynb
+-rw-r--r--   0        0        0     4983 2022-09-15 18:33:08.738128 nemo-bo-0.1.9/nemo_bo/tutorials/7. How to create a closed-loop optimisation using a machine learning model as the benchmark function.ipynb
+-rw-r--r--   0        0        0     5606 2022-09-16 15:41:51.772243 nemo-bo-0.1.9/nemo_bo/tutorials/8. How to create a closed-loop optimisation using a multiobjective synthetic function as the benchmark function.ipynb
+-rw-r--r--   0        0        0     5641 2022-09-15 18:34:44.425609 nemo-bo-0.1.9/nemo_bo/tutorials/9. How to create a closed-loop optimisation using a single objective synthetic function as the benchmark function.ipynb
+-rw-r--r--   0        0        0    14355 2022-09-11 18:05:51.667887 nemo-bo-0.1.9/nemo_bo/tutorials/extract_excel_example_template.xlsx
+-rw-r--r--   0        0        0        0 2022-06-14 15:06:55.200765 nemo-bo-0.1.9/nemo_bo/utils/__init__.py
+-rw-r--r--   0        0        0      159 2022-09-11 17:11:38.111353 nemo-bo-0.1.9/nemo_bo/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8253 2022-09-11 17:11:58.321633 nemo-bo-0.1.9/nemo_bo/utils/__pycache__/data_proc.cpython-39.pyc
+-rw-r--r--   0        0        0     3431 2022-09-11 17:11:38.123323 nemo-bo-0.1.9/nemo_bo/utils/__pycache__/extract_excel.cpython-39.pyc
+-rw-r--r--   0        0        0     1393 2022-09-11 17:11:58.179035 nemo-bo-0.1.9/nemo_bo/utils/__pycache__/logger.cpython-39.pyc
+-rw-r--r--   0        0        0     3806 2022-09-11 17:11:58.200955 nemo-bo-0.1.9/nemo_bo/utils/__pycache__/perf_metrics.cpython-39.pyc
+-rw-r--r--   0        0        0    16289 2022-09-11 17:11:58.234868 nemo-bo-0.1.9/nemo_bo/utils/__pycache__/plotter.cpython-39.pyc
+-rw-r--r--   0        0        0     8619 2022-10-08 08:48:35.105693 nemo-bo-0.1.9/nemo_bo/utils/data_proc.py
+-rw-r--r--   0        0        0     7194 2022-09-17 17:50:32.017371 nemo-bo-0.1.9/nemo_bo/utils/extract_excel.py
+-rw-r--r--   0        0        0     1890 2022-10-08 08:48:34.971052 nemo-bo-0.1.9/nemo_bo/utils/logger.py
+-rw-r--r--   0        0        0     4435 2022-06-19 14:45:16.260837 nemo-bo-0.1.9/nemo_bo/utils/perf_metrics.py
+-rw-r--r--   0        0        0    28591 2022-10-08 08:48:35.691124 nemo-bo-0.1.9/nemo_bo/utils/plotter.py
+-rw-r--r--   0        0        0     1550 2022-10-08 09:10:27.107750 nemo-bo-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    10918 2022-10-08 09:15:31.111182 nemo-bo-0.1.9/README.md
+-rw-r--r--   0        0        0    12562 2022-10-08 09:16:34.176148 nemo-bo-0.1.9/setup.py
+-rw-r--r--   0        0        0    12443 2022-10-08 09:16:34.179141 nemo-bo-0.1.9/PKG-INFO
```

### Comparing `nemo-bo-0.1.8/LICENSE` & `nemo-bo-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nemo-bo-0.1.8/nemo_bo/acquisition_functions/expected_improvement/ehvi.py` & `nemo-bo-0.1.9/nemo_bo/acquisition_functions/expected_improvement/ehvi.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,42 +18,65 @@
 
     Class for the Expected Hypervolume Improvement acquisition function adapted from the BoTorch package
 
     """
 
     def __init__(self, ref_point: Tensor, Y: Tensor):
         self.ref_point = ref_point
-        self.partitioning = FastNondominatedPartitioning(ref_point=self.ref_point, Y=Y,)
+        self.partitioning = FastNondominatedPartitioning(
+            ref_point=self.ref_point,
+            Y=Y,
+        )
 
         cell_bounds = self.partitioning.get_hypercell_bounds()
         self.cell_lower_bounds = cell_bounds[0]
         self.cell_upper_bounds = cell_bounds[1]
 
         self._cross_product_indices = torch.tensor(
-            list(product(*[[0, 1] for _ in range(ref_point.shape[0])])), dtype=torch.long, device=ref_point.device,
+            list(product(*[[0, 1] for _ in range(ref_point.shape[0])])),
+            dtype=torch.long,
+            device=ref_point.device,
         )
 
     def psi(self, lower: Tensor, upper: Tensor, mu: Tensor, sigma: Tensor) -> Tensor:
         u = (upper - mu) / sigma
         return sigma * Normal(0, 1).log_prob(u).exp() + (mu - lower) * (1 - Normal(0, 1).cdf(u))
 
     def nu(self, lower: Tensor, upper: Tensor, mu: Tensor, sigma: Tensor) -> Tensor:
         return (upper - lower) * (1 - Normal(0, 1).cdf((upper - mu) / sigma))
 
-    def ehvi_calc(self, Y_new: Tensor, Y_new_stddev: Tensor) -> Tensor:
+    def ehvi_calc(self, Y_new: Tensor, Y_new_stddev: Tensor, exploration_factor: int = 2) -> Tensor:
         # Reshaped to batch_size number of rows in the tensors
         Y_new = Y_new.reshape(Y_new.shape[0], 1, Y_new.shape[1])
         Y_new_stddev = Y_new_stddev.reshape(Y_new_stddev.shape[0], 1, Y_new_stddev.shape[1])
 
+        # Promoting exploration
+        Y_new_stddev = Y_new_stddev * exploration_factor
+
         cell_upper_bounds = self.cell_upper_bounds.clamp_max(1e10 if Y_new.dtype == torch.double else 1e8)
 
-        psi_lu = self.psi(lower=self.cell_lower_bounds, upper=cell_upper_bounds, mu=Y_new, sigma=Y_new_stddev,)
-        psi_ll = self.psi(lower=self.cell_lower_bounds, upper=self.cell_lower_bounds, mu=Y_new, sigma=Y_new_stddev,)
+        psi_lu = self.psi(
+            lower=self.cell_lower_bounds,
+            upper=cell_upper_bounds,
+            mu=Y_new,
+            sigma=Y_new_stddev,
+        )
+        psi_ll = self.psi(
+            lower=self.cell_lower_bounds,
+            upper=self.cell_lower_bounds,
+            mu=Y_new,
+            sigma=Y_new_stddev,
+        )
 
-        nu = self.nu(lower=self.cell_lower_bounds, upper=cell_upper_bounds, mu=Y_new, sigma=Y_new_stddev,)
+        nu = self.nu(
+            lower=self.cell_lower_bounds,
+            upper=cell_upper_bounds,
+            mu=Y_new,
+            sigma=Y_new_stddev,
+        )
 
         psi_diff = psi_ll - psi_lu
 
         stacked_factors = torch.stack([psi_diff, nu], dim=-2)
 
         all_factors_up_to_last = stacked_factors.gather(
             dim=-2,
```

### Comparing `nemo-bo-0.1.8/nemo_bo/acquisition_functions/nsga_improvement/genetic.py` & `nemo-bo-0.1.9/nemo_bo/acquisition_functions/nsga_improvement/genetic.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,14 @@
         # other run specific data updated whenever solve is called - to share them in all algorithms
         self.n_gen = None
         self.pop = None
         self.off = None
 
     def _initialize_infill(self):
         pop = self.initialization.do(self.problem, self.pop_size, algorithm=self)
-        pop.set("n_gen", self.n_gen)
 
         # Converts the feature values that correspond to descriptors for categorical variables generated by the
         # algorithm to their closest actual descriptor values by euclidean distance
         if self.problem.variables.num_cat_var > 0:
             for individual_idx, individual in enumerate(pop):
                 # Undo min-max normalisation of the X values according to the defined variables' lower and upper bounds
                 X_temp = (
@@ -102,15 +101,15 @@
                     np.array(self.problem.variables.upper_bounds) - np.array(self.problem.variables.lower_bounds)
                 )
 
         return pop
 
     def _initialize_advance(self, infills=None, **kwargs):
         if self.advance_after_initial_infill:
-            self.pop = self.survival.do(self.problem, infills, n_survive=len(infills))
+            self.pop = self.survival.do(self.problem, infills, n_survive=len(infills), algorithm=self, **kwargs)
 
     def _infill(self):
 
         # do the mating using the current population
         off = self.mating.do(self.problem, self.pop, self.n_offsprings, algorithm=self)
 
         # if the mating could not generate any new offspring (duplicate elimination might make that happen)
@@ -142,13 +141,16 @@
                     np.array(self.problem.variables.upper_bounds) - np.array(self.problem.variables.lower_bounds)
                 )
 
         return off
 
     def _advance(self, infills=None, **kwargs):
 
+        # the current population
+        pop = self.pop
+
         # merge the offsprings with the current population
         if infills is not None:
-            self.pop = Population.merge(self.pop, infills)
+            pop = Population.merge(self.pop, infills)
 
         # execute the survival to find the fittest solutions
-        self.pop = self.survival.do(self.problem, self.pop, n_survive=self.pop_size, algorithm=self)
+        self.pop = self.survival.do(self.problem, pop, n_survive=self.pop_size, algorithm=self, **kwargs)
```

### Comparing `nemo-bo-0.1.8/nemo_bo/acquisition_functions/nsga_improvement/nsga2.py` & `nemo-bo-0.1.9/nemo_bo/acquisition_functions/nsga_improvement/nsga2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # The NSGA-based methods were copied and adapted from J. Blank and K. Deb, pymoo: Multi-Objective Optimization in
 # Python, in IEEE Access, vol. 8, pp. 89497-89509, 2020, doi: 10.1109/ACCESS.2020.2990567
 # https://ieeexplore.ieee.org/document/9078759
 # https://github.com/anyoptimization/pymoo
 
 import numpy as np
+
 from pymoo.core.survival import Survival
 from pymoo.docs import parse_doc_string
-from pymoo.operators.crossover.sbx import SimulatedBinaryCrossover
-from pymoo.operators.mutation.pm import PolynomialMutation
+from pymoo.operators.crossover.sbx import SBX
+from pymoo.operators.mutation.pm import PM
 from pymoo.operators.sampling.rnd import FloatRandomSampling
-from pymoo.operators.selection.tournament import TournamentSelection, compare
-from pymoo.util.display import MultiObjectiveDisplay
+from pymoo.operators.selection.tournament import compare, TournamentSelection
+from pymoo.termination.default import DefaultMultiObjectiveTermination
+from pymoo.util.display.multi import MultiObjectiveOutput
 from pymoo.util.dominator import Dominator
 from pymoo.util.misc import find_duplicates, has_feasible
 from pymoo.util.nds.non_dominated_sorting import NonDominatedSorting
 from pymoo.util.randomized_argsort import randomized_argsort
-from pymoo.util.termination.default import MultiObjectiveDefaultTermination
 
 from nemo_bo.acquisition_functions.nsga_improvement.genetic import GeneticAlgorithm
 
 
 # ---------------------------------------------------------------------------------------------------------
 # Binary Tournament Selection Function
 # ---------------------------------------------------------------------------------------------------------
@@ -33,26 +34,21 @@
 
     tournament_type = algorithm.tournament_type
     S = np.full(n_tournaments, np.nan)
 
     for i in range(n_tournaments):
 
         a, b = P[i, 0], P[i, 1]
-        a_cv, a_f, b_cv, b_f, = (
-            pop[a].CV[0],
-            pop[a].F,
-            pop[b].CV[0],
-            pop[b].F,
-        )
+        a_cv, a_f, b_cv, b_f = pop[a].CV[0], pop[a].F, pop[b].CV[0], pop[b].F
         rank_a, cd_a = pop[a].get("rank", "crowding")
         rank_b, cd_b = pop[b].get("rank", "crowding")
 
         # if at least one solution is infeasible
         if a_cv > 0.0 or b_cv > 0.0:
-            S[i] = compare(a, a_cv, b, b_cv, method="smaller_is_better", return_random_if_equal=True,)
+            S[i] = compare(a, a_cv, b, b_cv, method="smaller_is_better", return_random_if_equal=True)
 
         # both solutions are feasible
         else:
 
             if tournament_type == "comp_by_dom_and_crowding":
                 rel = Dominator.get_relation(a_f, b_f)
                 if rel == 1:
@@ -64,15 +60,15 @@
                 S[i] = compare(a, rank_a, b, rank_b, method="smaller_is_better")
 
             else:
                 raise Exception("Unknown tournament type.")
 
             # if rank or domination relation didn't make a decision compare by crowding
             if np.isnan(S[i]):
-                S[i] = compare(a, cd_a, b, cd_b, method="larger_is_better", return_random_if_equal=True,)
+                S[i] = compare(a, cd_a, b, cd_b, method="larger_is_better", return_random_if_equal=True)
 
     return S[:, None].astype(int, copy=False)
 
 
 # ---------------------------------------------------------------------------------------------------------
 # Survival Selection
 # ---------------------------------------------------------------------------------------------------------
@@ -126,50 +122,33 @@
 
 class NSGA2(GeneticAlgorithm):
     def __init__(
         self,
         pop_size=100,
         sampling=FloatRandomSampling(),
         selection=TournamentSelection(func_comp=binary_tournament),
-        crossover=SimulatedBinaryCrossover(eta=15, prob=0.9),
-        mutation=PolynomialMutation(prob=None, eta=20),
+        crossover=SBX(eta=15, prob=0.9),
+        mutation=PM(eta=20),
         survival=RankAndCrowdingSurvival(),
-        eliminate_duplicates=True,
-        n_offsprings=None,
-        display=MultiObjectiveDisplay(),
+        output=MultiObjectiveOutput(),
         **kwargs
     ):
-        """
-
-        Parameters
-        ----------
-        pop_size : {pop_size}
-        sampling : {sampling}
-        selection : {selection}
-        crossover : {crossover}
-        mutation : {mutation}
-        eliminate_duplicates : {eliminate_duplicates}
-        n_offsprings : {n_offsprings}
-
-        """
-
         super().__init__(
             pop_size=pop_size,
             sampling=sampling,
             selection=selection,
             crossover=crossover,
             mutation=mutation,
             survival=survival,
-            eliminate_duplicates=eliminate_duplicates,
-            n_offsprings=n_offsprings,
-            display=display,
+            output=output,
             advance_after_initial_infill=True,
             **kwargs
         )
-        self.default_termination = MultiObjectiveDefaultTermination()
+
+        self.termination = DefaultMultiObjectiveTermination()
         self.tournament_type = "comp_by_dom_and_crowding"
 
     def _set_optimum(self, **kwargs):
         if not has_feasible(self.pop):
             self.opt = self.pop[[np.argmin(self.pop.get("CV"))]]
         else:
             self.opt = self.pop[self.pop.get("rank") == 0]
@@ -212,15 +191,15 @@
 
         # if we divide by zero because all values in one columns are equal replace by none
         dist_to_last[np.isnan(dist_to_last)] = 0.0
         dist_to_next[np.isnan(dist_to_next)] = 0.0
 
         # sum up the distance to next and last and norm by objectives - also reorder from sorted list
         J = np.argsort(I, axis=0)
-        _cd = np.sum(dist_to_last[J, np.arange(n_obj)] + dist_to_next[J, np.arange(n_obj)], axis=1,) / n_obj
+        _cd = np.sum(dist_to_last[J, np.arange(n_obj)] + dist_to_next[J, np.arange(n_obj)], axis=1) / n_obj
 
         # save the final vector which sets the crowding distance for duplicates to zero to be eliminated
         crowding = np.zeros(n_points)
         crowding[is_unique] = _cd
 
     # crowding[np.isinf(crowding)] = 1e+14
     return crowding
```

### Comparing `nemo-bo-0.1.8/nemo_bo/acquisition_functions/nsga_improvement/nsga3.py` & `nemo-bo-0.1.9/nemo_bo/acquisition_functions/nsga_improvement/nsga3.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 # https://ieeexplore.ieee.org/document/9078759
 # https://github.com/anyoptimization/pymoo
 
 import warnings
 
 import numpy as np
 from numpy.linalg import LinAlgError
+
 from pymoo.core.survival import Survival
 from pymoo.docs import parse_doc_string
-from pymoo.operators.crossover.sbx import SimulatedBinaryCrossover
-from pymoo.operators.mutation.pm import PolynomialMutation
+from pymoo.operators.crossover.sbx import SBX
+from pymoo.operators.mutation.pm import PM
 from pymoo.operators.sampling.rnd import FloatRandomSampling
 from pymoo.operators.selection.tournament import TournamentSelection, compare
-from pymoo.util.display import MultiObjectiveDisplay
+from pymoo.util.display.multi import MultiObjectiveOutput
 from pymoo.util.function_loader import load_function
-from pymoo.util.misc import has_feasible, intersect
+from pymoo.util.misc import intersect, has_feasible
 from pymoo.util.nds.non_dominated_sorting import NonDominatedSorting
 
 from nemo_bo.acquisition_functions.nsga_improvement.genetic import GeneticAlgorithm
 
 
 # =========================================================================================================
 # Implementation
@@ -30,15 +31,15 @@
     S = np.full(P.shape[0], np.nan)
 
     for i in range(P.shape[0]):
         a, b = P[i, 0], P[i, 1]
 
         # if at least one solution is infeasible
         if pop[a].CV > 0.0 or pop[b].CV > 0.0:
-            S[i] = compare(a, pop[a].CV, b, pop[b].CV, method="smaller_is_better", return_random_if_equal=True,)
+            S[i] = compare(a, pop[a].CV, b, pop[b].CV, method="smaller_is_better", return_random_if_equal=True)
 
         # both solutions are feasible just set random
         else:
             S[i] = np.random.choice([a, b])
 
     return S[:, None].astype(int)
 
@@ -46,19 +47,19 @@
 class NSGA3(GeneticAlgorithm):
     def __init__(
         self,
         ref_dirs,
         pop_size=None,
         sampling=FloatRandomSampling(),
         selection=TournamentSelection(func_comp=comp_by_cv_then_random),
-        crossover=SimulatedBinaryCrossover(eta=30, prob=1.0),
-        mutation=PolynomialMutation(eta=20, prob=None),
+        crossover=SBX(eta=30, prob=1.0),
+        mutation=PM(eta=20),
         eliminate_duplicates=True,
         n_offsprings=None,
-        display=MultiObjectiveDisplay(),
+        output=MultiObjectiveOutput(),
         **kwargs,
     ):
         """
 
         Parameters
         ----------
 
@@ -81,15 +82,16 @@
         if self.ref_dirs is not None:
 
             if pop_size is None:
                 pop_size = len(self.ref_dirs)
 
             if pop_size < len(self.ref_dirs):
                 print(
-                    f"WARNING: pop_size={pop_size} is less than the number of reference directions ref_dirs={len(self.ref_dirs)}.\n"
+                    f"WARNING: pop_size={pop_size} is less than the number of reference directions "
+                    f"ref_dirs={len(self.ref_dirs)}.\n"
                     "This might cause unwanted behavior of the algorithm. \n"
                     "Please make sure pop_size is equal or larger than the number of reference directions. "
                 )
 
         if "survival" in kwargs:
             survival = kwargs["survival"]
             del kwargs["survival"]
@@ -101,15 +103,15 @@
             sampling=sampling,
             selection=selection,
             crossover=crossover,
             mutation=mutation,
             survival=survival,
             eliminate_duplicates=eliminate_duplicates,
             n_offsprings=n_offsprings,
-            display=display,
+            output=output,
             advance_after_initial_infill=True,
             **kwargs,
         )
 
     def _setup(self, problem, **kwargs):
 
         if self.ref_dirs is not None:
@@ -186,15 +188,15 @@
             # if some individuals already survived
             else:
                 until_last_front = np.concatenate(fronts[:-1])
                 niche_count = calc_niche_count(len(self.ref_dirs), niche_of_individuals[until_last_front])
                 n_remaining = n_survive - len(until_last_front)
 
             S = niching(
-                pop[last_front], n_remaining, niche_count, niche_of_individuals[last_front], dist_to_niche[last_front],
+                pop[last_front], n_remaining, niche_count, niche_of_individuals[last_front], dist_to_niche[last_front]
             )
 
             survivors = np.concatenate((until_last_front, last_front[S].tolist()))
             pop = pop[survivors]
 
         return pop
 
@@ -295,15 +297,15 @@
         self.extreme_points = get_extreme_points_c(F[nds, :], self.ideal_point, extreme_points=self.extreme_points)
 
         # find the intercepts for normalization and do backup if gaussian elimination fails
         worst_of_population = np.max(F, axis=0)
         worst_of_front = np.max(F[nds, :], axis=0)
 
         self.nadir_point = get_nadir_point(
-            self.extreme_points, self.ideal_point, self.worst_point, worst_of_population, worst_of_front,
+            self.extreme_points, self.ideal_point, self.worst_point, worst_of_population, worst_of_front
         )
 
 
 def get_extreme_points_c(F, ideal_point, extreme_points=None):
     # calculate the asf which is used for the extreme point decomposition
     weights = np.eye(F.shape[1])
     weights[weights == 0] = 1e6
```

### Comparing `nemo-bo-0.1.8/nemo_bo/acquisition_functions/nsga_improvement/nsga_improvement.py` & `nemo-bo-0.1.9/nemo_bo/models/nn_ensemble.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,370 +1,463 @@
+from __future__ import annotations
+
+import math
 import os
-from dataclasses import dataclass
-from itertools import combinations
-from typing import Optional, Tuple
+from datetime import datetime
+from functools import partial
+from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple
 
 import numpy as np
-import torch
-from botorch.utils.multi_objective.hypervolume import Hypervolume
-from botorch.utils.multi_objective.pareto import is_non_dominated
-from pymoo.core.result import Result
-from pymoo.factory import get_reference_directions, get_termination
-from pymoo.optimize import minimize
-from scipy import spatial
+import tensorflow as tf
+import tensorflow_probability as tfp
+from hyperopt import STATUS_OK, Trials, fmin, hp, tpe
+from hyperopt.pyll.base import scope
+from keras import backend as K
+from keras import callbacks
+from keras.layers import Dense, Dropout, Input
+from keras.models import Model
+from keras.optimizers import Optimizer
+from sklearn.model_selection import train_test_split
+from tensorflow import keras
+
+tf.keras.backend.set_floatx("float64")
 
 import nemo_bo.utils.logger as logging_nemo
-from nemo_bo.acquisition_functions.base_acq_function import AcquisitionFunction
-from nemo_bo.acquisition_functions.nsga_improvement.problem_wrapper import NSGAProblemWrapper
-from nemo_bo.acquisition_functions.nsga_improvement.unsga3 import UNSGA3
-from nemo_bo.opt.constraints import ConstraintsList
-from nemo_bo.opt.objectives import ObjectivesList
-from nemo_bo.opt.samplers import LatinHyperCubeSampling, PoolBased, SampleGenerator
-from nemo_bo.opt.variables import VariablesList
-from nemo_bo.utils.data_proc import remove_all_nan_rows
+import nemo_bo.utils.perf_metrics as pm
+from nemo_bo.models.base.base_model import Base_Model
+from nemo_bo.models.base.nn_save_checkpoint import SaveModelCheckPoint
+from nemo_bo.utils.data_proc import sort_train_test_split_shuffle
+
+if TYPE_CHECKING:
+    from nemo_bo.opt.objectives import RegressionObjective
+    from nemo_bo.opt.variables import VariablesList
 
 try:
     logging_nemo.logging_path
     logger = logging_nemo.logging_nemo_child(os.path.basename(__file__))
 except AttributeError:
     logger = logging_nemo.logging_nemo_master(os.path.basename(__file__))
 
 
-@dataclass
-class NSGAImprovement(AcquisitionFunction):
-    """
+tfpl = tfp.layers
+tfd = tfp.distributions
 
-    For single-objective and multi-objective problems, this acquisition function can select between a method that
-    identifies the highest hypervolume improvement using a U-NSGA3 algorithm for selecting candidates, or an
-    explorative method that identifies the approximate region of the variable space that has the highest uncertainty
-    in the objective prediction
-
-    Parameters
-    ----------
-    num_candidates: int
-        The number of sets of X arrays to be suggested by the acquisition function
+gpus = tf.config.list_physical_devices("GPU")
+if gpus:
+    try:
+        # Memory growth needs to be the same across GPUs
+        for gpu in gpus:
+            tf.config.experimental.set_memory_growth(gpu, True)
+        logical_gpus = tf.config.list_logical_devices("GPU")
+        print(len(gpus), "Physical GPUs,", len(logical_gpus), "Logical GPUs")
+    except RuntimeError as e:
+        print(e)
 
+
+class NNEnsembleModel(Base_Model):
     """
 
-    num_candidates: int
+    Used to create an ensemble of neural network models for the RegressionObjective
+
+    See docstring for Base_Model __init__ function for information
 
-    def generate_candidates(
+    """
+
+    def __init__(
         self,
-        Y: np.ndarray,
         variables: VariablesList,
-        objectives: ObjectivesList,
-        sampler: Optional[SampleGenerator] = None,
-        constraints: Optional[ConstraintsList] = None,
-        **acq_func_kwargs,
-    ) -> Tuple[np.ndarray, np.ndarray]:
+        objective: RegressionObjective,
+        always_hyperparam_opt: bool = False,
+        es_patience: int = 300,  # normally 300
+    ):
+        super().__init__(variables, objective, always_hyperparam_opt)
+        self.default_X_transform_type = "standardisation"
+        self.default_Y_transform_type = "standardisation"
+        self.include_validation = True
+        self.name = "nn_ensemble"
+
+        # Creates the callback method to stop fitting before the all epochs are completed based on the prediction
+        # accuracy of the validation set
+        self.earlystopping = callbacks.EarlyStopping(
+            monitor="val_loss",
+            min_delta=0.001,
+            patience=es_patience,
+            verbose=0,
+            mode="min",
+        )
+
+        # The directory to save the model parameters when it detects a model with better prediction accuracy of the
+        # validation set
+        self.dirname_checkpoint = os.path.join(os.getcwd(), "ML Models", "nn_ensemble", "Checkpoints")
+        if not os.path.exists(self.dirname_checkpoint):
+            os.makedirs(self.dirname_checkpoint)
+
+    @staticmethod
+    def negloglik(y_data, rv_y):
+        """
+
+        Function to calculate the value of the negative loglikelihood function
+
+        """
+        return -rv_y.log_prob(y_data)
+
+    # function for creating a fully connected neural network of any architecture
+    # the number of neurons in each layer is defined by layers_shape
+    # the droupout_proba indicates if dropout layers should be added
+    def structure(
+        self,
+        learning_rate: float,
+        hidden_units: int,
+        hidden_layers: int,
+        dropout_proba: float,
+        act_func: str,
+        optimizer: Optimizer,
+    ) -> Model:
         """
 
-        Function that is called when generate the best candidates using the expected improvement or expected
-        hypervolume acquisition functions. This selection is made automatically based on the number of objectives
+        Function that defines the structure of the input, hidden layers, and output for the neural network models in
+        the ensemble
 
         Parameters
         ----------
-        Y: np.ndarray
-            An array containing Y-values for all objectives
-        variables: VariablesList
-            VariablesList object that contains information about all variables
-        objectives: ObjectivesList
-            ObjectivesList object that contains information about all objectives
-        sampler: SampleGenerator, Default = None
-            Used to generate samples (SampleGenerator). PoolBased is not supported
-        constraints: ConstraintsList, Default = None
-            ConstraintsList object that contains information about all constraints
+        learning_rate: float
+            Assigns the learning rate for the optimiser
+        hidden_units: int
+            The number of hidden units within every hidden layer. Currently, all hidden layers will have this number
+            of hidden units
+        hidden_layers: int
+            The number of hidden layers in the neural network
+        dropout_proba: float
+            The dropout probability to be applied to the hidden layers
+        act_func: str
+            The activation function to apply on every hidden layer
+        optimizer: Optimizer
+            The type of optimiser to use to fit the model
 
         Returns
         -------
-        selected_X: np.ndarray
-            Array of X-values of the identified candidates' that have the highest hypervolume improvement
-        selected_Y: np.ndarray
-            Array of Y-values of the identified candidates' that have the highest hypervolume improvement
+        model:
+            The neural network model with specified hidden layers
 
         """
-        if isinstance(sampler, PoolBased):
-            raise NotImplementedError(
-                "The PoolBased sampler is incompatible with the NSGAImprovement acquisition function. Please select a different sampler if you wish to continue using this acquisition function. Alternatively, you may use the ExpectedImprovement acquisition function with the PoolBased sampler instead"
-            )
+        K.clear_session()
+        tf.random.set_seed(1)
+        tf.random.uniform([1], seed=1)
+        input_data = Input((self.X_train.shape[1],))
+        input_data = tf.cast(input_data, tf.float64)
+        x = input_data
+        for _ in range(hidden_layers):
+            x = Dense(hidden_units, activation=act_func, dtype=tf.float64)(x)
+            if dropout_proba > 0:
+                x = Dropout(dropout_proba)(x)
+
+        x = Dense(2)(x)
+        x = tfpl.DistributionLambda(lambda t: tfd.Normal(loc=t[..., :1], scale=1e-3 + tf.math.softplus(t[..., 1:])))(x)
+        model = Model(input_data, x)
+        # model.summary()
+
+        model.compile(
+            optimizer=optimizer(learning_rate=learning_rate),
+            loss=self.negloglik,
+            metrics=["mse"],
+        )
+
+        return model
 
-        self.exploit_or_explore = acq_func_kwargs.get("exploit_or_explore", "exploit")
-        self.pop_size = acq_func_kwargs.get("pop_size")
-        self.generations = acq_func_kwargs.get("generations")
-
-        Y = remove_all_nan_rows(Y)
-
-        if self.pop_size is None:
-            if self.num_candidates == 1:
-                self.pop_size = 200
-            elif self.num_candidates == 2:
-                self.pop_size = 100
-            elif self.num_candidates == 3:
-                self.pop_size = 70
-            elif self.num_candidates == 4:
-                # self.pop_size = 40
-                self.pop_size = 200
-
-        if self.generations is None:
-            self.generations = 30
-            # if self.num_candidates == 1:
-            #     self.generations = 50
-            # elif self.num_candidates == 2:
-            #     self.generations = 30
-            # elif self.num_candidates == 3:
-            #     self.generations = 30
-            # elif self.num_candidates == 4:
-            #     self.generations = 30
-
-        if self.exploit_or_explore == "exploit":
-            self.generate_pareto(variables, objectives, constraints)
-            selected_X, selected_Y = self.hvi(self.res.X, self.res.F, Y, variables, objectives)
-
-            self.reset = False
-
-        if self.exploit_or_explore == "explore" or not self.hvi_search_pass:
-            selected_X, selected_Y, total_Y_std = self.highest_uncertainty(variables, objectives, sampler, constraints)
-
-            self.exploit_or_explore = "exploit"
-            self.reset = True
-
-        return selected_X, selected_Y
-
-    def generate_pareto(
-        self, variables: VariablesList, objectives: ObjectivesList, constraints: ConstraintsList
-    ) -> Result:
+    def fit(
+        self, X: np.ndarray, Y: np.ndarray, test_ratio: float = 0.2, sort_before_split: bool = None, **params
+    ) -> None:
         """
-        Runs the U-NSGA3 method to generate the samples that have the highest hypervolume
+
+        Function that is called to start the probabilistic neural network model fitting procedure
 
         Parameters
         ----------
-        variables: VariablesList
-            VariablesList object that contains information about all variables
-        objectives: ObjectivesList
-            ObjectivesList object that contains information about all objectives
-        constraints: ConstraintsList, Default = None
-            ConstraintsList object that contains information about all constraints
-
-        Returns
-        -------
-        res: Result
-            Contains all of the information and results from the U-NSGA3 method
+        X: np.ndarray,
+            X array that contains the unprocessed variables data to be fitted to the model, i.e. The data has not yet
+            undergone any transformations related to converted categorical variables to their respective descriptors
+            or transformations related to standardisation/normalisation
+        Y: np.ndarray,
+            Y array that contains the unprocessed objective data, i.e. The data has not yet undergone any
+            transformations related to standardisation/normalisation
+        test_ratio: float, Default = 0.2,
+            The proportion of inputted X and Y arrays to be split for the validation set where applicable
+        sort_before_split: bool, Default = True,
+            Whether the inputted X and Y arrays should be sorted such that the Y-values are in ascending order before
+            splitting into the training and test sets (and validation sets if applicable)
+        params: Dict[str, Any]
+            Dictionary that contains the hyperparameters for the model
 
         """
+        if sort_before_split:
+            (
+                X_train,
+                X_val,
+                Y_train,
+                Y_val,
+            ) = sort_train_test_split_shuffle(X, Y, test_ratio=test_ratio, seed=1)
+        else:
+            X_train, X_val, Y_train, Y_val = train_test_split(X, Y, test_size=test_ratio, random_state=1)
 
-        xl = 0
-        xu = 1
+        Y_train = Y_train.astype("float")
+        Y_val = Y_val.astype("float")
 
-        ref_dirs = get_reference_directions("energy", objectives.n_obj, self.pop_size * 0.9, seed=1)
+        self.X_train, self.X_val, self.Y_train, self.Y_val = (
+            X_train,
+            X_val,
+            Y_train,
+            Y_val,
+        )
+        if self.variables.num_cat_var > 0:
+            self.X_train = self.variables.categorical_transform(self.X_train).astype("float")
+            self.X_val = self.variables.categorical_transform(self.X_val).astype("float")
+
+        self.X_train, self.Y_train = self.transform_by_predictor_type(self.X_train, Y=self.Y_train)
+        self.X_val, self.Y_val = self.transform_only_by_predictor_type(self.X_val, self.Y_val)
+
+        self.fit_model(params)
+
+        self.Y_train_pred, self.Y_train_pred_stddev = self.predict(X_train)
+        self.Y_val_pred, self.Y_val_pred_stddev = self.predict(X_val)
+        self.performance_metrics = pm.all_performance_metrics_train_val(
+            Y_train, self.Y_train_pred, Y_val, self.Y_val_pred
+        )
 
-        logger.info(f"Performing U-NSGA3 opt")
-        algorithm = UNSGA3(ref_dirs, pop_size=self.pop_size)
-        problem = NSGAProblemWrapper(xl, xu, variables, objectives, constraints)
-        termination = get_termination("n_gen", self.generations)
+        self.Y_train_error = 1.96 * self.Y_train_pred_stddev
+        self.Y_val_error = 1.96 * self.Y_val_pred_stddev
 
-        # Performs the U-NSGA3 optimisation
-        self.res = minimize(problem, algorithm, termination, verbose=True)
+    def fit_model(self, params: Dict[str, Any]) -> None:
+        """
 
-        # Correct by * -1 for maximising objectives in U-NSGA3 optimisation
-        for obj_index, obj in enumerate(objectives.max_bool_dict):
-            if objectives.max_bool_dict[obj]:
-                if objectives.n_obj > 1:
-                    self.res.F[:, obj_index] *= -1
-                else:
-                    self.res.F[obj_index] *= -1
+        Called by the fit and cv-related functions for fitting the neural network models in the ensemble using
+        pre-processed X and Y training data in the class instance
 
-        # Undo min-max normalisation of X values identified by U-NSGA3
-        self.res.X = (self.res.X * (np.array(variables.upper_bounds) - np.array(variables.lower_bounds))) + np.array(
-            variables.lower_bounds
+        """
+        hidden_units = int(params.get("hidden_units", self.X_train.shape[1] + 1))
+        hidden_layers = int(params.get("hidden_layers", 2))
+        batch_size = int(params.get("batch_size", 32))
+        learning_rate = params.get("learning_rate", 0.001)
+        dropout_proba = params.get("dropout_proba", 0.001)
+        ensemble_size = int(params.get("ensemble_size", 5))
+        max_epochs = int(params.get("max_epochs", 4000))
+        act_func = params.get("act_func", "relu")
+        optimizer = params.get("optimizer", keras.optimizers.Adam)
+
+        self.filepath = os.path.join(
+            self.dirname_checkpoint,
+            f"Checkpoint, Ensemble, {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}.h5",
         )
 
-        return self.res
+        self.ensemble_model_list = []
+        for _ in range(ensemble_size):
+            self.model = self.structure(
+                learning_rate,
+                hidden_units,
+                hidden_layers,
+                dropout_proba,
+                act_func,
+                optimizer,
+            )
+            self.savemodelcheckpoint = SaveModelCheckPoint(self.model, self.filepath)  # A Simon Original
+            self.history = self.model.fit(
+                self.X_train,
+                self.Y_train,
+                validation_data=(self.X_val, self.Y_val),
+                epochs=max_epochs,
+                verbose=0,
+                batch_size=batch_size,
+                callbacks=[
+                    callbacks.LambdaCallback(on_epoch_end=self.savemodelcheckpoint.save_weights),
+                    self.earlystopping,
+                ],
+            )
 
-    def hvi(
-        self,
-        X_nsga: np.ndarray,
-        Y_nsga: np.ndarray,
-        Y: np.ndarray,
-        variables: VariablesList,
-        objectives: ObjectivesList,
-    ) -> Tuple[np.ndarray, np.ndarray]:
+            self.model = self.structure(
+                learning_rate,
+                hidden_units,
+                hidden_layers,
+                dropout_proba,
+                act_func,
+                optimizer,
+            )
+            self.model.load_weights(self.filepath)
+            self.ensemble_model_list.append(self.model)
+
+    def predict(self, X: np.ndarray, X_transform: bool = True) -> Tuple[np.ndarray, np.ndarray]:
         """
 
-        Identifies the candidate(s) from the solutions from the U-NSGA3 optimisation that will produce the highest
-        hypervolume improvement
+        Determines the model output and its standard deviation of the X array passed into the function
 
         Parameters
         ----------
-        X_nsga: np.ndarray
-            Variable values for the solutions from the U-NSGA3 optimisation
-        Y_nsga : np.ndarray
-            Objective values for the solutions from the U-NSGA3 optimisation
-        Y: np.ndarray
-            An array containing Y-values for all objectives
-        variables: VariablesList
-            VariablesList object that contains information about all variables
-        objectives: ObjectivesList
-            ObjectivesList object that contains information about all objectives
+        X: np.ndarray,
+            X array that contains the unprocessed variables data to be used in the prediction, i.e. The data has not
+            yet undergone any transformations related to converted categorical variables to their respective
+            descriptors or transformations related to standardisation/normalisation
+        X_transform: bool, Default = True
+            For the default models provided natively in NEMO, the initial transformation of categorical variables and
+            transformations related to standardisation/normalisation can be switched off by passing X_transform = False
 
         Returns
-        -------
-        selected_X: np.ndarray
-            Array of X-values of the identified candidates' that have the highest hypervolume improvement
-        selected_Y: np.ndarray
-            Array of Y-values of the identified candidates' that have the highest hypervolume improvement
-
-        """
-        logger.info(f"Identifying conditions with the largest hypervolume")
-
-        # Construct hvrefs refs
-        ref_point = self.build_ref_point(objectives.max_bool_dict)
-
-        # min-max normalisation for datasets
-        sign_adjusted_Y = self.Y_norm_minmax_transform(Y, objectives.bounds, objectives.max_bool_dict)
-        sign_adjusted_Y_nsga = self.Y_norm_minmax_transform(Y_nsga, objectives.bounds, objectives.max_bool_dict)
-
-        # Creates a list of hypervolumes after each candidate(s) that successfully improves the hypervolume
-        hv_list = []
-        candidates_X_list = []
-        candidates_Y_list = []
-        X_nsga_combos = list(combinations(X_nsga, self.num_candidates))
-        Y_nsga_combos = list(combinations(Y_nsga, self.num_candidates))
-        sign_adjusted_Y_nsga_combos = list(combinations(sign_adjusted_Y_nsga, self.num_candidates))
-        for x, y, candidates_Y in zip(X_nsga_combos, Y_nsga_combos, sign_adjusted_Y_nsga_combos):
-            # Adds the candidate objective values to the experimental data set
-            YappF = np.vstack([sign_adjusted_Y, np.array(candidates_Y)])
-            # Identifies which data points are non-dominated
-            pareto_mask_YappF = is_non_dominated(torch.tensor(YappF, dtype=torch.double))
-            # Creates an numpy.ndarray containing the non-dominated points
-            pareto_front_YappF = YappF[pareto_mask_YappF]
-
-            # The following are checks to confirm that all new points in the candidates_Y set are on the pareto front
-            candidate_in_pareto_counter = 0
-            for a in candidates_Y:
-                if any((a == b).all() for b in pareto_front_YappF):
-                    candidate_in_pareto_counter += 1
-                else:
-                    break
-            # So if all new points in the candidates_Y set are on the pareto front, then it will append the x and y and calculate the predicted hypervolume
-            if candidate_in_pareto_counter == len(candidates_Y):
-                candidates_X_list.append(x)
-                candidates_Y_list.append(y)
-                # Calculates the hypervolume
-                hv = Hypervolume(ref_point=torch.tensor(ref_point, dtype=torch.double))
-                hv_list.append(hv.compute(torch.tensor(pareto_front_YappF, dtype=torch.double)))
-
-        # Selects the variable and objective values of the candidate(s) that produced the largest hypervolume
-        # if hv_list is not empty
-        if hv_list:
-            logger.info("Conditions were successfully selected using hypervolume improvement")
-            max_idx = hv_list.index(max(hv_list))
-            selected_X = np.array(candidates_X_list[max_idx])
-            selected_Y = np.array(candidates_Y_list[max_idx])
-            self.hvi_search_pass = True
+        ----------
+        Y_pred: np.ndarray
+            The predictive mean of the objective calculated using the model and the inputted X array. The outputted
+            values have been un-transformed
+        Y_pred_stddev: np.ndarray
+            The predictive standard deviation of the objective calculated using the model and the inputted X array. The
+            outputted values have been un-transformed
 
-            if variables.num_cat_descriptor_var > 0:
-                selected_X = variables.descriptor_to_name(selected_X)
+        """
+        # X needs to be a 2D array
+        if X.ndim == 1:
+            X = X.reshape(1, -1)
+
+        if X_transform:
+            if self.variables.num_cat_var > 0:
+                X = self.variables.categorical_transform(X).astype("float")
+            X = self.transform_only_by_predictor_type(X)
+
+        observed_Y_pred = [ensemble_model(X) for ensemble_model in self.ensemble_model_list]
+        Y_pred = np.array([prediction.loc.numpy() for prediction in observed_Y_pred])
+        Y_pred_stddev = np.array([prediction.scale.numpy() for prediction in observed_Y_pred])
+
+        # Code adapted from:
+        #     1. João Caldeira, Brian Nord, Deeply Uncertain: Comparing Methods of Uncertainty Quantification in Deep
+        #     Learning Algorithms, arXiv:2004.10710, https://github.com/deepskies/DeeplyUncertain-Public,
+        #     2. Yarin Gal, Jiri Hron, Alex Kendall, Concrete Dropout, arXiv:1705.07832,
+        #     https://github.com/yaringal/ConcreteDropout
+        Y_val_epistemic_unc = np.std(np.array(Y_pred), axis=0)  # Equation 4 from paper
+        Y_val_aleatoric_unc = np.sqrt(np.mean(np.array(Y_pred_stddev) * np.array(Y_pred_stddev), axis=0))
+        Y_val_total_unc = np.sqrt(Y_val_aleatoric_unc**2 + Y_val_epistemic_unc**2)
+
+        Y_pred = np.mean(Y_pred, axis=0)
+        Y_pred_upper = Y_pred + (1.96 * Y_val_total_unc)
+
+        Y_pred = self.objective.inverse_transform(Y_pred)
+        Y_pred_upper = self.objective.inverse_transform(Y_pred_upper)
+        Y_pred_stddev = (np.subtract(Y_pred_upper, Y_pred)) / 1.96
 
-        else:
-            logger.info(
-                "Failed to identify a set of conditions that would improve the hypervolume at the desired batch size"
-            )
-            selected_X = np.array([0])
-            selected_Y = np.array([0])
-            self.hvi_search_pass = False
+        return Y_pred.flatten(), Y_pred_stddev.flatten()
 
-        return selected_X, selected_Y
+    def draw_samples(self, X: np.ndarray, X_transform: bool = True) -> np.ndarray:
+        """
 
-    def highest_uncertainty(
+        Generates samples from a normal distribution using the X array
+
+        Parameters
+        ----------
+        X: np.ndarray,
+            X array that contains the unprocessed variables data to be used in the prediction, i.e. The data has not
+            yet undergone any transformations related to converted categorical variables to their respective
+            descriptors or transformations related to standardisation/normalisation
+        X_transform: bool, Default = True
+            For the default models provided natively in NEMO, the initial transformation of categorical variables and
+            transformations related to standardisation/normalisation can be switched off by passing X_transform = False
+
+        Returns
+        ----------
+        np.ndarray
+            Drawn samples of the objective using the model and the inputted X array. The outputted values have been
+            un-transformed
+
+        """
+        Y_pred, Y_pred_stddev = self.predict(X, X_transform=X_transform)
+
+        return np.random.default_rng().normal(Y_pred, Y_pred_stddev)
+
+    @staticmethod
+    def default_params(X: np.ndarray):
+        """
+
+        Function that returns the default hyperparameters to use for the hyperparameter optimisation of ensemble
+        neural network models using the hyperopt package. Returns a dictionary that is used for the space argument in
+        the hyperopt.fmin function
+
+        """
+        return {
+            "learning_rate": hp.uniform("learning_rate", 0.001, 0.01),
+            "hidden_units": scope.int(hp.quniform("hidden_units", math.ceil(X.shape[1] / 2), (X.shape[1] + 1), 1)),
+            "hidden_layers": scope.int(hp.quniform("hidden_layers", 1, 2, 1)),
+            "batch_size": scope.int(hp.quniform("batch_size", math.ceil(X.shape[0] / 10), X.shape[0], 1)),
+            "dropout_proba": hp.uniform("dropout_proba", 0.001, 0.05),
+        }
+
+    def hyperparam_opt(
         self,
-        variables: VariablesList,
-        objectives: ObjectivesList,
-        sampler: Optional[SampleGenerator] = None,
-        constraints: Optional[ConstraintsList] = None,
-        num_new_points: int = 2000000,
-    ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        X: np.ndarray,
+        Y: np.ndarray,
+        test_ratio: float,
+        sort_before_split: bool = True,
+        predictor_params_dict: Optional[Dict[str, Dict[str, Callable]]] = None,
+        **kwargs,
+    ) -> Tuple[NNEnsembleModel, Dict[str, Any]]:
         """
 
-        Function to identify a set of input variables from the variable space that has the highest uncertainty for
-        predicted output value(s)
+        Function to be called for performing hyperparameter optimisation for ensemble neural network models using
+        the hyperopt package. Returns the model fitted with the best hyperparameters and a dictionary containing the
+        best hyperparameters
 
         Parameters
         ----------
-        variables: VariablesList
-            VariablesList object that contains information about all variables
-        objectives: ObjectivesList
-            ObjectivesList object that contains information about all objectives
-        sampler: SampleGenerator, Default = None
-            Used to generate samples (SampleGenerator). PoolBased is not supported
-        constraints: ConstraintsList, Default = None
-            ConstraintsList object that contains information about all constraints
-        num_new_points: int, Default: 200,000
-            Number of new sets of input variables to generate
+        X: np.ndarray,
+            X array that contains the unprocessed variables data to be fitted to the model, i.e. The data has not yet
+            undergone any transformations related to converted categorical variables to their respective descriptors
+            or transformations related to standardisation/normalisation
+        Y: np.ndarray,
+            Y array that contains the unprocessed objective data, i.e. The data has not yet undergone any
+            transformations related to standardisation/normalisation
+        test_ratio: float
+            The proportion of inputted X and Y arrays to be split for the validation set where applicable
+        sort_before_split: bool, Default = True,
+            Whether the inputted X and Y arrays should be sorted such that the Y-values are in ascending order before
+            splitting into the training and test sets (and validation sets if applicable)
+        predictor_params_dict: Dict[str, Dict[str, Callable]], Default = None
+            Dictionary with a key 'nn_ensemble' and a corresponding value that is a dictionary that is used for the
+            space argument in the hyperopt.fmin function
 
         Returns
         -------
-        selected_X: np.ndarray
-            Array of X-values of the identified candidates' that have the highest hypervolume improvement
-        selected_Y: np.ndarray
-            Array of Y-values of the identified candidates' that have the highest hypervolume improvement
-        total_Y_std: np.ndarray
-            Array of total min-max normalised standard deviations for Y-values of the identified candidates' that have
-            the highest hypervolume improvement
+        model: NNBayesianModel
+            The model fitted with the best hyperparameters found using the hyperopt package
 
-        """
-        logger.info(f"Identifying conditions with the highest uncertainty")
+        model_params: Dict[str, Any]
+            Dictionary containing the best hyperparameters found using the hyperopt package
 
-        if sampler is None:
-            sampler = LatinHyperCubeSampling(num_new_points)
+        """
+        if predictor_params_dict is None:
+            predictor_params_dict = self.default_params(X)
         else:
-            # if sampler.num_new_points is None:
-            # sampler.num_new_points = num_new_points
-            sampler.num_new_points = num_new_points
-            # sampler = sampler
-
-        X_new_points = sampler.generate_samples(variables, constraints)
-
-        Y_new_points, Y_new_points_stddev = objectives.evaluate(X_new_points)
-
-        # Min_max normalisation of Y standard deviation
-        # I think this should be fine to minmax normalise like this
-        for obj_index, _ in enumerate(objectives.bounds):
-            Y_new_points_stddev[:, obj_index] = Y_new_points_stddev[:, obj_index] / (
-                objectives.bounds[obj_index, 1] - objectives.bounds[obj_index, 0]
-            )
+            predictor_params_dict = predictor_params_dict.get(self.name, self.default_params(X))
 
-        Y_new_points_stddev_sum = np.sum(Y_new_points_stddev, axis=1).reshape(-1, 1)
-        sorting_indices = Y_new_points_stddev_sum[:, -1].argsort()
+        # if self.objective.hyperopt_evals is None:
+        #     hyperopt_evals = 1
+        # else:
+        #     hyperopt_evals = self.objective.hyperopt_evals.get(self.name, 1)
+        if self.objective.hyperopt_evals is None:
+            hyperopt_evals = 15
+        else:
+            hyperopt_evals = self.objective.hyperopt_evals.get(f"{self.name}", 15)
 
-        X_new_points_sorted = X_new_points[sorting_indices][::-1]
+        def func(X: np.ndarray, Y: np.ndarray, model_params: Dict[str, Any]) -> Dict[str, Any]:
+            loss = self.non_cv_train_val_test(
+                X, Y, model_params, test_ratio=test_ratio, sort_before_split=sort_before_split, **kwargs
+            )
 
-        if variables.num_cat_var > 0:
-            X_new_points = variables.categorical_transform(X_new_points).astype("float")
-        X_new_points_norm_sorted = (
-            (X_new_points[sorting_indices][::-1] - np.array(variables.lower_bounds))
-            / (np.array(variables.upper_bounds) - np.array(variables.lower_bounds))
-        )[sorting_indices][::-1]
-        Y_new_points_sorted = Y_new_points[sorting_indices][::-1]
-        Y_new_points_stddev_sum_sorted = Y_new_points_stddev_sum[sorting_indices][::-1]
-
-        # 0 index for the highest uncertainty one at the top of the array
-        chosen_indices = [0]
-        # cosine similarity index of 1.0 for the highest uncertainty one at the top of the array
-        cosine_simularity_list = [1.0]
-        # Comparing the X_values for the highest uncertainty with every other entry down the sorted X_array
-        for index, x in enumerate(X_new_points_norm_sorted):
-            cosine_simularity_index = 1 - spatial.distance.cosine(X_new_points_norm_sorted[0], x)
-            # Only passes if the cosine similarity index of a given x row is greater than 0.1 different from all of the x's in the list
-            if all((((x - cosine_simularity_index) ** 2) ** 0.5) > 0.1 for x in cosine_simularity_list):
-                cosine_simularity_list.append(cosine_simularity_index)
-                chosen_indices.append(index)
-
-            if len(chosen_indices) == self.num_candidates:
-                break
-
-        selected_X = X_new_points_sorted[chosen_indices]
-        selected_Y = Y_new_points_sorted[chosen_indices].astype(np.float64)
-        total_Y_std = Y_new_points_stddev_sum_sorted[chosen_indices].astype(np.float64)
+            return {
+                "loss": loss,
+                "status": STATUS_OK,
+            }
+
+        trials = Trials()
+        model_params = fmin(
+            fn=partial(func, X, Y),
+            space=predictor_params_dict,
+            algo=tpe.suggest,
+            max_evals=hyperopt_evals,
+            trials=trials,
+        )
 
-        logger.info(f"Identified variables with the most uncertain output values")
+        model = self.new_instance(self.__class__, **kwargs)
+        model.fit(X, Y, test_ratio=test_ratio, **model_params, **kwargs)
 
-        return selected_X, selected_Y, total_Y_std
+        logger.info(f"Completed hyperparameter opt")
+        return model, model_params
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nemo-bo-0.1.8/nemo_bo/acquisition_functions/nsga_improvement/problem_wrapper.py` & `nemo-bo-0.1.9/nemo_bo/acquisition_functions/nsga_improvement/problem_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from dataclasses import dataclass
 from typing import Dict, List, Union
 
 import numpy as np
 from pymoo.core.problem import Problem
 
 from nemo_bo.opt.constraints import ConstraintsList
 from nemo_bo.opt.objectives import ObjectivesList
 from nemo_bo.opt.variables import VariablesList
 
 
-@dataclass
 class NSGAProblemWrapper(Problem):
     """
 
     Class for defining a problem for the minimise function in NSGA-based methods
 
     Parameters
     ----------
     xl: int | float | List[int | float]
-        Lower bounds for the variables for the NSGA algorithm. If integer, all lower bounds are equal to the integer value
+        Lower bounds for the variables for the NSGA algorithm. If integer, all lower bounds are equal to the integer
+        value
     xu: int | float | List[int | float]
-        Upper bounds for the variables for the NSGA algorithm. If integer, all upper bounds are equal to the integer value
+        Upper bounds for the variables for the NSGA algorithm. If integer, all upper bounds are equal to the integer
+        value
     variables: VariablesList
         VariablesList object that contains information about all variables
     objectives: ObjectivesList
         ObjectivesList object that contains information about all objectives
     constraints: ConstraintsList
         ConstraintsList object that contains information about all constraints
 
@@ -41,44 +41,52 @@
         self.variables = variables
         self.objectives = objectives
         self.constraints = constraints
 
         n_constr = self.constraints.n_constr if constraints is not None else 0
 
         super().__init__(
-            n_var=self.variables.n_var, n_obj=self.objectives.n_obj, n_constr=n_constr, xl=xl, xu=xu,
+            n_var=self.variables.n_var,
+            n_obj=self.objectives.n_obj,
+            n_constr=n_constr,
+            xl=xl,
+            xu=xu,
         )
 
     def _evaluate(self, X: np.ndarray, out: Dict[str, np.ndarray], **kwargs) -> None:
         """
 
         Function to calculate the objective(s) and constraint(s) (if any) values
 
         Parameters
         ----------
         X: np.ndarray
-            NSGA generated candidates' X-values
+            NSGA generated candidates' X-values, which are min-max normalised
         out: Dict[str, np.ndarray]
             Contains the objective(s) and constraint(s) (if any) values for the generated candidates
 
         """
+        # Un-transform the min-max normalised X array
         X = (X * (np.array(self.variables.upper_bounds) - np.array(self.variables.lower_bounds))) + np.array(
             self.variables.lower_bounds
         )
 
+        # Infer the objective values by drawing samples from the distribution at the X-values
         if self.variables.num_cat_descriptor_var > 0:
-            F, _ = self.objectives.evaluate(self.variables.descriptor_to_name(X))
+            F = self.objectives.draw_samples(self.variables.descriptor_to_name(X))
         else:
-            F, _ = self.objectives.evaluate(X)
+            F = self.objectives.draw_samples(X)
 
+        # * -1 for objectives that are maximising
         for obj_index, obj in enumerate(self.objectives.max_bool_dict):
             if self.objectives.max_bool_dict[obj]:
                 F[:, obj_index] *= -1
         out["F"] = F
 
+        # Evaluate the pymoo constraints
         if self.n_constr > 0:
             # Min-max normalises the X array
             X = (X - np.array(self.variables.lower_bounds)) / (
                 np.array(self.variables.upper_bounds) - np.array(self.variables.lower_bounds)
             )
             G = np.zeros((X.shape[0], self.n_constr))
             for index, constr in enumerate(self.constraints.constraints):
```

### Comparing `nemo-bo-0.1.8/nemo_bo/acquisition_functions/nsga_improvement/unsga3.py` & `nemo-bo-0.1.9/nemo_bo/acquisition_functions/nsga_improvement/unsga3.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # The NSGA-based methods were copied and adapted from J. Blank and K. Deb, pymoo: Multi-Objective Optimization in
 # Python, in IEEE Access, vol. 8, pp. 89497-89509, 2020, doi: 10.1109/ACCESS.2020.2990567
 # https://ieeexplore.ieee.org/document/9078759
 # https://github.com/anyoptimization/pymoo
-
 import numpy as np
-from pymoo.operators.selection.tournament import TournamentSelection, compare
+
+from pymoo.operators.selection.tournament import compare, TournamentSelection
 
 from nemo_bo.acquisition_functions.nsga_improvement.nsga3 import NSGA3
 
 
 # =========================================================================================================
 # Implementation
 # =========================================================================================================
@@ -18,28 +18,28 @@
     S = np.full(P.shape[0], np.nan)
 
     for i in range(P.shape[0]):
         a, b = P[i, 0], P[i, 1]
 
         # if at least one solution is infeasible
         if pop[a].CV > 0.0 or pop[b].CV > 0.0:
-            S[i] = compare(a, pop[a].CV, b, pop[b].CV, method="smaller_is_better", return_random_if_equal=True,)
+            S[i] = compare(a, pop[a].CV, b, pop[b].CV, method="smaller_is_better", return_random_if_equal=True)
 
         # both solutions are feasible
         else:
 
             # if in the same niche select by rank
             if pop[a].get("niche") == pop[b].get("niche"):
 
                 if pop[a].get("rank") != pop[b].get("rank"):
-                    S[i] = compare(a, pop[a].get("rank"), b, pop[b].get("rank"), method="smaller_is_better",)
+                    S[i] = compare(a, pop[a].get("rank"), b, pop[b].get("rank"), method="smaller_is_better")
 
                 else:
                     S[i] = compare(
-                        a, pop[a].get("dist_to_niche"), b, pop[b].get("dist_to_niche"), method="smaller_is_better",
+                        a, pop[a].get("dist_to_niche"), b, pop[b].get("dist_to_niche"), method="smaller_is_better"
                     )
 
         if np.isnan(S[i]):
             S[i] = np.random.choice([a, b])
 
     return S[:, None].astype(int)
```

### Comparing `nemo-bo-0.1.8/nemo_bo/models/base/available_models.py` & `nemo-bo-0.1.9/nemo_bo/models/base/available_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 def create_predictor_list(predictor_type: List[Union[str, Base_Model]]) -> List[Base_Model]:
     """
 
     Parameters
     ----------
     predictor_type: List[str | Base_Model]
         List of predictors to use defined by the user. It can contain strings which correspond to particular model
-        types that are built-in to NEMO, or can be any model inherits from the Base_Model class
+        types that are built-in to NEMO, or can be any model that inherits from the Base_Model class
 
     Returns
     -------
     List[str | Base_Model]
-        List of predictors which are all inherited from the Base_Model class
+        List of predictors which are all inherited the Base_Model class
 
     """
     if predictor_type is not None:
         if isinstance(predictor_type, list):
             predictor_type_list = []
             for predictor in predictor_type:
                 if isinstance(predictor, str):
@@ -42,21 +42,22 @@
                         predictor_type_list.append(XGBoostModel)
                     elif predictor == "ngb":
                         predictor_type_list.append(NGBoostModel)
                     elif predictor == "rf":
                         predictor_type_list.append(RFModel)
                     else:
                         raise ValueError(
-                            f'Predictor type "{predictor}" is not natively supported. Please provide the class of the external predictor that inherits from the Base_Model class'
+                            f'Predictor type "{predictor}" is not natively supported. Please provide the class of the '
+                            f"external predictor that inherits from the Base_Model class"
                         )
                 else:
                     if isinstance(predictor, Base_Model):
                         predictor_type_list.append(predictor)
                     else:
-                        raise ValueError(f'Predictor type "{predictor}" does not inherit from the Base_Model class')
+                        raise TypeError(f'Predictor type "{predictor}" does not inherit from the Base_Model class')
             return predictor_type_list
 
         elif isinstance(predictor_type, str):
             if predictor_type == "gp":
                 return [GPModel]
             elif predictor_type == "nn_concrete":
                 return [NNConcreteDropoutModel]
@@ -66,17 +67,18 @@
                 return [NNBayesianModel]
             elif predictor_type == "xgb":
                 return [XGBoostModel]
             elif predictor_type == "ngb":
                 return [NGBoostModel]
             elif predictor_type == "rf":
                 return [RFModel]
-            elif isinstance(predictor_type, Base_Model):
-                return [predictor_type]
             else:
                 raise ValueError(
-                    f'Predictor type "{predictor_type}" is not natively supported. Please provide the class of the external predictor that inherits from the Base_Model class'
+                    f'Predictor type "{predictor_type}" is not natively supported. Please provide the class of the '
+                    f"external predictor that inherits from the Base_Model class"
                 )
+        elif isinstance(predictor_type, Base_Model):
+            return [predictor_type]
         else:
-            raise TypeError(f'Please pass the predictor type "{predictor_type}" in a list or as a string')
+            raise TypeError(f'Predictor type "{predictor_type}" does not inherit from the Base_Model class')
     else:
         return [GPModel, NNConcreteDropoutModel, NNEnsembleModel, NNBayesianModel, XGBoostModel, NGBoostModel, RFModel]
```

### Comparing `nemo-bo-0.1.8/nemo_bo/models/base/base_model.py` & `nemo-bo-0.1.9/nemo_bo/models/base/base_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,31 +59,36 @@
         # Four variables that need to be pre-defined by the author in the child classes that inherit Base_Model:
         # The name given to the type of model
         self.name = None
 
         # Boolean for whether a validation set is used for the model fitting process
         self.include_validation = None
 
-        # The default X and Y transform types to use during the fit and predict processes when the
-        # transformation_type attributes in any self.variables.variables and/or self.objective are None
+        # The default X and Y transform types to use during the fit and predict processes when the transformer
+        # attributes in any self.variables.variables and/or self.objective are None
         self.default_X_transform_type = None
         self.default_Y_transform_type = None
 
     def new_instance(self, cls: Base_Model, **kwargs):
         """
 
         Returns a new instance of the model class that is passed into the function
 
         """
         return cls(
             copy.copy(self.input_variables), copy.copy(self.input_objective), self.always_hyperparam_opt, **kwargs
         )
 
     def fit(
-        self, X: np.ndarray, Y: np.ndarray, test_ratio: float = 0.2, sort_before_split: bool = True, **params,
+        self,
+        X: np.ndarray,
+        Y: np.ndarray,
+        test_ratio: float = 0.2,
+        sort_before_split: bool = True,
+        **params,
     ) -> None:
         """
 
         Function that is called to start the fitting procedure. For example, the typical order steps here could include
         firstly data transformations and splitting, followed by fitting the model using the self.fit_model function,
         and then testing the model quality
 
@@ -132,14 +137,32 @@
         X_transform: bool, Default = True
             For the default models provided natively in NEMO, the initial transformation of categorical variables and
             transformations related to standardisation/normalisation can be switched off by passing X_transform = False
 
         """
         pass
 
+    def draw_samples(self, X: np.ndarray, X_transform: bool = True) -> np.ndarray:
+        """
+
+        Generates samples from the distribution using the X array
+
+        Parameters
+        ----------
+        X: np.ndarray,
+            X array that contains the unprocessed variables data to be used in the prediction, i.e. The data has not
+            yet undergone any transformations related to converted categorical variables to their respective
+            descriptors or transformations related to standardisation/normalisation
+        X_transform: bool, Default = True
+            For the default models provided natively in NEMO, the initial transformation of categorical variables and
+            transformations related to standardisation/normalisation can be switched off by passing X_transform = False
+
+        """
+        pass
+
     def cv(
         self,
         X: np.ndarray,
         Y: np.ndarray,
         model_params: Dict[str, Any],
         test_ratio: float = 0.2,
         sort_before_split: bool = True,
@@ -190,16 +213,15 @@
 
         """
         pass
 
     def default_params(self, *args, **kwargs) -> Dict[str, Any]:
         """
 
-        Function that returns the default hyperparameters to use for the hyperparameter optimisation using the
-        hyperopt package. Returns a dictionary that is used for the space argument in the hyperopt.fmin function
+        Function that returns the default hyperparameters to use for the hyperparameter optimisation
 
         """
         pass
 
     def cv_train_test(
         self, X: np.ndarray, Y: np.ndarray, model_params: Dict[str, Any], test_ratio: float = 0.2, **kwargs
     ) -> Dict[str, Any]:
@@ -232,25 +254,19 @@
         self.model_params = model_params
 
         cv_results = {}
         test_rmse_list = []
         test_r2_list = []
         fold_number = 0
 
-        kf = KFold(n_splits=int(1 / test_ratio), shuffle=True, random_state=1)
-
-        # Split the data
         X_temp = copy.copy(X)
         Y_temp = copy.copy(Y)
 
-        # remainder = X.shape[0] % int(1 / test_ratio)
-        # if remainder > 0:
-        #     X_temp = X_temp[: (-1 * remainder)]
-        #     Y_temp = Y_temp[: (-1 * remainder)]
-
+        # Split the data
+        kf = KFold(n_splits=int(1 / test_ratio), shuffle=True, random_state=1)
         for train_index, test_index in kf.split(X_temp):
             fold_number += 1
             X_train, X_test = X_temp[train_index], X_temp[test_index]
             Y_train, Y_test = (
                 Y_temp[train_index].astype("float"),
                 Y_temp[test_index].astype("float"),
             )
@@ -288,15 +304,16 @@
             test_rmse_list.append(model.performance_metrics["Validation RMSE"])
             test_r2_list.append(model.performance_metrics["Validation r2"])
 
         cv_results["Mean Test RMSE"] = np.mean(test_rmse_list)
         cv_results["Mean Test r2"] = np.mean(test_r2_list)
 
         logger.info(
-            f"Completed {self.name} CV (k = {int(1/test_ratio)}) model checking | Mean Test Loss: {cv_results['Mean Test RMSE']}"
+            f"Completed {self.name} CV (k = {int(1/test_ratio)}) model checking | Mean Test Loss: "
+            f"{cv_results['Mean Test RMSE']}"
         )
 
         return cv_results
 
     def cv_train_val_test(
         self,
         X: np.ndarray,
@@ -340,24 +357,27 @@
         cv_results = {}
         test_rmse_list = []
         test_r2_list = []
         test_pred_list = []
         test_error_list = []
         fold_number = 0
 
-        kf = KFold(n_splits=int(1 / test_ratio), shuffle=True, random_state=1)
-
+        # Split the data
         if sort_before_split:
-            (X_train_val, X_test, Y_train_val, Y_test,) = sort_train_test_split_shuffle(
-                X, Y, test_ratio=test_ratio, seed=1
-            )
+            (
+                X_train_val,
+                X_test,
+                Y_train_val,
+                Y_test,
+            ) = sort_train_test_split_shuffle(X, Y, test_ratio=test_ratio, seed=1)
         else:
             X_train_val, X_test, Y_train_val, Y_test = train_test_split(X, Y, test_size=test_ratio, random_state=1)
         Y_test = Y_test.astype("float")
 
+        kf = KFold(n_splits=int(1 / test_ratio), shuffle=True, random_state=1)
         for train_index, test_index in kf.split(X_train_val):
             fold_number += 1
             X_train, X_val = X_train_val[train_index], X_train_val[test_index]
             Y_train, Y_val = (
                 Y_train_val[train_index].astype("float"),
                 Y_train_val[test_index].astype("float"),
             )
@@ -381,24 +401,32 @@
             else:
                 model.X_train = X_train
                 model.X_val = X_val
                 model.X_test = X_test
 
             model.X_train, model.Y_train = model.transform_by_predictor_type(model.X_train, model.Y_train)
             model.X_val, model.Y_val = model.transform_only_by_predictor_type(model.X_val, model.Y_val)
-            (model.X_test, model.Y_test,) = model.transform_only_by_predictor_type(model.X_test, model.Y_test)
+            (
+                model.X_test,
+                model.Y_test,
+            ) = model.transform_only_by_predictor_type(model.X_test, model.Y_test)
 
             model.fit_model(self.model_params)
 
             # Make predictions and calculate model performance
             model.Y_train_pred, model.Y_train_pred_stddev = model.predict(X_train)
             model.Y_val_pred, model.Y_val_pred_stddev = model.predict(X_val)
             model.Y_test_pred, model.Y_test_pred_stddev = model.predict(X_test)
             model.performance_metrics = pm.all_performance_metrics_train_val_test(
-                Y_train, model.Y_train_pred, Y_val, model.Y_val_pred, Y_test, model.Y_test_pred,
+                Y_train,
+                model.Y_train_pred,
+                Y_val,
+                model.Y_val_pred,
+                Y_test,
+                model.Y_test_pred,
             )
             model.Y_test_error = 1.96 * model.Y_test_pred_stddev
 
             cv_results[f"Fold {fold_number}"] = {
                 "Performance Metrics": model.performance_metrics,
                 "Model": model.model,
             }
@@ -409,15 +437,16 @@
 
         cv_results["Mean Test RMSE"] = np.mean(test_rmse_list)
         cv_results["Mean Test r2"] = np.mean(test_r2_list)
         cv_results["Mean Y Test Parity Data"] = pm.paritydata(Y_test, np.mean(test_pred_list, axis=0))
         cv_results["Mean Y Test Error (CI 95%)"] = np.mean(test_error_list, axis=0)
 
         logger.info(
-            f"Completed {self.name} CV (k = {int(1/test_ratio)}) model checking | Mean Test Loss: {cv_results['Mean Test RMSE']}"
+            f"Completed {self.name} CV (k = {int(1/test_ratio)}) model checking | Mean Test Loss: "
+            f"{cv_results['Mean Test RMSE']}"
         )
 
         return cv_results
 
     def non_cv_train_test(
         self,
         X: np.ndarray,
@@ -457,15 +486,20 @@
         The RMSE of the test set prediction
 
         """
         self.model_params = model_params
 
         # Split the dataset
         if sort_before_split:
-            (X_train, X_test, Y_train, Y_test,) = sort_train_test_split_shuffle(X, Y, test_ratio=test_ratio, seed=1)
+            (
+                X_train,
+                X_test,
+                Y_train,
+                Y_test,
+            ) = sort_train_test_split_shuffle(X, Y, test_ratio=test_ratio, seed=1)
         else:
             X_train, X_test, Y_train, Y_test = train_test_split(X, Y, test_size=test_ratio, random_state=1)
 
         # Create copy for the model
         model = self.new_instance(self.__class__, **kwargs)
 
         # Transform the data
@@ -487,14 +521,16 @@
         # Make predictions and calculate model performance
         model.Y_train_pred, model.Y_train_pred_stddev = model.predict(X_train)
         model.Y_test_pred, model.Y_test_pred_stddev = model.predict(X_test)
         model.performance_metrics = pm.all_performance_metrics_train_val(
             Y_train, model.Y_train_pred, Y_test, model.Y_test_pred
         )
 
+        logger.info(f"Completed model checking | Mean Test Loss: {model.performance_metrics['Test RMSE']}")
+
         return model.performance_metrics["Test RMSE"]
 
     def non_cv_train_val_test(
         self,
         X: np.ndarray,
         Y: np.ndarray,
         model_params: Dict[str, Any],
@@ -532,17 +568,22 @@
         The RMSE of the test set prediction
 
         """
         self.model_params = model_params
 
         # Split the dataset
         if sort_before_split:
-            (X_train, X_val, X_test, Y_train, Y_val, Y_test,) = sort_train_val_test_split_shuffle(
-                X, Y, test_ratio=test_ratio, seed=1
-            )
+            (
+                X_train,
+                X_val,
+                X_test,
+                Y_train,
+                Y_val,
+                Y_test,
+            ) = sort_train_val_test_split_shuffle(X, Y, test_ratio=test_ratio, seed=1)
         else:
             X_train_val, X_test, Y_train_val, Y_test = train_test_split(X, Y, test_size=test_ratio, random_state=1)
             X_train, X_val, Y_train, Y_val = train_test_split(
                 X_train_val, Y_train_val, test_size=test_ratio, random_state=1
             )
 
         # Create copy for the model
@@ -568,14 +609,16 @@
         model.Y_train_pred, model.Y_train_pred_stddev = model.predict(X_train)
         model.Y_val_pred, model.Y_val_pred_stddev = model.predict(X_val)
         model.Y_test_pred, model.Y_test_pred_stddev = model.predict(X_test)
         model.performance_metrics = pm.all_performance_metrics_train_val_test(
             Y_train, model.Y_train_pred, Y_val, model.Y_val_pred, Y_test, model.Y_test_pred
         )
 
+        logger.info(f"Completed model checking | Mean Test Loss: {model.performance_metrics['Test RMSE']}")
+
         return model.performance_metrics["Test RMSE"]
 
     def y_scrambling_cv(
         self,
         X: np.ndarray,
         Y: np.ndarray,
         model_params: Dict[str, Any],
@@ -623,19 +666,21 @@
 
         """
 
         dirname_y_scrambling = os.path.join(os.getcwd(), "ML Models", f"{self.name}", "Y-Scrambling")
         if not os.path.exists(dirname_y_scrambling):
             os.makedirs(dirname_y_scrambling)
 
+        # CV for non-y-scrambled data
         cv_results = self.cv(X, Y, model_params, test_ratio=test_ratio, sort_before_split=sort_before_split, **kwargs)
 
         np.random.seed(0)
         np.random.shuffle(Y)
 
+        # CV for y-scrambled data
         cv_results_y_scrambling = self.cv(
             X, Y, model_params, test_ratio=test_ratio, sort_before_split=sort_before_split, **kwargs
         )
 
         if plot_parity:
             # Produces a 2D scatter plot showing the parity plot data points, and the x = y line as a line plot
             original_paritydata = cv_results["Mean Y Test Parity Data"]
@@ -658,15 +703,20 @@
                 [min_parity, min_parity],
                 [max_parity, max_parity],
             ]
             scatter_legend = (
                 f"Original ({original_paritydata.shape[0]} Test Data Points)",
                 f"Y-Scrambling ({y_scrambling_paritydata.shape[0]} Test Data Points)",
             )
-            plot_title = f"Original and Y-Scrambling Test Data Parity Plot\nOriginal Test RMSE = {round(original_rmse.astype('float'), 2)}, Original Test r2 = {round(original_r2, 2)}\nY-Scrambling Test RMSE = {round(y_scrambling_rmse.astype('float'), 2)}, Y-Scrambling Test r2 = {round(y_scrambling_r2, 2)}"
+            plot_title = (
+                f"Original and Y-Scrambling Test Data Parity Plot\nOriginal Test RMSE = "
+                f"{round(original_rmse.astype('float'), 2)}, Original Test r2 = {round(original_r2, 2)}\n"
+                f"Y-Scrambling Test RMSE = {round(y_scrambling_rmse.astype('float'), 2)}, Y-Scrambling Test "
+                f"r2 = {round(y_scrambling_r2, 2)}"
+            )
             output_file = os.path.join(
                 dirname_y_scrambling,
                 f"Y-Scrambling Test Data Parity Plot, {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}",
             )
             if inc_error_bars:
                 plotter.plot(
                     plot_dim="2D",
@@ -692,88 +742,26 @@
                     ylabel=f"Predicted",
                     plottitle=plot_title,
                     output_file=output_file,
                 )
             plt.close()
 
         logger.info(
-            f"Completed Y-scrambling CV tests | Mean Test Loss: {cv_results['Mean Test RMSE']} | Y-scrambling Mean Test Loss: {cv_results_y_scrambling['Mean Test RMSE']}"
+            f"Completed Y-scrambling CV tests | Mean Test Loss: {cv_results['Mean Test RMSE']} | Y-scrambling Mean "
+            f"Test Loss: {cv_results_y_scrambling['Mean Test RMSE']}"
         )
 
         return cv_results, cv_results_y_scrambling
 
     def permutation_feature_importance(
-        self, X: np.ndarray, Y: np.ndarray, repeats: int = 50
-    ) -> Tuple[pd.Series, pd.Series]:
-        """
-
-        Provides a measure of the feature importance by shuffling (permuting) each feature individually to observe its
-        effect on the mean-square-error (MSE) of the prediction against the MSE calculated from an unaltered X array.
-        The permutation feature importance of categorical variables are returned per categorical variable instead of by
-        their respective descriptors
-
-        Parameters
-        ----------
+        self,
         X: np.ndarray,
-            X array that contains the unprocessed variables data to be fitted to the model, i.e. The data has not yet
-            undergone any transformations related to converted categorical variables to their respective descriptors
-            or transformations related to standardisation/normalisation
         Y: np.ndarray,
-            Y array that contains the unprocessed objective data, i.e. The data has not yet undergone any
-            transformations related to standardisation/normalisation
-        repeats: int, Default = 50
-            The number of times to shuffle (permute) each feature. The average MSE over all repeats is calculated
-
-        Returns
-        -------
-        feature_importance_mean: pd.Series
-            The normalised permutation feature importance over all repeats
-        feature_importance_stddev: pd.Series
-            The standard deviation of the MSE after shuffling each feature over all repeats
-
-        """
-        logger.info(f"Performing permutation feature importance calculation for {self.name} model")
-
-        Y_pred_base, _ = self.predict(X)
-        mse_score_base = mean_squared_error(Y, Y_pred_base)
-
-        results = []
-        for i in range(X.shape[1]):
-            temp_i_store = copy.copy(X[:, i])
-
-            mse_score_i_shuffled_list = []
-            for repeat in range(repeats):
-                np.random.shuffle(X[:, i])
-                Y_pred_i_shuffled, _ = self.predict(X)
-                mse_score_i_shuffled = mean_squared_error(Y, Y_pred_i_shuffled)
-                mse_score_i_shuffled_list.append(mse_score_i_shuffled)
-                if repeat % 10 == 0:
-                    print(
-                        f"Variable {i + 1}, Repeat {repeat + 1}, Permutation MSE: {mse_score_i_shuffled}, Difference to Base MSE: {mse_score_i_shuffled - mse_score_base}"
-                    )
-            X[:, i] = copy.copy(temp_i_store)
-            results.append(np.array(mse_score_i_shuffled_list))
-
-        results = np.array(results).T
-        results_diff = results - mse_score_base
-        feature_importance_mean = np.mean(results_diff, axis=0)
-        feature_importance_mean = feature_importance_mean / np.sum(feature_importance_mean)
-        feature_importance_stddev = np.std(results_diff, axis=0)
-
-        feature_importance_mean = pd.Series(feature_importance_mean, index=self.variables.names)
-        feature_importance_stddev = pd.Series(feature_importance_stddev, index=self.variables.names)
-
-        print(f"Permutation feature importance: {np.around(feature_importance_mean, decimals=3)}")
-
-        logger.info(f"Completed permutation feature importance calculation")
-
-        return feature_importance_mean, feature_importance_stddev
-
-    def permutation_feature_importance_continuous(
-        self, X: np.ndarray, Y: np.ndarray, repeats: int = 50
+        repeats: int = 50,
+        transform_cat_to_cont=True,
     ) -> Tuple[pd.Series, pd.Series]:
         """
 
         Provides a measure of the feature importance by shuffling (permuting) each feature individually to observe its
         effect on the mean-square-error (MSE) of the prediction against the MSE calculated from an unaltered X array.
         The permutation feature importance of categorical variables are returned as their respective descriptors
 
@@ -784,14 +772,18 @@
             undergone any transformations related to converted categorical variables to their respective descriptors
             or transformations related to standardisation/normalisation
         Y: np.ndarray,
             Y array that contains the unprocessed objective data, i.e. The data has not yet undergone any
             transformations related to standardisation/normalisation
         repeats: int, Default = 50
             The number of times to shuffle (permute) each feature. The average MSE over all repeats is calculated
+        transform_cat_to_cont: bool, Default = True
+            If True, the permutation feature importance will be calculated for every descriptor of the
+            CategoricalVariableWithDescriptors variables. When False, the permutation feature importance will be
+            calculated for the categorical level directly
 
         Returns
         -------
         feature_importance_mean: pd.Series
             The normalised permutation feature importance over all repeats
         feature_importance_stddev: pd.Series
             The standard deviation of the MSE after shuffling each feature over all repeats
@@ -799,47 +791,62 @@
         """
         logger.info(f"Performing permutation feature importance calculation for {self.name} model")
 
         Y_pred_base, _ = self.predict(X)
         mse_score_base = mean_squared_error(Y, Y_pred_base)
 
         # Convert categorical variables names to descriptors
-        if self.variables.num_cat_var > 0:
+        if self.variables.num_cat_var > 0 and transform_cat_to_cont:
             X = self.variables.categorical_transform(X)
 
-        # Transform the continuous variables and descriptors
-        X = self.transform_only_by_predictor_type(X)
+            # Transform the continuous variables and descriptors
+            X = self.transform_only_by_predictor_type(X)
 
         results = []
         for i in range(X.shape[1]):
             temp_i_store = copy.copy(X[:, i])
 
             mse_score_i_shuffled_list = []
             for repeat in range(repeats):
                 np.random.shuffle(X[:, i])
 
-                Y_pred_i_shuffled, _ = self.predict(X, X_transform=False)
+                Y_pred_i_shuffled, _ = (
+                    self.predict(X, X_transform=False)
+                    if (self.variables.num_cat_var > 0 and transform_cat_to_cont)
+                    else self.predict(X, X_transform=True)
+                )
 
                 mse_score_i_shuffled = mean_squared_error(Y, Y_pred_i_shuffled.flatten())
                 mse_score_i_shuffled_list.append(mse_score_i_shuffled)
-                if repeat % 10 == 0:
-                    print(
-                        f"Variable {i + 1}, Repeat {repeat + 1}, Permutation MSE: {mse_score_i_shuffled}, Difference to Base MSE: {mse_score_i_shuffled - mse_score_base}"
-                    )
+                # if repeat % 10 == 0:
+                # print(
+                #     f"Variable {i + 1}, Repeat {repeat + 1}, Permutation MSE: {mse_score_i_shuffled}, Difference "
+                #     f"to Base MSE: {mse_score_i_shuffled - mse_score_base}"
+                # )
             X[:, i] = copy.copy(temp_i_store)
             results.append(np.array(mse_score_i_shuffled_list))
 
         results = np.array(results).T
         results_diff = results - mse_score_base
         feature_importance_mean = np.mean(results_diff, axis=0)
         feature_importance_mean = feature_importance_mean / np.sum(feature_importance_mean)
         feature_importance_stddev = np.std(results_diff, axis=0)
 
-        feature_importance_mean = pd.Series(feature_importance_mean, index=self.variables.continuous_var_names)
-        feature_importance_stddev = pd.Series(feature_importance_stddev, index=self.variables.continuous_var_names)
+        feature_importance_mean = pd.Series(
+            feature_importance_mean,
+            index=self.variables.continuous_var_names
+            if (self.variables.num_cat_var > 0 and transform_cat_to_cont)
+            else self.variables.names,
+        )
+        feature_importance_stddev = pd.Series(
+            feature_importance_stddev,
+            index=self.variables.continuous_var_names
+            if (self.variables.num_cat_var > 0 and transform_cat_to_cont)
+            else self.variables.names,
+        )
 
         print(f"Permutation feature importance:\n{np.around(feature_importance_mean, decimals=3)}")
 
         logger.info(f"Completed permutation feature importance calculation")
 
         return feature_importance_mean, feature_importance_stddev
 
@@ -880,28 +887,38 @@
                 X_copy[:, index] = value
 
                 Y_pred, _ = self.predict(X_copy, X_transform=False)
                 Y_pred_pdp.append([value, Y_pred.mean()])
 
             Y_pred_pdp_np = np.array(Y_pred_pdp)
             pdp_dict[self.variables.continuous_var_names[index]] = pd.DataFrame(
-                Y_pred_pdp_np, columns=[f"{self.variables.continuous_var_names[index]}", f"{self.objective.name}",],
+                Y_pred_pdp_np,
+                columns=[
+                    f"{self.variables.continuous_var_names[index]}",
+                    f"{self.objective.name}",
+                ],
             )
             X_copy[:, index] = col
 
             plotter.plot(
                 plot_dim="2D",
                 scatter_data=Y_pred_pdp_np,
                 scatter_legend=f"Number of Grid Points = {Y_pred_pdp_np.shape[0]}",
-                xlabel=f"{self.variables.continuous_var_names[index]}",
-                ylabel=f"{self.objective.name} ({self.objective.units})",
-                plottitle=f"Partial Dependence Plot for {self.objective.name} against {self.variables.continuous_var_names[index]}",
+                xlabel=f"{self.variables.continuous_var_names[index]} ({self.variables.cont_var_units[index]})"
+                if self.variables.cont_var_units[index] != ""
+                else f"{self.variables.continuous_var_names[index]}",
+                ylabel=f"{self.objective.name} ({self.objective.units})"
+                if self.objective.units != ""
+                else f"{self.objective.names}",
+                plottitle=f"Partial Dependence Plot for {self.objective.name} against "
+                f"{self.variables.continuous_var_names[index]}",
                 output_file=os.path.join(
                     path,
-                    rf"Partial Dependence Plot for {self.objective.name} against {self.variables.continuous_var_names[index]}, {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}",
+                    rf"Partial Dependence Plot for {self.objective.name} against "
+                    rf"{self.variables.continuous_var_names[index]}, {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}",
                 ),
             )
             plt.close("all")
 
         logger.info(f"Completed partial dependence plot calculations")
 
         return pdp_dict
@@ -922,16 +939,16 @@
             Y array that contains the unprocessed objective dataready for transformations related to
             standardisation/normalisation
 
         """
         X = self.variables.transform(X, self.default_X_transform_type)
 
         if Y is not None:
-            if self.objective.transformation_type is None:
-                self.objective.transformation_type = self.default_Y_transform_type
+            if self.objective.transformer is None:
+                self.objective.transformer = self.default_Y_transform_type
             Y = self.objective.transform(Y)
             return X.astype("float"), Y.astype("float")
         else:
             return X.astype("float")
 
     def transform_only_by_predictor_type(
         self, X: np.ndarray, Y: Optional[np.ndarray] = None
```

### Comparing `nemo-bo-0.1.8/nemo_bo/models/base/nn_save_checkpoint.py` & `nemo-bo-0.1.9/nemo_bo/models/base/nn_save_checkpoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 from keras.models import Model
 
 
 class SaveModelCheckPoint:
     """
 
-    Class that enables tensorflow neural network model saving based on both the train loss and validation loss values
+    Class that enables saving of tensorflow neural network models based on both the train loss and validation loss
+    values
 
     Parameters
     ----------
     model : KerasRegressor type object that contains the neural network being trained
     filepath : str type of the file path to save the .h5 file that stores the model parameters
 
     """
@@ -21,15 +22,15 @@
         self.filepath = filepath
         self.reset()
 
     def reset(self) -> None:
         """
 
         Function to reset the values that are monitored during the checkpointing process. This function can be called
-        at the end of model training to allow multiple models to be trained using the same class instantiation of
+        at the end of model training to allow multiple models to be trained using the same class instance of
         SaveModelCheckPoint. An example use-case would be during cross validation
 
         """
         self.best_epoch = 0
         self.best_loss = sys.float_info.max
         self.best_val_loss = sys.float_info.max
 
@@ -58,19 +59,19 @@
                 except OSError as e:
                     print(e)
 
         elif loss < self.best_loss and val_loss < self.best_val_loss:
             self.best_loss = loss
             self.best_val_loss = val_loss
             self.best_epoch = epoch
-            print(
-                f"This epoch's loss ({loss}) and validation loss ({val_loss}) are both the best so far. Saving the model weights.\n"
-            )
+            # print(
+            #     f"This epoch's loss ({loss}) and validation loss ({val_loss}) are both the best so far. Saving the "
+            #     f"model weights.\n"
+            # )
             for _ in range(10):
                 try:
                     self.model.save_weights(self.filepath)
                     break
                 except OSError as e:
                     print(e)
-
-        else:
-            print(f"Number of epochs since the weights were last saved = {epoch - self.best_epoch}.\n")
+        # else:
+        #     print(f"Number of epochs since the weights were last saved = {epoch - self.best_epoch}.\n")
```

### Comparing `nemo-bo-0.1.8/nemo_bo/models/gp.py` & `nemo-bo-0.1.9/nemo_bo/models/gp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+# Utilises the BoToroch package for creating GP models
+# M. Balandat, B. Karrer, D. R. Jiang, S. Daulton, B. Letham, A. G. Wilson, and E. Bakshy. BoTorch: A Framework for
+# Efficient Monte-Carlo Bayesian Optimization. Advances in Neural Information Processing Systems 33, 2020.
+# http://arxiv.org/abs/1910.06403
+# https://github.com/pytorch/botorch
+# https://botorch.org/
+
 from __future__ import annotations
 
 import copy
 import os
-from functools import partial
+import time
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple
 
-import gpytorch
 import numpy as np
 import torch
 from botorch.models import SingleTaskGP
 from botorch.fit import fit_gpytorch_model
 from gpytorch.mlls import ExactMarginalLogLikelihood
 from gpytorch.distributions import MultivariateNormal
 from gpytorch.kernels import AdditiveStructureKernel, Kernel, MaternKernel, ScaleKernel
-from gpytorch.likelihoods import GaussianLikelihood, Likelihood
+from gpytorch.likelihoods import Likelihood
 from gpytorch.means import ConstantMean
 from gpytorch.models import ExactGP
 from gpytorch.priors.torch_priors import GammaPrior
-from hyperopt import STATUS_OK, Trials, fmin, hp, tpe
-from hyperopt.pyll.base import Literal
 from torch import Tensor
 
 import nemo_bo.utils.logger as logging_nemo
 import nemo_bo.utils.perf_metrics as pm
 from nemo_bo.models.base.base_model import Base_Model
 
 if TYPE_CHECKING:
@@ -108,16 +112,22 @@
     def fit_model(self, params: Dict[str, Any]) -> None:
         """
 
         Called by the fit and cv-related functions for fitting the GP model using pre-processed X and Y training data
         in the class instance
 
         """
-        X_tensor = torch.tensor(self.X_train, device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu"),)
-        Y_tensor = torch.tensor(self.Y_train, device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu"),)
+        X_tensor = torch.tensor(
+            self.X_train,
+            device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu"),
+        )
+        Y_tensor = torch.tensor(
+            self.Y_train,
+            device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu"),
+        )
         if Y_tensor.ndim == 1:
             Y_tensor = Y_tensor.reshape(-1, 1)
 
         self.n_iterations = int(params.get("n_iterations", 50))
         self.kernel = params.get(
             "kernel",
             ScaleKernel(
@@ -127,15 +137,19 @@
         )
 
         self.model = SingleTaskGP(X_tensor, Y_tensor, covar_module=copy.deepcopy(self.kernel))
         if torch.cuda.is_available():
             self.model = self.model.to("cuda")
 
         mll = ExactMarginalLogLikelihood(self.model.likelihood, self.model)
-        fit_gpytorch_model(mll)
+        for _ in range(5):
+            try:
+                fit_gpytorch_model(mll)
+            except AttributeError as e:
+                print(e)
 
     def predict(self, X: np.ndarray, X_transform: bool = True) -> Tuple[np.ndarray, np.ndarray]:
         """
 
         Determines the model output and its standard deviation of the X array passed into the function
 
         Parameters
@@ -165,23 +179,26 @@
         if X_transform:
             if self.variables.num_cat_var > 0:
                 X = self.variables.categorical_transform(X).astype("float")
             X = self.transform_only_by_predictor_type(X)
 
         # Split to reduce memory requirements. I think this is not ideal for the quality of the prediction but it helps
         # to prevent crashing caused by memory limitations when the X array is too large
-        split_size = 50000
+        split_size = 32000
         X_split = np.split(X, np.array((range(1, int(X.shape[0] / split_size) + 1))) * split_size)
         observed_Y_pred_list = []
         for X_split_each in X_split:
             if X_split_each.shape[0] == 0:
                 continue
             with torch.no_grad():
                 observed_Y_pred = self.model.posterior(
-                    torch.tensor(X_split_each, device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu"),)
+                    torch.tensor(
+                        X_split_each,
+                        device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu"),
+                    )
                 )
 
             observed_Y_pred_list.append(observed_Y_pred)
 
         Y_pred = np.vstack([observed_Y_pred.mean.cpu().detach().numpy() for observed_Y_pred in observed_Y_pred_list])
         Y_pred_upper = np.hstack(
             [
@@ -193,14 +210,68 @@
 
         Y_pred = self.objective.inverse_transform(Y_pred)
         Y_pred_upper = self.objective.inverse_transform(Y_pred_upper)
         Y_pred_stddev = (np.subtract(Y_pred_upper, Y_pred)) / 1.96
 
         return Y_pred.flatten(), Y_pred_stddev.flatten()
 
+    def draw_samples(self, X: np.ndarray, X_transform: bool = True) -> np.ndarray:
+        """
+
+        Generates samples from the distribution using the X array
+
+        Parameters
+        ----------
+        X: np.ndarray,
+            X array that contains the unprocessed variables data to be used in the prediction, i.e. The data has not
+            yet undergone any transformations related to converted categorical variables to their respective
+            descriptors or transformations related to standardisation/normalisation
+        X_transform: bool, Default = True
+            For the default models provided natively in NEMO, the initial transformation of categorical variables and
+            transformations related to standardisation/normalisation can be switched off by passing X_transform = False
+
+        Returns
+        ----------
+        Y_samples: np.ndarray
+            Drawn samples of the objective using the model and the inputted X array. The outputted values have been
+            un-transformed
+
+        """
+        # X needs to be a 2D array
+        if X.ndim == 1:
+            X = X.reshape(1, -1)
+
+        if X_transform:
+            if self.variables.num_cat_var > 0:
+                X = self.variables.categorical_transform(X).astype("float")
+            X = self.transform_only_by_predictor_type(X)
+
+        # Split to reduce memory requirements. I think this is not ideal for the quality of the prediction but it helps
+        # to prevent crashing caused by memory limitations when the X array is too large
+        split_size = 50000
+        X_split = np.split(X, np.array((range(1, int(X.shape[0] / split_size) + 1))) * split_size)
+        observed_Y_pred_list = []
+        for X_split_each in X_split:
+            if X_split_each.shape[0] == 0:
+                continue
+            with torch.no_grad():
+                observed_Y_pred = self.model.posterior(
+                    torch.tensor(
+                        X_split_each,
+                        device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu"),
+                    )
+                )
+            observed_Y_pred_list.append(observed_Y_pred)
+        Y_pred = np.vstack(
+            [observed_Y_pred.sample().cpu().detach().numpy()[0] for observed_Y_pred in observed_Y_pred_list]
+        )
+        Y_samples = self.objective.inverse_transform(Y_pred)
+
+        return Y_samples.flatten()
+
     @staticmethod
     def default_params(n_var: int, gp_kernel_choices: Optional[List[Kernel]] = None) -> Dict[str, Any]:
         """
 
         Function that returns the default kernels to use for the optimisation of GP models
 
         Parameters
@@ -298,27 +369,31 @@
                 self.name, self.default_params(self.variables.n_var, gp_kernel_choices)
             )
 
         test_rmse_list = []
         kernel_list = []
         best_loss = None
         for index, kernel in enumerate(predictor_params_dict["kernel"]):
+            start_time = time.perf_counter()
+
             cv_results = self.cv(X, Y, {"kernel": kernel}, test_ratio=test_ratio, **kwargs)
 
             test_rmse_list.append(cv_results["Mean Test RMSE"])
             kernel_list.append(kernel)
 
             if best_loss is None:
                 best_loss = cv_results["Mean Test RMSE"]
             else:
                 if cv_results["Mean Test RMSE"] < best_loss:
                     best_loss = cv_results["Mean Test RMSE"]
 
             print(
-                f'{index + 1}/{len(predictor_params_dict["kernel"])}, current loss: {cv_results["Mean Test RMSE"]}, best loss: {best_loss}'
+                f'{index + 1}/{len(predictor_params_dict["kernel"])}, iteration time (s) = '
+                f'{time.perf_counter() - start_time:>4.2f}, current loss: {cv_results["Mean Test RMSE"]}, best loss: '
+                f"{best_loss}"
             )
 
         best_kernel_index = test_rmse_list.index(min(test_rmse_list))
         model_params = {"kernel": kernel_list[best_kernel_index]}
 
         model = self.new_instance(self.__class__, **kwargs)
         model.fit(X, Y, test_ratio=test_ratio, **model_params, **kwargs)
```

### Comparing `nemo-bo-0.1.8/nemo_bo/models/gp_gpytorch.py` & `nemo-bo-0.1.9/nemo_bo/models/gp_gpytorch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# Utilises the GPyTorch package for creating GP models
+# Gardner, Jacob R., Geoff Pleiss, David Bindel, Kilian Q. Weinberger, and Andrew Gordon Wilson. "GPyTorch: Blackbox
+# Matrix-Matrix Gaussian Process Inference with GPU Acceleration." In Advances in Neural Information Processing
+# Systems (2018)
+# https://arxiv.org/abs/1809.11165
+# https://github.com/cornellius-gp/gpytorch
+# https://https://gpytorch.ai/
+
 from __future__ import annotations
 
 import copy
 import os
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple
 
@@ -104,17 +112,21 @@
     def fit_model(self, params: Dict[str, Any]) -> None:
         """
 
         Called by the fit and cv-related functions for fitting the GP model using pre-processed X and Y training data
         in the class instance
 
         """
-        X_tensor = torch.tensor(self.X_train, device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu"),)
+        X_tensor = torch.tensor(
+            self.X_train,
+            device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu"),
+        )
         Y_tensor = torch.tensor(
-            self.Y_train, device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu"),
+            self.Y_train,
+            device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu"),
         ).flatten()
 
         self.n_iterations = int(params.get("n_iterations", 50))
         self.kernel = params.get("kernel", ScaleKernel(MaternKernel(nu=2.5)))
 
         self.likelihood = GaussianLikelihood()
         self.model = ExactGPModel(X_tensor, Y_tensor, self.likelihood, copy.deepcopy(self.kernel))
@@ -181,15 +193,16 @@
         for X_split_each in X_split:
             if X_split_each.shape[0] == 0:
                 continue
             with torch.no_grad():
                 observed_Y_pred = self.likelihood(
                     self.model(
                         torch.tensor(
-                            X_split_each, device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu"),
+                            X_split_each,
+                            device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu"),
                         )
                     )
                 )
             observed_Y_pred_list.append(observed_Y_pred)
 
         Y_pred = np.hstack([observed_Y_pred.mean.cpu().detach().numpy() for observed_Y_pred in observed_Y_pred_list])
         Y_pred_upper = np.hstack(
@@ -217,21 +230,24 @@
         gp_kernel_choices: List[Kernel], Default = None
             The types of kernels to use for the GP hyperparameter optimisation
 
         """
         if gp_kernel_choices is None:
             gp_kernel_choices = [
                 AdditiveStructureKernel(
-                    base_kernel=ScaleKernel(MaternKernel(ard_num_dims=n_var, nu=0.5)), num_dims=n_var,
+                    base_kernel=ScaleKernel(MaternKernel(ard_num_dims=n_var, nu=0.5)),
+                    num_dims=n_var,
                 ),
                 AdditiveStructureKernel(
-                    base_kernel=ScaleKernel(MaternKernel(ard_num_dims=n_var, nu=1.5)), num_dims=n_var,
+                    base_kernel=ScaleKernel(MaternKernel(ard_num_dims=n_var, nu=1.5)),
+                    num_dims=n_var,
                 ),
                 AdditiveStructureKernel(
-                    base_kernel=ScaleKernel(MaternKernel(ard_num_dims=n_var, nu=2.5)), num_dims=n_var,
+                    base_kernel=ScaleKernel(MaternKernel(ard_num_dims=n_var, nu=2.5)),
+                    num_dims=n_var,
                 ),
                 ScaleKernel(MaternKernel(nu=0.5, ard_num_dims=n_var)),
                 ScaleKernel(MaternKernel(nu=1.5, ard_num_dims=n_var)),
                 ScaleKernel(MaternKernel(nu=2.5, ard_num_dims=n_var)),
             ]
         return {
             "n_iterations": hp.quniform("n_iterations", 5, 500, 1),
@@ -282,21 +298,17 @@
             predictor_params_dict = self.default_params(self.variables.n_var, gp_kernel_choices)
         else:
             predictor_params_dict = predictor_params_dict.get(
                 self.name, self.default_params(self.variables.n_var, gp_kernel_choices)
             )
 
         if self.objective.hyperopt_evals is None:
-            hyperopt_evals = 1
+            hyperopt_evals = 40
         else:
-            hyperopt_evals = self.objective.hyperopt_evals.get(self.name, 1)
-        # if self.objective.hyperopt_evals is None:
-        #     hyperopt_evals = 40
-        # else:
-        #     hyperopt_evals = self.objective.hyperopt_evals.get(f"{self.name}", 40)
+            hyperopt_evals = self.objective.hyperopt_evals.get(f"{self.name}", 40)
 
         def func(X: np.ndarray, Y: np.ndarray, model_params: Dict[str, Any]) -> Dict[str, Any]:
             cv_results = self.cv(X, Y, model_params, test_ratio=test_ratio, **kwargs)
 
             return {
                 "loss": cv_results["Mean Test RMSE"],
                 "status": STATUS_OK,
```

### Comparing `nemo-bo-0.1.8/nemo_bo/models/ngb.py` & `nemo-bo-0.1.9/nemo_bo/models/ngb.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Tony Duan, Anand Avati, Daisy Yi Ding, Khanh K. Thai, Sanjay Basu, Andrew Y. Ng, Alejandro Schuler. 2019. NGBoost: Natural Gradient Boosting for Probabilistic Prediction.
+# Tony Duan, Anand Avati, Daisy Yi Ding, Khanh K. Thai, Sanjay Basu, Andrew Y. Ng, Alejandro Schuler. 2019. NGBoost:
+# Natural Gradient Boosting for Probabilistic Prediction.
 # https://arxiv.org/abs/1910.03225
 # https://github.com/stanfordmlgroup/ngboost
 
 from __future__ import annotations
 
 import os
 from functools import partial
@@ -73,15 +74,20 @@
             Whether the inputted X and Y arrays should be sorted such that the Y-values are in ascending order before
             splitting into the training and test sets (and validation sets if applicable)
         params: Dict[str, Any]
             Dictionary that contains the hyperparameters for the model
 
         """
         if sort_before_split:
-            (X_train, X_val, Y_train, Y_val,) = sort_train_test_split_shuffle(X, Y, test_ratio=test_ratio, seed=1)
+            (
+                X_train,
+                X_val,
+                Y_train,
+                Y_val,
+            ) = sort_train_test_split_shuffle(X, Y, test_ratio=test_ratio, seed=1)
         else:
             X_train, X_val, Y_train, Y_val = train_test_split(X, Y, test_size=test_ratio, random_state=1)
 
         Y_train = Y_train.astype("float")
         Y_val = Y_val.astype("float")
 
         self.X_train, self.X_val, self.Y_train, self.Y_val = (
@@ -198,15 +204,41 @@
         Y_mean = Y_pred.loc
         Y_pred_upper = Y_mean + (1.96 * Y_pred.scale)
 
         Y_pred = self.objective.inverse_transform(Y_mean)
         Y_pred_upper = self.objective.inverse_transform(Y_pred_upper)
         Y_pred_stddev = (np.subtract(Y_pred_upper, Y_pred)) / 1.96
 
-        return Y_mean.flatten(), Y_pred_stddev.flatten()
+        return Y_pred.flatten(), Y_pred_stddev.flatten()
+
+    def draw_samples(self, X: np.ndarray, X_transform: bool = True) -> np.ndarray:
+        """
+
+        Generates samples from a normal distribution using the X array
+
+        Parameters
+        ----------
+        X: np.ndarray,
+            X array that contains the unprocessed variables data to be used in the prediction, i.e. The data has not
+            yet undergone any transformations related to converted categorical variables to their respective
+            descriptors or transformations related to standardisation/normalisation
+        X_transform: bool, Default = True
+            For the default models provided natively in NEMO, the initial transformation of categorical variables and
+            transformations related to standardisation/normalisation can be switched off by passing X_transform = False
+
+        Returns
+        ----------
+        np.ndarray
+            Drawn samples of the objective using the model and the inputted X array. The outputted values have been
+            un-transformed
+
+        """
+        Y_pred, Y_pred_stddev = self.predict(X, X_transform=X_transform)
+
+        return np.random.default_rng().normal(Y_pred, Y_pred_stddev)
 
     @staticmethod
     def default_params():
         """
 
         Function that returns the default hyperparameters to use for the hyperparameter optimisation of NGBoost models
         using the hyperopt package. Returns a dictionary that is used for the space argument in the hyperopt.fmin
@@ -262,22 +294,22 @@
 
         """
         if predictor_params_dict is None:
             predictor_params_dict = self.default_params()
         else:
             predictor_params_dict = predictor_params_dict.get(self.name, self.default_params())
 
-        if self.objective.hyperopt_evals is None:
-            hyperopt_evals = 1
-        else:
-            hyperopt_evals = self.objective.hyperopt_evals.get(self.name, 1)
         # if self.objective.hyperopt_evals is None:
-        #     hyperopt_evals = 30
+        #     hyperopt_evals = 1
         # else:
-        #     hyperopt_evals = self.objective.hyperopt_evals.get(f"{self.name}", 30)
+        #     hyperopt_evals = self.objective.hyperopt_evals.get(self.name, 1)
+        if self.objective.hyperopt_evals is None:
+            hyperopt_evals = 30
+        else:
+            hyperopt_evals = self.objective.hyperopt_evals.get(f"{self.name}", 30)
 
         def func(X: np.ndarray, Y: np.ndarray, model_params: Dict[str, Any]) -> Dict[str, Any]:
             cv_results = self.cv(
                 X, Y, model_params, test_ratio=test_ratio, sort_before_split=sort_before_split, **kwargs
             )
 
             return {
```

### Comparing `nemo-bo-0.1.8/nemo_bo/models/nn_bayesian.py` & `nemo-bo-0.1.9/nemo_bo/models/nn_concrete.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import math
 import os
 from datetime import datetime
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple
 
 import numpy as np
-import six
 import tensorflow as tf
 import tensorflow_probability as tfp
 from hyperopt import STATUS_OK, Trials, fmin, hp, tpe
 from hyperopt.pyll.base import scope
 from keras import backend as K
 from keras import callbacks
-from keras.layers import Dropout, Input
+from keras.layers import Dense, Input, InputSpec, Wrapper, concatenate
 from keras.models import Model
 from keras.optimizers import Optimizer
 from sklearn.model_selection import train_test_split
 from tensorflow import keras
-from tensorflow_probability.python.internal import tensorshape_util
+
+tf.keras.backend.set_floatx("float64")
 
 import nemo_bo.utils.logger as logging_nemo
 import nemo_bo.utils.perf_metrics as pm
 from nemo_bo.models.base.base_model import Base_Model
 from nemo_bo.models.base.nn_save_checkpoint import SaveModelCheckPoint
 from nemo_bo.utils.data_proc import sort_train_test_split_shuffle
 
@@ -49,45 +49,108 @@
             tf.config.experimental.set_memory_growth(gpu, True)
         logical_gpus = tf.config.list_logical_devices("GPU")
         print(len(gpus), "Physical GPUs,", len(logical_gpus), "Logical GPUs")
     except RuntimeError as e:
         print(e)
 
 
-class MeanMetricWrapper(tf.keras.metrics.Mean):
+class ConcreteDropout(Wrapper):
     """
 
-    Code by @mcourteaux from https://github.com/tensorflow/probability/issues/742#issuecomment-580433644
-    João Caldeira, Brian Nord, Deeply Uncertain: Comparing Methods of Uncertainty Quantification in Deep Learning Algorithms,
-    https://arxiv.org/abs/2004.10710
-    https://github.com/deepskies/DeeplyUncertain-Public
+    Code copied from:
+    João Caldeira, Brian Nord, Deeply Uncertain: Comparing Methods of Uncertainty Quantification in Deep Learning
+    Algorithms, arXiv:2004.10710, https://github.com/deepskies/DeeplyUncertain-Public
 
     """
 
-    def __init__(self, fn, name=None, dtype=None, **kwargs):
-        super(MeanMetricWrapper, self).__init__(name=name, dtype=dtype)
-        self._fn = fn
-        self._fn_kwargs = kwargs
-
-    def update_state(self, y_true, y_pred, sample_weight=None):
-        matches = self._fn(y_true, y_pred, **self._fn_kwargs)
-        return super(MeanMetricWrapper, self).update_state(matches, sample_weight=sample_weight)
-
-    def get_config(self):
-        config = {}
-        for k, v in six.iteritems(self._fn_kwargs):
-            config[k] = K.eval(v) if tensorshape_util.is_tensor_or_variable(v) else v
-        base_config = super(MeanMetricWrapper, self).get_config()
-        return dict(list(base_config.items()) + list(config.items()))
+    def __init__(
+        self,
+        layer,
+        weight_regularizer=0,
+        dropout_regularizer=1e-5,
+        init_min=0.1,
+        init_max=0.1,
+        is_mc_dropout=True,
+        **kwargs,
+    ):
+        assert "kernel_regularizer" not in kwargs
+        super(ConcreteDropout, self).__init__(layer, **kwargs)
+        self.weight_regularizer = weight_regularizer
+        self.dropout_regularizer = dropout_regularizer
+        self.is_mc_dropout = is_mc_dropout
+        self.supports_masking = True
+        self.p_logit = None
+        self.init_min = np.log(init_min) - np.log(1.0 - init_min)
+        self.init_max = np.log(init_max) - np.log(1.0 - init_max)
+
+    def build(self, input_shape=None):
+        self.input_spec = InputSpec(shape=input_shape, dtype=tf.float64)
+        if not self.layer.built:
+            self.layer.build(input_shape)
+            self.layer.built = True
+        super(ConcreteDropout, self).build()
+
+        # initialise p
+        self.p_logit = self.add_weight(
+            name="p_logit",
+            shape=(1,),
+            initializer=tf.random_uniform_initializer(self.init_min, self.init_max),
+            dtype=tf.dtypes.float64,
+            trainable=True,
+        )
+
+    def compute_output_shape(self, input_shape):
+        return self.layer.compute_output_shape(input_shape)
+
+    def concrete_dropout(self, x, p):
+        eps = 1e-07
+        temp = 0.1
+
+        unif_noise = tf.random.uniform(shape=tf.shape(x), dtype=tf.float64)
+        drop_prob = (
+            tf.math.log(p + eps)
+            - tf.math.log(1.0 - p + eps)
+            + tf.math.log(unif_noise + eps)
+            - tf.math.log(1.0 - unif_noise + eps)
+        )
+        drop_prob = tf.math.sigmoid(drop_prob / temp)
+        random_tensor = 1.0 - drop_prob
+
+        retain_prob = 1.0 - p
+        x *= random_tensor
+        x /= retain_prob
+        return x
+
+    def call(self, inputs, training=None):
+        p = tf.math.sigmoid(self.p_logit)
+
+        # initialise regulariser / prior KL term
+        input_dim = inputs.shape[-1]  # last dim
+        weight = self.layer.kernel
+        kernel_regularizer = self.weight_regularizer * tf.reduce_sum(tf.square(weight)) / (1.0 - p)
+        dropout_regularizer = p * tf.math.log(p) + (1.0 - p) * tf.math.log(1.0 - p)
+        dropout_regularizer *= self.dropout_regularizer * input_dim
+        regularizer = tf.reduce_sum(kernel_regularizer + dropout_regularizer)
+        if self.is_mc_dropout:
+            return self.layer.call(self.concrete_dropout(inputs, p)), regularizer
+        else:
 
+            def relaxed_dropped_inputs():
+                return self.layer.call(self.concrete_dropout(inputs, p)), regularizer
 
-class NNBayesianModel(Base_Model):
+            return (
+                tf.keras.backend.in_train_phase(relaxed_dropped_inputs, self.layer.call(inputs), training=training),
+                regularizer,
+            )
+
+
+class NNConcreteDropoutModel(Base_Model):
     """
 
-    Used to create a probabilistic neural network model for the RegressionObjective
+    Used to create a neural network model with self-learned dropout probability for the RegressionObjective
 
     See docstring for Base_Model __init__ function for information
 
     """
 
     def __init__(
         self,
@@ -96,120 +159,143 @@
         always_hyperparam_opt: bool = False,
         es_patience: int = 300,  # normally 300
     ):
         super().__init__(variables, objective, always_hyperparam_opt)
         self.default_X_transform_type = "standardisation"
         self.default_Y_transform_type = "standardisation"
         self.include_validation = True
-        self.name = "nn_bayesian"
+        self.name = "nn_concrete"
 
         # Creates the callback method to stop fitting before the all epochs are completed based on the prediction
         # accuracy of the validation set
         self.earlystopping = callbacks.EarlyStopping(
-            monitor="val_loss", min_delta=0.001, patience=es_patience, verbose=0, mode="min",
+            monitor="val_loss",
+            min_delta=0.001,
+            patience=es_patience,
+            verbose=0,
+            mode="min",
         )
 
         # The directory to save the model parameters when it detects a model with better prediction accuracy of the
         # validation set
         self.dirname_checkpoint = os.path.join(os.getcwd(), "ML Models", f"{self.name}", "Checkpoints")
         if not os.path.exists(self.dirname_checkpoint):
             os.makedirs(self.dirname_checkpoint)
 
-    def scaled_kl_fn(self, a, b, _):
-        """
-
-        Function that approximates the KL divergence scaled against the number of training samples by taking the surrogate posterior distribution and prior distribution
-        Yaniv Ovadia, Emily Fertig, Jie Ren, Zachary Nado, D Sculley, Sebastian Nowozin, Joshua V. Dillon, Balaji Lakshminarayanan, Jasper Snoek,
-        Can You Trust Your Model's Uncertainty? Evaluating Predictive Uncertainty Under Dataset Shift, arXiv:1906.02530
-        https://gitlab.ilabt.imec.be/ahadifar/google-research/-/tree/master/uq_benchmark_2019
-
-        """
-        return tfd.kl_divergence(a, b) / self.X_train.shape[0]
-
     @staticmethod
-    def negloglik(y_data, rv_y):
+    def mse_loss(true, pred):
         """
 
-        Function to calculate the value of the negative loglikelihood function
+        Function to calculate the mean squared error (MSE) during training as a monitoring metric
 
         """
-        return -rv_y.log_prob(y_data)
+        n_outputs = pred.shape[1] // 2
+        mean = pred[:, :n_outputs]
+        return tf.reduce_mean((true - mean) ** 2, -1)
 
     @staticmethod
-    def negloglik_met(y_true, y_pred):
+    def heteroscedastic_loss(true, pred):
         """
 
-        Function to calculate the loss value for a neural network model that uses variational inference to fit a surrogate posterior to the distribution over the weights and bias
+        Function to calculate the heteroscedastic uncertainty during training as the loss function
 
         """
-        return tf.reduce_mean(-y_pred.log_prob(tf.cast(y_true, tf.float64)))
+        n_outputs = pred.shape[1] // 2
+        mean = pred[:, :n_outputs]
+        log_var = pred[:, n_outputs:]
+        precision = tf.math.exp(-log_var)
+        return tf.reduce_sum(precision * (true - mean) ** 2.0 + log_var, -1)
 
     def structure(
         self,
         learning_rate: float,
         hidden_units: int,
         hidden_layers: int,
-        dropout_proba: float,
         act_func: str,
         optimizer: Optimizer,
+        wd: float = 0.0,
     ) -> Model:
         """
 
-        Function that defines the structure of the input, hidden layers, and output for a probabilistic neural network model fit over weight and bias distributions
+        Function that defines the structure of the input, hidden layers, and output for a neural network model with
+        self-learned dropout probability
 
         Parameters
         ----------
         learning_rate: float
             Assigns the learning rate for the optimiser
         hidden_units: int
-            The number of hidden units within every hidden layer. Currently, all hidden layers will have this number of hidden units
+            The number of hidden units within every hidden layer. Currently, all hidden layers will have this number
+            of hidden units
         hidden_layers: int
             The number of hidden layers in the neural network
         dropout_proba: float
             The dropout probability to be applied to the hidden layers
         act_func: str
             The activation function to apply on every hidden layer
         optimizer: Optimizer
             The type of optimiser to use to fit the model
+        wd: float
+            The weight regulariser to use in the model
 
         Returns
         -------
         model:
-            The probabilistic neural network model with hidden layers that are fit over weight and bias distributions
+            The neural network model that can learn the dropout probability
 
         """
         K.clear_session()
         tf.random.set_seed(1)
         tf.random.uniform([1], seed=1)
-        input = Input(self.X_train.shape[1])
-        x = input
-        for _ in range(hidden_layers):
-            x = tfpl.DenseFlipout(hidden_units, activation=act_func, kernel_divergence_fn=self.scaled_kl_fn,)(x)
-            if dropout_proba > 0:
-                x = Dropout(dropout_proba)(x)
-        x = tfpl.DenseFlipout(2, kernel_divergence_fn=self.scaled_kl_fn)(x)
-        x = tfpl.DistributionLambda(lambda t: tfd.Normal(loc=t[..., :1], scale=1e-3 + tf.math.softplus(t[..., 1:])))(x)
-        model = Model(input, x)
+        dropout_reg = 2 / self.X_train.shape[0]
+        losses = []
+        inputs = Input(shape=(self.X_train.shape[1],))
+        x = inputs
+        for i in range(hidden_layers):
+            x, loss = ConcreteDropout(
+                Dense(hidden_units, activation=act_func),
+                weight_regularizer=wd,
+                dropout_regularizer=dropout_reg,
+            )(x)
+            losses.append(loss)
+        mean, loss = ConcreteDropout(
+            Dense(self.Y_train.shape[1]),
+            weight_regularizer=wd,
+            dropout_regularizer=dropout_reg,
+        )(x)
+        losses.append(loss)
+        log_var, loss = ConcreteDropout(
+            Dense(self.Y_train.shape[1]),
+            weight_regularizer=wd,
+            dropout_regularizer=dropout_reg,
+        )(x)
+        losses.append(loss)
+        out = concatenate([mean, log_var])
+        model = Model(inputs, out)
+
+        for loss in losses:
+            model.add_loss(loss)
 
-        model.summary()
+        # model.summary()
 
         model.compile(
             optimizer=optimizer(learning_rate=learning_rate),
-            loss=self.negloglik,
-            metrics=["mse", MeanMetricWrapper(self.negloglik_met, name="nll")],
+            loss=self.heteroscedastic_loss,
+            metrics=[self.mse_loss],
         )
+        assert len(model.layers[1].trainable_weights) == 3
 
         return model
 
     def fit(
         self, X: np.ndarray, Y: np.ndarray, test_ratio: float = 0.2, sort_before_split: bool = None, **params
     ) -> None:
         """
 
-        Function that is called to start the probabilistic neural network model fitting procedure
+        Function that is called to start the concrete dropout neural network model fitting procedure
 
         Parameters
         ----------
         X: np.ndarray,
             X array that contains the unprocessed variables data to be fitted to the model, i.e. The data has not yet
             undergone any transformations related to converted categorical variables to their respective descriptors
             or transformations related to standardisation/normalisation
@@ -222,15 +308,20 @@
             Whether the inputted X and Y arrays should be sorted such that the Y-values are in ascending order before
             splitting into the training and test sets (and validation sets if applicable)
         params: Dict[str, Any]
             Dictionary that contains the hyperparameters for the model
 
         """
         if sort_before_split:
-            (X_train, X_val, Y_train, Y_val,) = sort_train_test_split_shuffle(X, Y, test_ratio=test_ratio, seed=1)
+            (
+                X_train,
+                X_val,
+                Y_train,
+                Y_val,
+            ) = sort_train_test_split_shuffle(X, Y, test_ratio=test_ratio, seed=1)
         else:
             X_train, X_val, Y_train, Y_val = train_test_split(X, Y, test_size=test_ratio, random_state=1)
 
         Y_train = Y_train.astype("float")
         Y_val = Y_val.astype("float")
 
         self.X_train, self.X_val, self.Y_train, self.Y_val = (
@@ -256,47 +347,59 @@
 
         self.Y_train_error = 1.96 * self.Y_train_pred_stddev
         self.Y_val_error = 1.96 * self.Y_val_pred_stddev
 
     def fit_model(self, params: Dict[str, Any]) -> None:
         """
 
-        Called by the fit and cv-related functions for fitting the probabilistic neural network model using
-        pre-processed X and Y training data in the class instance
+        Called by the fit and cv-related functions for fitting the neural network model with self-learned dropout
+        probability using pre-processed X and Y training data in the class instance
 
         """
         hidden_units = int(params.get("hidden_units", self.X_train.shape[1] + 1))
         hidden_layers = int(params.get("hidden_layers", 2))
         batch_size = int(params.get("batch_size", 32))
         learning_rate = params.get("learning_rate", 0.001)
-        dropout_proba = params.get("dropout_proba", 0.001)
         max_epochs = int(params.get("max_epochs", 4000))
         act_func = params.get("act_func", "relu")
         optimizer = params.get("optimizer", keras.optimizers.Adam)
 
         self.filepath = os.path.join(
-            self.dirname_checkpoint, f"Checkpoint, Bayesian, {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}.h5",
+            self.dirname_checkpoint,
+            f"Checkpoint, Concrete Dropout, {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}.h5",
         )
 
-        self.model = self.structure(learning_rate, hidden_units, hidden_layers, dropout_proba, act_func, optimizer,)
-        self.savemodelcheckpoint = SaveModelCheckPoint(self.model, self.filepath)
+        self.model = self.structure(
+            learning_rate,
+            hidden_units,
+            hidden_layers,
+            act_func,
+            optimizer,
+        )
+        self.savemodelcheckpoint = SaveModelCheckPoint(self.model, self.filepath)  # A Simon Original
         self.history = self.model.fit(
             self.X_train,
             self.Y_train,
             validation_data=(self.X_val, self.Y_val),
             epochs=max_epochs,
-            verbose=2,
+            verbose=0,
             batch_size=batch_size,
             callbacks=[
                 callbacks.LambdaCallback(on_epoch_end=self.savemodelcheckpoint.save_weights),
                 self.earlystopping,
             ],
         )
 
-        self.model = self.structure(learning_rate, hidden_units, hidden_layers, dropout_proba, act_func, optimizer,)
+        self.model = self.structure(
+            learning_rate,
+            hidden_units,
+            hidden_layers,
+            act_func,
+            optimizer,
+        )
         self.model.load_weights(self.filepath)
 
     def predict(self, X: np.ndarray, X_transform: bool = True) -> Tuple[np.ndarray, np.ndarray]:
         """
 
         Determines the model output and its standard deviation of the X array passed into the function
 
@@ -325,65 +428,92 @@
             X = X.reshape(1, -1)
 
         if X_transform:
             if self.variables.num_cat_var > 0:
                 X = self.variables.categorical_transform(X).astype("float")
             X = self.transform_only_by_predictor_type(X)
 
-        observed_Y_pred = [self.model(X) for _ in range(10)]
-        Y_pred = np.array([prediction.loc.numpy() for prediction in observed_Y_pred])
-        Y_pred_stddev = np.array([prediction.scale.numpy() for prediction in observed_Y_pred])
+        observed_Y_pred = np.array([self.model.predict(X) for _ in range(10)])
+        Y_pred = observed_Y_pred[:, :, :1]
+        Y_pred_stddev = np.sqrt(np.exp(observed_Y_pred[:, :, 1:]))
 
         # Code adapted from:
-        #     1. João Caldeira, Brian Nord, Deeply Uncertain: Comparing Methods of Uncertainty Quantification in Deep Learning Algorithms, arXiv:2004.10710, https://github.com/deepskies/DeeplyUncertain-Public,
-        #     2. Yarin Gal, Jiri Hron, Alex Kendall, Concrete Dropout, arXiv:1705.07832, https://github.com/yaringal/ConcreteDropout
+        #     1. João Caldeira, Brian Nord, Deeply Uncertain: Comparing Methods of Uncertainty Quantification in Deep
+        #     Learning Algorithms, arXiv:2004.10710, https://github.com/deepskies/DeeplyUncertain-Public,
+        #     2. Yarin Gal, Jiri Hron, Alex Kendall, Concrete Dropout, arXiv:1705.07832,
+        #     https://github.com/yaringal/ConcreteDropout
         Y_val_epistemic_unc = np.std(np.array(Y_pred), axis=0)
         Y_val_aleatoric_unc = np.sqrt(np.mean(np.array(Y_pred_stddev) * np.array(Y_pred_stddev), axis=0))
-        Y_val_total_unc = np.sqrt(Y_val_aleatoric_unc ** 2 + Y_val_epistemic_unc ** 2)
+        Y_val_total_unc = np.sqrt(Y_val_aleatoric_unc**2 + Y_val_epistemic_unc**2)
 
         Y_pred = np.mean(Y_pred, axis=0)
         Y_pred_upper = Y_pred + (1.96 * Y_val_total_unc)
 
         Y_pred = self.objective.inverse_transform(Y_pred)
         Y_pred_upper = self.objective.inverse_transform(Y_pred_upper)
         Y_pred_stddev = (np.subtract(Y_pred_upper, Y_pred)) / 1.96
 
         return Y_pred.flatten(), Y_pred_stddev.flatten()
 
+    def draw_samples(self, X: np.ndarray, X_transform: bool = True) -> np.ndarray:
+        """
+
+        Generates samples from a normal distribution using the X array
+
+        Parameters
+        ----------
+        X: np.ndarray,
+            X array that contains the unprocessed variables data to be used in the prediction, i.e. The data has not
+            yet undergone any transformations related to converted categorical variables to their respective
+            descriptors or transformations related to standardisation/normalisation
+        X_transform: bool, Default = True
+            For the default models provided natively in NEMO, the initial transformation of categorical variables and
+            transformations related to standardisation/normalisation can be switched off by passing X_transform = False
+
+        Returns
+        ----------
+        np.ndarray
+            Drawn samples of the objective using the model and the inputted X array. The outputted values have been
+            un-transformed
+
+        """
+        Y_pred, Y_pred_stddev = self.predict(X, X_transform=X_transform)
+
+        return np.random.default_rng().normal(Y_pred, Y_pred_stddev)
+
     @staticmethod
     def default_params(X: np.ndarray):
         """
 
-        Function that returns the default hyperparameters to use for the hyperparameter optimisation of probabilistic
-        neural network models using the hyperopt package. Returns a dictionary that is used for the space argument in
-        the hyperopt.fmin function
+        Function that returns the default hyperparameters to use for the hyperparameter optimisation of a neural
+        network model that can self-learn dropout probability using the hyperopt package. Returns a dictionary that is
+        used for the space argument in the hyperopt.fmin function
 
         """
         return {
             "learning_rate": hp.uniform("learning_rate", 0.001, 0.01),
             "hidden_units": scope.int(hp.quniform("hidden_units", math.ceil(X.shape[1] / 2), (X.shape[1] + 1), 1)),
             "hidden_layers": scope.int(hp.quniform("hidden_layers", 1, 2, 1)),
             "batch_size": scope.int(hp.quniform("batch_size", math.ceil(X.shape[0] / 10), X.shape[0], 1)),
-            "dropout_proba": hp.uniform("dropout_proba", 0.001, 0.05),
         }
 
     def hyperparam_opt(
         self,
         X: np.ndarray,
         Y: np.ndarray,
         test_ratio: float,
         sort_before_split: bool = True,
         predictor_params_dict: Optional[Dict[str, Dict[str, Callable]]] = None,
         **kwargs,
-    ) -> Tuple[NNBayesianModel, Dict[str, Any]]:
+    ) -> Tuple[NNConcreteDropoutModel, Dict[str, Any]]:
         """
 
-        Function to be called for performing hyperparameter optimisation for probabilistic neural network models using
-        the hyperopt package. Returns the model fitted with the best hyperparameters and a dictionary containing the
-        best hyperparameters
+        Function to be called for performing hyperparameter optimisation for neural network models with self-learned
+        dropout probability using the hyperopt package. Returns the model fitted with the best hyperparameters and a
+        dictionary containing the best hyperparameters
 
         Parameters
         ----------
         X: np.ndarray,
             X array that contains the unprocessed variables data to be fitted to the model, i.e. The data has not yet
             undergone any transformations related to converted categorical variables to their respective descriptors
             or transformations related to standardisation/normalisation
@@ -392,16 +522,16 @@
             transformations related to standardisation/normalisation
         test_ratio: float
             The proportion of inputted X and Y arrays to be split for the validation set where applicable
         sort_before_split: bool, Default = True,
             Whether the inputted X and Y arrays should be sorted such that the Y-values are in ascending order before
             splitting into the training and test sets (and validation sets if applicable)
         predictor_params_dict: Dict[str, Dict[str, Callable]], Default = None
-            Dictionary with a key 'nn_bayesian' and a corresponding value that is a dictionary that is used for the space
-            argument in the hyperopt.fmin function
+            Dictionary with a key 'nn_concrete' and a corresponding value that is a dictionary that is used for the
+            space argument in the hyperopt.fmin function
 
         Returns
         -------
         model: NNBayesianModel
             The model fitted with the best hyperparameters found using the hyperopt package
 
         model_params: Dict[str, Any]
@@ -409,22 +539,22 @@
 
         """
         if predictor_params_dict is None:
             predictor_params_dict = self.default_params(X)
         else:
             predictor_params_dict = predictor_params_dict.get(self.name, self.default_params(X))
 
-        if self.objective.hyperopt_evals is None:
-            hyperopt_evals = 1
-        else:
-            hyperopt_evals = self.objective.hyperopt_evals.get(self.name, 1)
         # if self.objective.hyperopt_evals is None:
-        #     hyperopt_evals = 20
+        #     hyperopt_evals = 1
         # else:
-        #     hyperopt_evals = self.objective.hyperopt_evals.get(f"{self.name}", 20)
+        #     hyperopt_evals = self.objective.hyperopt_evals.get(self.name, 1)
+        if self.objective.hyperopt_evals is None:
+            hyperopt_evals = 20
+        else:
+            hyperopt_evals = self.objective.hyperopt_evals.get(f"{self.name}", 20)
 
         def func(X: np.ndarray, Y: np.ndarray, model_params: Dict[str, Any]) -> Dict[str, Any]:
             loss = self.non_cv_train_val_test(
                 X, Y, model_params, test_ratio=test_ratio, sort_before_split=sort_before_split, **kwargs
             )
 
             return {
```

### Comparing `nemo-bo-0.1.8/nemo_bo/models/nn_ensemble.py` & `nemo-bo-0.1.9/nemo_bo/models/nn_bayesian.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,25 +3,29 @@
 import math
 import os
 from datetime import datetime
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple
 
 import numpy as np
+import six
 import tensorflow as tf
 import tensorflow_probability as tfp
 from hyperopt import STATUS_OK, Trials, fmin, hp, tpe
 from hyperopt.pyll.base import scope
 from keras import backend as K
 from keras import callbacks
-from keras.layers import Dense, Dropout, Input
+from keras.layers import Dropout, Input
 from keras.models import Model
 from keras.optimizers import Optimizer
 from sklearn.model_selection import train_test_split
 from tensorflow import keras
+from tensorflow_probability.python.internal import tensorshape_util
+
+tf.keras.backend.set_floatx("float64")
 
 import nemo_bo.utils.logger as logging_nemo
 import nemo_bo.utils.perf_metrics as pm
 from nemo_bo.models.base.base_model import Base_Model
 from nemo_bo.models.base.nn_save_checkpoint import SaveModelCheckPoint
 from nemo_bo.utils.data_proc import sort_train_test_split_shuffle
 
@@ -47,18 +51,45 @@
             tf.config.experimental.set_memory_growth(gpu, True)
         logical_gpus = tf.config.list_logical_devices("GPU")
         print(len(gpus), "Physical GPUs,", len(logical_gpus), "Logical GPUs")
     except RuntimeError as e:
         print(e)
 
 
-class NNEnsembleModel(Base_Model):
+class MeanMetricWrapper(tf.keras.metrics.Mean):
+    """
+
+    Code by @mcourteaux from https://github.com/tensorflow/probability/issues/742#issuecomment-580433644
+    João Caldeira, Brian Nord, Deeply Uncertain: Comparing Methods of Uncertainty Quantification in Deep Learning Algorithms,
+    https://arxiv.org/abs/2004.10710
+    https://github.com/deepskies/DeeplyUncertain-Public
+
+    """
+
+    def __init__(self, fn, name=None, dtype=None, **kwargs):
+        super(MeanMetricWrapper, self).__init__(name=name, dtype=dtype)
+        self._fn = fn
+        self._fn_kwargs = kwargs
+
+    def update_state(self, y_true, y_pred, sample_weight=None):
+        matches = self._fn(y_true, y_pred, **self._fn_kwargs)
+        return super(MeanMetricWrapper, self).update_state(matches, sample_weight=sample_weight)
+
+    def get_config(self):
+        config = {}
+        for k, v in six.iteritems(self._fn_kwargs):
+            config[k] = K.eval(v) if tensorshape_util.is_tensor_or_variable(v) else v
+        base_config = super(MeanMetricWrapper, self).get_config()
+        return dict(list(base_config.items()) + list(config.items()))
+
+
+class NNBayesianModel(Base_Model):
     """
 
-    Used to create an ensemble of neural network models for the RegressionObjective
+    Used to create a probabilistic neural network model for the RegressionObjective
 
     See docstring for Base_Model __init__ function for information
 
     """
 
     def __init__(
         self,
@@ -67,92 +98,124 @@
         always_hyperparam_opt: bool = False,
         es_patience: int = 300,  # normally 300
     ):
         super().__init__(variables, objective, always_hyperparam_opt)
         self.default_X_transform_type = "standardisation"
         self.default_Y_transform_type = "standardisation"
         self.include_validation = True
-        self.name = "nn_ensemble"
+        self.name = "nn_bayesian"
 
         # Creates the callback method to stop fitting before the all epochs are completed based on the prediction
         # accuracy of the validation set
         self.earlystopping = callbacks.EarlyStopping(
-            monitor="val_loss", min_delta=0.001, patience=es_patience, verbose=0, mode="min",
+            monitor="val_loss",
+            min_delta=0.001,
+            patience=es_patience,
+            verbose=0,
+            mode="min",
         )
 
         # The directory to save the model parameters when it detects a model with better prediction accuracy of the
         # validation set
-        self.dirname_checkpoint = os.path.join(os.getcwd(), "ML Models", "nn_ensemble", "Checkpoints")
+        self.dirname_checkpoint = os.path.join(os.getcwd(), "ML Models", f"{self.name}", "Checkpoints")
         if not os.path.exists(self.dirname_checkpoint):
             os.makedirs(self.dirname_checkpoint)
 
+    def scaled_kl_fn(self, a, b, _):
+        """
+
+        Function that approximates the KL divergence scaled against the number of training samples by taking the
+        surrogate posterior distribution and prior distribution
+        Yaniv Ovadia, Emily Fertig, Jie Ren, Zachary Nado, D Sculley, Sebastian Nowozin, Joshua V. Dillon, Balaji
+        Lakshminarayanan, Jasper Snoek, Can You Trust Your Model's Uncertainty? Evaluating Predictive Uncertainty Under
+        Dataset Shift, arXiv:1906.02530
+        https://gitlab.ilabt.imec.be/ahadifar/google-research/-/tree/master/uq_benchmark_2019
+
+        """
+        return tfd.kl_divergence(a, b) / self.X_train.shape[0]
+
     @staticmethod
     def negloglik(y_data, rv_y):
         """
 
         Function to calculate the value of the negative loglikelihood function
 
         """
         return -rv_y.log_prob(y_data)
 
-    # function for creating a fully connected neural network of any architecture
-    # the number of neurons in each layer is defined by layers_shape
-    # the droupout_proba indicates if dropout layers should be added
+    @staticmethod
+    def negloglik_met(y_true, y_pred):
+        """
+
+        Function to calculate the loss value for a neural network model that uses variational inference to fit a
+        surrogate posterior to the distribution over the weights and bias
+
+        """
+        return tf.reduce_mean(-y_pred.log_prob(tf.cast(y_true, tf.float64)))
+
     def structure(
         self,
         learning_rate: float,
         hidden_units: int,
         hidden_layers: int,
         dropout_proba: float,
         act_func: str,
         optimizer: Optimizer,
     ) -> Model:
         """
 
-        Function that defines the structure of the input, hidden layers, and output for the neural network models in
-        the ensemble
+        Function that defines the structure of the input, hidden layers, and output for a probabilistic neural network
+        model fit over weight and bias distributions
 
         Parameters
         ----------
         learning_rate: float
             Assigns the learning rate for the optimiser
         hidden_units: int
-            The number of hidden units within every hidden layer. Currently, all hidden layers will have this number of hidden units
+            The number of hidden units within every hidden layer. Currently, all hidden layers will have this number
+            of hidden units
         hidden_layers: int
             The number of hidden layers in the neural network
         dropout_proba: float
             The dropout probability to be applied to the hidden layers
         act_func: str
             The activation function to apply on every hidden layer
         optimizer: Optimizer
             The type of optimiser to use to fit the model
 
         Returns
         -------
         model:
-            The neural network model with specified hidden layers
+            The probabilistic neural network model with hidden layers that are fit over weight and bias distributions
 
         """
         K.clear_session()
         tf.random.set_seed(1)
         tf.random.uniform([1], seed=1)
-        input_data = Input((self.X_train.shape[1],))
-        x = input_data
+        input = Input(self.X_train.shape[1])
+        x = input
         for _ in range(hidden_layers):
-            x = Dense(hidden_units, activation=act_func)(x)
+            x = tfpl.DenseFlipout(
+                hidden_units,
+                activation=act_func,
+                kernel_divergence_fn=self.scaled_kl_fn,
+            )(x)
             if dropout_proba > 0:
                 x = Dropout(dropout_proba)(x)
-
-        x = Dense(2)(x)
+        x = tfpl.DenseFlipout(2, kernel_divergence_fn=self.scaled_kl_fn)(x)
         x = tfpl.DistributionLambda(lambda t: tfd.Normal(loc=t[..., :1], scale=1e-3 + tf.math.softplus(t[..., 1:])))(x)
-        model = Model(input_data, x)
-        model.summary()
+
+        model = Model(input, x)
+
+        # model.summary()
 
         model.compile(
-            optimizer=optimizer(learning_rate=learning_rate), loss=self.negloglik, metrics=["mse"],
+            optimizer=optimizer(learning_rate=learning_rate),
+            loss=self.negloglik,
+            metrics=["mse", MeanMetricWrapper(self.negloglik_met, name="nll")],
         )
 
         return model
 
     def fit(
         self, X: np.ndarray, Y: np.ndarray, test_ratio: float = 0.2, sort_before_split: bool = None, **params
     ) -> None:
@@ -175,15 +238,20 @@
             Whether the inputted X and Y arrays should be sorted such that the Y-values are in ascending order before
             splitting into the training and test sets (and validation sets if applicable)
         params: Dict[str, Any]
             Dictionary that contains the hyperparameters for the model
 
         """
         if sort_before_split:
-            (X_train, X_val, Y_train, Y_val,) = sort_train_test_split_shuffle(X, Y, test_ratio=test_ratio, seed=1)
+            (
+                X_train,
+                X_val,
+                Y_train,
+                Y_val,
+            ) = sort_train_test_split_shuffle(X, Y, test_ratio=test_ratio, seed=1)
         else:
             X_train, X_val, Y_train, Y_val = train_test_split(X, Y, test_size=test_ratio, random_state=1)
 
         Y_train = Y_train.astype("float")
         Y_val = Y_val.astype("float")
 
         self.X_train, self.X_val, self.Y_train, self.Y_val = (
@@ -209,52 +277,63 @@
 
         self.Y_train_error = 1.96 * self.Y_train_pred_stddev
         self.Y_val_error = 1.96 * self.Y_val_pred_stddev
 
     def fit_model(self, params: Dict[str, Any]) -> None:
         """
 
-        Called by the fit and cv-related functions for fitting the neural network models in the ensemble using
+        Called by the fit and cv-related functions for fitting the probabilistic neural network model using
         pre-processed X and Y training data in the class instance
 
         """
         hidden_units = int(params.get("hidden_units", self.X_train.shape[1] + 1))
         hidden_layers = int(params.get("hidden_layers", 2))
         batch_size = int(params.get("batch_size", 32))
         learning_rate = params.get("learning_rate", 0.001)
         dropout_proba = params.get("dropout_proba", 0.001)
-        ensemble_size = int(params.get("ensemble_size", 5))
         max_epochs = int(params.get("max_epochs", 4000))
         act_func = params.get("act_func", "relu")
         optimizer = params.get("optimizer", keras.optimizers.Adam)
 
         self.filepath = os.path.join(
-            self.dirname_checkpoint, f"Checkpoint, Ensemble, {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}.h5",
+            self.dirname_checkpoint,
+            f"Checkpoint, Bayesian, {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}.h5",
         )
 
-        self.ensemble_model_list = []
-        for _ in range(ensemble_size):
-            self.model = self.structure(learning_rate, hidden_units, hidden_layers, dropout_proba, act_func, optimizer,)
-            self.savemodelcheckpoint = SaveModelCheckPoint(self.model, self.filepath)  # A Simon Original
-            self.history = self.model.fit(
-                self.X_train,
-                self.Y_train,
-                validation_data=(self.X_val, self.Y_val),
-                epochs=max_epochs,
-                verbose=2,
-                batch_size=batch_size,
-                callbacks=[
-                    callbacks.LambdaCallback(on_epoch_end=self.savemodelcheckpoint.save_weights),
-                    self.earlystopping,
-                ],
-            )
+        self.model = self.structure(
+            learning_rate,
+            hidden_units,
+            hidden_layers,
+            dropout_proba,
+            act_func,
+            optimizer,
+        )
+        self.savemodelcheckpoint = SaveModelCheckPoint(self.model, self.filepath)
+        self.history = self.model.fit(
+            self.X_train,
+            self.Y_train,
+            validation_data=(self.X_val, self.Y_val),
+            epochs=max_epochs,
+            verbose=0,
+            batch_size=batch_size,
+            callbacks=[
+                callbacks.LambdaCallback(on_epoch_end=self.savemodelcheckpoint.save_weights),
+                self.earlystopping,
+            ],
+        )
 
-            self.model = self.structure(learning_rate, hidden_units, hidden_layers, dropout_proba, act_func, optimizer,)
-            self.model.load_weights(self.filepath)
-            self.ensemble_model_list.append(self.model)
+        self.model = self.structure(
+            learning_rate,
+            hidden_units,
+            hidden_layers,
+            dropout_proba,
+            act_func,
+            optimizer,
+        )
+        self.model.load_weights(self.filepath)
 
     def predict(self, X: np.ndarray, X_transform: bool = True) -> Tuple[np.ndarray, np.ndarray]:
         """
 
         Determines the model output and its standard deviation of the X array passed into the function
 
         Parameters
@@ -282,39 +361,77 @@
             X = X.reshape(1, -1)
 
         if X_transform:
             if self.variables.num_cat_var > 0:
                 X = self.variables.categorical_transform(X).astype("float")
             X = self.transform_only_by_predictor_type(X)
 
-        observed_Y_pred = [ensemble_model(X) for ensemble_model in self.ensemble_model_list]
+        observed_Y_pred = [self.model(X) for _ in range(10)]
         Y_pred = np.array([prediction.loc.numpy() for prediction in observed_Y_pred])
         Y_pred_stddev = np.array([prediction.scale.numpy() for prediction in observed_Y_pred])
 
         # Code adapted from:
-        #     1. João Caldeira, Brian Nord, Deeply Uncertain: Comparing Methods of Uncertainty Quantification in Deep Learning Algorithms, arXiv:2004.10710, https://github.com/deepskies/DeeplyUncertain-Public,
-        #     2. Yarin Gal, Jiri Hron, Alex Kendall, Concrete Dropout, arXiv:1705.07832, https://github.com/yaringal/ConcreteDropout
-        Y_val_epistemic_unc = np.std(np.array(Y_pred), axis=0)  # Equation 4 from paper
+        #     1. João Caldeira, Brian Nord, Deeply Uncertain: Comparing Methods of Uncertainty Quantification in Deep
+        #     Learning Algorithms, arXiv:2004.10710, https://github.com/deepskies/DeeplyUncertain-Public,
+        #     2. Yarin Gal, Jiri Hron, Alex Kendall, Concrete Dropout, arXiv:1705.07832,
+        #     https://github.com/yaringal/ConcreteDropout
+        Y_val_epistemic_unc = np.std(np.array(Y_pred), axis=0)
         Y_val_aleatoric_unc = np.sqrt(np.mean(np.array(Y_pred_stddev) * np.array(Y_pred_stddev), axis=0))
-        Y_val_total_unc = np.sqrt(Y_val_aleatoric_unc ** 2 + Y_val_epistemic_unc ** 2)
+        Y_val_total_unc = np.sqrt(Y_val_aleatoric_unc**2 + Y_val_epistemic_unc**2)
 
         Y_pred = np.mean(Y_pred, axis=0)
         Y_pred_upper = Y_pred + (1.96 * Y_val_total_unc)
 
         Y_pred = self.objective.inverse_transform(Y_pred)
         Y_pred_upper = self.objective.inverse_transform(Y_pred_upper)
         Y_pred_stddev = (np.subtract(Y_pred_upper, Y_pred)) / 1.96
 
         return Y_pred.flatten(), Y_pred_stddev.flatten()
 
+    def draw_samples(self, X: np.ndarray, X_transform: bool = True) -> Tuple[np.ndarray, np.ndarray]:
+        """
+
+        Generates samples from the distribution using the X array
+
+        Parameters
+        ----------
+        X: np.ndarray,
+            X array that contains the unprocessed variables data to be used in the prediction, i.e. The data has not
+            yet undergone any transformations related to converted categorical variables to their respective
+            descriptors or transformations related to standardisation/normalisation
+        X_transform: bool, Default = True
+            For the default models provided natively in NEMO, the initial transformation of categorical variables and
+            transformations related to standardisation/normalisation can be switched off by passing X_transform = False
+
+        Returns
+        ----------
+        Y_samples: np.ndarray
+            Drawn samples of the objective using the model and the inputted X array. The outputted values have been
+            un-transformed
+
+        """
+        # X needs to be a 2D array
+        if X.ndim == 1:
+            X = X.reshape(1, -1)
+
+        if X_transform:
+            if self.variables.num_cat_var > 0:
+                X = self.variables.categorical_transform(X).astype("float")
+            X = self.transform_only_by_predictor_type(X)
+
+        Y_pred = self.model(X).sample().numpy()
+        Y_samples = self.objective.inverse_transform(Y_pred)
+
+        return Y_samples.flatten()
+
     @staticmethod
     def default_params(X: np.ndarray):
         """
 
-        Function that returns the default hyperparameters to use for the hyperparameter optimisation of ensemble
+        Function that returns the default hyperparameters to use for the hyperparameter optimisation of probabilistic
         neural network models using the hyperopt package. Returns a dictionary that is used for the space argument in
         the hyperopt.fmin function
 
         """
         return {
             "learning_rate": hp.uniform("learning_rate", 0.001, 0.01),
             "hidden_units": scope.int(hp.quniform("hidden_units", math.ceil(X.shape[1] / 2), (X.shape[1] + 1), 1)),
@@ -327,18 +444,18 @@
         self,
         X: np.ndarray,
         Y: np.ndarray,
         test_ratio: float,
         sort_before_split: bool = True,
         predictor_params_dict: Optional[Dict[str, Dict[str, Callable]]] = None,
         **kwargs,
-    ) -> Tuple[NNEnsembleModel, Dict[str, Any]]:
+    ) -> Tuple[NNBayesianModel, Dict[str, Any]]:
         """
 
-        Function to be called for performing hyperparameter optimisation for ensemble neural network models using
+        Function to be called for performing hyperparameter optimisation for probabilistic neural network models using
         the hyperopt package. Returns the model fitted with the best hyperparameters and a dictionary containing the
         best hyperparameters
 
         Parameters
         ----------
         X: np.ndarray,
             X array that contains the unprocessed variables data to be fitted to the model, i.e. The data has not yet
@@ -349,16 +466,16 @@
             transformations related to standardisation/normalisation
         test_ratio: float
             The proportion of inputted X and Y arrays to be split for the validation set where applicable
         sort_before_split: bool, Default = True,
             Whether the inputted X and Y arrays should be sorted such that the Y-values are in ascending order before
             splitting into the training and test sets (and validation sets if applicable)
         predictor_params_dict: Dict[str, Dict[str, Callable]], Default = None
-            Dictionary with a key 'nn_ensemble' and a corresponding value that is a dictionary that is used for the space
-            argument in the hyperopt.fmin function
+            Dictionary with a key 'nn_bayesian' and a corresponding value that is a dictionary that is used for the
+            space argument in the hyperopt.fmin function
 
         Returns
         -------
         model: NNBayesianModel
             The model fitted with the best hyperparameters found using the hyperopt package
 
         model_params: Dict[str, Any]
@@ -366,22 +483,22 @@
 
         """
         if predictor_params_dict is None:
             predictor_params_dict = self.default_params(X)
         else:
             predictor_params_dict = predictor_params_dict.get(self.name, self.default_params(X))
 
-        if self.objective.hyperopt_evals is None:
-            hyperopt_evals = 1
-        else:
-            hyperopt_evals = self.objective.hyperopt_evals.get(self.name, 1)
         # if self.objective.hyperopt_evals is None:
-        #     hyperopt_evals = 15
+        #     hyperopt_evals = 1
         # else:
-        #     hyperopt_evals = self.objective.hyperopt_evals.get(f"{self.name}", 15)
+        #     hyperopt_evals = self.objective.hyperopt_evals.get(self.name, 1)
+        if self.objective.hyperopt_evals is None:
+            hyperopt_evals = 20
+        else:
+            hyperopt_evals = self.objective.hyperopt_evals.get(f"{self.name}", 20)
 
         def func(X: np.ndarray, Y: np.ndarray, model_params: Dict[str, Any]) -> Dict[str, Any]:
             loss = self.non_cv_train_val_test(
                 X, Y, model_params, test_ratio=test_ratio, sort_before_split=sort_before_split, **kwargs
             )
 
             return {
```

### Comparing `nemo-bo-0.1.8/nemo_bo/models/rf.py` & `nemo-bo-0.1.9/nemo_bo/models/rf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Based on forest-confidence-interval: Confidence intervals for Forest algorithms, Kivan Polimis, Ariel Rokem, Bryna Hazelton, The University of Washington, https://github.com/scikit-learn-contrib/forest-confidence-interval
+# Based on forest-confidence-interval: Confidence intervals for Forest algorithms, Kivan Polimis, Ariel Rokem, Bryna
+# Hazelton, The University of Washington, https://github.com/scikit-learn-contrib/forest-confidence-interval
 
 from __future__ import annotations
 
 import os
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple
 
@@ -137,14 +138,40 @@
 
         Y_pred = self.objective.inverse_transform(Y_mean)
         Y_pred_upper = self.objective.inverse_transform(Y_pred_upper)
         Y_pred_stddev = (np.subtract(Y_pred_upper, Y_pred)) / 1.96
 
         return Y_pred.flatten(), Y_pred_stddev.flatten()
 
+    def draw_samples(self, X: np.ndarray, X_transform: bool = True) -> np.ndarray:
+        """
+
+        Generates samples from a normal distribution using the X array
+
+        Parameters
+        ----------
+        X: np.ndarray,
+            X array that contains the unprocessed variables data to be used in the prediction, i.e. The data has not
+            yet undergone any transformations related to converted categorical variables to their respective
+            descriptors or transformations related to standardisation/normalisation
+        X_transform: bool, Default = True
+            For the default models provided natively in NEMO, the initial transformation of categorical variables and
+            transformations related to standardisation/normalisation can be switched off by passing X_transform = False
+
+        Returns
+        ----------
+        np.ndarray
+            Drawn samples of the objective using the model and the inputted X array. The outputted values have been
+            un-transformed
+
+        """
+        Y_pred, Y_pred_stddev = self.predict(X, X_transform=X_transform)
+
+        return np.random.default_rng().normal(Y_pred, Y_pred_stddev)
+
     @staticmethod
     def default_params():
         """
 
         Function that returns the default hyperparameters to use for the hyperparameter optimisation of Random Forest
         models using the hyperopt package. Returns a dictionary that is used for the space argument in the hyperopt.fmin
         function
@@ -196,22 +223,22 @@
 
         """
         if predictor_params_dict is None:
             predictor_params_dict = self.default_params()
         else:
             predictor_params_dict = predictor_params_dict.get(self.name, self.default_params())
 
-        if self.objective.hyperopt_evals is None:
-            hyperopt_evals = 1
-        else:
-            hyperopt_evals = self.objective.hyperopt_evals.get(self.name, 1)
         # if self.objective.hyperopt_evals is None:
-        #     hyperopt_evals = 30
+        #     hyperopt_evals = 1
         # else:
-        #     hyperopt_evals = self.objective.hyperopt_evals.get(f"{self.name}", 30)
+        #     hyperopt_evals = self.objective.hyperopt_evals.get(self.name, 1)
+        if self.objective.hyperopt_evals is None:
+            hyperopt_evals = 30
+        else:
+            hyperopt_evals = self.objective.hyperopt_evals.get(f"{self.name}", 30)
 
         def func(X: np.ndarray, Y: np.ndarray, model_params: Dict[str, Any]) -> Dict[str, Any]:
             cv_results = self.cv(X, Y, model_params, test_ratio=test_ratio, **kwargs)
 
             return {
                 "loss": cv_results["Mean Test RMSE"],
                 "status": STATUS_OK,
```

### Comparing `nemo-bo-0.1.8/nemo_bo/models/xgb.py` & `nemo-bo-0.1.9/nemo_bo/models/xgb.py`

 * *Files 16% similar despite different names*

```diff
@@ -68,15 +68,20 @@
             Whether the inputted X and Y arrays should be sorted such that the Y-values are in ascending order before
             splitting into the training and test sets (and validation sets if applicable)
         params: Dict[str, Any]
             Dictionary that contains the hyperparameters for the model
 
         """
         if sort_before_split:
-            (X_train, X_val, Y_train, Y_val,) = sort_train_test_split_shuffle(X, Y, test_ratio=test_ratio, seed=1)
+            (
+                X_train,
+                X_val,
+                Y_train,
+                Y_val,
+            ) = sort_train_test_split_shuffle(X, Y, test_ratio=test_ratio, seed=1)
         else:
             X_train, X_val, Y_train, Y_val = train_test_split(X, Y, test_size=test_ratio, random_state=1)
 
         Y_train = Y_train.astype("float")
         Y_val = Y_val.astype("float")
 
         self.X_train, self.X_val, self.Y_train, self.Y_val = (
@@ -126,15 +131,18 @@
 
         self.model = XGBDistribution(early_stopping_rounds=10, **params)
 
         # Re-attempts fitting
         for x in range(10):
             try:
                 self.model.fit(
-                    self.X_train, self.Y_train, eval_set=[(self.X_val, self.Y_val)], verbose=False,
+                    self.X_train,
+                    self.Y_train,
+                    eval_set=[(self.X_val, self.Y_val)],
+                    verbose=False,
                 )
                 break
             except np.linalg.LinAlgError as e:
                 print(e)
             except TypeError as e:
                 print(e)
             except sklearn.exceptions.NotFittedError as e:
@@ -178,15 +186,41 @@
         Y_mean = Y_pred.loc
         Y_pred_upper = Y_mean + (1.96 * Y_pred.scale)
 
         Y_pred = self.objective.inverse_transform(Y_mean)
         Y_pred_upper = self.objective.inverse_transform(Y_pred_upper)
         Y_pred_stddev = (np.subtract(Y_pred_upper, Y_pred)) / 1.96
 
-        return Y_mean.flatten(), Y_pred_stddev.flatten()
+        return Y_pred.flatten(), Y_pred_stddev.flatten()
+
+    def draw_samples(self, X: np.ndarray, X_transform: bool = True) -> np.ndarray:
+        """
+
+        Generates samples from a normal distribution using the X array
+
+        Parameters
+        ----------
+        X: np.ndarray,
+            X array that contains the unprocessed variables data to be used in the prediction, i.e. The data has not
+            yet undergone any transformations related to converted categorical variables to their respective
+            descriptors or transformations related to standardisation/normalisation
+        X_transform: bool, Default = True
+            For the default models provided natively in NEMO, the initial transformation of categorical variables and
+            transformations related to standardisation/normalisation can be switched off by passing X_transform = False
+
+        Returns
+        ----------
+        np.ndarray
+            Drawn samples of the objective using the model and the inputted X array. The outputted values have been
+            un-transformed
+
+        """
+        Y_pred, Y_pred_stddev = self.predict(X, X_transform=X_transform)
+
+        return np.random.default_rng().normal(Y_pred, Y_pred_stddev)
 
     @staticmethod
     def default_params():
         """
 
         Function that returns the default hyperparameters to use for the hyperparameter optimisation of XGBoost
         Distribution models using the hyperopt package. Returns a dictionary that is used for the space argument in
```

### Comparing `nemo-bo-0.1.8/nemo_bo/opt/constraints.py` & `nemo-bo-0.1.9/nemo_bo/opt/constraints.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import os
 from attrs import define, field
-from typing import Callable, List, Tuple, Union
+from typing import Callable, List, Tuple, Union, Dict, Any, Optional
 
 import numpy as np
 import torch
 from torch import Tensor
 
 import nemo_bo.utils.logger as logging_nemo
-from nemo_bo.opt.variables import VariablesList
+from nemo_bo.opt.variables import CategoricalVariable, VariablesList
 
 try:
     logging_nemo.logging_path
     logger = logging_nemo.logging_nemo_child(os.path.basename(__file__))
 except AttributeError:
     logger = logging_nemo.logging_nemo_master(os.path.basename(__file__))
 
 
 @define
 class LinearConstraint:
     """
 
-    Implements a linear constraint on the input variables for the optimisation. For example, linear constraints could be:
+    Implements a linear constraint on the input variables for the optimisation. For example, linear constraints could
+    be:
 
         a(F1) + b(F2) = 0
         a(F1) + b(F2) >= 0
 
     where a and b are coefficients for the features F1 and F2 respectively, and the right-hand side of the equation is
     0. Using an equals sign, =, would form a linear equality constraint whereas defining as 'greater than or equal to'
     forms an inequality constraint.
@@ -128,15 +129,16 @@
 
         """
         # Un-normalise the variables
         x = (x * (np.array(self.variables.upper_bounds) - np.array(self.variables.lower_bounds))) + np.array(
             self.variables.lower_bounds
         )
 
-        # Multiply coefficients and rhs by -1 because pymoo uses the less than or equal to inequality operator for its constraints
+        # Multiply coefficients and rhs by -1 because pymoo uses the less than or equal to inequality operator for its
+        # constraints
         if self.constraint_type == "ineq":
             return np.sum(x[:, self.index] * [-coeff for coeff in self.coefficients], axis=1) - (self.rhs * -1)
         else:
             # an equality constraint can be expressed in this manner by squaring the inequality expression
             # See https://pymoo.org/misc/constraints.html for more details
             return (np.sum(x[:, self.index] * [-coeff for coeff in self.coefficients], axis=1) - (self.rhs * -1)) ** 2
 
@@ -158,20 +160,24 @@
 
         """
         if self.constraint_type == "ineq":
             return np.around(np.sum(X[:, self.index] * self.coefficients, axis=1), 4) >= round(float(self.rhs), 4)
         else:
             return np.around(np.sum(X[:, self.index] * self.coefficients, axis=1), 4) == round(float(self.rhs), 4)
 
+    def build_botorch_constraint(self) -> Tuple[Tensor, Tensor, float]:
+        return (torch.tensor(self.index), torch.tensor(self.coefficients), float(self.rhs))
+
 
 @define
-class NonLinearConstraint:
+class NonLinearPowerConstraint:
     """
 
-    Implements a linear constraint on the input variables for the optimisation. For example, linear constraints could be:
+    Implements a linear constraint on the input variables for the optimisation. For example, linear constraints could
+    be:
 
         a(F1)^x + b(F2)^y = 0
         a(F1)^x + b(F2)^y >= 0
 
     where a and b are coefficients, and x and y are powers (exponents) for the features F1 and F2 respectively, and the
     right-hand side of the equation is 0. Using an equals sign, =, would form a linear equality constraint whereas
     defining as 'greater than or equal to' forms an inequality constraint.
@@ -278,15 +284,16 @@
 
         """
         # Un-normalise the variables
         x = (x * (np.array(self.variables.upper_bounds) - np.array(self.variables.lower_bounds))) + np.array(
             self.variables.lower_bounds
         )
 
-        # Multiply coefficients and rhs by -1 because pymoo uses the less than or equal to inequality operator for its constraints
+        # Multiply coefficients and rhs by -1 because pymoo uses the less than or equal to inequality operator for its
+        # constraints
         lhs_eval_list = []
         if self.constraint_type == "ineq":
             for i, c, p in zip(self.index, self.coefficients, self.powers):
                 lhs_eval_list.append((((x[:, i]) ** p) * -c))
 
             return np.sum(lhs_eval_list, axis=0) - (self.rhs * -1)
 
@@ -318,14 +325,310 @@
         if self.constraint_type == "ineq":
             return np.around(np.sum(X[:, self.index] * self.coefficients, axis=1), 4) >= round(float(self.rhs), 4)
         else:
             return np.around(np.sum(X[:, self.index] * self.coefficients, axis=1), 4) == round(float(self.rhs), 4)
 
 
 @define
+class FunctionalConstraint:
+    """
+
+    Implements a constraint on the input variables for the optimisation that is calculated using a pass function. This
+    allows any type of non-linear function to be used. The constraint can be utilised as either an equality or
+    inequality constraint. For example:
+
+        x[0] - sin(x[1]) = 0
+        x[0] - sin(x[1]) >= 0
+
+        def fun(x, **fun_kwargs):
+            return x[0] - np.sin(x[1])
+
+        or
+
+        fun = lambda x: x[0] - np.sin(x[1])
+
+    By default in NEMO, all inequality constraints must be defined as 'greater than or equal to'. Note: This aligns
+    with how constraints are defined in the scipy package, but is the opposite when compared to the pymoo package
+
+    Parameters
+    ----------
+    constraint_type: str
+        Defines whether the linear constraint should be an equality or inequality linear constraint by assigning as
+        either 'eq' or 'ineq' respectively
+    variables: VariablesList
+        VariablesList object that contains information about all variables
+    features: List[str]
+        The name of the features to constrain, e.g. ['F1', 'F2'] for the example equation shown above
+    fun: Callable
+        A callable that calculates the lhs of the constraint by taking the X-values of the constraint, and also any
+        kwargs that are passed using the fun_kwargs
+    rhs: Union[int, float]
+        The value to set for the right-hand side of the equation, e.g. 0 for the example equation shown above
+    fun_kwargs: Dict[str, Any], Deafult = None
+        A dictionary of keyword arguments to use with the passed function, fun
+    """
+
+    constraint_type: str
+    variables: VariablesList
+    features: List[str]
+    fun: Callable
+    rhs: Union[int, float]
+    fun_kwargs: Optional[Dict[str, Any]] = None
+    index: List[int] = field(init=False)
+
+    def __attrs_post_init__(self):
+        self.index = [self.variables.continuous_var_names.index(f) for f in self.features]
+
+        if self.fun_kwargs is None:
+            self.fun_kwargs = {}
+
+    def build_polytope_sampler_constraint(self):
+        raise RuntimeError("The polytope sampler cannot be used with functional constraints")
+
+    def build_scipy_constraint(self, add_to_index: int, num_candidates: int) -> Callable:
+        """
+
+        Creates the constraint function that is supplied into the scipy minimize function
+
+        Parameters
+        ----------
+        add_to_index: int
+            Offsets the position of the feature to account for its position when more than one candidate is desired per
+            iteration from the optimisation. This is offset is required because multiple candidates are supplied to the
+            scipy minimize function in a flattened array
+        num_candidates: int
+            The number of candidates desired per iteration from the optimisation
+
+        Returns
+        -------
+        constraint_fun: Callable
+            Function that can take an X array and is supplied to the scipy minimize function as a constraint
+
+        """
+        new_index = [i + add_to_index for i in self.index]
+
+        def constraint_fun(x: np.ndarray) -> np.ndarray:
+            # Saves the original shape of the X array
+            x_shape = x.shape
+
+            # Reshapes the X array
+            x = x.reshape(num_candidates, -1)
+
+            # Un-normalise the variables
+            x = (x * (np.array(self.variables.upper_bounds) - np.array(self.variables.lower_bounds))) + np.array(
+                self.variables.lower_bounds
+            )
+
+            # Re-shape the X array back to the original shape
+            x = x.reshape(x_shape)
+
+            # Evaluate the X array for the constraint
+            return self.fun(x[:, new_index], **self.fun_kwargs) - self.rhs
+
+        return constraint_fun
+
+    def evaluate_pymoo_constraint(self, x: np.ndarray) -> np.ndarray:
+        """
+
+        Evaluate the X array for the constraint in pymoo
+
+        Parameters
+        ----------
+        x: np.ndarray
+            The X array to be evaluated. Can be more than one row of X-values
+
+        Returns
+        -------
+        np.ndarray:
+            The output value in the array for a given row in the supplied X array will be used by the pymoo package to
+            evaluate whether the constraint was met
+
+
+        """
+        # Un-normalise the variables
+        x = (x * (np.array(self.variables.upper_bounds) - np.array(self.variables.lower_bounds))) + np.array(
+            self.variables.lower_bounds
+        )
+
+        # Multiply coefficients and rhs by -1 because pymoo uses the less than or equal to inequality operator for its
+        # constraints
+        lhs_eval_list = []
+        if self.constraint_type == "ineq":
+            return self.fun(x[:, self.index], **self.fun_kwargs) - (self.rhs * -1)
+
+        else:
+            # an equality constraint can be expressed in this manner by squaring the inequality expression
+            # See https://pymoo.org/misc/constraints.html for more details
+            return (self.fun(x[:, self.index], **self.fun_kwargs) - (self.rhs * -1)) ** 2
+
+    def bool_evaluate_constraint(self, X: np.ndarray) -> np.ndarray:
+        """
+
+        Evaluate whether the constraint is met and returns a boolean array
+
+        Parameters
+        ----------
+        X: np.ndarray
+            The X array to be evaluated that contains the categorical variables in their categorical form (e.g. as
+            categorical level names and not as descriptors for CategoricalVariableWithDescriptors)
+
+        Returns
+        -------
+        np.ndarray:
+            A boolean is returned for all rows in the supplied X array that indicates whether the constraint was met
+
+        """
+        if self.constraint_type == "ineq":
+            return np.around(self.fun(X[:, self.index], **self.fun_kwargs), 4) >= round(float(self.rhs), 4)
+        else:
+            return np.around(self.fun(X[:, self.index], **self.fun_kwargs), 4) == round(float(self.rhs), 4)
+
+
+@define
+class StoichiometricConstraint:
+    """
+
+    Implements a constraint on the input variables for the optimisation for controlling the ratio between two
+    variables. The ratio between the two variables can either be set to be equal to a particular value or the ratio
+    between feature2 to feature 1 to be greater than a particular value
+
+    Parameters
+    ----------
+    constraint_type: str
+        Defines whether the stoichiometric ratio of feature2/feature1 constraint should be exactly the same as the
+        defined ratio or if it can be any value greater than the ratio by assigning as either 'eq' or 'ineq'
+        respectively
+    variables: VariablesList
+        VariablesList object that contains information about all variables
+    feature1: str
+        The name of one of the feature to consider in the constraint, e.g. 'Solvent'
+    feature2: str
+        The name of the other feature to consider in the constraint, e.g. 'Base'
+    ratio: int | float
+        The stoichiometric ratio of feature2/feature1
+
+    """
+
+    constraint_type: str
+    variables: VariablesList
+    feature1: str
+    feature2: str
+    ratio: Union[int, float]
+    index: List[int] = field(init=False)
+
+    def __attrs_post_init__(self):
+        self.index1 = [self.variables.names.index(self.feature1)]
+        self.index2 = [self.variables.names.index(self.feature2)]
+
+    def build_polytope_sampler_constraint(self) -> [Tuple[Tensor, Tensor, float]]:
+        """
+
+        Function that creates the constraint tuple that is used in the polytope sampler
+
+        """
+        raise RuntimeError("The polytope sampler cannot be used with stoichiometric constraints")
+
+    def build_scipy_constraint(self, add_to_index: int, num_candidates: int) -> Callable:
+        """
+
+        Creates the constraint function that is supplied into the scipy minimize function
+
+        Parameters
+        ----------
+        add_to_index: int
+            Offsets the position of the feature to account for its position when more than one candidate is desired per
+            iteration from the optimisation. This is offset is required because multiple candidates are supplied to the
+            scipy minimize function in a flattened array
+        num_candidates: int
+            The number of candidates desired per iteration from the optimisation
+
+        Returns
+        -------
+        constraint_fun: Callable
+            Function that can take an X array and is supplied to the scipy minimize function as a constraint
+
+        """
+        # new_index = [i + add_to_index for i in self.index]
+        #
+        def constraint_fun(x: np.ndarray) -> np.ndarray:
+            # Saves the original shape of the X array
+            x_shape = x.shape
+
+            # Reshapes the X array
+            x = x.reshape(num_candidates, -1)
+
+            # Un-normalise the variables
+            x = (x * (np.array(self.variables.upper_bounds) - np.array(self.variables.lower_bounds))) + np.array(
+                self.variables.lower_bounds
+            )
+
+            # Re-shape the X array back to the original shape
+            x = x.reshape(x_shape)
+
+            # Evaluate the X array for the constraint
+            return (x[:, self.index1 + add_to_index] / x[:, self.index2 + add_to_index]) - self.ratio
+
+        return constraint_fun
+
+    def evaluate_pymoo_constraint(self, x: np.ndarray) -> np.ndarray:
+        """
+
+        Evaluate the X array for the constraint in pymoo
+
+        Parameters
+        ----------
+        x: np.ndarray
+            The X array to be evaluated. Can be more than one row of X-values
+
+        Returns
+        -------
+        np.ndarray:
+            The output value in the array for a given row in the supplied X array will be used by the pymoo package to
+            evaluate whether the constraint was met
+
+
+        """
+        # Un-normalise the variables
+        x = (x * (np.array(self.variables.upper_bounds) - np.array(self.variables.lower_bounds))) + np.array(
+            self.variables.lower_bounds
+        )
+
+        # Multiply coefficients and rhs by -1 because pymoo uses the less than or equal to inequality operator for its
+        # constraints
+        if self.constraint_type == "ineq":
+            return (x[:, self.index1] / x[:, self.index2]) - (self.ratio * -1)
+        else:
+            # an equality constraint can be expressed in this manner by squaring the inequality expression
+            # See https://pymoo.org/misc/constraints.html for more details
+            return ((x[:, self.index1] / x[:, self.index2]) - (self.ratio * -1)) ** 2
+
+    def bool_evaluate_constraint(self, X: np.ndarray) -> np.ndarray:
+        """
+
+        Evaluate whether the constraint is met and returns a boolean array
+
+        Parameters
+        ----------
+        X: np.ndarray
+            The X array to be evaluated that contains the categorical variables in their categorical form (e.g. as
+            categorical level names and not as descriptors for CategoricalVariableWithDescriptors)
+
+        Returns
+        -------
+        np.ndarray:
+            A boolean is returned for all rows in the supplied X array that indicates whether the constraint was met
+
+        """
+        if self.constraint_type == "ineq":
+            return np.around((X[:, self.index1] / X[:, self.index2]), 4) >= round(float(self.rhs), 4)
+        else:
+            return np.around((X[:, self.index1] / X[:, self.index2]), 4) == round(float(self.rhs), 4)
+
+
+@define
 class MaxActiveFeaturesConstraint:
     """
 
     Implements a constraint that limits the number of variables/features that have values greater than 0. For example,
     if max_active = 2, the examples 1 and 2 below would pass the constraint whereas example 3 would fail the
     constraint:
 
@@ -348,14 +651,15 @@
 
     """
 
     variables: VariablesList
     features: List[str]
     max_active: int
     index: List[int] = field(init=False)
+    constraint_type: str = field(init=False)
 
     def __attrs_post_init__(self):
         self.index = [self.variables.continuous_var_names.index(f) for f in self.features]
 
     def build_polytope_sampler_constraint(self):
         raise RuntimeError("The polytope sampler cannot be used with max active number of features constraints")
 
@@ -404,15 +708,16 @@
         np.ndarray:
             The output value in the array for a given row in the supplied X array will be used by the pymoo package to
             evaluate whether the constraint was met
 
 
         """
         # The values in the x array that come from pymoo need to be normalised between 0 and 1
-        # Multiply coefficients and rhs by -1 because pymoo uses the less than or equal to inequality operator for its constraints
+        # Multiply coefficients and rhs by -1 because pymoo uses the less than or equal to inequality operator for its
+        # constraints
         X = np.where(x > 0, 1, 0)
         return np.sum(X[:, self.index], axis=1) - self.max_active
 
     def bool_evaluate_constraint(self, X: np.ndarray) -> np.ndarray:
         """
 
         Evaluate whether the constraint is met and returns a boolean array
@@ -437,15 +742,15 @@
 class CategoricalConstraint:
     """
 
     Implements a constraint that prevents chosen categorical levels (e.g. chemicals) from two variables/features from
     being simultaneously selected. For example, the examples 1 and 2 below would pass the constraint whereas examples
     3 and 4 would fail the constraint:
 
-        - Exampler where variables at indexes 0 and 1 are 'Solvent' and 'Base' respectively
+        - Example where variables at indexes 0 and 1 are 'Solvent' and 'Base' respectively
         - In the 'Solvent' variable, the categorical level called 'Water' cannot be selected at the same time as
         categorical levels called 'Sodium' or 'Potassium' in the 'Base' variable
 
         1. X = ['Water', 'Triethylamine'] -> Pass
         2. X = ['Toluene', 'Sodium'] -> Pass
         3. X = ['Water', 'Sodium'] -> Fail
         4. X = ['Water', 'Potassium'] -> Fail
@@ -454,33 +759,40 @@
     ----------
     variables: VariablesList
         VariablesList object that contains information about all variables
     feature1: str
         The name of one of the feature to consider in the constraint, e.g. 'Solvent'
     feature2: str
         The name of the other feature to consider in the constraint, e.g. 'Base'
-    categorical_levels1: List[Union[str, int, float]]
+    categorical_levels1: List[str | int | float]
         The categorical levels in feature1 that cannot be simultaneously selected with categorical levels in feature2,
         e.g. ['Water']
-    categorical_levels2: List[Union[str, int, float]]
+    categorical_levels2: List[str | int | float]
         The categorical levels in feature2 that cannot be simultaneously selected with categorical levels in feature1,
         e.g. ['Sodium', 'Potassium']
 
     """
 
     variables: VariablesList
     feature1: str
     feature2: str
     categorical_levels1: List[Union[str, int, float]]
     categorical_levels2: List[Union[str, int, float]]
-    index: List[int] = field(init=False)
+    index1: int = field(init=False)
+    index2: int = field(init=False)
 
     def __attrs_post_init__(self):
-        self.index1 = [self.variables.names.index(self.feature1)]
-        self.index2 = [self.variables.names.index(self.feature2)]
+        self.index1 = self.variables.names.index(self.feature1)
+        self.index2 = self.variables.names.index(self.feature2)
+
+        if not isinstance(self.variables.variables[self.index1], CategoricalVariable):
+            raise TypeError(f"The variable {self.feature1} is not a categorical variable")
+
+        if not isinstance(self.variables.variables[self.index2], CategoricalVariable):
+            raise TypeError(f"The variable {self.feature2} is not a categorical variable")
 
     def build_polytope_sampler_constraint(self):
         raise RuntimeError("The polytope sampler cannot be used with categorical constraints")
 
     def build_scipy_constraint(self, add_to_index: int, num_candidates: int) -> Callable:
         """
 
@@ -552,16 +864,16 @@
 
         """
         # Un-normalise the variables
         x = (x * (np.array(self.variables.upper_bounds) - np.array(self.variables.lower_bounds))) + np.array(
             self.variables.lower_bounds
         )
 
-        # Converts the descriptor values generated by the scipy minimize function into the categorical level that
-        # is the closest by Euclidean distance
+        # Converts the descriptor values generated by pymoo into the categorical level that is the closest by
+        # Euclidean distance
         x = self.variables.descriptor_to_name(x)
 
         # Checks if the forbidden categorical levels are in the chosen features
         for row_index, (x1, x2) in enumerate(zip(x[:, self.index1], x[:, self.index2])):
             if x1 in self.categorical_levels1:
                 x[row_index, self.index1] = 1
             if x2 in self.categorical_levels2:
@@ -605,15 +917,24 @@
     Parameters
     ----------
     constraints: List[Union[LinearConstraint, NonLinearConstraint, MaxActiveFeaturesConstraint, CategoricalConstraint]]
         List of all constraints
 
     """
 
-    constraints: List[Union[LinearConstraint, NonLinearConstraint, MaxActiveFeaturesConstraint, CategoricalConstraint]]
+    constraints: List[
+        Union[
+            LinearConstraint,
+            NonLinearPowerConstraint,
+            FunctionalConstraint,
+            StoichiometricConstraint,
+            MaxActiveFeaturesConstraint,
+            CategoricalConstraint,
+        ]
+    ]
     n_constr: int = field(init=False)
     variables: VariablesList = field(init=False)
 
     def __attrs_post_init__(self):
         self.n_constr = len(self.constraints)
         self.variables = self.constraints[0].variables
 
@@ -638,22 +959,29 @@
         scipy_constraints = []
         for constr in self.constraints:
             for candidate_number in range(num_candidates):
                 if not isinstance(constr, CategoricalConstraint):
                     add_to_index = candidate_number * constr.variables.n_var
                 else:
                     add_to_index = candidate_number * len(constr.variables.variables)
-                scipy_constraints.append(
-                    {
+                if (
+                    isinstance(constr, LinearConstraint)
+                    or isinstance(constr, NonLinearPowerConstraint)
+                    or isinstance(constr, FunctionalConstraint)
+                    or isinstance(constr, StoichiometricConstraint)
+                ):
+                    constraint = {
                         "type": constr.constraint_type,
-                        "fun": constr.build_scipy_constraint(add_to_index, num_candidates)
-                        if not isinstance(constr, MaxActiveFeaturesConstraint)
-                        else constr.build_scipy_constraint(add_to_index),
+                        "fun": constr.build_scipy_constraint(add_to_index, num_candidates),
                     }
-                )
+                elif isinstance(constr, MaxActiveFeaturesConstraint):
+                    constraint = {"type": "ineq", "fun": constr.build_scipy_constraint(add_to_index)}
+                elif isinstance(constr, CategoricalConstraint):
+                    constraint = {"type": "ineq", "fun": constr.build_scipy_constraint(add_to_index, num_candidates)}
+                scipy_constraints.append(constraint)
 
         return scipy_constraints
 
     def bool_evaluate_constraints(self, X: np.ndarray) -> np.ndarray:
         """
 
         Evaluate whether all constraints are met and returns a boolean array
@@ -682,7 +1010,16 @@
                 pass_fail[:, constr_index] = constr.bool_evaluate_constraint(X)
             else:
                 # CategoricalConstraint requires all descriptors that are part of CategoricalVariableWithDescriptors
                 # variables to be converted to their categorical level name
                 pass_fail[:, constr_index] = constr.bool_evaluate_constraint(self.variables.descriptor_to_name(X))
 
         return np.all(pass_fail, axis=1)
+
+    def create_botorch_constraints(self, constraint_type: str) -> List[Tuple[Tensor, Tensor, float]]:
+        constraints_list = []
+        for constr_index, constr in enumerate(self.constraints):
+            if isinstance(constr, LinearConstraint):
+                if constr.constraint_type == constraint_type:
+                    constraints_list.append(constr.build_botorch_constraint())
+
+        return constraints_list
```

### Comparing `nemo-bo-0.1.8/nemo_bo/opt/objectives.py` & `nemo-bo-0.1.9/nemo_bo/opt/objectives.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 from sklearn.preprocessing import MinMaxScaler, StandardScaler
 
 import nemo_bo.utils.logger as logging_nemo
 import nemo_bo.utils.perf_metrics as pm
 import nemo_bo.utils.plotter as plotter
 from nemo_bo.models.base.available_models import create_predictor_list
 from nemo_bo.models.base.base_model import Base_Model
+from nemo_bo.models.nn_bayesian import NNBayesianModel
+from nemo_bo.models.nn_concrete import NNConcreteDropoutModel
 from nemo_bo.opt.variables import VariablesList
 from nemo_bo.utils.data_proc import sort_train_test_split_shuffle, remove_nan
-from nemo_bo.utils.transformations import Transformations
 
 try:
     logging_nemo.logging_path
     logger = logging_nemo.logging_nemo_child(os.path.basename(__file__))
 except AttributeError:
     logger = logging_nemo.logging_nemo_master(os.path.basename(__file__))
 
@@ -39,99 +40,113 @@
         Name of the objective
     obj_max_bool: bool
         Whether the objective is to be maximised (True) or minimised (False)
     lower_bound: int | float
         The lower bound of the objective
     upper_bound: int | float
         The upper bound of the objective
-    transformation_type: str. Default = None
-        The type of transformation that should be applied to the objective for modelling. When left as the default
-        None, the modelling uses the default transformations specified by the model type. When specified, can be
-        "normalisation", "standardisation", or "none" for min-max normalisation, standardisation to a mean of 0 and a
-        standard deviation of 1, or no transformation respectively
+    transformer: Optional. Default = None
+        The transformation that will be applied to the objective for modelling. When left as the default
+        None, the modelling uses the default transformations specified by the model type. Can be specified as the
+        strings "normalisation", "standardisation", or "none" for min-max normalisation, standardisation to a mean of 0
+        and a standard deviation of 1, or no transformation respectively. Alternatively, a class instance with
+        fit_transform, transform, and inverse_transform functions, such as a scikit-learn transformer can be provided
+        directly too.
     units: str, Default = ""
         The units for the objective
 
     """
 
     name: str
     obj_max_bool: bool
     lower_bound: Union[int, float]
     upper_bound: Union[int, float]
-    transformation_type: Optional[str] = None
+    transformer: Optional = None
     units: str = ""
 
     def transform(self, Y: np.ndarray) -> np.ndarray:
         """
 
-        Fit the transformation scalar to the inputted Y array when self.transformation_type is "normalisation" or
-        "standardisation". The Y array is subsequently transformed according to the fit scalar. When
-        self.transformation_type = "none", no transformation occurs
+        Fits a transformation scalar to the inputted Y array when self.transformer is "normalisation",
+        "standardisation" or a transformer object. The Y array is subsequently transformed according to the
+        fitted scalar. When self.transformer = "none", no transformation occurs
 
         Parameters
         ----------
         Y: np.ndarray
             Y array containing untransformed values for one objective
 
         """
-        if self.transformation_type is None:
+        if self.transformer is None:
             raise AttributeError(
-                "Please either: 1. Fit the model first, or 2. Set transformation_type = 'none', 'normalisation', or 'standarisation' when creating the objective instance"
+                "Please either: 1. Fit the model first, 2. Set transformer = 'none', 'normalisation', or "
+                "'standarisation' when creating the variable instance, or 3. Pass a transformer such as a scikit-learn "
+                "transformer when creating the variable instance"
             )
 
-        if self.transformation_type == "none":
+        if Y.ndim == 1:
+            Y = Y.reshape(-1, 1)
+
+        if self.transformer == "none":
             return Y
-        self.transformations = Transformations()
-        if self.transformation_type == "normalisation":
-            return self.transformations.minmaxscaler(Y)
-        elif self.transformation_type == "standardisation":
-            return self.transformations.standardscaler(Y)
+        elif self.transformer == "normalisation":
+            self.transformer = MinMaxScaler()
+        elif self.transformer == "standardisation":
+            self.transformer = StandardScaler()
+
+        return self.transformer.fit_transform(Y)
 
     def transform_only(self, Y: np.ndarray) -> np.ndarray:
         """
 
-        The Y array is transformed according to the fit scalar in the self.transformations object. When
-        self.transformation_type = "none", no transformation occurs
+        The Y array is transformed according to the fit scalar in the self.transformer object. When
+        self.transformer = "none", no transformation occurs
 
         Parameters
         ----------
         Y: np.ndarray
             Y array containing untransformed values for one objective
 
         """
-        if self.transformation_type is None:
+
+        if Y.ndim == 1:
+            Y = Y.reshape(-1, 1)
+
+        if self.transformer is None:
             raise AttributeError(
-                "Please either: 1. Fit the model first, or 2. Set transformation_type = 'none', 'normalisation', or 'standarisation' when creating the objective instance"
+                "Please either: 1. Fit the model first, 2. Set transformer = 'none', 'normalisation', or "
+                "'standarisation' when creating the variable instance, or 3. Pass a transformer such as a scikit-learn "
+                "transformer when creating the variable instance"
             )
 
-        if self.transformation_type == "none":
+        if self.transformer == "none":
             return Y
-        if self.transformation_type == "normalisation":
-            return self.transformations.minmaxscaler_transform_only(Y)
-        elif self.transformation_type == "standardisation":
-            return self.transformations.standardscaler_transform_only(Y)
+        else:
+            return self.transformer.transform(Y)
 
     def inverse_transform(self, Y_transform: np.ndarray) -> np.ndarray:
         """
 
-        The Y_transform array undergoes an inverse transform according to the fit scalar in the self.transformations
-        object. When self.transformation_type = "none", no transformation occurs
+        The Y_transform array undergoes an inverse transform according to the fit scalar in the self.transformer
+        object. When self.transformer = "none", no transformation occurs
 
         Parameters
         ----------
         Y_transform: np.ndarray
             Y array containing transformed values for one objective
 
         """
-        if self.transformation_type == "none":
+
+        if Y_transform.ndim == 1:
+            Y_transform = Y_transform.reshape(-1, 1)
+
+        if self.transformer == "none":
             return Y_transform
-        if isinstance(self.transformations.scaler, MinMaxScaler):
-            return self.transformations.inverse_minmaxscaler(Y_transform)
-        elif isinstance(self.transformations.scaler, StandardScaler):
-            return self.transformations.inverse_standardscaler(Y_transform)
+        else:
+            return self.transformer.inverse_transform(Y_transform)
 
 
 @define(kw_only=True)
 class RegressionObjective(Objective):
     """
 
     Class for an objective to be modelled using a regression machine learning model
@@ -142,19 +157,21 @@
         Name of the objective
     obj_max_bool: bool
         Whether the objective is to be maximised (True) or minimised (False)
     lower_bound: int | float
         The lower bound of the objective
     upper_bound: int | float
         The upper bound of the objective
-    transformation_type: str. Default = None
-        The type of transformation that should be applied to the objective for modelling. When left as the default
-        None, the modelling uses the default transformations specified by the model type. When specified, can be
-        "normalisation", "standardisation", or "none" for min-max normalisation, standardisation to a mean of 0 and a
-        standard deviation of 1, or no transformation respectively
+    transformer: Optional. Default = None
+        The transformation that should be applied to the objective for modelling. When left as the default
+        None, the modelling uses the default transformations specified by the model type. Can be specified as the
+        strings "normalisation", "standardisation", or "none" for min-max normalisation, standardisation to a mean of 0
+        and a standard deviation of 1, or no transformation respectively. Alternatively, a class instance with
+        fit_transform, transform, and inverse_transform functions, such as a scikit-learn transformer can be provided
+        directly too.
     units: str, Default = ""
         The units for the objective
     predictor_type: str | Base_Model | List[str | Base_Model], Default = None
         Specifies the type of predictor/model to use for the objective. If unspecified, it will use all of the default
         predictors/models built-in NEMO
     predictor_params_dict: Dict[str, Dict[str, Callable]], Default = None
         Specifies the predictor/model hyperparameters to optimise during model fitting using the HyperOpt package.
@@ -177,25 +194,21 @@
 
     predictor_type: Optional[Union[str, Base_Model, List[Union[str, Base_Model]]]] = None
     predictor_params_dict: Optional[Dict[str, Dict[str, Callable]]] = None
     gp_kernel_choices: Optional[list] = None
     model_params: Optional[Dict[str, Any]] = None
     hyperopt_evals: Optional[Dict[str, int]] = None
     input_predictor_type: str = field(init=False)
-    # input_predictor_params_dict: Dict[str, Dict[str, Callable]] = field(init=False)
     obj_function: Base_Model = field(init=False)
     permutation_feature_importance: pd.Series = field(init=False)
-    transformations: Transformations = field(init=False)
 
     def __attrs_post_init__(self):
         self.input_predictor_type = self.predictor_type = create_predictor_list(self.predictor_type)
-        # self.input_predictor_params_dict = self.predictor_params_dict
         self.obj_function = None
         self.permutation_feature_importance = None
-        self.transformations = None
 
     def fit_regressor(
         self, X: np.ndarray, Y: np.ndarray, variables: VariablesList, test_ratio: Optional[float] = 0.2, **kwargs
     ) -> None:
         """
 
         Fits regression objectives to a specific predictor/model type (self.predictor_type) and defined model
@@ -217,17 +230,14 @@
 
         """
         X, Y = remove_nan(X, Y)
 
         self.obj_function = self.predictor_type(variables, self)
         self.obj_function.fit(X, Y, test_ratio=test_ratio, **self.model_params, **kwargs)
 
-        # Calculate permutation feature importance
-        (self.permutation_feature_importance, _,) = self.obj_function.permutation_feature_importance_continuous(X, Y)
-
     def predict(self, X: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
         """
 
         Returns the untransformed predicted mean and standard deviation using the fitted machine learning models at
         the X values
 
         Parameters
@@ -245,14 +255,35 @@
             The untransformed predicted standard deviations using the fitted machine learning models at the X values
 
         """
         Y_pred, Y_pred_stddev = self.obj_function.predict(X)
 
         return Y_pred.astype("float"), Y_pred_stddev.astype("float")
 
+    def draw_samples(self, X: np.ndarray) -> np.ndarray:
+        """
+
+        Generates samples from a normal distribution using the X array
+
+        Parameters
+        ----------
+        X: np.ndarray
+            X array that contains the unprocessed variables data to be fitted to the model, i.e. The data has not yet
+            undergone any transformations related to converted categorical variables to their respective descriptors
+            or transformations related to standardisation/normalisation
+
+        Returns
+        -------
+        np.ndarray
+            Drawn samples using the model and the inputted X array. The outputted values have been un-transformed
+
+        """
+
+        return self.obj_function.draw_samples(X).astype("float")
+
     def model_and_hyperparameter_opt(
         self,
         X: np.ndarray,
         Y: np.ndarray,
         variables: VariablesList,
         model_search_bool: bool,
         test_ratio: Optional[float] = None,
@@ -275,42 +306,47 @@
         model_search_bool: bool
             Whether automated model and hyperparameter optimisation is to be performed during fitting the regression
             models
         test_ratio: float, Default = 0.2,
             The proportion of inputted X and Y arrays to be split for the validation and test sets where applicable
         test_data: List[np.ndarray], Default = None,
             Test data to use for the initial model and hyperparameter optimisation, instead of creating it
-            automatically. The X array is at index 0 and the Y array is at index 1
+            automatically from the provided X and Y arrays. The test X array is at index 0 and the test Y array is at
+            index 1
 
         """
         X, Y = remove_nan(X, Y)
 
         if model_search_bool:
             test_loss_list = []
             model_list = []
             model_params_list = []
 
             if test_data is None:
                 # Splits the dataset to create training and test datasets
                 if test_ratio is None:
                     test_ratio = 0.2
                 if kwargs.get("sort_before_split", True):
-                    (X_train, X_test, Y_train, Y_test,) = sort_train_test_split_shuffle(
-                        X, Y, test_ratio=test_ratio, seed=1
-                    )
+                    (
+                        X_train,
+                        X_test,
+                        Y_train,
+                        Y_test,
+                    ) = sort_train_test_split_shuffle(X, Y, test_ratio=test_ratio, seed=1)
                 else:
                     X_train, X_test, Y_train, Y_test = train_test_split(X, Y, test_size=test_ratio, random_state=1)
             else:
                 # Uses the supplied test dataset
                 X_train = X
                 X_test = test_data[0]
                 Y_train = Y
                 Y_test = test_data[1]
 
-            # Performs hyperopt for each predictor type passed into this function and appends each respective best model and hyperparameters
+            # Performs hyperopt for each predictor type passed into this function and appends each respective best
+            # model and hyperparameters
             for predictor_class in self.input_predictor_type:
                 predictor_instance = predictor_class(variables, self)
                 model, model_params = predictor_instance.hyperparam_opt(
                     X_train, Y_train, test_ratio, predictor_params_dict=self.predictor_params_dict, **kwargs
                 )
                 model_list.append(model)
                 model_params_list.append(model_params)
@@ -322,24 +358,29 @@
                 test_loss_list.append(dict["RMSE"])
 
             # Identifies which predictor type had the most accurate test set prediction
             best_index = test_loss_list.index(min(test_loss_list))
             self.predictor_type = self.input_predictor_type[best_index]
             self.model_params = model_params_list[best_index]
 
-        # The always_hyperparam_opt attribute is from the predictor/model. When True, the identified previously best
+        # The always_hyperparam_opt attribute is from the predictor/model. When True, the previously identified best
         # predictor type undergoes hyperparameter optimisation every Bayesian optimisation iteration
         elif self.obj_function.always_hyperparam_opt:
             # No model search; only hyperopt for the current best predictor type (identified previously)
             predictor_instance = self.predictor_type(variables, self)
             _, self.model_params = predictor_instance.hyperparam_opt(
                 X, Y, test_ratio, predictor_params_dict=self.predictor_params_dict, **kwargs
             )
 
         # Re-fits the model but with the complete dataset
+        # If test data was supplied, it is appended to the training data for the final model fitting
+        if test_data is not None:
+            X = np.vstack((X, X_test))
+            Y = np.vstack((Y, Y_test))
+
         self.fit_regressor(X, Y, variables, test_ratio=test_ratio, **kwargs)
 
     def parity_plot(self) -> None:
         """
 
         Creates a parity plot for evaluating the fit quality of the regression model for the objective
 
@@ -367,21 +408,27 @@
                 [min_parity, min_parity],
                 [max_parity, max_parity],
             ]
             scatter_legend = (
                 f"Train ({train_paritydata.shape[0]} experiments) (95% CI)",
                 f"Validation ({val_paritydata.shape[0]} experiments) (95% CI)",
             )
-            plot_title = f"{self.name} Parity Plot ({self.obj_function.name} Model)\nTrain RMSE = {round(train_rmse.astype('float'), 2)} {self.units}, Train r2 = {round(train_r2, 2)}, \nValidation RMSE = {round(val_rmse.astype('float'), 2)} {self.units}, Validation r2 = {round(val_r2, 2)}"
+            plot_title = (
+                f"{self.name} Parity Plot ({self.obj_function.name} Model)\nTrain RMSE = "
+                f"{round(train_rmse.astype('float'), 2)} {self.units}, Train r2 = {round(train_r2, 2)}, \n"
+                f"Validation RMSE = {round(val_rmse.astype('float'), 2)} {self.units}, Validation r2 = "
+                f"{round(val_r2, 2)}"
+            )
             path = os.path.join(os.getcwd(), "ML Models", f"{self.obj_function.name}", "Parity Plots")
             if not os.path.exists(path):
                 os.makedirs(path)
             output_file = os.path.join(
                 path,
-                rf"{self.name} Parity Plot ({self.obj_function.name} Model), {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}",
+                rf"{self.name} Parity Plot ({self.obj_function.name} Model), "
+                rf"{datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}",
             )
 
         else:
             train_paritydata = self.obj_function.performance_metrics["Parity Data"]
             train_rmse = self.obj_function.performance_metrics["RMSE"]
             train_r2 = self.obj_function.performance_metrics["r2"]
             scatter_parity_data = train_paritydata
@@ -390,32 +437,36 @@
             min_parity = np.amin(np.vstack([train_paritydata]))
             # Array for the x = y line in the parity plot
             x_equals_y = [
                 [min_parity, min_parity],
                 [max_parity, max_parity],
             ]
             scatter_legend = f"Train ({train_paritydata.shape[0]} experiments) (95% CI)"
-            plot_title = f"{self.name} Parity Plot ({self.obj_function.name} Model)\nRMSE = {round(train_rmse.astype('float'), 2)} {self.units}, r2 = {round(train_r2, 2)}"
+            plot_title = (
+                f"{self.name} Parity Plot ({self.obj_function.name} Model)\nRMSE = "
+                f"{round(train_rmse.astype('float'), 2)} {self.units}, r2 = {round(train_r2, 2)}"
+            )
             path = os.path.join(os.getcwd(), "ML Models", f"{self.obj_function.name}", "Parity Plots")
             if not os.path.exists(path):
                 os.makedirs(path)
             output_file = os.path.join(
                 path,
-                rf"{self.name} Parity Plot ({self.obj_function.name} Model), {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}",
+                rf"{self.name} Parity Plot ({self.obj_function.name} Model), "
+                rf"{datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}",
             )
 
         plotter.plot(
             plot_dim="2D",
             scatter_data=scatter_parity_data,
             error=error,
             line_data=x_equals_y,
             scatter_legend=scatter_legend,
             line_legend="x = y",
-            xlabel=f"Actual {self.name} ({self.units})",
-            ylabel=f"Predicted {self.name} ({self.units})",
+            xlabel=f"Actual {self.name} ({self.units})" if self.units != "" else f"Actual {self.name}",
+            ylabel=f"Predicted {self.name} ({self.units})" if self.units != "" else f"Actual {self.name}",
             plottitle=plot_title,
             output_file=output_file,
         )
         plt.close()
 
     def partial_dependence_plot(self, X: np.ndarray) -> Dict[str, pd.DataFrame]:
         """
@@ -463,15 +514,21 @@
         Dict[str, Any]
         Dictionary containing the models, their respective prediction quality for all k-folds and average cv statistics
         across all k-folds
 
         """
         X, Y = remove_nan(X, Y)
 
-        cv_results = self.obj_function.cv(X, Y, self.model_params, test_ratio=test_ratio, **kwargs,)
+        cv_results = self.obj_function.cv(
+            X,
+            Y,
+            self.model_params,
+            test_ratio=test_ratio,
+            **kwargs,
+        )
 
         return cv_results
 
     def y_scrambling_cv(
         self,
         X: np.ndarray,
         Y: np.ndarray,
@@ -537,14 +594,15 @@
     obj_function_data: Any
         Information that is required for the evaluate function
 
     """
 
     def __init__(self, obj_function_data: Optional[Any] = None):
         self.obj_function_data = obj_function_data
+        self.name = "deterministic_function"
 
     def evaluate(self, X: np.ndarray, *args, **kwargs) -> Tuple[np.ndarray, np.ndarray]:
         """
 
         The script to calculate and return the corresponding output values and standard deviations using the inputted
         X array
 
@@ -571,19 +629,21 @@
         Name of the objective
     obj_max_bool: bool
         Whether the objective is to be maximised (True) or minimised (False)
     lower_bound: int | float
         The lower bound of the objective
     upper_bound: int | float
         The upper bound of the objective
-    transformation_type: str. Default = None
-        The type of transformation that should be applied to the objective for modelling. When left as the default
-        None, the modelling uses the default transformations specified by the model type. When specified, can be
-        "normalisation", "standardisation", or "none" for min-max normalisation, standardisation to a mean of 0 and a
-        standard deviation of 1, or no transformation respectively
+    transformer: Optional. Default = None
+        The transformation that should be applied to the objective for modelling. When left as the default
+        None, the modelling uses the default transformations specified by the model type. Can be specified as the
+        strings "normalisation", "standardisation", or "none" for min-max normalisation, standardisation to a mean of 0
+        and a standard deviation of 1, or no transformation respectively. Alternatively, a class instance with
+        fit_transform, transform, and inverse_transform functions, such as a scikit-learn transformer can be provided
+        directly too.
     units: str, Default = ""
         The units for the objective
     obj_function: DeterministicFunction, Default = None
         Contains the information and script to calculate the output values and standard deviations of the calculable
         objective.
 
     """
@@ -611,14 +671,36 @@
             objectives
 
         """
         Y, Y_stddev = self.obj_function.evaluate(X, *args, **kwargs)
 
         return Y.astype("float"), Y_stddev
 
+    def draw_samples(self, X: np.ndarray, *args, **kwargs) -> np.ndarray:
+        """
+
+        Generates samples from a normal distribution when the X array passed
+
+        Parameters
+        ----------
+        X: np.ndarray
+            X array that contains the unprocessed variables data to be fitted to the model, i.e. The data has not yet
+            undergone any transformations related to converted categorical variables to their respective descriptors
+            or transformations related to standardisation/normalisation
+
+        Returns
+        -------
+        np.ndarray
+            Drawn samples using the model and the inputted X array. The outputted values have been un-transformed
+
+        """
+        Y_pred, Y_pred_stddev = self.calculate(X, *args, **kwargs)
+
+        return np.random.default_rng().normal(Y_pred, Y_pred_stddev).astype("float")
+
     def add_obj_function(self, obj_function: DeterministicFunction) -> None:
         """
 
         If the extract_excel functionality was used to import a calculable objective, this function can be used to add
         the calculable objective information and script
 
         Parameters
@@ -654,15 +736,18 @@
 
     def __attrs_post_init__(self):
         self.n_obj = len(self.objectives)
         self.names = [obj.name for obj in self.objectives]
         self.units = [obj.units for obj in self.objectives]
         self.max_bool_dict = {obj.name: obj.obj_max_bool for obj in self.objectives}
         self.bounds = np.array(
-            [[obj.lower_bound for obj in self.objectives], [obj.upper_bound for obj in self.objectives],]
+            [
+                [obj.lower_bound for obj in self.objectives],
+                [obj.upper_bound for obj in self.objectives],
+            ]
         ).T
         self.predictor_types = {}
 
     def fit(
         self,
         X: np.ndarray,
         Y: np.ndarray,
@@ -691,15 +776,16 @@
         model_search_bool: bool
             Whether automated model and hyperparameter optimisation is to be performed during fitting the regression
             models
         test_ratio: float, Default = 0.2,
             The proportion of inputted X and Y arrays to be split for the validation and test sets where applicable
         test_data: List[np.ndarray], Default = None,
             Test data to use for the initial model and hyperparameter optimisation, instead of creating it
-            automatically. The X array is at index 0 and the Y array is at index 1
+            automatically from the provided X and Y arrays. The test X array is at index 0 and the test Y array is at
+            index 1
 
         """
         if model_search_bool is None:
             model_search_bool = kwargs.get("model_search_bool", False)
 
         # Fit the ML regression models
         for obj_index, obj in enumerate(self.objectives):
@@ -710,17 +796,20 @@
                     variables,
                     model_search_bool=model_search_bool,
                     test_ratio=test_ratio,
                     test_data=test_data,
                     **kwargs,
                 )
                 self.predictor_types[self.names[obj_index]] = self.objectives[obj_index].obj_function.name
+
             else:
                 self.predictor_types[self.names[obj_index]] = "calculable objective"
 
+        logger.info(f"The identified best objective functions: {self.predictor_types}")
+
     def evaluate(self, X: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
         """
 
         Function that uses the inputted X array to predict the RegressionObjective and/or calculate the
         CalculableObjective outputs
 
         Parameters
@@ -780,14 +869,61 @@
         partial_dependence_plots_dict = {}
         for obj in self.objectives:
             if isinstance(obj, RegressionObjective):
                 partial_dependence_plots_dict[obj.name] = obj.partial_dependence_plot(X)
 
         return partial_dependence_plots_dict
 
+    def feature_importance(
+        self, X: np.ndarray, Y: np.ndarray, transform_cat_to_cont: bool = True
+    ) -> Dict[str, pd.Series]:
+        """
+
+        Returns a dictionary that shows the permutation feature importance for every machine learning model
+
+        Parameters
+        ----------
+        X: np.ndarray,
+            X array that contains the unprocessed variables data to be fitted to the model, i.e. The data has not yet
+            undergone any transformations related to converted categorical variables to their respective descriptors
+            or transformations related to standardisation/normalisation
+        Y: np.ndarray,
+            Y array that contains the unprocessed objective data, i.e. The data has not yet undergone any
+            transformations related to standardisation/normalisation
+        transform_cat_to_cont: bool, Default = True
+            If True, the permutation feature importance will be calculated for every descriptor of the
+            CategoricalVariableWithDescriptors variables. When False, the permutation feature importance will be
+            calculated for the categorical level directly
+
+        Returns
+        -------
+        feature_importance_dict: Dict[str, pd.Series]
+            Dictionary where the keys are the names of the objectives and the values are a pd.Series of the permutation
+            feature importance for every feature
+
+        """
+        feature_importance_dict = {}
+        for obj in self.objectives:
+            if isinstance(obj, RegressionObjective):
+                # Calculate permutation feature importance
+                if isinstance(obj.predictor_type, NNBayesianModel) or isinstance(
+                    obj.predictor_type, NNConcreteDropoutModel
+                ):
+                    repeats = 20
+                else:
+                    repeats = 50
+
+                (obj.permutation_feature_importance, _,) = obj.obj_function.permutation_feature_importance(
+                    X, Y, repeats=repeats, transform_cat_to_cont=transform_cat_to_cont
+                )
+
+                feature_importance_dict[obj.name] = obj.permutation_feature_importance
+
+        return feature_importance_dict
+
     def cv(self, X: np.ndarray, Y: np.ndarray, test_ratio: float = 0.2, **kwargs) -> Dict[str, Dict[str, Any]]:
         """
 
         Function that is called to start the cross validation procedure for every regression objective using their
         respective fitted model hyperparameters and returns a dictionary containing the fitting results with emphasis
         on the test results for each. The number of k-folds is determined by the reciprocal of the test_ratio
 
@@ -895,16 +1031,41 @@
         the calculable objective information and script to the named calculable objective
 
         Parameters
         ----------
         name: str
             Name of the calculable objective to add the obj_function data to
         obj_function: DeterministicFunction
-            Contains the information and script to calculate the output values and standard deviations of the calculable
-            objective
+            Contains the information and script to calculate the output values and standard deviations of the
+            calculable objective
 
         """
         for obj in self.objectives:
             if isinstance(obj, CalculableObjective):
                 if name == obj.name:
                     obj.obj_function = obj_function
                     break
+
+    def draw_samples(self, X: np.ndarray) -> np.ndarray:
+        """
+
+        Function that uses the inputted X array to draw samples from the distributions of the RegressionObjective
+        and/or CalculableObjective outputs
+
+        Parameters
+        ----------
+        X: np.ndarray
+            X array that contains the unprocessed variables data to be fitted to the model, i.e. The data has not yet
+            undergone any transformations related to converted categorical variables to their respective descriptors
+            or transformations related to standardisation/normalisation
+
+        Returns
+        -------
+        Y: np.ndarray
+            The output values obtained from the regression and/or calculable objectives
+
+        """
+        Y = np.zeros((X.shape[0], len(self.objectives)), dtype=np.float64)
+        for obj_index, obj in enumerate(self.objectives):
+            Y[:, obj_index] = obj.draw_samples(X)
+
+        return Y.astype("float")
```

### Comparing `nemo-bo-0.1.8/nemo_bo/opt/optimisation.py` & `nemo-bo-0.1.9/nemo_bo/opt/optimisation.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,22 +7,25 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import torch
 from botorch.utils.multi_objective.hypervolume import Hypervolume
 from botorch.utils.multi_objective.pareto import is_non_dominated
-from gpytorch.kernels import AdditiveStructureKernel
+from gpytorch.kernels import AdditiveStructureKernel, Kernel, MaternKernel, ScaleKernel
+from gpytorch.priors.torch_priors import GammaPrior
 
 import nemo_bo.utils.logger as logging_nemo
 import nemo_bo.utils.plotter as plotter
 from nemo_bo.acquisition_functions.base_acq_function import AcquisitionFunction
 from nemo_bo.acquisition_functions.expected_improvement.expected_improvement import ExpectedImprovement
-from nemo_bo.opt.benchmark import Benchmark, ModelBenchmark, SyntheticBenchmark
+from nemo_bo.acquisition_functions.highest_uncertainty.highest_uncertainty import HighestUncertainty
+from nemo_bo.opt.benchmark import Benchmark, ModelBenchmark
 from nemo_bo.opt.constraints import ConstraintsList
+from nemo_bo.models.base.available_models import create_predictor_list
 from nemo_bo.opt.objectives import ObjectivesList, RegressionObjective
 from nemo_bo.opt.samplers import LatinHyperCubeSampling, PoolBased, SampleGenerator
 from nemo_bo.opt.variables import VariablesList
 from nemo_bo.utils.data_proc import remove_nan, remove_all_nan_rows
 
 try:
     logging_nemo.logging_path
@@ -48,39 +51,46 @@
         Specifies the method used to suggest new candidates
     sampler: SampleGenerator, PoolBased, Default = None
         Specifies the method to obtain samples, either using a generator or from a sample pool
     constraints: ConstraintsList, Default = None
         ConstraintsList object that contains information about all constraints
     benchmark_func: Benchmark, Default = None
         Provides a method to predict the outcome of the suggested candidates made by the acquisition function when a
-        simulated optimisation is being performed
+        simulated optimisation is being performed. If the benchmark provided is a ModelBenchmark object, please ensure
+        that it has been fitted first
+    opt_name: str, Default = None
+        The name of the sub-folder to save the optimisation data inside
 
     """
 
     variables: VariablesList
     objectives: ObjectivesList
     acquisition_func: AcquisitionFunction
     sampler: Optional[Union[SampleGenerator, PoolBased]] = None
     constraints: Optional[ConstraintsList] = None
     benchmark_func: Optional[Benchmark] = None
+    opt_name: Optional[str] = None
     optimisation_dict: Dict[str, Any] = field(init=False)
     X_columns: List[str] = field(init=False)
     Y_columns: List[str] = field(init=False)
     X: np.ndarray = field(init=False)
     Y: np.ndarray = field(init=False)
     optimisation_only: pd.DataFrame = field(init=False)
     selected_X: np.ndarray = field(init=False)
     selected_Y: np.ndarray = field(init=False)
 
     def __attrs_post_init__(self):
-        if isinstance(self.acquisition_func, ExpectedImprovement) and self.sampler is None:
-            self.sampler = LatinHyperCubeSampling(num_new_points=1024)
-
-        # Dictionary that stores the optimisation information for every iteration
-        self.optimisation_dict = {}
+        if (
+            isinstance(self.acquisition_func, ExpectedImprovement)
+            or isinstance(self.acquisition_func, HighestUncertainty)
+        ) and self.sampler is None:
+            raise TypeError(
+                "ExpectedImprovement or HighestUncertainty acquisition functions were passed as the acquisition "
+                "function but no sampler was provided. Please pass a sampler too"
+            )
 
         # Constructs lists of variables and objectives with their respective units where provided
         self.X_columns = []
         for name, units in zip(self.variables.names, self.variables.units):
             if units == "":
                 self.X_columns.append(name)
             else:
@@ -89,96 +99,193 @@
         self.Y_columns = []
         for name, units in zip(self.objectives.names, self.objectives.units):
             if units == "":
                 self.Y_columns.append(name)
             else:
                 self.Y_columns.append(f"{name} ({units})")
 
+        # The name given to the optimisation run
+        if self.opt_name is None:
+            self.opt_name = f"Optimisation (start - {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')})"
+
+        # When a ModelBenchmark function has been provided, this checks that it has been fitted
+        if self.benchmark_func is not None and isinstance(self.benchmark_func, ModelBenchmark):
+            if not self.benchmark_func.fitted:
+                raise AttributeError("Please firstly fit the benchmark function(s) and check its quality")
+            else:
+                self.benchmark_func.save(os.path.join(os.getcwd(), "Results", self.opt_name))
+
     def run(
         self,
         X: Optional[np.ndarray] = None,
         Y: Optional[np.ndarray] = None,
-        number_of_iterations: int = 200,
+        number_of_iterations: int = 100,
         test_ratio: float = 0.2,
-        number_opt_iterations_completed: int = 0,
         model_run_counter: int = 0,
         model_run_counter_threshold: int = 5,
-        plot_pareto_hypervolume: bool = False,
+        plot_progress: bool = False,
+        plot_hypervolume: bool = False,
         test_data: Optional[List[np.ndarray]] = None,
+        resume_run: bool = False,
+        optimisation_pkl_path: Optional[str] = None,
         **kwargs,
     ) -> Dict[str, Dict[str, Any]]:
         """
 
         A convenient function to start a Bayesian optimisation, including model fitting. It will also request the results
         at the end of each iteration and save all optimisation data, and then automatically start the next iteration.
 
         Parameters
         ----------
-        X: np.ndarray
+        X: np.ndarray, Default = None,
             X array that contains the unprocessed variables data to be fitted to the model, i.e. The data has not yet
             undergone any transformations related to converted categorical variables to their respective descriptors
             or transformations related to standardisation/normalisation
-        Y: np.ndarray
+        Y: np.ndarray, Default = None,
             Y array that contains the unprocessed objective data for all calculable and regression objectives, i.e.
             The data has not yet undergone any transformations related to standardisation/normalisation
-        number_of_iterations: int, Default = 200,
+        number_of_iterations: int, Default = 100,
             Number of optimisation iterations to perform
         test_ratio: float, Default = 0.2,
             The proportion of inputted X and Y arrays to be split for the validation and test sets where applicable
-        number_opt_iterations_completed: int, Default = 0,
-            The number of optimisation iterations completed so far. This is used to identify the training data in the
-            provided X and Y arrays
         model_run_counter: int, Default = 0,
             Assigns the run counter for the first iteration when this function is called. When the model_run_counter is
             equal to model_run_counter_threshold, an automated model and hyperparameter optimisation will occur at the
             next opportunity
         model_run_counter_threshold: int, Default = 5,
             Sets the threshold value for when an automated model and hyperparameter optimisation should occur
-        plot_pareto_hypervolume: bool, Default = False,
-            Sets whether to generate the 2D pareto plot (2 objectives) and hypervolume over iterations plot every
-            iteration
+        plot_progress: bool, Default = False,
+            Sets whether to generate an objective values over iterations scatter plot for 1 objective optimisations or
+            a 2D/3D pareto plot (2/3 objectives) every iteration
+        plot_hypervolume: bool, Default = False,
+            Sets whether to generate a multiobjective hypervolume over iterations plot every iteration
         test_data: List[np.ndarray], Default = None,
             Test data to use for the initial model and hyperparameter optimisation, instead of creating it
-            automatically. The X array is at index 0 and the Y array is at index 1
+            automatically from the provided X and Y arrays. The test X array is at index 0 and the test Y array is at
+            index 1. Note: the test data are appended to the X and Y arrays for the final model fitting (after the best
+            model type has been identified) and the acquisition function
+        resume_run: bool, Default = False,
+            Sets whether to resume an optimisation using NEMO. Ensure that optimisation_pkl_path is passed too
+        optimisation_pkl_path: str, Default = None,
+            String of the file path of the pickle file written during the previous NEMO optimisation run
 
         Returns
         -------
         self.optimisation_dict: Dict[str, Dict[str, Any]]
             Dictionary that stores the optimisation information for every iteration
 
         """
-        if isinstance(self.benchmark_func, SyntheticBenchmark):
-            # X = self.sampler.__class__((2 * self.variables.n_var) + 2 if self.variables.n_var >= 4 else 10).generate_samples(self.variables, self.constraints)
-            X = self.sampler.__class__(
-                (5 * self.variables.n_var) if self.variables.n_var >= 2 else 10
-            ).generate_samples(self.variables, self.constraints)
-            Y, _ = self.benchmark_func.evaluate(X)
-            Y = Y.reshape(-1, 1)
+        # if number_opt_completed is None:
+        if not resume_run:
+            number_opt_completed = []
+
+            # Dictionary that stores the optimisation information for every iteration
+            self.optimisation_dict = {}
+
+        # If resuming a previous optimisation
+        if resume_run and optimisation_pkl_path is not None:
+            # Reads the optimisation pickle file at optimisation_pkl_path
+            with open(optimisation_pkl_path, "rb") as file:
+                self.optimisation_dict = pickle.load(file)
+
+            # Loads the information from the most recent iteration
+            last_dict = self.optimisation_dict[list(self.optimisation_dict.keys())[-1]]
+
+            # Extracts the X and Y arrays from the optimisation run so far
+            XY = last_dict["Training + Optimisation Table"]
+            X = XY.to_numpy()[:, : (-1 * self.objectives.n_obj)]
+            Y = XY.to_numpy()[:, (-1 * self.objectives.n_obj) :].astype(float)
+
+            # Loads the optimisation run information
+            self.optimisation_only = last_dict["Optimisation Table"]
+            model_run_counter = int(self.optimisation_only["Model Run Counter"].iloc[-1])
+
+            # Creates number_opt_completed list
+            number_opt_completed = [
+                (
+                    self.optimisation_only["Number of Candidates in Iteration"][
+                        self.optimisation_only["Iteration Number"] == i
+                    ]
+                ).iloc[0]
+                for i in range(1, int(self.optimisation_only["Iteration Number"].iloc[-1]) + 1)
+            ]
+
+            # Assigns the model types and hyperparameters to the objectives
+            for obj_index, (obj_name, obj) in enumerate(zip(self.objectives.names, self.objectives.objectives)):
+                if isinstance(obj, RegressionObjective):
+                    self.objectives.objectives[obj_index].predictor_type = create_predictor_list(
+                        last_dict[f"{obj_name} Model Type"]
+                    )[0]
+
+                    if last_dict[f"{obj_name} Model Type"] == "gp":
+                        self.objectives.objectives[obj_index].model_params = {
+                            "kernel": eval(last_dict[f"{obj_name} Model Hyperparameters"])
+                        }
+                    else:
+                        self.objectives.objectives[obj_index].model_params = last_dict[
+                            f"{obj_name} Model Hyperparameters"
+                        ]
+
+                    self.objectives.objectives[obj_index].obj_function = self.objectives.objectives[
+                        obj_index
+                    ].predictor_type(self.variables, self.objectives.objectives[obj_index])
+
+        # If no X and Y arrays are provided
+        if X is None and Y is None:
+            # Only valid to supply no X and Y arrays when a benchmark function is also provided
+            if self.benchmark_func is None:
+                raise ValueError(
+                    f"No X and Y arrays were provided. If you wish to simulate the outcome of experiments "
+                    f"in a closed-loop manner, please provide a benchmark function and then a set of X and "
+                    f"Y values will be automatically generated. If you wish to carry out actual Bayesian "
+                    f"optimisation experiments, please pass X and Y arrays"
+                )
+            else:
+                # Generates an initial training set using the supplied sampler and benchmark function
+                X = self.sampler.__class__(
+                    (2 * self.variables.n_var) + 2 if self.variables.n_var >= 4 else 10
+                ).generate_samples(self.variables, self.constraints)
+                Y, _ = self.benchmark_func.evaluate(X)
+                if Y.ndim == 1:
+                    Y = Y.reshape(-1, 1)
 
         self.X = X
         self.Y = Y
 
-        for iteration in range(number_of_iterations):
-            if model_run_counter % model_run_counter_threshold == 0:
+        # (Re-)Starts the optimisation run
+        for iteration in range(len(number_opt_completed), number_of_iterations):
+            # Checks if automated model and hyperparameter selection will be performed in this iteration
+            if model_run_counter % model_run_counter_threshold == 0 or model_run_counter > model_run_counter_threshold:
                 model_search_bool = True
-                print("Will perform automated model and hyperparameter selection")
+                logger.info("Will perform automated model and hyperparameter selection")
+
             else:
                 model_search_bool = False
-                print("Depending on predictor type, will perform model fitting with stored hyperparameters")
+                logger.info("Will perform model fitting using the previously identified best model type")
 
-            if plot_pareto_hypervolume:
+            if plot_progress:
                 # Scatter plot of the Y data
                 self.plot_scatter_opt(
-                    Y=self.Y, number_opt_iterations=number_opt_iterations_completed,
+                    Y=self.Y,
+                    number_opt_completed=number_opt_completed,
+                    best=self.benchmark_func.best_result() if self.benchmark_func is not None else None,
                 )
 
-                # Plot hypervolume over iterations plot
-                self.plot_hypervolume(
-                    Y=self.Y, number_opt_iterations=number_opt_iterations_completed,
-                )
+            # Plot hypervolume over iterations plot
+            if plot_hypervolume:
+                if self.objectives.n_obj > 1:
+                    self.plot_hypervolume(
+                        Y=self.Y,
+                        number_opt_completed=number_opt_completed,
+                    )
+                else:
+                    raise AttributeError(
+                        f"The number of objectives ({self.objectives.n_obj}) needs to be 2 or more to "
+                        f"create a hypervolume plot"
+                    )
 
             # Obtain suggested candidates
             self.selected_X, self.selected_Y = self.find_candidates(
                 self.X,
                 self.Y,
                 model_search_bool=model_search_bool,
                 test_ratio=test_ratio,
@@ -186,38 +293,43 @@
                 **kwargs,
             )
             if self.selected_Y.ndim == 1:
                 self.selected_Y = self.selected_Y.reshape(-1, 1)
 
             # Creates a DataFrame of the suggested candidates
             suggested_XY = pd.DataFrame(
-                np.hstack((self.selected_X, self.selected_Y)), columns=self.X_columns + self.Y_columns,
+                np.hstack((self.selected_X, self.selected_Y)),
+                columns=self.X_columns + self.Y_columns,
             )
             with pd.option_context("display.max_rows", None, "display.max_columns", None):
                 print(suggested_XY)
 
             # If the optimisation is not a simulated one that used a sample pool or a benchmark function
             if not isinstance(self.sampler, PoolBased) and self.benchmark_func is None:
                 if not os.path.exists(os.path.join(os.getcwd(), "Results")):
                     os.makedirs(os.path.join(os.getcwd(), "Results"))
                 # Creates an Excel file containing the suggested candidates
                 suggested_XY.to_excel(
                     os.path.join(
                         os.getcwd(),
                         "Results",
-                        f"Iteration {iteration + 1} suggested candidates {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}.xlsx",
+                        self.opt_name,
+                        f"Iteration {iteration + 1} suggested candidates "
+                        f"{datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}.xlsx",
                     )
                 )
                 while True:
                     try:
                         # Requests a new array containing the actual Y-values. The array has to be the correct shape
                         # and a list type to be accepted
                         actual_result = ast.literal_eval(
                             input(
-                                f"Variables for the current opt iteration have been suggested (see print or 'Iteration {iteration + 1} suggested candidates.xlsx')\nPlease input the actual results in a python list:\n"
+                                f"Variables for the current opt iteration have been suggested (see print or "
+                                f"'Iteration {iteration + 1} suggested candidates.xlsx')\nPlease input the actual "
+                                f"results in a python list:\n"
                             )
                         )
                         assert isinstance(actual_result, list)
 
                         self.selected_Y = (
                             np.array(actual_result)
                             if self.acquisition_func.num_candidates > 1
@@ -229,31 +341,55 @@
                             and self.selected_Y.shape[1] == self.objectives.n_obj
                             and np.issubdtype(self.selected_Y.dtype, np.number)
                         )
 
                         break
                     except AssertionError or IndexError or ValueError or SyntaxError:
                         print(
-                            "\nAssertionError: Please ensure that you have inputted the actual numerical results in a python list with the correct dimensions for the number of candidates (x) and number of objectives (y)\n"
+                            "\nAssertionError: Please ensure that you have inputted the actual numerical results in a "
+                            "python list with the correct dimensions for the number of candidates (x) and number of "
+                            "objectives (y)\n"
                         )
 
             # Updates the X and Y arrays with the new candidates
             self.X = np.vstack((self.X, self.selected_X))
             self.Y = np.vstack((self.Y, self.selected_Y))
 
-            # Saves the optimisation and model information for the current iteration
-            self.save(iteration, model_search_bool, model_run_counter)
-
             # After every iteration, adds 1 to the model_run_counter number
-            if self.acquisition_func.reset or model_search_bool:
+            if model_search_bool:
                 model_run_counter = 1
             else:
                 model_run_counter += 1
 
-            number_opt_iterations_completed += 1
+            # Saves the optimisation and model information for the current iteration
+            self.save(iteration + 1, model_search_bool, model_run_counter)
+
+            number_opt_completed.append(self.acquisition_func.num_candidates)
+
+        # When all iterations ahve been completed, the final plots will be generated
+        if plot_progress:
+            # Scatter plot of the Y data
+            self.plot_scatter_opt(
+                Y=self.Y,
+                number_opt_completed=number_opt_completed,
+                best=self.benchmark_func.best_result() if self.benchmark_func is not None else None,
+            )
+
+        # Plot hypervolume over iterations plot
+        if plot_hypervolume:
+            if self.objectives.n_obj > 1:
+                self.plot_hypervolume(
+                    Y=self.Y,
+                    number_opt_completed=number_opt_completed,
+                )
+            else:
+                raise AttributeError(
+                    f"The number of objectives ({self.objectives.n_obj}) needs to be 2 or more to "
+                    f"create a hypervolume plot"
+                )
 
         return self.optimisation_dict
 
     def find_candidates(
         self,
         X: np.ndarray,
         Y: np.ndarray,
@@ -281,15 +417,17 @@
         model_search_bool: bool
             Whether automated model and hyperparameter optimisation is to be performed when fitting the regression
             models
         test_ratio: float, Default = 0.2,
             The proportion of inputted X and Y arrays to be split for the validation and test sets where applicable
         test_data: List[np.ndarray], Default = None,
             Test data to use for the initial model and hyperparameter optimisation, instead of creating it
-            automatically. The X array is at index 0 and the Y array is at index 1
+            automatically from the provided X and Y arrays. The test X array is at index 0 and the test Y array is at
+            index 1. Note: the test data are appended to the X and Y arrays for the final model fitting (after the best
+            model type has been identified) and the acquisition function
 
         Returns
         -------
         selected_X: np.ndarray
             The X array of the suggested candidates
         selected_Y: np.ndarray
             The Y array of the suggested candidates
@@ -298,18 +436,29 @@
         if any(isinstance(obj, RegressionObjective) for obj in self.objectives.objectives):
 
             # Fit the ML regression models
             self.objectives.fit(
                 X, Y, self.variables, model_search_bool, test_ratio=test_ratio, test_data=test_data, **kwargs
             )
 
-        # Use the fitted regression models, calculable objectives, and acquisition function to suggest new candidates
-        selected_X, selected_Y = self.acquisition_func.generate_candidates(
-            Y, self.variables, self.objectives, self.sampler, self.constraints, **kwargs
-        )
+        # Use the fitted regression models, calculable objectives, and acquisition function to suggest new candidates.
+        # If test data was supplied, it is appended to X and Y for the acquisition function
+        if test_data is not None:
+            X = np.vstack((X, test_data[0]))
+            Y = np.vstack((Y, test_data[1]))
+
+        if isinstance(self.acquisition_func, ExpectedImprovement):
+            selected_X, selected_Y = self.acquisition_func.generate_candidates(
+                X, Y, self.variables, self.objectives, self.sampler, self.constraints, **kwargs
+            )
+
+        else:
+            selected_X, selected_Y = self.acquisition_func.generate_candidates(
+                Y, self.variables, self.objectives, sampler=self.sampler, constraints=self.constraints, **kwargs
+            )
 
         # If a sample pool was used, obtain the actual Y-values and removing the chosen samples from the sample pool
         if isinstance(self.sampler, PoolBased):
             selected_Y = self.sampler.Y_and_update_pool(self.sampler.index)
 
         else:
             # If a benchmark function is provided, use it to predict the outcome of the suggested X array
@@ -332,24 +481,30 @@
             Iteration number for the current optimisation
         model_search_bool: bool
             Whether automated model and hyperparameter optimisation was performed when the regression models were fitted
         model_run_counter: int
             The run counter for this optimisation iteration
 
         """
-        # Save excel for current iteration data
-        if not os.path.exists(os.path.join(os.getcwd(), "Results")):
-            os.makedirs(os.path.join(os.getcwd(), "Results"))
+        if not os.path.exists(os.path.join(os.getcwd(), "Results", self.opt_name)):
+            os.makedirs(os.path.join(os.getcwd(), "Results", self.opt_name))
 
-        # Temporarily stored the information in these lists
-        model_info_list = [model_search_bool, model_run_counter]
+        # Temporarily store the information in these lists
+        model_info_list = [iteration, self.acquisition_func.num_candidates, model_search_bool, model_run_counter]
         model_info_columns = [
+            "Iteration Number",
+            "Number of Candidates in Iteration",
             "Model and Hyperparameter Optimisation",
             "Model Run Counter",
         ]
+
+        if self.objectives.n_obj > 1:
+            model_info_list.append(self.calc_hypervolume(self.Y))
+            model_info_columns.append("Normalised Hypervolume")
+
         for obj in self.objectives.objectives:
             if isinstance(obj, RegressionObjective):
                 if obj.obj_function.include_validation:
                     model_info_list.append(obj.obj_function.performance_metrics["Train RMSE"])
                     model_info_list.append(obj.obj_function.performance_metrics["Train r2"])
                     model_info_list.append(obj.obj_function.performance_metrics["Validation RMSE"])
                     model_info_list.append(obj.obj_function.performance_metrics["Validation r2"])
@@ -363,34 +518,40 @@
                     model_info_columns.append(f"{obj.name} Model Train RMSE")
                     model_info_columns.append(f"{obj.name} Model Train r2")
                 model_info_list.append(obj.obj_function.name)
 
                 if obj.obj_function.name == "gp":
                     if isinstance(obj.model_params["kernel"], AdditiveStructureKernel):
                         model_info_list.append(
-                            f"AdditiveStructureKernel(ScaleKernel(MaternKernel(ard_num_dims=n_var, nu={obj.model_params['kernel'].base_kernel.base_kernel.nu}, lengthscale_prior=GammaPrior(3.0, 6.0)), outputscale_prior=GammaPrior(2.0, 0.15)), num_dims=n_var)"
+                            f"AdditiveStructureKernel(ScaleKernel(MaternKernel(ard_num_dims={self.variables.n_var}, "
+                            f"nu={obj.model_params['kernel'].base_kernel.base_kernel.nu}, "
+                            f"lengthscale_prior=GammaPrior(3.0, 6.0)), outputscale_prior=GammaPrior(2.0, 0.15)), "
+                            f"num_dims={self.variables.n_var})"
                         )
                     else:
                         model_info_list.append(
-                            f"ScaleKernel(MaternKernel(nu={obj.model_params['kernel'].base_kernel.nu}, ard_num_dims=n_var, lengthscale_prior=GammaPrior(3.0, 6.0)), outputscale_prior=GammaPrior(2.0, 0.15))"
+                            f"ScaleKernel(MaternKernel(nu={obj.model_params['kernel'].base_kernel.nu}, "
+                            f"ard_num_dims={self.variables.n_var}, lengthscale_prior=GammaPrior(3.0, 6.0)), "
+                            f"outputscale_prior=GammaPrior(2.0, 0.15))"
                         )
                 else:
                     model_info_list.append(obj.model_params)
 
                 model_info_columns.append(f"{obj.name} Model Type")
                 model_info_columns.append(f"{obj.name} Model Hyperparameters")
 
         model_info_list.append(datetime.now().strftime("%d-%m-%Y, %H-%M-%S"))
         model_info_columns.append("Date and Time")
+
         # Duplicates this information for every candidate
         model_info = np.array([model_info_list] * self.acquisition_func.num_candidates)
 
         # Creates the DataFrames of optimisation information
         optimisation_results = pd.DataFrame(np.hstack((self.X, self.Y)), columns=self.X_columns + self.Y_columns)
-        if iteration == 0:
+        if iteration == 1:
             self.optimisation_only = pd.DataFrame(
                 np.hstack((self.selected_X, self.selected_Y, model_info)),
                 columns=self.X_columns + self.Y_columns + model_info_columns,
             )
         else:
             self.optimisation_only = pd.concat(
                 (
@@ -405,75 +566,81 @@
             )
 
         # Writes the optimisation information DataFrames into Excel files
         with pd.ExcelWriter(
             os.path.join(
                 os.getcwd(),
                 "Results",
-                f'Optimisation Results (after {iteration + 1} iteration(s)) {datetime.now().strftime("%d-%m-%Y, %H-%M-%S")}.xlsx',
+                self.opt_name,
+                f"Optimisation Results (after {iteration} iteration(s)) "
+                f'{datetime.now().strftime("%d-%m-%Y, %H-%M-%S")}.xlsx',
             )
         ) as writer:
             optimisation_results.to_excel(writer, sheet_name="Training + Opt")
             self.optimisation_only.to_excel(writer, sheet_name="Only Opt")
             for obj in self.objectives.objectives:
                 if isinstance(obj, RegressionObjective):
                     if obj.obj_function.include_validation:
                         obj.obj_function.performance_metrics["Train Parity Data"].to_excel(
                             writer, sheet_name=f"{obj.name} Train Parity Data"
                         )
                         obj.obj_function.performance_metrics["Validation Parity Data"].to_excel(
-                            writer, sheet_name=f"{obj.name} Validation Parity Data"
+                            writer, sheet_name=f"{obj.name} Val Parity Data"
                         )
                     else:
                         obj.obj_function.performance_metrics["Parity Data"].to_excel(
                             writer, sheet_name=f"{obj.name} Train Parity Data"
                         )
 
         # Writes pickle files containing every iteration's optimisation information
-        self.optimisation_dict[f"Iteration {iteration + 1}"] = {}
-        self.optimisation_dict[f"Iteration {iteration + 1}"]["Date and Time"] = datetime.now().strftime(
-            "%d-%m-%Y, %H-%M-%S"
-        )
-        self.optimisation_dict[f"Iteration {iteration + 1}"]["Training + Optimisation Table"] = optimisation_results
-        self.optimisation_dict[f"Iteration {iteration + 1}"]["Optimisation Table"] = self.optimisation_only
-        self.optimisation_dict[f"Iteration {iteration + 1}"]["Optimisation Selected X"] = self.selected_X
-        self.optimisation_dict[f"Iteration {iteration + 1}"]["Optimisation Selected Y"] = self.selected_Y
-        self.optimisation_dict[f"Iteration {iteration + 1}"][
-            "Model and Hyperparameter Optimisation"
-        ] = model_search_bool
-        self.optimisation_dict[f"Iteration {iteration + 1}"]["Model Run Counter"] = model_run_counter
+        self.optimisation_dict[f"Iteration {iteration}"] = {
+            "Date and Time": datetime.now().strftime("%d-%m-%Y, %H-%M-%S"),
+            "Training + Optimisation Table": optimisation_results,
+            "Optimisation Table": self.optimisation_only,
+            "Optimisation Selected X": self.selected_X,
+            "Optimisation Selected Y": self.selected_Y,
+            "Model and Hyperparameter Optimisation": model_search_bool,
+            "Model Run Counter": model_run_counter,
+        }
         for obj in self.objectives.objectives:
             if isinstance(obj, RegressionObjective):
-                self.optimisation_dict[f"Iteration {iteration + 1}"][f"{obj.name} Model Type"] = obj.obj_function.name
+                self.optimisation_dict[f"Iteration {iteration}"][f"{obj.name} Model Type"] = obj.obj_function.name
                 if obj.obj_function.name == "gp":
                     if isinstance(obj.model_params["kernel"], AdditiveStructureKernel):
-                        self.optimisation_dict[f"Iteration {iteration + 1}"][
-                            f"{obj.name} Model Hyperparameters"
-                        ] = f"AdditiveStructureKernel(ScaleKernel(MaternKernel(ard_num_dims=n_var, nu={obj.model_params['kernel'].base_kernel.base_kernel.nu}, lengthscale_prior=GammaPrior(3.0, 6.0)), outputscale_prior=GammaPrior(2.0, 0.15)), num_dims=n_var)"
+                        self.optimisation_dict[f"Iteration {iteration}"][f"{obj.name} Model Hyperparameters"] = (
+                            f"AdditiveStructureKernel(ScaleKernel(MaternKernel(ard_num_dims={self.variables.n_var}, "
+                            f"nu={obj.model_params['kernel'].base_kernel.base_kernel.nu}, "
+                            f"lengthscale_prior=GammaPrior(3.0, 6.0)), outputscale_prior=GammaPrior(2.0, 0.15)), "
+                            f"num_dims={self.variables.n_var})"
+                        )
                     else:
-                        self.optimisation_dict[f"Iteration {iteration + 1}"][
-                            f"{obj.name} Model Hyperparameters"
-                        ] = f"ScaleKernel(MaternKernel(nu={obj.model_params['kernel'].base_kernel.nu}, ard_num_dims=n_var, lengthscale_prior=GammaPrior(3.0, 6.0)), outputscale_prior=GammaPrior(2.0, 0.15))"
+                        self.optimisation_dict[f"Iteration {iteration}"][f"{obj.name} Model Hyperparameters"] = (
+                            f"ScaleKernel(MaternKernel(nu={obj.model_params['kernel'].base_kernel.nu}, "
+                            f"ard_num_dims={self.variables.n_var}, lengthscale_prior=GammaPrior(3.0, 6.0)), "
+                            f"outputscale_prior=GammaPrior(2.0, 0.15))"
+                        )
                 else:
-                    self.optimisation_dict[f"Iteration {iteration + 1}"][
+                    self.optimisation_dict[f"Iteration {iteration}"][
                         f"{obj.name} Model Hyperparameters"
                     ] = obj.model_params
-                self.optimisation_dict[f"Iteration {iteration + 1}"][
+                self.optimisation_dict[f"Iteration {iteration}"][
                     f"{obj.name} Model Performance Metrics"
                 ] = obj.obj_function.performance_metrics
 
         with open(
             os.path.join(
                 os.getcwd(),
                 "Results",
-                f"Optimisation Results (after {iteration + 1} iteration(s)) {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}.pickle",
+                self.opt_name,
+                f"Optimisation Results (after {iteration} iteration(s)) "
+                f"{datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}.pickle",
             ),
             "wb",
-        ) as handle:
-            pickle.dump(self.optimisation_dict, handle, protocol=pickle.HIGHEST_PROTOCOL)
+        ) as file:
+            pickle.dump(self.optimisation_dict, file, protocol=pickle.HIGHEST_PROTOCOL)
 
     def calc_hypervolume(self, Y: np.ndarray) -> float:
         """
 
         Calculates the hypervolume of a Y-array that has been min-max normalised by the pre-defined objective bounds
 
         Parameters
@@ -496,30 +663,40 @@
         pareto_mask = is_non_dominated(torch.tensor(sign_adjusted_Y, dtype=torch.double))
         pareto_front = sign_adjusted_Y[pareto_mask]
 
         # Calculates the hypervolume
         hv = Hypervolume(ref_point=torch.tensor(ref_point, dtype=torch.double))
         return hv.compute(torch.tensor(pareto_front, dtype=torch.double))
 
-    def plot_scatter_opt(self, Y: np.ndarray, number_opt_iterations: int) -> None:
+    def plot_scatter_opt(
+        self, Y: np.ndarray, number_opt_completed: List[int], best: Optional[Union[int, float, np.ndarray]] = None
+    ) -> None:
         """
 
         Plots the Y-array for 1, 2, or 3 objective optimisation problems, with multi-objective pareto fronts when
         applicable
 
         Parameters
         ----------
         Y: np.ndarray
             Y-array with objective data. Any data points with NaN values will be removed
-        number_opt_iterations: int
-            Number of Bayesian optimisation iterations performed so far
+        number_opt_completed: List[int]
+            List containing the number of optimisation candidates completed per iteration, e.g. [2, 4] means
+            2 candidates were run in the first iteration and 4 candidates in the second iteration
+        best: [int | float | np.ndarray], Default = None
+            The actual best result. Would be a single value for a single objective problem or a np.ndarray for a
+            multiobjective problem
 
         """
-        train_num = Y.shape[0] - (number_opt_iterations * self.acquisition_func.num_candidates)
-        opt_num = number_opt_iterations * self.acquisition_func.num_candidates
+        if not os.path.exists(os.path.join(os.getcwd(), "Results", self.opt_name)):
+            os.makedirs(os.path.join(os.getcwd(), "Results", self.opt_name))
+
+        # Calculates the number of training and optimisation experiments
+        opt_num = sum(number_opt_completed)
+        train_num = Y.shape[0] - opt_num
 
         if self.objectives.n_obj == 1:
             iterations = np.array((range(Y.shape[0]))) + 1
             Y = np.hstack((iterations.reshape(-1, 1), Y))
 
         else:
             Y_no_nan = remove_all_nan_rows(Y)
@@ -538,92 +715,127 @@
                 # Uses the first objective in the array that has all non-zero values
                 pareto_front_sorted = pareto_front[pareto_front[:, non_zero_objs[0]].argsort()]
             else:
                 # Else just use the first objective
                 pareto_front_sorted = pareto_front[pareto_front[:, 0].argsort()]
 
         train_experiments = Y[
-            :train_num, :,
+            :train_num,
+            :,
         ]
         opt_experiments = Y[
-            train_num:, :,
+            train_num:,
+            :,
         ]
 
         train_experiments = remove_all_nan_rows(train_experiments)
         opt_experiments = remove_all_nan_rows(opt_experiments)
 
         scatter_data = [train_experiments, opt_experiments]
         scatter_legend = [
             f"Training ({train_num} experiments)"
             if train_num == train_experiments.shape[0]
             else f"Training ({train_num} expt, showing {train_experiments.shape[0]} expt)",
             f"Optimisation ({opt_num} experiments)"
-            if train_num == opt_experiments.shape[0]
+            if opt_num == opt_experiments.shape[0]
             else f"Optimisation ({opt_num} expt, showing {opt_experiments.shape[0]} expt)",
         ]
 
-        title = "Pareto Plot"
-        output = os.path.join(os.getcwd(), f'Pareto Plot {datetime.now().strftime("%d-%m-%Y, %H-%M-%S")}.png',)
+        output = os.path.join(
+            os.getcwd(),
+            "Results",
+            self.opt_name,
+            f'Pareto Plot (after {len(number_opt_completed)} iteration(s)) {datetime.now().strftime("%d-%m-%Y, %H-%M-%S")}'
+            if self.objectives.n_obj > 1
+            else f'Progress Plot (after {len(number_opt_completed)} iteration(s)) {datetime.now().strftime("%d-%m-%Y, %H-%M-%S")}',
+        )
 
+        # If single objective
         if self.objectives.n_obj == 1:
+            opt_line = [[train_num + 0.5, min(Y[:, 1])], [train_num + 0.5, max(Y[:, 1])]]
+            best_line = [[0, best], [Y.shape[0], best]]
+            line_data = [opt_line, best_line] if best is not None else opt_line
+
             plotter.plot(
                 plot_dim="2D",
                 scatter_data=scatter_data,
                 # Create array to use for drawing the start of the optimisation line
-                line_data=[[train_num + 0.5, min(Y[:, 1])], [train_num + 0.5, max(Y[:, 1])]],
+                line_data=line_data,
                 scatter_legend=scatter_legend,
-                line_legend="Start of Optimisation",
-                xlabel=f"Number of Iterations",
-                ylabel=f"{self.objectives.names[0]} {self.objectives.units[0]}",
-                plottitle=f"{title}\n{self.objectives.names[0]} vs. Number of Iterations",
+                line_legend=["Start of optimisation", "Best possible result"]
+                if best is not None
+                else "Start of optimisation",
+                xlabel=f"Number of experiments",
+                ylabel=f"{self.objectives.names[0]} ({self.objectives.units[0]})"
+                if self.objectives.units[0] != ""
+                else f"{self.objectives.names[0]}",
+                plottitle=f"Progress Plot\n{self.objectives.names[0]} vs. Number of experiments",
                 output_file=rf"{output}",
             )
+        # If two objectives
         elif self.objectives.n_obj == 2:
             plotter.plot(
                 plot_dim="2D",
-                scatter_data=scatter_data,
+                scatter_data=scatter_data + [best] if best is not None else scatter_data,
                 line_data=pareto_front_sorted,
-                scatter_legend=scatter_legend,
-                line_legend="Pareto front",
-                xlabel=f"{self.objectives.names[0]} {self.objectives.units[0]}",
-                ylabel=f"{self.objectives.names[1]} {self.objectives.units[1]}",
-                plottitle=f"{title}\n{self.objectives.names[0]} vs. {self.objectives.names[1]}",
+                scatter_legend=scatter_legend + ["Approx. best pareto front"] if best is not None else scatter_legend,
+                line_legend="Observed pareto front",
+                xlabel=f"{self.objectives.names[0]} ({self.objectives.units[0]})"
+                if self.objectives.units[0] != ""
+                else f"{self.objectives.names[0]}",
+                ylabel=f"{self.objectives.names[1]} ({self.objectives.units[1]})"
+                if self.objectives.units[1] != ""
+                else f"{self.objectives.names[1]}",
+                plottitle=f"Pareto Plot\n{self.objectives.names[0]} vs. {self.objectives.names[1]}",
                 output_file=rf"{output}",
             )
+
+        # If three objectives
         elif self.objectives.n_obj == 3:
             plotter.plot(
                 plot_dim="3D",
                 scatter_data=scatter_data,
-                surface_data=pareto_front_sorted,
+                surface_data=[pareto_front_sorted, best],
                 scatter_legend=scatter_legend,
                 surface_legend="Pareto front",
-                xlabel=f"{self.objectives.names[0]} {self.objectives.units[0]}",
-                ylabel=f"{self.objectives.names[1]} {self.objectives.units[1]}",
-                zlabel=f"{self.objectives.names[2]} {self.objectives.units[2]}",
-                plottitle=f"{title}\n{self.objectives.names[0]} vs. {self.objectives.names[1]} vs. {self.objectives.names[2]}",
+                xlabel=f"{self.objectives.names[0]} ({self.objectives.units[0]})"
+                if self.objectives.units[0] != ""
+                else f"{self.objectives.names[0]}",
+                ylabel=f"{self.objectives.names[1]} ({self.objectives.units[1]})"
+                if self.objectives.units[1] != ""
+                else f"{self.objectives.names[1]}",
+                zlabel=f"{self.objectives.names[2]} ({self.objectives.units[2]})"
+                if self.objectives.units[2] != ""
+                else f"{self.objectives.names[2]}",
+                plottitle=f"Pareto Plot\n{self.objectives.names[0]} vs. {self.objectives.names[1]} vs. {self.objectives.names[2]}",
                 output_file=rf"{output}",
             )
 
         plt.close()
 
-    def plot_hypervolume(self, Y: np.ndarray, number_opt_iterations: int) -> None:
+    def plot_hypervolume(self, Y: np.ndarray, number_opt_completed: List[int]) -> None:
         """
 
         Plots the hypervolume over all iterations
 
         Parameters
         ----------
         Y: np.ndarray
             Y-array with objective data. Any data points with NaN values will be removed
-        number_opt_iterations: int
-            Number of Bayesian optimisation iterations performed so far
+        number_opt_completed: List[int]
+            List containing the number of optimisation candidates completed per iteration, e.g. [2, 4] means
+            2 candidates were run in the first iteration and 4 candidates in the second iteration
 
         """
-        train_num = Y.shape[0] - (number_opt_iterations * self.acquisition_func.num_candidates)
-        opt_num = number_opt_iterations * self.acquisition_func.num_candidates
+        if not os.path.exists(os.path.join(os.getcwd(), "Results", self.opt_name)):
+            os.makedirs(os.path.join(os.getcwd(), "Results", self.opt_name))
+
+        # Calculates the number of training and optimisation experiments
+        opt_num = sum(number_opt_completed)
+        train_num = Y.shape[0] - opt_num
 
         iterations = np.array((range(Y.shape[0]))) + 1
         del_index = [index for index in range(Y.shape[0]) if np.any(np.isnan(Y[index]), axis=0)]
         iterations = np.delete(iterations, del_index, axis=0)
 
         no_nan_train_num = sum(expt_number <= train_num for expt_number in iterations)
         no_nan_opt_num = sum(expt_number > train_num for expt_number in iterations)
@@ -646,26 +858,32 @@
             # Calculates the hypervolume
             hv = Hypervolume(ref_point=torch.tensor(ref_point, dtype=torch.double))
             hv_list.append(hv.compute(torch.tensor(pareto_front_to_expnum, dtype=torch.double)))
 
         if Y.shape[0] == len(iterations):
             title = f"Hypervolume\nTraining: {train_num} expt\nOptimisation: {opt_num} expt"
         else:
-            title = f"Hypervolume\nTraining: {train_num} expt, showing {no_nan_train_num} expt\nOptimisation: {opt_num} expt, showing {no_nan_opt_num} expt"
+            title = (
+                f"Hypervolume\nTraining: {train_num} expt, showing {no_nan_train_num} expt\n"
+                f"Optimisation: {opt_num} expt, showing {no_nan_opt_num} expt"
+            )
 
         output_file = os.path.join(
-            os.getcwd(), rf"Hypervolume vs. Iteration {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}.png",
+            os.getcwd(),
+            "Results",
+            self.opt_name,
+            f"Hypervolume (after {len(number_opt_completed)} iteration(s)) {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}",
         )
 
         hv_array = np.array([[expt_number, hv_list[index]] for index, expt_number in enumerate(iterations)])
         plotter.plot(
             plot_dim="2D",
             scatter_data=hv_array,
             line_data=[[train_num + 0.5, 0.0], [train_num + 0.5, 1.0]],
             scatter_legend="Hypervolume",
             line_legend="Start of Optimisation",
-            xlabel=f"Iteration",
-            ylabel=f"Normalised Hypervolume",
+            xlabel="Number of experiments",
+            ylabel="Normalised Hypervolume",
             plottitle=title,
             output_file=output_file,
         )
         plt.close()
```

### Comparing `nemo-bo-0.1.8/nemo_bo/opt/samplers.py` & `nemo-bo-0.1.9/nemo_bo/opt/samplers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 import math
 import os
 import random
-from attrs import define
+from attrs import define, field
 from typing import List, Optional, Union
 
 import numpy as np
-import pandas as pd
 import torch
 from botorch.utils.sampling import get_polytope_samples
 from scipy.stats import qmc
 
-# from smt.applications.mixed_integer import ENUM, FLOAT, MixedIntegerSamplingMethod
-# from smt.sampling_methods import LHS, Random
-
 import nemo_bo.utils.logger as logging_nemo
 from nemo_bo.opt.constraints import ConstraintsList
 from nemo_bo.opt.utils_samplers.sampling import *
 from nemo_bo.opt.variables import ContinuousVariable, VariablesList
 
 try:
     logging_nemo.logging_path
@@ -99,15 +95,17 @@
                 if constr.constraint_type == "ineq":
                     kwargs["inequality_constraints"] = [constr.build_polytope_sampler_constraint()]
                 else:
                     kwargs["equality_constraints"] = [constr.build_polytope_sampler_constraint()]
 
         X = (
             get_polytope_samples(
-                n=self.num_new_points, bounds=torch.tensor([variables.lower_bounds, variables.upper_bounds]), **kwargs,
+                n=self.num_new_points,
+                bounds=torch.tensor([variables.lower_bounds, variables.upper_bounds]),
+                **kwargs,
             )
             .cpu()
             .numpy()
         )
 
         if variables.num_cat_var > 0:
             return variables.descriptor_to_name(X)
@@ -147,15 +145,16 @@
             Array of generated samples that are within the defined bounds and passes all constraints
 
         """
         xlimits = np.array(
             [
                 [var.lower_bound, var.upper_bound] if isinstance(var, ContinuousVariable) else var.categorical_levels
                 for var in variables.variables
-            ]
+            ],
+            dtype=object,
         )
 
         if variables.num_cat_var > 0:
             xtypes = [
                 FLOAT if isinstance(var, ContinuousVariable) else (ENUM, var.num_categorical_levels)
                 for var in variables.variables
             ]
@@ -188,15 +187,16 @@
 
         else:
             sampler = LHS(xlimits=xlimits, **kwargs)
 
             X = sampler(self.num_new_points)
 
             # To do: Improve the implementation for constraints for LHS.
-            # Currently this does not sample the available space in a guaranteed LHS manner after constraints are applied
+            # Currently this does not sample the available space in a guaranteed LHS manner after constraints are
+            # applied
             if constraints is not None:
                 num_points_temp = self.num_new_points
                 X = X[constraints.bool_evaluate_constraints(X)]
                 while X.shape[0] < self.num_new_points:
                     num_points_temp = math.ceil(num_points_temp * 1.2)
                     X = sampler(num_points_temp)
                     X = X[constraints.bool_evaluate_constraints(X)]
@@ -238,15 +238,16 @@
             Array of generated samples that are within the defined bounds and passes all constraints
 
         """
         xlimits = np.array(
             [
                 [var.lower_bound, var.upper_bound] if isinstance(var, ContinuousVariable) else var.categorical_levels
                 for var in variables.variables
-            ]
+            ],
+            dtype=object,
         )
 
         if variables.num_cat_var > 0:
             logger.info(f"Generating {self.num_new_points} mixed integer random sampling points in the variable space")
             xtypes = [
                 FLOAT if isinstance(var, ContinuousVariable) else (ENUM, var.num_categorical_levels)
                 for var in variables.variables
@@ -314,15 +315,15 @@
         X: np.ndarray
             Array of generated samples that are within the defined bounds and passes all constraints
 
         """
         sampler = qmc.Sobol(d=variables.n_var)
 
         num_samples_power = math.ceil(math.log2(self.num_new_points))
-        if 2 ** num_samples_power != self.num_new_points:
+        if 2**num_samples_power != self.num_new_points:
             logger.info(
                 f"Generating {2 ** num_samples_power} sobol sampling points in the variable "
                 f"space (different to the desired {self.num_new_points} to guarantee the balance properties "
                 f"of the sobol sequence)."
             )
 
         X = sampler.random_base2(m=num_samples_power)
@@ -362,14 +363,30 @@
     Y_pool: np.ndarray
         The Y array to be used in the sample pool
 
     """
 
     X_pool: np.ndarray
     Y_pool: np.ndarray
+    index: str = field(init=False)
+
+    def __attrs_post_init__(self):
+        self.index = None
+
+    def generate_samples(self) -> np.ndarray:
+        """
+
+        Returns
+        -------
+        np.ndarray
+            Array of X-values that are in the user-supplied pool
+
+        """
+
+        return self.X_pool
 
     def Y_and_update_pool(self, index: Union[int, List[int]]) -> np.ndarray:
         """
 
         Uses the index to select Y-values, delete them from the Y sample pool and return them
 
         Parameters
@@ -382,13 +399,15 @@
         Y: np.ndarray
             The selected Y-values based on the index/indexes
 
         """
         if isinstance(index, int):
             index = [index]
 
+        # Identifies the Y values to be returned
         Y = np.array([self.Y_pool[i] for i in index])
 
+        # Removes the samples in the sample pool based on the supplied index/indexes
         self.X_pool = np.delete(self.X_pool, index, 0)
         self.Y_pool = np.delete(self.Y_pool, index, 0)
 
         return Y
```

### Comparing `nemo-bo-0.1.8/nemo_bo/opt/utils_samplers/sampling.py` & `nemo-bo-0.1.9/nemo_bo/opt/utils_samplers/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,15 +174,19 @@
                 name,
                 value,
             ) + "value must be %s or type must be %s" % (
                 values,
                 types,
             )
         elif values is not None:
-            assert value in values, "Option %s: value %s is invalid - must be %s" % (name, value, values,)
+            assert value in values, "Option %s: value %s is invalid - must be %s" % (
+                name,
+                value,
+                values,
+            )
         elif types is not None:
             assert isinstance(value, types), "Option %s: type of %s is invalid - must be %s" % (name, value, types)
 
     def update(self, dict_):
         """
         Loop over and set all the entries in the given dictionary into self.
 
@@ -654,15 +658,25 @@
 
 
 class LHS(ScaledSamplingMethod):
     def _initialize(self):
         self.options.declare(
             "criterion",
             "c",
-            values=["center", "maximin", "centermaximin", "correlation", "c", "m", "cm", "corr", "ese",],
+            values=[
+                "center",
+                "maximin",
+                "centermaximin",
+                "correlation",
+                "c",
+                "m",
+                "cm",
+                "corr",
+                "ese",
+            ],
             types=str,
             desc="criterion used to construct the LHS design "
             + "c, m, cm and corr are abbreviation of center, maximin, centermaximin and correlation, respectively",
         )
         self.options.declare(
             "random_state",
             types=(type(None), int, np.random.RandomState),
@@ -692,20 +706,34 @@
             self.random_state = self.options["random_state"]
         elif isinstance(self.options["random_state"], int):
             self.random_state = np.random.RandomState(self.options["random_state"])
         else:
             self.random_state = np.random.RandomState()
 
         if self.options["criterion"] != "ese":
-            return lhs(nx, samples=nt, criterion=self.options["criterion"], random_state=self.random_state,)
+            return lhs(
+                nx,
+                samples=nt,
+                criterion=self.options["criterion"],
+                random_state=self.random_state,
+            )
         elif self.options["criterion"] == "ese":
             return self._ese(nx, nt)
 
     def _maximinESE(
-        self, X, T0=None, outer_loop=None, inner_loop=None, J=20, tol=1e-3, p=10, return_hist=False, fixed_index=[],
+        self,
+        X,
+        T0=None,
+        outer_loop=None,
+        inner_loop=None,
+        J=20,
+        tol=1e-3,
+        p=10,
+        return_hist=False,
+        fixed_index=[],
     ):
         """
 
         Returns an optimized design starting from design X. For more information,
         see R. Jin, W. Chen and A. Sudjianto (2005):
         An efficient algorithm for constructing optimal design of computer
         experiments. Journal of Statistical Planning and Inference, 134:268-287.
@@ -896,18 +924,18 @@
         while i2 == i1 or i2 in fixed_index:
             i2 = self.random_state.randint(X.shape[0])
 
         X_ = np.delete(X, [i1, i2], axis=0)
 
         dist1 = cdist([X[i1, :]], X_)
         dist2 = cdist([X[i2, :]], X_)
-        d1 = np.sqrt(dist1 ** 2 + (X[i2, k] - X_[:, k]) ** 2 - (X[i1, k] - X_[:, k]) ** 2)
-        d2 = np.sqrt(dist2 ** 2 - (X[i2, k] - X_[:, k]) ** 2 + (X[i1, k] - X_[:, k]) ** 2)
+        d1 = np.sqrt(dist1**2 + (X[i2, k] - X_[:, k]) ** 2 - (X[i1, k] - X_[:, k]) ** 2)
+        d2 = np.sqrt(dist2**2 - (X[i2, k] - X_[:, k]) ** 2 + (X[i1, k] - X_[:, k]) ** 2)
 
-        res = (PhiP_ ** p + (d1 ** (-p) - dist1 ** (-p) + d2 ** (-p) - dist2 ** (-p)).sum()) ** (1.0 / p)
+        res = (PhiP_**p + (d1 ** (-p) - dist1 ** (-p) + d2 ** (-p) - dist2 ** (-p)).sum()) ** (1.0 / p)
         X[i1, k], X[i2, k] = X[i2, k], X[i1, k]
 
         return res
 
     def _ese(self, dim, nt, fixed_index=[], P0=[]):
         """
         Parameters
```

### Comparing `nemo-bo-0.1.8/nemo_bo/opt/variables.py` & `nemo-bo-0.1.9/nemo_bo/opt/variables.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import copy
 import os
 from attrs import define, field
 
-# from dataclasses import dataclass
-from typing import Any, List, Optional, Union
+from typing import List, Optional, Union
 
 import numpy as np
-import pandas as pd
 from sklearn.preprocessing import MinMaxScaler, OneHotEncoder, StandardScaler
 
 import nemo_bo.utils.logger as logging_nemo
-from nemo_bo.utils.transformations import Transformations
 
 try:
     logging_nemo.logging_path
     logger = logging_nemo.logging_nemo_child(os.path.basename(__file__))
 except AttributeError:
     logger = logging_nemo.logging_nemo_master(os.path.basename(__file__))
 
@@ -29,102 +26,111 @@
     ----------
     name: str
         Name of the variable
     lower_bound: int | float
         The lower bound of the variable
     upper_bound: int | float
         The upper bound of the variable
-    transformation_type: str. Default = None
-        The type of transformation that should be applied to the variable for modelling. When left as the default
-        None, the modelling uses the default transformations specified by the model type. When specified, can be
-        "normalisation", "standardisation", or "none" for min-max normalisation, standardisation to a mean of 0 and a
-        standard deviation of 1, or no transformation respectively
+    transformer: Optional. Default = None
+        The transformation that will be applied to the variable for modelling. When left as the default
+        None, the modelling uses the default transformations specified by the model type. Can be specified as the
+        strings "normalisation", "standardisation", or "none" for min-max normalisation, standardisation to a mean of 0
+        and a standard deviation of 1, or no transformation respectively. Alternatively, a class instance with
+        fit_transform, transform, and inverse_transform functions, such as a scikit-learn transformer can be provided
+        directly too.
     units: str, Default = ""
         The units for the variable
 
     """
 
     name: str
     lower_bound: Union[int, float]
     upper_bound: Union[int, float]
-    transformation_type: Optional[str] = None
+    transformer: Optional = None
     units: str = ""
-    transformations: Transformations = field(init=False)
-
-    def __attrs_post_init__(self):
-        self.transformations = None
 
     def transform(self, X: np.ndarray) -> np.ndarray:
         """
 
-        Fit the transformation scalar to the inputted X array when self.transformation_type is "normalisation" or
-        "standardisation". The X array is subsequently transformed according to the fit scalar. When
-        self.transformation_type = "none", no transformation occurs
+        Fits a transformation scalar to the inputted X array when self.transformer is "normalisation",
+        "standardisation" or a transformer object. The X array is subsequently transformed according to the
+        fitted scalar. When self.transformation_type = "none", no transformation occurs
 
         Parameters
         ----------
         X: np.ndarray
             X array containing untransformed values for one variable
 
         """
-        if self.transformation_type is None:
+        if self.transformer is None:
             raise AttributeError(
-                "Please either: 1. Fit the model first, or 2. Set transformation_type = 'none', 'normalisation', or 'standarisation' when creating the variable instance"
+                "Please either: 1. Fit the model first, 2. Set transformer = 'none', 'normalisation', or "
+                "'standarisation' when creating the variable instance, or 3. Pass a transformer such as a scikit-learn "
+                "transformer when creating the variable instance"
             )
 
-        if self.transformation_type == "none":
+        if X.ndim == 1:
+            X = X.reshape(-1, 1)
+
+        if self.transformer == "none":
             return X
-        self.transformations = Transformations()
-        if self.transformation_type == "normalisation":
-            return self.transformations.minmaxscaler(X)
-        elif self.transformation_type == "standardisation":
-            return self.transformations.standardscaler(X)
+        elif self.transformer == "normalisation":
+            self.transformer = MinMaxScaler()
+        elif self.transformer == "standardisation":
+            self.transformer = StandardScaler()
+
+        return self.transformer.fit_transform(X)
 
     def transform_only(self, X: np.ndarray) -> np.ndarray:
         """
 
-        The X array is transformed according to the fit scalar in the self.transformations object. When
-        self.transformation_type = "none", no transformation occurs
+        The X array is transformed according to the fit scalar in the self.transformer object. When
+        self.transformer = "none", no transformation occurs
 
         Parameters
         ----------
         X: np.ndarray
             X array containing untransformed values for one variable
 
         """
-        if self.transformation_type is None:
+        if self.transformer is None:
             raise AttributeError(
-                "Please either: 1. Fit the model first, or 2. Set transformation_type = 'none', 'normalisation', or 'standarisation' when creating the variable instance"
+                "Please either: 1. Fit the model first, 2. Set transformer = 'none', 'normalisation', or "
+                "'standarisation' when creating the variable instance, or 3. Pass a transformer such as a scikit-learn "
+                "transformer when creating the variable instance"
             )
 
-        if self.transformation_type == "none":
+        if X.ndim == 1:
+            X = X.reshape(-1, 1)
+
+        if self.transformer == "none":
             return X
-        if self.transformation_type == "normalisation":
-            return self.transformations.minmaxscaler_transform_only(X)
-        elif self.transformation_type == "standardisation":
-            return self.transformations.standardscaler_transform_only(X)
+        else:
+            return self.transformer.transform(X)
 
     def inverse_transform(self, X_transform: np.ndarray) -> np.ndarray:
         """
 
-        The X_transform array undergoes an inverse transform according to the fit scalar in the self.transformations
-        object. When self.transformation_type = "none", no transformation occurs
+        The X_transform array undergoes an inverse transform according to the fit scalar in the self.transformer
+        object. When self.transformer = "none", no transformation occurs
 
         Parameters
         ----------
         X_transform: np.ndarray
             X array containing transformed values for one variable
 
         """
-        if self.transformation_type == "none":
+
+        if X_transform.ndim == 1:
+            X_transform = X_transform.reshape(-1, 1)
+
+        if self.transformer == "none":
             return X_transform
-        if isinstance(self.transformations.scaler, MinMaxScaler):
-            return self.transformations.inverse_minmaxscaler(X_transform)
-        elif isinstance(self.transformations.scaler, StandardScaler):
-            return self.transformations.inverse_standardscaler(X_transform)
+        else:
+            return self.transformer.inverse_transform(X_transform)
 
 
 @define(kw_only=True)
 class CategoricalVariable:
     """
 
     Base class for categorical variables
@@ -139,15 +145,14 @@
         The units for the variable
 
     """
 
     name: str
     categorical_levels: List[Union[str, int, float]]
     units: str = ""
-    transformations: Transformations = field(init=False)
 
     def enum_to_cat_level(self, X_array: np.ndarray) -> np.ndarray:
         """
 
         Converts the categorical level index to its respective name/value
 
         Parameters
@@ -219,104 +224,115 @@
         The categories/choices/levels for a given categorical variable
     units: str, Default = ""
         The units for the variable
     lower_bound: int | float, Default = None
         The lower bound of the variable
     upper_bound: int | float, Default = None
         The upper bound of the variable
-    transformation_type: str. Default = None
-        The type of transformation that should be applied to the variable for modelling. When left as the default
-        None, the modelling uses the default transformations specified by the model type. When specified, can be
-        "normalisation", "standardisation", or "none" for min-max normalisation, standardisation to a mean of 0 and a
-        standard deviation of 1, or no transformation respectively
+    transformer: Optional. Default = None
+        The transformation that should be applied to the variable for modelling. When left as the default
+        None, the modelling uses the default transformations specified by the model type. Can be specified as the
+        strings "normalisation", "standardisation", or "none" for min-max normalisation, standardisation to a mean of 0
+        and a standard deviation of 1, or no transformation respectively. Alternatively, a class instance with
+        fit_transform, transform, and inverse_transform functions, such as a scikit-learn transformer can be provided
+        directly too.
 
     """
 
     lower_bound: Optional[Union[int, float]] = None
     upper_bound: Optional[Union[int, float]] = None
-    transformation_type: Optional[str] = None
+    transformer: Optional = None
     num_categorical_levels: int = field(init=False)
 
     def __attrs_post_init__(self):
         self.num_categorical_levels = len(self.categorical_levels)
-        self.transformations = None
         if self.lower_bound is None:
             self.lower_bound = min(self.categorical_levels)
 
         if self.upper_bound is None:
             self.upper_bound = max(self.categorical_levels)
 
     def transform(self, X: np.ndarray) -> np.ndarray:
         """
 
-        Fit the transformation scalar to the inputted X array when self.transformation_type is "normalisation" or
-        "standardisation". The X array is subsequently transformed according to the fit scalar. When
-        self.transformation_type = "none", no transformation occurs
+        Fits a transformation scalar to the inputted X array when self.transformer is "normalisation",
+        "standardisation" or a transformer object. The X array is subsequently transformed according to the
+        fitted scalar. When self.transformer = "none", no transformation occurs
 
         Parameters
         ----------
         X: np.ndarray
             X array containing untransformed values for one variable
 
         """
-        if self.transformation_type is None:
+        if self.transformer is None:
             raise AttributeError(
-                "Please either: 1. Fit the model first, or 2. Set transformation_type = 'none', 'normalisation', or 'standarisation' when creating the variable instance"
+                "Please either: 1. Fit the model first, 2. Set transformer = 'none', 'normalisation', or "
+                "'standarisation' when creating the variable instance, or 3. Pass a transformer such as a scikit-learn "
+                "transformer when creating the variable instance"
             )
 
-        if self.transformation_type == "none":
+        if X.ndim == 1:
+            X = X.reshape(-1, 1)
+
+        if self.transformer == "none":
             return X
-        self.transformations = Transformations()
-        if self.transformation_type == "normalisation":
-            return self.transformations.minmaxscaler(X)
-        elif self.transformation_type == "standardisation":
-            return self.transformations.standardscaler(X)
+        elif self.transformer == "normalisation":
+            self.transformer = MinMaxScaler()
+        elif self.transformer == "standardisation":
+            self.transformer = StandardScaler()
+
+        return self.transformer.fit_transform(X)
 
     def transform_only(self, X: np.ndarray) -> np.ndarray:
         """
 
-        The X array is transformed according to the fit scalar in the self.transformations object. When
-        self.transformation_type = "none", no transformation occurs
+        The X array is transformed according to the fit scalar in the self.transformer object. When
+        self.transformer = "none", no transformation occurs
 
         Parameters
         ----------
         X: np.ndarray
             X array containing untransformed values for one variable
 
         """
-        if self.transformation_type is None:
+        if self.transformer is None:
             raise AttributeError(
-                "Please either: 1. Fit the model first, or 2. Set transformation_type = 'none', 'normalisation', or 'standarisation' when creating the variable instance"
+                "Please either: 1. Fit the model first, 2. Set transformer = 'none', 'normalisation', or "
+                "'standarisation' when creating the variable instance, or 3. Pass a transformer such as a scikit-learn "
+                "transformer when creating the variable instance"
             )
 
-        if self.transformation_type == "none":
+        if X.ndim == 1:
+            X = X.reshape(-1, 1)
+
+        if self.transformer == "none":
             return X
-        if self.transformation_type == "normalisation":
-            return self.transformations.minmaxscaler_transform_only(X)
-        elif self.transformation_type == "standardisation":
-            return self.transformations.standardscaler_transform_only(X)
+        else:
+            return self.transformer.transform(X)
 
     def inverse_transform(self, X_transform: np.ndarray) -> np.ndarray:
         """
 
-        The X_transform array undergoes an inverse transform according to the fit scalar in the self.transformations
-        object. When self.transformation_type = "none", no transformation occurs
+        The X_transform array undergoes an inverse transform according to the fit scalar in the self.transformer
+        object. When self.transformer = "none", no transformation occurs
 
         Parameters
         ----------
         X_transform: np.ndarray
             X array containing transformed values for one variable
 
         """
-        if self.transformation_type == "none":
+        if X_transform.ndim == 1:
+            X_transform = X_transform.reshape(-1, 1)
+
+        if self.transformer == "none":
             return X_transform
-        if isinstance(self.transformations.scaler, MinMaxScaler):
-            return self.transformations.inverse_minmaxscaler(X_transform)
-        elif isinstance(self.transformations.scaler, StandardScaler):
-            return self.transformations.inverse_standardscaler(X_transform)
+        else:
+            return self.transformer.inverse_transform(X_transform)
 
     def value_to_discrete(self, X: np.ndarray) -> np.ndarray:
         """
 
         Converts the categorical level index to their closest discrete value
 
         Parameters
@@ -329,15 +345,15 @@
         np.ndarray
             Array where the X values have been converted to their closest discrete values
 
         """
 
         X_new = copy.copy(X)
         for index, value in enumerate(X):
-            diff = ((self.categorical_levels - value) ** 2) ** 0.5
+            diff = ((np.array(self.categorical_levels) - value) ** 2) ** 0.5
             diff_min_index = np.argmin(diff)
             X_new[index] = self.categorical_levels[diff_min_index]
 
         return X_new
 
     def enum_to_discrete(self, X: np.ndarray) -> np.ndarray:
         """
@@ -373,54 +389,67 @@
     units: str, Default = ""
         The units for the variable
     descriptor_names: List[str]
         The names for each type of descriptor in the descriptor arrays
     categorical_descriptors: List[Any] | np.ndarray
         The array of descriptor values where the shape is [{number of categorical levels}, {number of descriptor types}],
         where each row in the array are the descriptors for each categorical level
-    transformation_type: str. Default = None
-        The type of transformation that should be applied to the variable for modelling. When left as the default
-        None, the modelling uses the default transformations specified by the model type. When specified, can be
-        "normalisation", "standardisation", or "none" for min-max normalisation, standardisation to a mean of 0 and a
-        standard deviation of 1, or no transformation respectively
+    transformer: Optional. Default = None
+        The transformation that should be applied to the variable for modelling. When left as the default
+        None, the modelling uses the default transformations specified by the model type. Can be specified as the
+        strings "normalisation", "standardisation", or "none" for min-max normalisation, standardisation to a mean of 0
+        and a standard deviation of 1, or no transformation respectively. Alternatively, a class instance with
+        fit_transform, transform, and inverse_transform functions, such as a scikit-learn transformer can be provided
+        directly too.
     lower_bound: int | float, Default = None
         The lower bound of the variable
     upper_bound: int | float, Default = None
         The upper bound of the variable
 
     """
 
     descriptor_names: List[str]
-    categorical_descriptors: Union[List[Any], np.ndarray]
-    transformation_type: Optional[str] = None
+    categorical_descriptors: Union[List[List[Union[int, float]]], np.ndarray]
+    transformer: Optional = None
     lower_bound: Optional[Union[int, float]] = None
     upper_bound: Optional[Union[int, float]] = None
     num_categorical_levels: int = field(init=False)
     num_descriptors: int = field(init=False)
 
     def __attrs_post_init__(self):
         self.num_categorical_levels = len(self.categorical_levels)
-        self.transformations = None
+
+        if not isinstance(self.categorical_descriptors, np.ndarray):
+            self.categorical_descriptors = np.array(self.categorical_descriptors)
+
+        if self.categorical_descriptors.ndim != 2:
+            raise ValueError(
+                f"The categorical descriptor array was provided is a {self.categorical_descriptors.ndim}D "
+                f"array. Please ensure that it is a 2D array"
+            )
+
         if self.lower_bound is None:
             self.lower_bound = []
             descriptor_range = np.ptp(self.categorical_descriptors, axis=0)
-            for descriptor, range in zip(np.array(self.categorical_descriptors).T, descriptor_range):
+            for descriptor, range in zip(self.categorical_descriptors.T, descriptor_range):
                 self.lower_bound.append(descriptor.min() - (range * 0.10))
 
         if self.upper_bound is None:
             self.upper_bound = []
             descriptor_range = np.ptp(self.categorical_descriptors, axis=0)
-            for descriptor, range in zip(np.array(self.categorical_descriptors).T, descriptor_range):
+            for descriptor, range in zip(self.categorical_descriptors.T, descriptor_range):
                 self.upper_bound.append(descriptor.max() + (range * 0.10))
 
-        self.num_descriptors = (
-            len(self.categorical_descriptors)
-            if np.array(self.categorical_descriptors).ndim == 1
-            else len(self.categorical_descriptors[0])
-        )
+        self.num_descriptors = self.categorical_descriptors.shape[1]
+
+        if len(self.descriptor_names) != self.num_descriptors:
+            raise ValueError(
+                f"The number of names provided for the descriptors ({len(self.descriptor_names)}) is not "
+                f"the same as the number of descriptors types provided ({self.num_descriptors})"
+            )
 
     def name_to_descriptor(self, X: np.ndarray) -> np.ndarray:
         """
 
         Converts the categorical level names into an array of the corresponding descriptor values
 
         Parameters
@@ -471,79 +500,90 @@
 
         """
         return np.vstack([self.categorical_descriptors[int(x)] for x in X])
 
     def transform(self, X: np.ndarray) -> np.ndarray:
         """
 
-        Fit the transformation scalar to the inputted X array when self.transformation_type is "normalisation" or
-        "standardisation". The X array is subsequently transformed according to the fit scalar. When
-        self.transformation_type = "none", no transformation occurs
+        Fits a transformation scalar to the inputted X array when self.transformer is "normalisation",
+        "standardisation" or a transformer object. The X array is subsequently transformed according to the
+        fitted scalar. When self.transformer = "none", no transformation occurs
 
         Parameters
         ----------
         X: np.ndarray
             X array containing untransformed values for one variable
 
         """
-        if self.transformation_type is None:
+        if self.transformer is None:
             raise AttributeError(
-                "Please either: 1. Fit the model first, or 2. Set transformation_type = 'none', 'normalisation', or 'standarisation' when creating the variable instance"
+                "Please either: 1. Fit the model first, 2. Set transformer = 'none', 'normalisation', or "
+                "'standarisation' when creating the variable instance, or 3. Pass a transformer such as a scikit-learn "
+                "transformer when creating the variable instance"
             )
 
-        if self.transformation_type == "none":
+        if X.ndim == 1:
+            X = X.reshape(-1, 1)
+
+        if self.transformer == "none":
             return X
-        self.transformations = Transformations()
-        if self.transformation_type == "normalisation":
-            return self.transformations.minmaxscaler(X)
-        elif self.transformation_type == "standardisation":
-            return self.transformations.standardscaler(X)
+        elif self.transformer == "normalisation":
+            self.transformer = MinMaxScaler()
+        elif self.transformer == "standardisation":
+            self.transformer = StandardScaler()
+
+        return self.transformer.fit_transform(X)
 
     def transform_only(self, X: np.ndarray) -> np.ndarray:
         """
 
-        The X array is transformed according to the fit scalar in the self.transformations object. When
-        self.transformation_type = "none", no transformation occurs
+        The X array is transformed according to the fit scalar in the self.transformer object. When
+        self.transformer = "none", no transformation occurs
 
         Parameters
         ----------
         X: np.ndarray
             X array containing untransformed values for one variable
 
         """
-        if self.transformation_type is None:
+        if self.transformer is None:
             raise AttributeError(
-                "Please either: 1. Fit the model first, or 2. Set transformation_type = 'none', 'normalisation', or 'standarisation' when creating the variable instance"
+                "Please either: 1. Fit the model first, 2. Set transformer = 'none', 'normalisation', or "
+                "'standarisation' when creating the variable instance, or 3. Pass a transformer such as a scikit-learn "
+                "transformer when creating the variable instance"
             )
 
-        if self.transformation_type == "none":
+        if X.ndim == 1:
+            X = X.reshape(-1, 1)
+
+        if self.transformer == "none":
             return X
-        if self.transformation_type == "normalisation":
-            return self.transformations.minmaxscaler_transform_only(X)
-        elif self.transformation_type == "standardisation":
-            return self.transformations.standardscaler_transform_only(X)
+        else:
+            return self.transformer.transform(X)
 
     def inverse_transform(self, X_transform: np.ndarray) -> np.ndarray:
         """
 
-        The X_transform array undergoes an inverse transform according to the fit scalar in the self.transformations
-        object. When self.transformation_type = "none", no transformation occurs
+        The X_transform array undergoes an inverse transform according to the fit scalar in the self.transformer
+        object. When self.transformer = "none", no transformation occurs
 
         Parameters
         ----------
         X_transform: np.ndarray
             X array containing transformed values for one variable
 
         """
-        if self.transformation_type == "none":
+
+        if X_transform.ndim == 1:
+            X_transform = X_transform.reshape(-1, 1)
+
+        if self.transformer == "none":
             return X_transform
-        if isinstance(self.transformations.scaler, MinMaxScaler):
-            return self.transformations.inverse_minmaxscaler(X_transform)
-        elif isinstance(self.transformations.scaler, StandardScaler):
-            return self.transformations.inverse_standardscaler(X_transform)
+        else:
+            return self.transformer.inverse_transform(X_transform)
 
 
 @define
 class VariablesList:
     """
 
     Class that stores all variables and their respective properties
@@ -563,14 +603,15 @@
     num_cat_descriptor_var: int = field(init=False)
     num_cat_var: int = field(init=False)
     categorical_levels: List[List[Union[str, int]]] = field(init=False)
     num_categorical_levels: int = field(init=False)
     descriptor_names: List[List[str]] = field(init=False)
     categorical_descriptors: List[List[str]] = field(init=False)
     num_descriptors: List[int] = field(init=False)
+    cont_var_units: List[str] = field(init=False)
     lower_bounds: List[Union[int, float]] = field(init=False)
     upper_bounds: List[Union[int, float]] = field(init=False)
     var_splitter_indexes: List[int] = field(init=False)
     n_var: int = field(init=False)
     continuous_var_names: List[str] = field(init=False)
 
     def __attrs_post_init__(self):
@@ -611,30 +652,39 @@
         (self.lower_bounds, self.upper_bounds, self.var_splitter_indexes, categorical_descriptor_index_range,) = (
             [],
             [],
             [],
             [],
         )
         var_counter = 0
+        self.cont_var_units = []
         for var_index, var in enumerate(self.variables):
             if isinstance(var, ContinuousVariable) or isinstance(var, CategoricalVariableDiscreteValues):
                 self.lower_bounds.append(var.lower_bound)
                 self.upper_bounds.append(var.upper_bound)
+                self.cont_var_units.append(var.units)
                 var_counter += 1
             elif isinstance(var, CategoricalVariableOneHot):
                 var_counter += var.num_categorical_levels
             elif isinstance(var, CategoricalVariableWithDescriptors):
                 for lower_value, upper_value in zip(var.lower_bound, var.upper_bound):
                     self.lower_bounds.append(lower_value)
                     self.upper_bounds.append(upper_value)
 
                 categorical_descriptor_index_range.append(
-                    [var.name, var_index, var_counter, var_counter + var.num_descriptors,]
+                    [
+                        var.name,
+                        var_index,
+                        var_counter,
+                        var_counter + var.num_descriptors,
+                    ]
                 )
                 var_counter += var.num_descriptors
+                self.cont_var_units += [""] * var.num_descriptors
+
             if var_index + 1 < len(self.variables):
                 self.var_splitter_indexes.append(var_counter)
 
         self.n_var = var_counter
 
         # List of variables names for all continuous variables, categorical variables with discrete values, and the
         # descriptor names in categorical variables with descriptors
@@ -642,19 +692,19 @@
         for var in self.variables:
             if isinstance(var, ContinuousVariable) or isinstance(var, CategoricalVariableDiscreteValues):
                 self.continuous_var_names.append(var.name)
             elif isinstance(var, CategoricalVariableWithDescriptors):
                 for descriptor_name in var.descriptor_names:
                     self.continuous_var_names.append(descriptor_name)
 
-    def transform(self, X: np.ndarray, transform_type: Optional[str] = None) -> np.ndarray:
+    def transform(self, X: np.ndarray, transform_type: Optional = None) -> np.ndarray:
         """
 
         Fits and transforms the X array containing data for multiple variables based on each variables'
-        transformation_type attribute
+        transformer attribute
 
         Parameters
         ----------
         X: np.ndarray
             X array containing untransformed values for all variables
         transform_type: str, Default = None
             Assigns the transformation type if one was not specified when the variable object was created
@@ -664,28 +714,28 @@
         np.ndarray
             X array containing transformed values for all variables
 
         """
         X_split = self.split_var(X)
         for var_index, var in enumerate(self.variables):
             if not isinstance(var, CategoricalVariableOneHot):
-                if var.transformation_type is None:
-                    var.transformation_type = transform_type
+                if var.transformer is None:
+                    var.transformer = transform_type
 
                 if X_split[var_index].shape[1] == 1:
                     X_split[var_index] = var.transform(X_split[var_index]).reshape(-1, 1)
                 else:
                     X_split[var_index] = var.transform(X_split[var_index])
 
         return np.hstack(X_split)
 
     def transform_only(self, X: np.ndarray) -> np.ndarray:
         """
 
-        Transforms the X array containing data for multiple variables based on each variables' transformation_type
+        Transforms the X array containing data for multiple variables based on each variables' transformer
         attribute using the previously fitted scalars
 
         Parameters
         ----------
         X: np.ndarray
             X array containing untransformed values for all variables
 
@@ -865,18 +915,16 @@
                 cat_descriptor_list = []
                 for x in X_split[var_index]:
                     x_norm = (x - np.array(var.lower_bound)) / (np.array(var.upper_bound) - np.array(var.lower_bound))
                     norm_categorical_descriptors = (var.categorical_descriptors - np.array(var.lower_bound)) / (
                         np.array(var.upper_bound) - np.array(var.lower_bound)
                     )
                     euc_dist = [np.linalg.norm(cat_level - x_norm) for cat_level in norm_categorical_descriptors]
-                    # euc_dist = [np.linalg.norm(cat_level - x) for cat_level in np.array(var.categorical_descriptors)]
                     euc_dist_min_index = np.argmin(euc_dist)
                     cat_descriptor_list.append(var.categorical_descriptors[euc_dist_min_index])
-                # X_split[var_index] = np.array(cat_descriptor_list).reshape(1, -1)
                 X_split[var_index] = np.array(cat_descriptor_list)
 
         return np.hstack(X_split)
 
     def enum_to_values(self, X_array: np.ndarray) -> np.ndarray:
         """
 
@@ -923,17 +971,14 @@
         X_array_object = X_array.astype(np.object)
         for var_index, var in enumerate(self.variables):
             if isinstance(var, CategoricalVariableWithDescriptors):
                 X_array_object[:, var_index] = var.name_to_descriptor(X_array[:, var_index])
 
         return X_array_object.astype("float64")
 
-    # def reshape_to_2d(self, X_array: np.ndarray) -> np.ndarray:
-    #     return np.hstack(X_array.ravel().tolist()).reshape(X_array.shape[0], self.n_var)
-
     def split_var(self, X_array: np.ndarray) -> List[np.ndarray]:
         """
 
         Splits an X-array that contains the continuous and categorical variables into a list of sub-arrays for each
         individual variable
 
         Parameters
```

### Comparing `nemo-bo-0.1.8/nemo_bo/utils/data_proc.py` & `nemo-bo-0.1.9/nemo_bo/utils/data_proc.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def remove_nan(arr1: np.ndarray, arr2: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
     """
 
     Removes slices in two arrays,arr1 and arr2, based on the indexes where there are NaN values in arr2. This method is
     useful to allow ML models to be fitted when you have an irregular number of Y-values for different objectives.
-    Ignores any NaN values in arr1 that maybe in arr2.
+    Ignores any NaN values in arr1.
 
     Parameters
     ----------
     arr1: np.ndarray
         Array that will be manipulated based on the values in arr2
     arr2: np.ndarray
         The array with shape (n, ) that is used to identify the indexes where NaN values are. These indexes are applied
@@ -25,18 +25,22 @@
         Array with slices removed that corresponded with the indexes of any NaN in the arr2 array
     arr2: np.ndarray
         Array with all NaN values removed
 
     """
     if arr1.shape[0] != arr2.shape[0]:
         raise ValueError(
-            f"The arr1 shape at index 0 (arr1.shape[0]) is not the same as the arr2 shape at index 0 (arr2.shape[0])"
+            f"The arr1 shape at index 0 ({arr1.shape[0]}) is not the same as the arr2 shape at index 0 ({arr2.shape[0]})"
         )
 
-    nan_mask = ~np.isnan(arr2)
+    if arr2.ndim == 1:
+        nan_mask = ~np.isnan(arr2)
+    else:
+        nan_mask = ~np.isnan(arr2).any(axis=1)
+
     return arr1[nan_mask], arr2[nan_mask]
 
 
 def remove_all_nan_rows(Y: np.ndarray) -> np.ndarray:
     """
 
     Any rows that contain missing values (NaN) are removed. For example, useful for acquisition functions, which do not
@@ -108,16 +112,16 @@
     (splitnum/2) for the validation set. The remaining data in the array are used in the training set
 
     Parameters
     ----------
     array: np.ndarray
 
     splitnum: int
-        e.g. splitnum = 5 will cause every 5th row in the provided array to be extracted for the test set. Every 5th row
-        starting from the splitnum/2 row will be extracted for the validation set
+        e.g. splitnum = 5 will cause every 5th row in the provided array to be extracted for the test set. Every 5th
+        row starting from the splitnum/2 row will be extracted for the validation set
 
     Returns
     -------
     array_train: np.ndarray
         Training set created from the provided array
     array_val: np.ndarray
         Validation set created from the provided array
@@ -139,15 +143,19 @@
 def train_val_test_split_blocks(array: np.ndarray, test_ratio: float) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """
 
     Splits the inputted array into three equally sized parts for training, validation, and test sets
 
     """
     array_train, array_val, array_test = np.split(
-        array, [int((1 - (2 * test_ratio)) * array.shape[0]), int((1 - test_ratio) * array.shape[0]),],
+        array,
+        [
+            int((1 - (2 * test_ratio)) * array.shape[0]),
+            int((1 - test_ratio) * array.shape[0]),
+        ],
     )
 
     return array_train, array_val, array_test
 
 
 def shuffle(X: np.ndarray, Y: np.ndarray, seed: int) -> Tuple[np.ndarray, np.ndarray]:
     """
@@ -161,16 +169,16 @@
 
 
 def sort_train_test_split_shuffle(
     X: np.ndarray, Y: np.ndarray, test_ratio: float = 0.2, seed: int = None
 ) -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
     """
 
-    Sequentially (i) sorts the inputted X and Y arrays, (ii) splits into training and test sets, and then (iii) shuffles
-    the training and test sets
+    Sequentially (i) sorts the inputted X and Y arrays, (ii) splits into training and test sets, and then (iii)
+    shuffles the training and test sets
 
     Parameters
     ----------
     X: np.ndarray
         X array containing variables data
     Y: np.ndarray
         Y array containing objectives data with shape (y, )
```

### Comparing `nemo-bo-0.1.8/nemo_bo/utils/extract_excel.py` & `nemo-bo-0.1.9/nemo_bo/utils/extract_excel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+import ast
 import numpy as np
 import pandas as pd
-from typing import Tuple, Union
+from typing import Tuple
 
 from nemo_bo.opt.objectives import CalculableObjective, RegressionObjective, ObjectivesList
 from nemo_bo.opt.variables import (
     CategoricalVariableWithDescriptors,
     CategoricalVariableDiscreteValues,
     ContinuousVariable,
     VariablesList,
 )
 
 
 def extract_input_template(input_template_xlsx: str) -> Tuple[np.ndarray, np.ndarray, VariablesList, ObjectivesList]:
     """
-    Function that can extract user-inputted variables and objectives information and data from the input template provided
+    Function that can extract user-inputted variables and objectives information and data from the input template
+    provided
 
     Parameters
     ----------
     input_template_xlsx: str
         Excel file for the input template containing the variables, objectives, and data
 
     Returns
@@ -37,16 +39,16 @@
     for var_index, var_type in enumerate(input_template["Variables"].columns):
         if "ContinuousVariable" in var_type:
             var_list.append(
                 ContinuousVariable(
                     name=input_template["Variables"].loc["name"][var_index],
                     lower_bound=input_template["Variables"].loc["lower_bound"][var_index],
                     upper_bound=input_template["Variables"].loc["upper_bound"][var_index],
-                    transformation_type=input_template["Variables"].loc["transformation_type"][var_index]
-                    if not pd.isnull(input_template["Variables"].loc["transformation_type"][var_index])
+                    transformer=input_template["Variables"].loc["transformer"][var_index]
+                    if not pd.isnull(input_template["Variables"].loc["transformer"][var_index])
                     else None,
                     units=input_template["Variables"].loc["units"][var_index]
                     if not pd.isnull(input_template["Variables"].loc["units"][var_index])
                     else None,
                 )
             )
         elif "CategoricalVariableDiscreteValues" in var_type:
@@ -57,16 +59,16 @@
                     categorical_levels=list(input_template[name].index),
                     lower_bound=input_template["Variables"].loc["lower_bound"][var_index]
                     if not pd.isnull(input_template["Variables"].loc["lower_bound"][var_index])
                     else None,
                     upper_bound=input_template["Variables"].loc["upper_bound"][var_index]
                     if not pd.isnull(input_template["Variables"].loc["upper_bound"][var_index])
                     else None,
-                    transformation_type=input_template["Variables"].loc["transformation_type"][var_index]
-                    if not pd.isnull(input_template["Variables"].loc["transformation_type"][var_index])
+                    transformer=input_template["Variables"].loc["transformer"][var_index]
+                    if not pd.isnull(input_template["Variables"].loc["transformer"][var_index])
                     else None,
                     units=input_template["Variables"].loc["units"][var_index]
                     if not pd.isnull(input_template["Variables"].loc["units"][var_index])
                     else None,
                 )
             )
         elif "CategoricalVariableWithDescriptors" in var_type:
@@ -79,16 +81,16 @@
                     categorical_descriptors=input_template[name].values,
                     lower_bound=input_template["Variables"].loc["lower_bound"][var_index]
                     if not pd.isnull(input_template["Variables"].loc["lower_bound"][var_index])
                     else None,
                     upper_bound=input_template["Variables"].loc["upper_bound"][var_index]
                     if not pd.isnull(input_template["Variables"].loc["upper_bound"][var_index])
                     else None,
-                    transformation_type=input_template["Variables"].loc["transformation_type"][var_index]
-                    if not pd.isnull(input_template["Variables"].loc["transformation_type"][var_index])
+                    transformer=input_template["Variables"].loc["transformer"][var_index]
+                    if not pd.isnull(input_template["Variables"].loc["transformer"][var_index])
                     else None,
                     units=input_template["Variables"].loc["units"][var_index]
                     if not pd.isnull(input_template["Variables"].loc["units"][var_index])
                     else None,
                 )
             )
 
@@ -97,35 +99,39 @@
         if "RegressionObjective" in obj_type:
             obj_list.append(
                 RegressionObjective(
                     name=input_template["Objectives"].loc["name"][obj_index],
                     obj_max_bool=input_template["Objectives"].loc["obj_max_bool"][obj_index],
                     lower_bound=input_template["Objectives"].loc["lower_bound"][obj_index],
                     upper_bound=input_template["Objectives"].loc["upper_bound"][obj_index],
-                    transformation_type=input_template["Objectives"].loc["transformation_type"][obj_index]
-                    if not pd.isnull(input_template["Objectives"].loc["transformation_type"][obj_index])
+                    transformer=input_template["Objectives"].loc["transformer"][obj_index]
+                    if not pd.isnull(input_template["Objectives"].loc["transformer"][obj_index])
                     else None,
                     units=input_template["Objectives"].loc["units"][obj_index]
                     if not pd.isnull(input_template["Objectives"].loc["units"][obj_index])
                     else None,
-                    predictor_type=[input_template["Objectives"].loc["predictor_type"][obj_index]]
+                    predictor_type=ast.literal_eval(input_template["Objectives"].loc["predictor_type"][obj_index])
                     if not pd.isnull(input_template["Objectives"].loc["predictor_type"][obj_index])
                     else None,
                 )
             )
         elif "CalculableObjective" in obj_type:
             obj_list.append(
                 CalculableObjective(
                     name=input_template["Objectives"].loc["name"][obj_index],
                     obj_max_bool=input_template["Objectives"].loc["obj_max_bool"][obj_index],
                     lower_bound=input_template["Objectives"].loc["lower_bound"][obj_index],
                     upper_bound=input_template["Objectives"].loc["upper_bound"][obj_index],
+                    transformer=input_template["Variables"].loc["transformer"][obj_index]
+                    if not pd.isnull(input_template["Variables"].loc["transformer"][obj_index])
+                    else None,
                     units=input_template["Objectives"].loc["units"][obj_index]
                     if not pd.isnull(input_template["Objectives"].loc["units"][obj_index])
                     else None,
+                    obj_function=None,
                 )
             )
 
     X = input_template["Variables"].iloc[5:, :].values
     Y = input_template["Objectives"].iloc[7:, :].values.astype(float)
     var_list = VariablesList(var_list)
     obj_list = ObjectivesList(obj_list)
```

### Comparing `nemo-bo-0.1.8/nemo_bo/utils/logger.py` & `nemo-bo-0.1.9/nemo_bo/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,19 @@
         Name of the .py file that is creating the logging entry
     -------
 
     """
     global logging_path
     if not os.path.exists(os.path.join(os.getcwd(), "Log Files")):
         os.makedirs(os.path.join(os.getcwd(), "Log Files"))
-    logging_path = os.path.join(os.getcwd(), "Log Files", f"Log, {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}.log",)
+    logging_path = os.path.join(
+        os.getcwd(),
+        "Log Files",
+        f"Log, {datetime.now().strftime('%d-%m-%Y, %H-%M-%S')}.log",
+    )
 
     logger = logging.getLogger(name)
     logger.setLevel(logging.DEBUG)
     logger.propagate = False
 
     logfile = logging.FileHandler(logging_path, mode="a")
     logfile.setLevel(logging.DEBUG)
```

### Comparing `nemo-bo-0.1.8/nemo_bo/utils/perf_metrics.py` & `nemo-bo-0.1.9/nemo_bo/utils/perf_metrics.py`

 * *Files identical despite different names*

### Comparing `nemo-bo-0.1.8/nemo_bo/utils/plotter.py` & `nemo-bo-0.1.9/nemo_bo/utils/plotter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 from typing import Any, List, Optional, Tuple, Union
 
+import matplotlib.animation as animation
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+from matplotlib.animation import FuncAnimation
 from matplotlib.axes import Axes
 
 
 def scatter_plot(
     ax: Axes,
     data: Union[List[np.ndarray], np.ndarray],
     legend: Union[str, List[str]],
@@ -92,19 +94,29 @@
                         fillstyle="none",
                     )
         # Else if the array provided is 3D
         elif data_plot.shape[1] == 3:
             # If legend information was provided
             if legend is not None:
                 ax.scatter(
-                    data_plot[:, 0], data_plot[:, 1], data_plot[:, 2], label=legend, marker="o", s=40,
+                    data_plot[:, 0],
+                    data_plot[:, 1],
+                    data_plot[:, 2],
+                    label=legend,
+                    marker="o",
+                    s=40,
                 )
             else:
                 ax.scatter(
-                    data_plot[:, 0], data_plot[:, 1], data_plot[:, 2], label="Scatter plot", marker="o", s=40,
+                    data_plot[:, 0],
+                    data_plot[:, 1],
+                    data_plot[:, 2],
+                    label="Scatter plot",
+                    marker="o",
+                    s=40,
                 )
     # Else the data provided is a list of arrays
     else:
         # Iterate through the list of arrays and plot each one
         for plotnum in range(len(data)):
             data_plot = np.array(data[plotnum])
             # If the array provided is 2D
@@ -154,15 +166,20 @@
                             fillstyle="none",
                         )
             # Else if the array provided is 3D
             elif data_plot.shape[1] == 3:
                 # If legend information was provided
                 if legend is not None:
                     ax.scatter(
-                        data_plot[:, 0], data_plot[:, 1], data_plot[:, 2], label=legend[plotnum], marker="o", s=40,
+                        data_plot[:, 0],
+                        data_plot[:, 1],
+                        data_plot[:, 2],
+                        label=legend[plotnum],
+                        marker="o",
+                        s=40,
                     )
                 else:
                     ax.scatter(
                         data_plot[:, 0],
                         data_plot[:, 1],
                         data_plot[:, 2],
                         label=f"Scatter plot {plotnum + 1}",
@@ -204,49 +221,70 @@
         # If the array provided is 2D
         if data_plot.shape[1] == 2:
             # If legend information was provided
             if legend is not None:
                 plt.plot(data_plot[:, 0], data_plot[:, 1], label=legend, color=colorcycle[0])
             else:
                 plt.plot(
-                    data_plot[:, 0], data_plot[:, 1], label="Line plot", color=colorcycle[0],
+                    data_plot[:, 0],
+                    data_plot[:, 1],
+                    label="Line plot",
+                    color=colorcycle[0],
                 )
         # Else if the array provided is 3D
         elif data_plot.shape[1] == 3:
             # If legend information was provided
             if legend is not None:
                 plt.plot(
-                    data_plot[:, 0], data_plot[:, 1], data_plot[:, 2], label=legend, color=colorcycle[0],
+                    data_plot[:, 0],
+                    data_plot[:, 1],
+                    data_plot[:, 2],
+                    label=legend,
+                    color=colorcycle[0],
                 )
             else:
                 plt.plot(
-                    data_plot[:, 0], data_plot[:, 1], data_plot[:, 2], label="Line plot", color=colorcycle[0],
+                    data_plot[:, 0],
+                    data_plot[:, 1],
+                    data_plot[:, 2],
+                    label="Line plot",
+                    color=colorcycle[0],
                 )
     # Else the data provided is a list of arrays
     else:
         # Iterate through the list of arrays and plot each one
         for plotnum in range(len(data)):
             data_plot = np.array(data[plotnum])
             # If the array provided is 2D
             if data_plot.shape[1] == 2:
                 # If legend information was provided
                 if legend is not None:
                     plt.plot(
-                        data_plot[:, 0], data_plot[:, 1], label=legend[plotnum], color=colorcycle[plotnum],
+                        data_plot[:, 0],
+                        data_plot[:, 1],
+                        label=legend[plotnum],
+                        color=colorcycle[plotnum],
                     )
                 else:
                     plt.plot(
-                        data_plot[:, 0], data_plot[:, 1], label=f"Line plot {plotnum + 1}", color=colorcycle[plotnum],
+                        data_plot[:, 0],
+                        data_plot[:, 1],
+                        label=f"Line plot {plotnum + 1}",
+                        color=colorcycle[plotnum],
                     )
             # Else if the array provided is 3D
             elif data_plot.shape[1] == 3:
                 # If legend information was provided
                 if legend is not None:
                     plt.plot(
-                        data_plot[:, 0], data_plot[:, 1], data_plot[:, 2], label=legend[plotnum], color=colorcycle[0],
+                        data_plot[:, 0],
+                        data_plot[:, 1],
+                        data_plot[:, 2],
+                        label=legend[plotnum],
+                        color=colorcycle[0],
                     )
                 else:
                     plt.plot(
                         data_plot[:, 0],
                         data_plot[:, 1],
                         data_plot[:, 2],
                         label=f"Line plot {plotnum + 1}",
@@ -367,52 +405,61 @@
     for i, angle in enumerate(angles):
         ax.view_init(elev=None, azim=angle)  # elevation set to None
         fname = f"tmpimg_{i}.jpeg"
         ax.figure.savefig(fname, dpi=400)  # dpi set to 400
         imagefiles_list.append(fname)
 
     # Uses mencoder.exe in the home directory to produce a .mp4 movie from a list of image files.
-    command = f'mencoder "mf://{",".join(imagefiles_list)}" -mf fps={10} -o {output_file}.mp4 -ovc lavc -lavcopts vcodec=msmpeg4v2:vbitrate={8000}'  # fps=10, bitrate=8000
+    command = (
+        f'mencoder "mf://{",".join(imagefiles_list)}" -mf fps={10} -o {output_file}.mp4 -ovc lavc -lavcopts '
+        f"vcodec=msmpeg4v2:vbitrate={8000}"
+    )  # fps=10, bitrate=8000
     os.system(command)
 
     # Deleted the temporary image files created above
     for f in imagefiles_list:
         os.remove(f)
 
 
 def plot(
     plot_dim: str = "2D",
     scatter_data: Optional[Union[List[Union[np.ndarray, pd.DataFrame]], np.ndarray, pd.DataFrame]] = None,
     error: Optional[Union[List[np.ndarray], np.ndarray]] = None,
     line_data: Optional[Union[List[Union[np.ndarray, pd.DataFrame]], np.ndarray, pd.DataFrame]] = None,
     surface_data: Optional[Union[List[Union[np.ndarray, pd.DataFrame]], np.ndarray, pd.DataFrame]] = None,
+    animation_scatter_data: Optional[Union[np.ndarray, pd.DataFrame]] = None,
+    animated_scatter_fps: int = 2,
     scatter_legend: Optional[Union[str, List[str], Tuple[str]]] = None,
     line_legend: Optional[Union[str, List[str]]] = None,
     surface_legend: Optional[Union[str, List[str]]] = None,
     xlabel: str = "x",
     ylabel: str = "y",
     zlabel: str = "z",
     plottitle: str = "Title",
     output_file: str = "Plot",
     write_mp4: bool = False,
 ) -> None:
     """
 
-    Function to start the plotting of a new 2D or 3D figure
+    Function to start the plotting of a new 2D or 3D figure (including animated 2D scatter plots)
 
     Parameters
     ----------
     plot_dim: str, Default = '2D'
         Refers to the number of dimensions for the desired plot
     scatter_data: List[np.ndarray | pd.DataFrame] | np.ndarray | pd.DataFrame, Default is None
         The data used for the scatter plot can be either a 2D (x, y) or 3D (x, y, z) array or a list of 2D or 3D arrays
     line_data: List[np.ndarray | pd.DataFrame] | np.ndarray | pd.DataFrame, Default = None
         The data used for the line plot can be either a 2D (x, y) or 3D (x, y, z) array or a list of 2D or 3D arrays
     surface_data: List[np.ndarray | pd.DataFrame] | np.ndarray | pd.DataFrame, Default is None
         The data used for the surface plot can be either a 3D (x, y, z) array or a list of 3D arrays
+    animated_scatter_data: np.ndarray | pd.DataFrame, Default = 2
+        The 2D (x, y) data to be animated one point at a time
+    animated_scatter_fps: int, Default is None
+        The number of frames per second to animate at for the animated scatter data
     scatter_legend: str | List[str] | Tuple[str], Default is None
         The string or list of strings used to label the new scatter plot(s)
     line_legend: str | List[str], Default is None.
         The string or list of strings used to label the new line plot(s)
     surface_legend: str | List[str] | Tuple[str], Default is None
         The string or list of strings used to label the new surface plot(s)
     xlabel: str, Default is "x"
@@ -435,15 +482,16 @@
     if plot_dim == "2D":
         fig = plt.figure(figsize=(8, 8))
         ax = fig.add_subplot(1, 1, 1)
     elif plot_dim == "3D":
         fig = plt.figure()
         ax = fig.add_subplot(111, projection="3d")
 
-    # Creates the scatter, line, or surface plot Axes objects respectively, depending on if the data for each type of plot was provided
+    # Creates the scatter, line, or surface plot Axes objects respectively, depending on if the data for each type of
+    # plot was provided
     if scatter_data is not None:
         scatter_data = data_to_np(scatter_data)
         scatter_plot(ax, scatter_data, scatter_legend, error)
     if line_data is not None:
         line_data = data_to_np(line_data)
         line_plot(line_data, line_legend)
     if surface_data is not None:
@@ -464,14 +512,28 @@
         ax.set_title(plottitle, pad=24, fontsize=6)
         plt.legend(loc="best", fontsize=6)
 
     # Additional style settings for the figure
     ax.set_axisbelow(True)
     plt.grid(b=True, which="major", c="whitesmoke")
 
+    if animation_scatter_data is not None:
+        if plot_dim != "2D":
+            raise TypeError("Animated scatter plots are currently only supported for 2D scatter plots (plot_dim='2D')")
+
+        animation_scatter_data = data_to_np(animation_scatter_data)
+        (graph,) = plt.plot([], [], "o", color="red", markersize=10)
+
+        def animate(i):
+            graph.set_data(animation_scatter_data[: i + 1, 0], animation_scatter_data[: i + 1, 1])
+            return graph
+
+        ani = FuncAnimation(fig, animate, frames=animation_scatter_data.shape[0], repeat=False, interval=500)
+        ani.save(f"{output_file}.mp4", writer=animation.FFMpegWriter(fps=animated_scatter_fps), dpi=400)
+
     # Writes a .png image file of the figure
     plt.savefig(f"{output_file}.png", dpi=400)
 
     # Writes a .mp4 video file of a rotating 3D Matplotlib plot
     if plot_dim == "3D":
         if write_mp4 == True:
             plot3d_video(ax, output_file)
```

### Comparing `nemo-bo-0.1.8/pyproject.toml` & `nemo-bo-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nemo-bo"
-version = "0.1.8"
+version = "0.1.9"
 description = "Multi-objective optimization of chemical processes with automated machine learning workflows"
 authors = ["Simon Sung <simon.sung06@gmail.com>", "Mohammed Jeraal <m.jeraal@gmail.com>"]
 license = "MIT"
 readme = 'README.md'
 repository = "https://github.com/sustainable-processes/NEMO"
 homepage = "https://github.com/sustainable-processes/NEMO"
 keywords = ["machine-learning", "bayesian-optimization", "multi-objective-optimization"]
@@ -13,15 +13,15 @@
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 
 [tool.poetry.dependencies]
-python = ">= 3.7.0, <=3.9.13"
+python = ">= 3.9.0, <=3.9.13"
 
 # For opt
 attrs = "^21.4.0"
 cython = "^0.29.30"
 matplotlib = "^3.5.2"
 numpy = "^1.22.4"
 pandas = "^1.4.2"
```

