# Comparing `tmp/theseus-ai-nightly-2023.4.11.tar.gz` & `tmp/theseus-ai-nightly-2023.4.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theseus-ai-nightly-2023.4.11.tar", last modified: Tue Apr 11 23:05:02 2023, max compression
+gzip compressed data, was "theseus-ai-nightly-2023.4.12.tar", last modified: Wed Apr 12 22:35:58 2023, max compression
```

## Comparing `theseus-ai-nightly-2023.4.11.tar` & `theseus-ai-nightly-2023.4.12.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.881990 theseus-ai-nightly-2023.4.11/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/LICENSE
--rw-r--r--   0 root         (0) root         (0)       91 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    11642 2023-04-11 23:05:02.881990 theseus-ai-nightly-2023.4.11/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11035 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.849989 theseus-ai-nightly-2023.4.11/examples/
--rw-r--r--   0 root         (0) root         (0)      179 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/examples/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7193 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/examples/backward_modes.py
--rw-r--r--   0 root         (0) root         (0)     8158 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/examples/bundle_adjustment.py
--rw-r--r--   0 root         (0) root         (0)    19017 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/examples/homography_estimation.py
--rw-r--r--   0 root         (0) root         (0)     9181 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/examples/motion_planning_2d.py
--rw-r--r--   0 root         (0) root         (0)     2352 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/examples/se2_inverse.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/examples/se2_planning.py
--rw-r--r--   0 root         (0) root         (0)     1777 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/examples/simple_example.py
--rw-r--r--   0 root         (0) root         (0)    12290 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/examples/state_estimation_2d.py
--rw-r--r--   0 root         (0) root         (0)     4387 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/examples/tactile_pose_estimation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.849989 theseus-ai-nightly-2023.4.11/requirements/
--rw-r--r--   0 root         (0) root         (0)      192 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/requirements/dev.txt
--rw-r--r--   0 root         (0) root         (0)      174 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      176 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/requirements/main.txt
--rw-r--r--   0 root         (0) root         (0)      430 2023-04-11 23:05:02.881990 theseus-ai-nightly-2023.4.11/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6284 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.849989 theseus-ai-nightly-2023.4.11/tests/
--rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.853989 theseus-ai-nightly-2023.4.11/tests/core/
--rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7070 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/core/common.py
--rw-r--r--   0 root         (0) root         (0)    13514 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/core/test_cost_function.py
--rw-r--r--   0 root         (0) root         (0)     4442 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/core/test_cost_weight.py
--rw-r--r--   0 root         (0) root         (0)     2270 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/core/test_manifold.py
--rw-r--r--   0 root         (0) root         (0)    19419 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/core/test_objective.py
--rw-r--r--   0 root         (0) root         (0)     5416 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/core/test_robust_cost.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/core/test_theseus_function.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/core/test_variable.py
--rw-r--r--   0 root         (0) root         (0)    14670 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/core/test_vectorizer.py
--rw-r--r--   0 root         (0) root         (0)      857 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.853989 theseus-ai-nightly-2023.4.11/tests/extlib/
--rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/extlib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4777 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/extlib/test_baspacho.py
--rw-r--r--   0 root         (0) root         (0)     3106 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/extlib/test_baspacho_simple.py
--rw-r--r--   0 root         (0) root         (0)     3702 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/extlib/test_cusolver_lu_solver.py
--rw-r--r--   0 root         (0) root         (0)     4409 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/extlib/test_mat_mult.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.857990 theseus-ai-nightly-2023.4.11/tests/geometry/
--rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/geometry/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19548 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/geometry/common.py
--rw-r--r--   0 root         (0) root         (0)      792 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/geometry/point_types_mypy_check.py
--rw-r--r--   0 root         (0) root         (0)     4561 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/geometry/test_point_types.py
--rw-r--r--   0 root         (0) root         (0)     8862 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/geometry/test_se2.py
--rw-r--r--   0 root         (0) root         (0)    12861 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/geometry/test_se3.py
--rw-r--r--   0 root         (0) root         (0)     6566 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/geometry/test_so2.py
--rw-r--r--   0 root         (0) root         (0)    10391 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/geometry/test_so3.py
--rw-r--r--   0 root         (0) root         (0)     7443 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/geometry/test_vector.py
--rw-r--r--   0 root         (0) root         (0)     4011 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/tests/test_dlm_perturbation.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/tests/test_pgo_benchmark.py
--rw-r--r--   0 root         (0) root         (0)    21069 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/tests/test_theseus_layer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.857990 theseus-ai-nightly-2023.4.11/theseus/
--rw-r--r--   0 root         (0) root         (0)     2121 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.857990 theseus-ai-nightly-2023.4.11/theseus/core/
--rw-r--r--   0 root         (0) root         (0)      624 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15935 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/core/cost_function.py
--rw-r--r--   0 root         (0) root         (0)     4984 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/core/cost_weight.py
--rw-r--r--   0 root         (0) root         (0)    30933 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/core/objective.py
--rw-r--r--   0 root         (0) root         (0)     6131 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/core/robust_cost_function.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/core/robust_loss.py
--rw-r--r--   0 root         (0) root         (0)     6417 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/core/theseus_function.py
--rw-r--r--   0 root         (0) root         (0)     4800 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/core/variable.py
--rw-r--r--   0 root         (0) root         (0)    20067 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/core/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.857990 theseus-ai-nightly-2023.4.11/theseus/embodied/
--rw-r--r--   0 root         (0) root         (0)      581 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.857990 theseus-ai-nightly-2023.4.11/theseus/embodied/collision/
--rw-r--r--   0 root         (0) root         (0)      329 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/collision/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3616 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/collision/collision.py
--rw-r--r--   0 root         (0) root         (0)     4906 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/collision/eff_obj_contact.py
--rw-r--r--   0 root         (0) root         (0)     8782 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/collision/signed_distance_field.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.861990 theseus-ai-nightly-2023.4.11/theseus/embodied/kinematics/
--rw-r--r--   0 root         (0) root         (0)      257 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/kinematics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3894 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/kinematics/kinematics_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.861990 theseus-ai-nightly-2023.4.11/theseus/embodied/measurements/
--rw-r--r--   0 root         (0) root         (0)      301 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/measurements/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/measurements/between.py
--rw-r--r--   0 root         (0) root         (0)     2730 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/measurements/moving_frame_between.py
--rw-r--r--   0 root         (0) root         (0)     4090 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/measurements/reprojection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.861990 theseus-ai-nightly-2023.4.11/theseus/embodied/misc/
--rw-r--r--   0 root         (0) root         (0)      213 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/misc/local_cost_fn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.861990 theseus-ai-nightly-2023.4.11/theseus/embodied/motionmodel/
--rw-r--r--   0 root         (0) root         (0)      365 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/motionmodel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7715 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/motionmodel/double_integrator.py
--rw-r--r--   0 root         (0) root         (0)     6957 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/motionmodel/misc.py
--rw-r--r--   0 root         (0) root         (0)    11526 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/embodied/motionmodel/quasi_static_pushing_planar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.865990 theseus-ai-nightly-2023.4.11/theseus/extlib/
--rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/extlib/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14114 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/extlib/baspacho_solver.cpp
--rw-r--r--   0 root         (0) root         (0)     3751 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/extlib/baspacho_solver.h
--rw-r--r--   0 root         (0) root         (0)    12381 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/extlib/baspacho_solver_cuda.cu
--rw-r--r--   0 root         (0) root         (0)    16013 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/extlib/cusolver_lu_solver.cpp
--rw-r--r--   0 root         (0) root         (0)     3140 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/extlib/cusolver_sp_defs.cpp
--rw-r--r--   0 root         (0) root         (0)      744 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/extlib/cusolver_sp_defs.h
--rw-r--r--   0 root         (0) root         (0)    14555 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/extlib/mat_mult.cu
--rw-r--r--   0 root         (0) root         (0)     1186 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/extlib/utils.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.865990 theseus-ai-nightly-2023.4.11/theseus/geometry/
--rw-r--r--   0 root         (0) root         (0)      911 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/geometry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7224 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/geometry/lie_group.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/geometry/lie_group_check.py
--rw-r--r--   0 root         (0) root         (0)     5689 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/geometry/manifold.py
--rw-r--r--   0 root         (0) root         (0)     7322 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/geometry/point_types.py
--rw-r--r--   0 root         (0) root         (0)    16533 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/geometry/se2.py
--rw-r--r--   0 root         (0) root         (0)    29506 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/geometry/se3.py
--rw-r--r--   0 root         (0) root         (0)    11359 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/geometry/so2.py
--rw-r--r--   0 root         (0) root         (0)    25233 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/geometry/so3.py
--rw-r--r--   0 root         (0) root         (0)     2683 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/geometry/utils.py
--rw-r--r--   0 root         (0) root         (0)     9405 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/geometry/vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.865990 theseus-ai-nightly-2023.4.11/theseus/labs/
--rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/labs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.865990 theseus-ai-nightly-2023.4.11/theseus/labs/lie/
--rw-r--r--   0 root         (0) root         (0)      493 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/labs/lie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.869990 theseus-ai-nightly-2023.4.11/theseus/labs/lie/functional/
--rw-r--r--   0 root         (0) root         (0)      247 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/labs/lie/functional/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/labs/lie/functional/constants.py
--rw-r--r--   0 root         (0) root         (0)     7221 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/labs/lie/functional/lie_group.py
--rw-r--r--   0 root         (0) root         (0)    34776 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/labs/lie/functional/se3_impl.py
--rw-r--r--   0 root         (0) root         (0)    30196 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/labs/lie/functional/so3_impl.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/labs/lie/functional/utils.py
--rw-r--r--   0 root         (0) root         (0)    17619 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/labs/lie/lie_tensor.py
--rw-r--r--   0 root         (0) root         (0)     2661 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/labs/lie/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.869990 theseus-ai-nightly-2023.4.11/theseus/optimizer/
--rw-r--r--   0 root         (0) root         (0)      505 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.869990 theseus-ai-nightly-2023.4.11/theseus/optimizer/autograd/
--rw-r--r--   0 root         (0) root         (0)      454 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/autograd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5948 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/autograd/baspacho_sparse_autograd.py
--rw-r--r--   0 root         (0) root         (0)     5365 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/autograd/cholmod_sparse_autograd.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/autograd/common.py
--rw-r--r--   0 root         (0) root         (0)     7572 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py
--rw-r--r--   0 root         (0) root         (0)     2691 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/dense_linearization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.873990 theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/
--rw-r--r--   0 root         (0) root         (0)      520 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5161 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/baspacho_sparse_solver.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/cholmod_sparse_solver.py
--rw-r--r--   0 root         (0) root         (0)     5681 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/dense_solver.py
--rw-r--r--   0 root         (0) root         (0)     2630 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/linear_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     1107 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/linear_solver.py
--rw-r--r--   0 root         (0) root         (0)     6892 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/lu_cuda_sparse_solver.py
--rw-r--r--   0 root         (0) root         (0)     1221 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/utils.py
--rw-r--r--   0 root         (0) root         (0)     1346 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/linear_system.py
--rw-r--r--   0 root         (0) root         (0)     2437 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/linearization.py
--rw-r--r--   0 root         (0) root         (0)     6184 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/manifold_gaussian.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.873990 theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/
--rw-r--r--   0 root         (0) root         (0)      584 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8241 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/dcem.py
--rw-r--r--   0 root         (0) root         (0)     4354 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/dogleg.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/gauss_newton.py
--rw-r--r--   0 root         (0) root         (0)     7009 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/levenberg_marquardt.py
--rw-r--r--   0 root         (0) root         (0)    16237 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/nonlinear_least_squares.py
--rw-r--r--   0 root         (0) root         (0)    10762 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/nonlinear_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     5696 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/trust_region.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     8226 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/sparse_linearization.py
--rw-r--r--   0 root         (0) root         (0)     2068 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/optimizer/variable_ordering.py
--rw-r--r--   0 root         (0) root         (0)    12958 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/theseus_layer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.877990 theseus-ai-nightly-2023.4.11/theseus/third_party/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/third_party/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28031 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/third_party/easyaug.py
--rwxr-xr-x   0 root         (0) root         (0)     6703 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/third_party/lml.py
--rw-r--r--   0 root         (0) root         (0)     2040 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/third_party/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.877990 theseus-ai-nightly-2023.4.11/theseus/utils/
--rw-r--r--   0 root         (0) root         (0)      499 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.877990 theseus-ai-nightly-2023.4.11/theseus/utils/examples/
--rw-r--r--   0 root         (0) root         (0)     1526 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/utils/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.877990 theseus-ai-nightly-2023.4.11/theseus/utils/examples/bundle_adjustment/
--rw-r--r--   0 root         (0) root         (0)      244 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/utils/examples/bundle_adjustment/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12392 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/utils/examples/bundle_adjustment/data.py
--rw-r--r--   0 root         (0) root         (0)     2220 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/utils/examples/bundle_adjustment/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.877990 theseus-ai-nightly-2023.4.11/theseus/utils/examples/motion_planning/
--rw-r--r--   0 root         (0) root         (0)      435 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/utils/examples/motion_planning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9168 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/utils/examples/motion_planning/misc.py
--rw-r--r--   0 root         (0) root         (0)     9771 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/utils/examples/motion_planning/models.py
--rw-r--r--   0 root         (0) root         (0)    19745 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/utils/examples/motion_planning/motion_planner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.877990 theseus-ai-nightly-2023.4.11/theseus/utils/examples/pose_graph/
--rw-r--r--   0 root         (0) root         (0)      308 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/utils/examples/pose_graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16407 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/utils/examples/pose_graph/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.881990 theseus-ai-nightly-2023.4.11/theseus/utils/examples/tactile_pose_estimation/
--rw-r--r--   0 root         (0) root         (0)      510 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/utils/examples/tactile_pose_estimation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10221 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/utils/examples/tactile_pose_estimation/misc.py
--rw-r--r--   0 root         (0) root         (0)    10050 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/utils/examples/tactile_pose_estimation/models.py
--rw-r--r--   0 root         (0) root         (0)     9304 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py
--rw-r--r--   0 root         (0) root         (0)    12465 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/utils/examples/tactile_pose_estimation/trainer.py
--rw-r--r--   0 root         (0) root         (0)     8649 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.11/theseus/utils/sparse_matrix_utils.py
--rw-r--r--   0 root         (0) root         (0)     8089 2023-04-11 23:04:56.000000 theseus-ai-nightly-2023.4.11/theseus/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 23:05:02.881990 theseus-ai-nightly-2023.4.11/theseus_ai_nightly.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11642 2023-04-11 23:05:02.000000 theseus-ai-nightly-2023.4.11/theseus_ai_nightly.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5682 2023-04-11 23:05:02.000000 theseus-ai-nightly-2023.4.11/theseus_ai_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 23:05:02.000000 theseus-ai-nightly-2023.4.11/theseus_ai_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      406 2023-04-11 23:05:02.000000 theseus-ai-nightly-2023.4.11/theseus_ai_nightly.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-11 23:05:02.000000 theseus-ai-nightly-2023.4.11/theseus_ai_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.792434 theseus-ai-nightly-2023.4.12/
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       91 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11642 2023-04-12 22:35:58.792434 theseus-ai-nightly-2023.4.12/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11035 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.756432 theseus-ai-nightly-2023.4.12/examples/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/examples/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7193 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/examples/backward_modes.py
+-rw-r--r--   0 root         (0) root         (0)     8158 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/examples/bundle_adjustment.py
+-rw-r--r--   0 root         (0) root         (0)    19017 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/examples/homography_estimation.py
+-rw-r--r--   0 root         (0) root         (0)     9181 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/examples/motion_planning_2d.py
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/examples/se2_inverse.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/examples/se2_planning.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/examples/simple_example.py
+-rw-r--r--   0 root         (0) root         (0)    12290 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/examples/state_estimation_2d.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/examples/tactile_pose_estimation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.756432 theseus-ai-nightly-2023.4.12/requirements/
+-rw-r--r--   0 root         (0) root         (0)      192 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/requirements/dev.txt
+-rw-r--r--   0 root         (0) root         (0)      174 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      176 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/requirements/main.txt
+-rw-r--r--   0 root         (0) root         (0)      430 2023-04-12 22:35:58.792434 theseus-ai-nightly-2023.4.12/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6284 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.760433 theseus-ai-nightly-2023.4.12/tests/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.760433 theseus-ai-nightly-2023.4.12/tests/core/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7070 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/common.py
+-rw-r--r--   0 root         (0) root         (0)    13514 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_cost_function.py
+-rw-r--r--   0 root         (0) root         (0)     4442 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_cost_weight.py
+-rw-r--r--   0 root         (0) root         (0)     2270 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_manifold.py
+-rw-r--r--   0 root         (0) root         (0)    19419 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_objective.py
+-rw-r--r--   0 root         (0) root         (0)     5416 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_robust_cost.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_theseus_function.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_variable.py
+-rw-r--r--   0 root         (0) root         (0)    14670 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_vectorizer.py
+-rw-r--r--   0 root         (0) root         (0)      857 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.764433 theseus-ai-nightly-2023.4.12/tests/extlib/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/extlib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4777 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/extlib/test_baspacho.py
+-rw-r--r--   0 root         (0) root         (0)     3106 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/extlib/test_baspacho_simple.py
+-rw-r--r--   0 root         (0) root         (0)     3702 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/extlib/test_cusolver_lu_solver.py
+-rw-r--r--   0 root         (0) root         (0)     4409 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/extlib/test_mat_mult.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.764433 theseus-ai-nightly-2023.4.12/tests/geometry/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19548 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/common.py
+-rw-r--r--   0 root         (0) root         (0)      792 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/point_types_mypy_check.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/test_point_types.py
+-rw-r--r--   0 root         (0) root         (0)     8862 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/test_se2.py
+-rw-r--r--   0 root         (0) root         (0)    12861 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/test_se3.py
+-rw-r--r--   0 root         (0) root         (0)     6566 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/test_so2.py
+-rw-r--r--   0 root         (0) root         (0)    10391 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/test_so3.py
+-rw-r--r--   0 root         (0) root         (0)     7443 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/test_vector.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/test_dlm_perturbation.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/tests/test_pgo_benchmark.py
+-rw-r--r--   0 root         (0) root         (0)    21069 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/tests/test_theseus_layer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.764433 theseus-ai-nightly-2023.4.12/theseus/
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.768433 theseus-ai-nightly-2023.4.12/theseus/core/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15935 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/cost_function.py
+-rw-r--r--   0 root         (0) root         (0)     4984 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/cost_weight.py
+-rw-r--r--   0 root         (0) root         (0)    30933 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/core/objective.py
+-rw-r--r--   0 root         (0) root         (0)     6131 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/robust_cost_function.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/robust_loss.py
+-rw-r--r--   0 root         (0) root         (0)     6417 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/theseus_function.py
+-rw-r--r--   0 root         (0) root         (0)     4800 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/variable.py
+-rw-r--r--   0 root         (0) root         (0)    20067 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.768433 theseus-ai-nightly-2023.4.12/theseus/embodied/
+-rw-r--r--   0 root         (0) root         (0)      581 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.768433 theseus-ai-nightly-2023.4.12/theseus/embodied/collision/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/collision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3616 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/collision/collision.py
+-rw-r--r--   0 root         (0) root         (0)     4906 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/collision/eff_obj_contact.py
+-rw-r--r--   0 root         (0) root         (0)     9043 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/collision/signed_distance_field.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.768433 theseus-ai-nightly-2023.4.12/theseus/embodied/kinematics/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/kinematics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3894 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/kinematics/kinematics_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.768433 theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/between.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/moving_frame_between.py
+-rw-r--r--   0 root         (0) root         (0)     4090 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/reprojection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.772433 theseus-ai-nightly-2023.4.12/theseus/embodied/misc/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/misc/local_cost_fn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.772433 theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7715 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/double_integrator.py
+-rw-r--r--   0 root         (0) root         (0)     6957 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/misc.py
+-rw-r--r--   0 root         (0) root         (0)    11526 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/quasi_static_pushing_planar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.772433 theseus-ai-nightly-2023.4.12/theseus/extlib/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14114 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/baspacho_solver.cpp
+-rw-r--r--   0 root         (0) root         (0)     3751 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/baspacho_solver.h
+-rw-r--r--   0 root         (0) root         (0)    12381 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/baspacho_solver_cuda.cu
+-rw-r--r--   0 root         (0) root         (0)    16013 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/cusolver_lu_solver.cpp
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/cusolver_sp_defs.cpp
+-rw-r--r--   0 root         (0) root         (0)      744 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/cusolver_sp_defs.h
+-rw-r--r--   0 root         (0) root         (0)    14555 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/mat_mult.cu
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/utils.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.776433 theseus-ai-nightly-2023.4.12/theseus/geometry/
+-rw-r--r--   0 root         (0) root         (0)      911 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/lie_group.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/lie_group_check.py
+-rw-r--r--   0 root         (0) root         (0)     5689 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/manifold.py
+-rw-r--r--   0 root         (0) root         (0)     7322 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/point_types.py
+-rw-r--r--   0 root         (0) root         (0)    16533 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/se2.py
+-rw-r--r--   0 root         (0) root         (0)    29506 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/se3.py
+-rw-r--r--   0 root         (0) root         (0)    11359 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/so2.py
+-rw-r--r--   0 root         (0) root         (0)    25233 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/so3.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9405 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.776433 theseus-ai-nightly-2023.4.12/theseus/labs/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/labs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.776433 theseus-ai-nightly-2023.4.12/theseus/labs/lie/
+-rw-r--r--   0 root         (0) root         (0)      493 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.780433 theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7221 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/lie_group.py
+-rw-r--r--   0 root         (0) root         (0)    34776 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/se3_impl.py
+-rw-r--r--   0 root         (0) root         (0)    30196 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/so3_impl.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/utils.py
+-rw-r--r--   0 root         (0) root         (0)    17619 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/lie_tensor.py
+-rw-r--r--   0 root         (0) root         (0)     2661 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.780433 theseus-ai-nightly-2023.4.12/theseus/optimizer/
+-rw-r--r--   0 root         (0) root         (0)      505 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.780433 theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/
+-rw-r--r--   0 root         (0) root         (0)      454 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5948 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/baspacho_sparse_autograd.py
+-rw-r--r--   0 root         (0) root         (0)     5365 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/cholmod_sparse_autograd.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/common.py
+-rw-r--r--   0 root         (0) root         (0)     7572 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/dense_linearization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.784433 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5161 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/baspacho_sparse_solver.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/cholmod_sparse_solver.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/dense_solver.py
+-rw-r--r--   0 root         (0) root         (0)     2630 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/linear_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/linear_solver.py
+-rw-r--r--   0 root         (0) root         (0)     6892 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/lu_cuda_sparse_solver.py
+-rw-r--r--   0 root         (0) root         (0)     1221 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear_system.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linearization.py
+-rw-r--r--   0 root         (0) root         (0)     6184 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/manifold_gaussian.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.784433 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8241 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/dcem.py
+-rw-r--r--   0 root         (0) root         (0)     4354 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/dogleg.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/gauss_newton.py
+-rw-r--r--   0 root         (0) root         (0)     7009 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/levenberg_marquardt.py
+-rw-r--r--   0 root         (0) root         (0)    16237 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/nonlinear_least_squares.py
+-rw-r--r--   0 root         (0) root         (0)    10762 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/nonlinear_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     5696 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/trust_region.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     8226 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/sparse_linearization.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/variable_ordering.py
+-rw-r--r--   0 root         (0) root         (0)    12958 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/theseus_layer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.784433 theseus-ai-nightly-2023.4.12/theseus/third_party/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/third_party/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28031 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/third_party/easyaug.py
+-rwxr-xr-x   0 root         (0) root         (0)     6703 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/third_party/lml.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/third_party/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.788433 theseus-ai-nightly-2023.4.12/theseus/utils/
+-rw-r--r--   0 root         (0) root         (0)      499 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.788433 theseus-ai-nightly-2023.4.12/theseus/utils/examples/
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.788433 theseus-ai-nightly-2023.4.12/theseus/utils/examples/bundle_adjustment/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/bundle_adjustment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12392 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/bundle_adjustment/data.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/bundle_adjustment/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.788433 theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/
+-rw-r--r--   0 root         (0) root         (0)      435 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9168 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/misc.py
+-rw-r--r--   0 root         (0) root         (0)     9771 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/models.py
+-rw-r--r--   0 root         (0) root         (0)    19745 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/motion_planner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.788433 theseus-ai-nightly-2023.4.12/theseus/utils/examples/pose_graph/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/pose_graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16407 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/pose_graph/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.788433 theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/
+-rw-r--r--   0 root         (0) root         (0)      510 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10221 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/misc.py
+-rw-r--r--   0 root         (0) root         (0)    10050 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/models.py
+-rw-r--r--   0 root         (0) root         (0)     9304 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py
+-rw-r--r--   0 root         (0) root         (0)    12465 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/trainer.py
+-rw-r--r--   0 root         (0) root         (0)     8649 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/sparse_matrix_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.792434 theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11642 2023-04-12 22:35:58.000000 theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5682 2023-04-12 22:35:58.000000 theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 22:35:58.000000 theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      406 2023-04-12 22:35:58.000000 theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 22:35:58.000000 theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/top_level.txt
```

### Comparing `theseus-ai-nightly-2023.4.11/LICENSE` & `theseus-ai-nightly-2023.4.12/LICENSE`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/PKG-INFO` & `theseus-ai-nightly-2023.4.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theseus-ai-nightly
-Version: 2023.4.11
+Version: 2023.4.12
 Summary: A library for differentiable nonlinear optimization.
 Home-page: https://github.com/facebookresearch/theseus
 Author: Meta Research
 Keywords: differentiable optimization,nonlinear least squares,factor graphs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: theseus-ai-nightly Version: 2023.4.11 Summary: A
+Metadata-Version: 2.1 Name: theseus-ai-nightly Version: 2023.4.12 Summary: A
 library for differentiable nonlinear optimization. Home-page: https://
 github.com/facebookresearch/theseus Author: Meta Research Keywords:
 differentiable optimization,nonlinear least squares,factor graphs Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
```

### Comparing `theseus-ai-nightly-2023.4.11/README.md` & `theseus-ai-nightly-2023.4.12/README.md`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/examples/backward_modes.py` & `theseus-ai-nightly-2023.4.12/examples/backward_modes.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/examples/bundle_adjustment.py` & `theseus-ai-nightly-2023.4.12/examples/bundle_adjustment.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/examples/homography_estimation.py` & `theseus-ai-nightly-2023.4.12/examples/homography_estimation.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/examples/motion_planning_2d.py` & `theseus-ai-nightly-2023.4.12/examples/motion_planning_2d.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/examples/se2_inverse.py` & `theseus-ai-nightly-2023.4.12/examples/se2_inverse.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/examples/se2_planning.py` & `theseus-ai-nightly-2023.4.12/examples/se2_planning.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/examples/simple_example.py` & `theseus-ai-nightly-2023.4.12/examples/simple_example.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/examples/state_estimation_2d.py` & `theseus-ai-nightly-2023.4.12/examples/state_estimation_2d.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/examples/tactile_pose_estimation.py` & `theseus-ai-nightly-2023.4.12/examples/tactile_pose_estimation.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/setup.py` & `theseus-ai-nightly-2023.4.12/setup.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/core/common.py` & `theseus-ai-nightly-2023.4.12/tests/core/common.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/core/test_cost_function.py` & `theseus-ai-nightly-2023.4.12/tests/core/test_cost_function.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/core/test_cost_weight.py` & `theseus-ai-nightly-2023.4.12/tests/core/test_cost_weight.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/core/test_manifold.py` & `theseus-ai-nightly-2023.4.12/tests/core/test_manifold.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/core/test_objective.py` & `theseus-ai-nightly-2023.4.12/tests/core/test_objective.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/core/test_robust_cost.py` & `theseus-ai-nightly-2023.4.12/tests/core/test_robust_cost.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/core/test_theseus_function.py` & `theseus-ai-nightly-2023.4.12/tests/core/test_theseus_function.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/core/test_variable.py` & `theseus-ai-nightly-2023.4.12/tests/core/test_variable.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/core/test_vectorizer.py` & `theseus-ai-nightly-2023.4.12/tests/core/test_vectorizer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/decorators.py` & `theseus-ai-nightly-2023.4.12/tests/decorators.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/extlib/test_baspacho.py` & `theseus-ai-nightly-2023.4.12/tests/extlib/test_baspacho.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/extlib/test_baspacho_simple.py` & `theseus-ai-nightly-2023.4.12/tests/extlib/test_baspacho_simple.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/extlib/test_cusolver_lu_solver.py` & `theseus-ai-nightly-2023.4.12/tests/extlib/test_cusolver_lu_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/extlib/test_mat_mult.py` & `theseus-ai-nightly-2023.4.12/tests/extlib/test_mat_mult.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/geometry/common.py` & `theseus-ai-nightly-2023.4.12/tests/geometry/common.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/geometry/point_types_mypy_check.py` & `theseus-ai-nightly-2023.4.12/tests/geometry/point_types_mypy_check.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/geometry/test_point_types.py` & `theseus-ai-nightly-2023.4.12/tests/geometry/test_point_types.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/geometry/test_se2.py` & `theseus-ai-nightly-2023.4.12/tests/geometry/test_se2.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/geometry/test_se3.py` & `theseus-ai-nightly-2023.4.12/tests/geometry/test_se3.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/geometry/test_so2.py` & `theseus-ai-nightly-2023.4.12/tests/geometry/test_so2.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/geometry/test_so3.py` & `theseus-ai-nightly-2023.4.12/tests/geometry/test_so3.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/geometry/test_vector.py` & `theseus-ai-nightly-2023.4.12/tests/geometry/test_vector.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/test_dlm_perturbation.py` & `theseus-ai-nightly-2023.4.12/tests/test_dlm_perturbation.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/test_pgo_benchmark.py` & `theseus-ai-nightly-2023.4.12/tests/test_pgo_benchmark.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/tests/test_theseus_layer.py` & `theseus-ai-nightly-2023.4.12/tests/test_theseus_layer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/__init__.py` & `theseus-ai-nightly-2023.4.12/theseus/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/constants.py` & `theseus-ai-nightly-2023.4.12/theseus/constants.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/core/__init__.py` & `theseus-ai-nightly-2023.4.12/theseus/core/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/core/cost_function.py` & `theseus-ai-nightly-2023.4.12/theseus/core/cost_function.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/core/cost_weight.py` & `theseus-ai-nightly-2023.4.12/theseus/core/cost_weight.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/core/objective.py` & `theseus-ai-nightly-2023.4.12/theseus/core/objective.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/core/robust_cost_function.py` & `theseus-ai-nightly-2023.4.12/theseus/core/robust_cost_function.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/core/robust_loss.py` & `theseus-ai-nightly-2023.4.12/theseus/core/robust_loss.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/core/theseus_function.py` & `theseus-ai-nightly-2023.4.12/theseus/core/theseus_function.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/core/variable.py` & `theseus-ai-nightly-2023.4.12/theseus/core/variable.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/core/vectorizer.py` & `theseus-ai-nightly-2023.4.12/theseus/core/vectorizer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/embodied/__init__.py` & `theseus-ai-nightly-2023.4.12/theseus/embodied/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/embodied/collision/collision.py` & `theseus-ai-nightly-2023.4.12/theseus/embodied/collision/collision.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/embodied/collision/eff_obj_contact.py` & `theseus-ai-nightly-2023.4.12/theseus/embodied/collision/eff_obj_contact.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/embodied/collision/signed_distance_field.py` & `theseus-ai-nightly-2023.4.12/theseus/embodied/collision/signed_distance_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,39 +18,45 @@
     # sdf_data shape is: batch_size x field_height x field_width
     def __init__(
         self,
         origin: Union[Point2, torch.Tensor],
         cell_size: Union[float, torch.Tensor, Variable],
         sdf_data: Optional[Union[torch.Tensor, Variable]] = None,
         occupancy_map: Optional[Union[torch.Tensor, Variable]] = None,
+        occupancy_threshold: float = 0.75,
+        sdf_boundary_value: float = 0.0,
     ):
         if occupancy_map is not None:
             if sdf_data is not None:
                 raise ValueError(
                     "Only one of sdf_data and occupancy_map should be provided."
                 )
             sdf_data = self._compute_sdf_data_from_map(
-                occupancy_map, SignedDistanceField2D.convert_cell_size(cell_size).tensor
+                occupancy_map,
+                SignedDistanceField2D.convert_cell_size(cell_size).tensor,
+                threshold=occupancy_threshold,
             )
         else:
             if sdf_data is None:
                 raise ValueError(
                     "Either sdf_data or argument occupancy_map should be provided."
                 )
         self.origin: Point2
         self.cell_size: Variable
         self.sdf_data: Variable
         self.update_data(origin, sdf_data, cell_size)
         self._num_rows = sdf_data.shape[1]
         self._num_cols = sdf_data.shape[2]
+        self.sdf_boundary_value = sdf_boundary_value
 
     def _compute_sdf_data_from_map(
         self,
         occupancy_map_batch: Union[Variable, torch.Tensor],
         cell_size: torch.Tensor,
+        threshold: float = 0.75,
     ) -> Variable:
         if isinstance(occupancy_map_batch, Variable):
             occupancy_map_batch = occupancy_map_batch.tensor
         if cell_size.shape[0] != occupancy_map_batch.shape[0]:
             cell_size = cell_size.expand(occupancy_map_batch.shape[0], 1)
 
         # Code from https://github.com/gtrll/gpmp2/
@@ -61,15 +67,15 @@
             )
         num_maps = occupancy_map_batch.shape[0]
         all_sdf_data = []
 
         for i in range(num_maps):
             occupancy_map = occupancy_map_batch[i]
 
-            cur_map = occupancy_map > 0.75
+            cur_map = occupancy_map > threshold
             cur_map = cur_map.int()
 
             if torch.max(cur_map) == 0:
                 map_x, map_y = occupancy_map.size(0), occupancy_map.size(1)
                 max_map_size = 2 * cell_size[i].item() * max(map_x, map_y)
                 sdf_data = (
                     torch.ones(occupancy_map.shape, dtype=occupancy_map.dtype)
@@ -208,15 +214,15 @@
         lcdiff = cols - lc
         dist = (
             hrdiff * hcdiff * gather_sdf(lri, lci)
             + lrdiff * hcdiff * gather_sdf(hri, lci)
             + hrdiff * lcdiff * gather_sdf(lri, hci)
             + lrdiff * lcdiff * gather_sdf(hri, hci)
         )
-        dist[out_of_bounds_idx] = 0
+        dist[out_of_bounds_idx] = self.sdf_boundary_value
 
         # Compute the jacobians
 
         cell_size = (
             self.cell_size.tensor
             if self.cell_size.ndim == 2
             else self.cell_size.tensor.unsqueeze(-1)
```

### Comparing `theseus-ai-nightly-2023.4.11/theseus/embodied/kinematics/kinematics_model.py` & `theseus-ai-nightly-2023.4.12/theseus/embodied/kinematics/kinematics_model.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/embodied/measurements/between.py` & `theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/between.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/embodied/measurements/moving_frame_between.py` & `theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/moving_frame_between.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/embodied/measurements/reprojection.py` & `theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/reprojection.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/embodied/misc/local_cost_fn.py` & `theseus-ai-nightly-2023.4.12/theseus/embodied/misc/local_cost_fn.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/embodied/motionmodel/double_integrator.py` & `theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/double_integrator.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/embodied/motionmodel/misc.py` & `theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/misc.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/embodied/motionmodel/quasi_static_pushing_planar.py` & `theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/quasi_static_pushing_planar.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/extlib/baspacho_solver.cpp` & `theseus-ai-nightly-2023.4.12/theseus/extlib/baspacho_solver.cpp`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/extlib/baspacho_solver.h` & `theseus-ai-nightly-2023.4.12/theseus/extlib/baspacho_solver.h`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/extlib/baspacho_solver_cuda.cu` & `theseus-ai-nightly-2023.4.12/theseus/extlib/baspacho_solver_cuda.cu`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/extlib/cusolver_lu_solver.cpp` & `theseus-ai-nightly-2023.4.12/theseus/extlib/cusolver_lu_solver.cpp`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/extlib/cusolver_sp_defs.cpp` & `theseus-ai-nightly-2023.4.12/theseus/extlib/cusolver_sp_defs.cpp`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/extlib/cusolver_sp_defs.h` & `theseus-ai-nightly-2023.4.12/theseus/extlib/cusolver_sp_defs.h`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/extlib/mat_mult.cu` & `theseus-ai-nightly-2023.4.12/theseus/extlib/mat_mult.cu`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/extlib/utils.h` & `theseus-ai-nightly-2023.4.12/theseus/extlib/utils.h`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/geometry/__init__.py` & `theseus-ai-nightly-2023.4.12/theseus/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/geometry/lie_group.py` & `theseus-ai-nightly-2023.4.12/theseus/geometry/lie_group.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/geometry/lie_group_check.py` & `theseus-ai-nightly-2023.4.12/theseus/geometry/lie_group_check.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/geometry/manifold.py` & `theseus-ai-nightly-2023.4.12/theseus/geometry/manifold.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/geometry/point_types.py` & `theseus-ai-nightly-2023.4.12/theseus/geometry/point_types.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/geometry/se2.py` & `theseus-ai-nightly-2023.4.12/theseus/geometry/se2.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/geometry/se3.py` & `theseus-ai-nightly-2023.4.12/theseus/geometry/se3.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/geometry/so2.py` & `theseus-ai-nightly-2023.4.12/theseus/geometry/so2.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/geometry/so3.py` & `theseus-ai-nightly-2023.4.12/theseus/geometry/so3.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/geometry/utils.py` & `theseus-ai-nightly-2023.4.12/theseus/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/geometry/vector.py` & `theseus-ai-nightly-2023.4.12/theseus/geometry/vector.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/labs/lie/functional/constants.py` & `theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/constants.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/labs/lie/functional/lie_group.py` & `theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/lie_group.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/labs/lie/functional/se3_impl.py` & `theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/se3_impl.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/labs/lie/functional/so3_impl.py` & `theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/so3_impl.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/labs/lie/functional/utils.py` & `theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/labs/lie/lie_tensor.py` & `theseus-ai-nightly-2023.4.12/theseus/labs/lie/lie_tensor.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/labs/lie/types.py` & `theseus-ai-nightly-2023.4.12/theseus/labs/lie/types.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/autograd/baspacho_sparse_autograd.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/baspacho_sparse_autograd.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/autograd/cholmod_sparse_autograd.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/cholmod_sparse_autograd.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/autograd/common.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/common.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/dense_linearization.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/dense_linearization.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/__init__.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/baspacho_sparse_solver.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/baspacho_sparse_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/cholmod_sparse_solver.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/cholmod_sparse_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/dense_solver.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/dense_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/linear_optimizer.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/linear_optimizer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/linear_solver.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/linear_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/lu_cuda_sparse_solver.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/lu_cuda_sparse_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/linear/utils.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/linear_system.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear_system.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/linearization.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/linearization.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/manifold_gaussian.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/manifold_gaussian.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/__init__.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/dcem.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/dcem.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/dogleg.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/dogleg.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/gauss_newton.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/gauss_newton.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/levenberg_marquardt.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/levenberg_marquardt.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/nonlinear_least_squares.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/nonlinear_least_squares.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/nonlinear_optimizer.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/nonlinear_optimizer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/nonlinear/trust_region.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/trust_region.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/optimizer.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/sparse_linearization.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/sparse_linearization.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/optimizer/variable_ordering.py` & `theseus-ai-nightly-2023.4.12/theseus/optimizer/variable_ordering.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/theseus_layer.py` & `theseus-ai-nightly-2023.4.12/theseus/theseus_layer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/third_party/easyaug.py` & `theseus-ai-nightly-2023.4.12/theseus/third_party/easyaug.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/third_party/lml.py` & `theseus-ai-nightly-2023.4.12/theseus/third_party/lml.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/third_party/utils.py` & `theseus-ai-nightly-2023.4.12/theseus/third_party/utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/utils/examples/__init__.py` & `theseus-ai-nightly-2023.4.12/theseus/utils/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/utils/examples/bundle_adjustment/data.py` & `theseus-ai-nightly-2023.4.12/theseus/utils/examples/bundle_adjustment/data.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/utils/examples/bundle_adjustment/util.py` & `theseus-ai-nightly-2023.4.12/theseus/utils/examples/bundle_adjustment/util.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/utils/examples/motion_planning/misc.py` & `theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/misc.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/utils/examples/motion_planning/models.py` & `theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/models.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/utils/examples/motion_planning/motion_planner.py` & `theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/motion_planner.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/utils/examples/pose_graph/dataset.py` & `theseus-ai-nightly-2023.4.12/theseus/utils/examples/pose_graph/dataset.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/utils/examples/tactile_pose_estimation/misc.py` & `theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/misc.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/utils/examples/tactile_pose_estimation/models.py` & `theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/models.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py` & `theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/utils/examples/tactile_pose_estimation/trainer.py` & `theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/trainer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/utils/sparse_matrix_utils.py` & `theseus-ai-nightly-2023.4.12/theseus/utils/sparse_matrix_utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus/utils/utils.py` & `theseus-ai-nightly-2023.4.12/theseus/utils/utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.11/theseus_ai_nightly.egg-info/PKG-INFO` & `theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theseus-ai-nightly
-Version: 2023.4.11
+Version: 2023.4.12
 Summary: A library for differentiable nonlinear optimization.
 Home-page: https://github.com/facebookresearch/theseus
 Author: Meta Research
 Keywords: differentiable optimization,nonlinear least squares,factor graphs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: theseus-ai-nightly Version: 2023.4.11 Summary: A
+Metadata-Version: 2.1 Name: theseus-ai-nightly Version: 2023.4.12 Summary: A
 library for differentiable nonlinear optimization. Home-page: https://
 github.com/facebookresearch/theseus Author: Meta Research Keywords:
 differentiable optimization,nonlinear least squares,factor graphs Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
```

### Comparing `theseus-ai-nightly-2023.4.11/theseus_ai_nightly.egg-info/SOURCES.txt` & `theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

