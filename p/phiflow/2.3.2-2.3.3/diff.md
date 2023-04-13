# Comparing `tmp/phiflow-2.3.2.tar.gz` & `tmp/phiflow-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phiflow-2.3.2.tar", last modified: Tue Mar 28 12:17:10 2023, max compression
+gzip compressed data, was "phiflow-2.3.3.tar", last modified: Thu Apr 13 11:47:15 2023, max compression
```

## Comparing `phiflow-2.3.2.tar` & `phiflow-2.3.3.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.581549 phiflow-2.3.2/
--rw-rw-r--   0 holl      (1001) holl      (1001)     1085 2022-01-28 11:41:32.000000 phiflow-2.3.2/LICENSE.txt
--rw-rw-r--   0 holl      (1001) holl      (1001)       95 2022-08-29 12:54:06.000000 phiflow-2.3.2/MANIFEST.in
--rw-rw-r--   0 holl      (1001) holl      (1001)     2290 2023-03-28 12:17:10.581549 phiflow-2.3.2/PKG-INFO
--rw-rw-r--   0 holl      (1001) holl      (1001)     8330 2023-03-28 12:16:42.000000 phiflow-2.3.2/README.md
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.569549 phiflow-2.3.2/phi/
--rw-rw-r--   0 holl      (1001) holl      (1001)        5 2023-03-28 12:16:47.000000 phiflow-2.3.2/phi/VERSION
--rw-rw-r--   0 holl      (1001) holl      (1001)     1944 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     8988 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/_troubleshoot.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.569549 phiflow-2.3.2/phi/field/
--rw-rw-r--   0 holl      (1001) holl      (1001)     2349 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/field/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     2486 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/field/_angular_velocity.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3553 2023-03-28 11:02:46.000000 phiflow-2.3.2/phi/field/_embed.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    17864 2023-03-28 11:02:46.000000 phiflow-2.3.2/phi/field/_field.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     5093 2023-03-28 11:02:46.000000 phiflow-2.3.2/phi/field/_field_io.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    40385 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/field/_field_math.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    33090 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/field/_grid.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     1554 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/field/_mask.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     2837 2023-03-28 11:02:46.000000 phiflow-2.3.2/phi/field/_noise.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    12374 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/field/_point_cloud.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    21161 2023-03-28 12:16:47.000000 phiflow-2.3.2/phi/field/_scene.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     1549 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/flow.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.569549 phiflow-2.3.2/phi/geom/
--rw-rw-r--   0 holl      (1001) holl      (1001)      538 2023-03-28 11:02:46.000000 phiflow-2.3.2/phi/geom/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    21213 2023-03-28 11:02:46.000000 phiflow-2.3.2/phi/geom/_box.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    19879 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/geom/_geom.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     4410 2023-03-28 11:02:46.000000 phiflow-2.3.2/phi/geom/_sphere.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3929 2023-03-28 11:02:46.000000 phiflow-2.3.2/phi/geom/_stack.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     7884 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/geom/_transform.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3458 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/geom/_union.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.569549 phiflow-2.3.2/phi/jax/
--rw-rw-r--   0 holl      (1001) holl      (1001)      463 2022-08-02 08:31:06.000000 phiflow-2.3.2/phi/jax/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    20030 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/jax/_jax_backend.py
--rw-rw-r--   0 holl      (1001) holl      (1001)      907 2022-08-29 12:54:06.000000 phiflow-2.3.2/phi/jax/flow.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.569549 phiflow-2.3.2/phi/jax/stax/
--rw-rw-r--   0 holl      (1001) holl      (1001)        0 2022-08-29 12:54:06.000000 phiflow-2.3.2/phi/jax/stax/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)      795 2023-03-13 12:43:08.000000 phiflow-2.3.2/phi/jax/stax/flow.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    46153 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/jax/stax/nets.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.573549 phiflow-2.3.2/phi/math/
--rw-rw-r--   0 holl      (1001) holl      (1001)     4221 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/math/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3842 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/math/_fit.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    56741 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/math/_functional.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    35805 2023-03-28 12:16:47.000000 phiflow-2.3.2/phi/math/_magic_ops.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    32322 2023-03-13 12:43:08.000000 phiflow-2.3.2/phi/math/_nd.py
--rw-rw-r--   0 holl      (1001) holl      (1001)   109536 2023-03-28 12:16:47.000000 phiflow-2.3.2/phi/math/_ops.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    33258 2023-03-28 12:16:47.000000 phiflow-2.3.2/phi/math/_optimize.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    73037 2023-03-28 12:16:47.000000 phiflow-2.3.2/phi/math/_shape.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    37387 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/math/_sparse.py
--rw-rw-r--   0 holl      (1001) holl      (1001)   109308 2023-03-28 12:16:47.000000 phiflow-2.3.2/phi/math/_tensors.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    18437 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/math/_trace.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.573549 phiflow-2.3.2/phi/math/backend/
--rw-rw-r--   0 holl      (1001) holl      (1001)      787 2022-08-29 12:54:06.000000 phiflow-2.3.2/phi/math/backend/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    58953 2023-03-13 12:40:28.000000 phiflow-2.3.2/phi/math/backend/_backend.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     6140 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/math/backend/_dtype.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    22293 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/math/backend/_linalg.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     9054 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/math/backend/_minimize.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    21102 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/math/backend/_numpy_backend.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    22448 2022-08-02 08:31:06.000000 phiflow-2.3.2/phi/math/backend/_profile.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    59061 2023-03-28 12:16:47.000000 phiflow-2.3.2/phi/math/extrapolation.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    31605 2023-03-28 11:02:46.000000 phiflow-2.3.2/phi/math/magic.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    15528 2022-08-30 18:09:37.000000 phiflow-2.3.2/phi/net.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.573549 phiflow-2.3.2/phi/physics/
--rw-rw-r--   0 holl      (1001) holl      (1001)      480 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/physics/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    18206 2023-03-28 11:02:46.000000 phiflow-2.3.2/phi/physics/_boundaries.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     8446 2023-03-28 11:02:46.000000 phiflow-2.3.2/phi/physics/advect.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     4795 2023-03-28 11:02:46.000000 phiflow-2.3.2/phi/physics/diffuse.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    15513 2023-03-28 12:16:47.000000 phiflow-2.3.2/phi/physics/fluid.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.573549 phiflow-2.3.2/phi/tf/
--rw-rw-r--   0 holl      (1001) holl      (1001)     1224 2022-08-29 12:54:06.000000 phiflow-2.3.2/phi/tf/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     4228 2022-08-02 08:31:06.000000 phiflow-2.3.2/phi/tf/_compile_cuda.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     2085 2022-08-02 08:31:06.000000 phiflow-2.3.2/phi/tf/_profiling.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    29887 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/tf/_tf_backend.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3280 2022-08-29 12:54:06.000000 phiflow-2.3.2/phi/tf/_tf_cuda_resample.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.565549 phiflow-2.3.2/phi/tf/cuda/
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.573549 phiflow-2.3.2/phi/tf/cuda/build/
--rw-rw-r--   0 holl      (1001) holl      (1001)   888280 2022-08-08 09:28:29.000000 phiflow-2.3.2/phi/tf/cuda/build/resample.cu.o
--rw-rw-r--   0 holl      (1001) holl      (1001)     1175 2023-03-13 12:43:08.000000 phiflow-2.3.2/phi/tf/flow.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    34671 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/tf/nets.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.577549 phiflow-2.3.2/phi/torch/
--rw-rw-r--   0 holl      (1001) holl      (1001)      498 2022-08-02 08:31:06.000000 phiflow-2.3.2/phi/torch/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    55629 2023-03-22 10:07:02.000000 phiflow-2.3.2/phi/torch/_torch_backend.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     1145 2023-03-13 12:43:08.000000 phiflow-2.3.2/phi/torch/flow.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    39365 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/torch/nets.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.577549 phiflow-2.3.2/phi/vis/
--rw-rw-r--   0 holl      (1001) holl      (1001)     1089 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/vis/__init__.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.577549 phiflow-2.3.2/phi/vis/_console/
--rw-rw-r--   0 holl      (1001) holl      (1001)       36 2022-08-02 08:31:06.000000 phiflow-2.3.2/phi/vis/_console/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     6865 2022-08-02 08:31:06.000000 phiflow-2.3.2/phi/vis/_console/_console_gui.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3140 2022-08-29 12:54:06.000000 phiflow-2.3.2/phi/vis/_console/_console_plot.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     2360 2022-08-02 08:31:06.000000 phiflow-2.3.2/phi/vis/_console/_console_util.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.581549 phiflow-2.3.2/phi/vis/_dash/
--rw-rw-r--   0 holl      (1001) holl      (1001)        0 2022-08-02 08:31:06.000000 phiflow-2.3.2/phi/vis/_dash/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    21970 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/vis/_dash/_plotly_plots.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     7826 2022-08-29 12:54:06.000000 phiflow-2.3.2/phi/vis/_dash/board.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     4222 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/vis/_dash/colormaps.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     2954 2022-08-02 08:31:06.000000 phiflow-2.3.2/phi/vis/_dash/dash_app.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     7143 2022-08-29 12:54:06.000000 phiflow-2.3.2/phi/vis/_dash/dash_gui.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     2075 2022-08-02 08:31:06.000000 phiflow-2.3.2/phi/vis/_dash/info.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     1228 2022-08-02 08:31:06.000000 phiflow-2.3.2/phi/vis/_dash/log.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     5359 2022-08-29 12:54:06.000000 phiflow-2.3.2/phi/vis/_dash/model_controls.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3462 2022-08-02 08:31:06.000000 phiflow-2.3.2/phi/vis/_dash/player_controls.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     2710 2023-03-28 11:02:46.000000 phiflow-2.3.2/phi/vis/_dash/viewer.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     5890 2023-03-28 11:02:46.000000 phiflow-2.3.2/phi/vis/_dash/viewsettings.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3016 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/vis/_log.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.581549 phiflow-2.3.2/phi/vis/_matplotlib/
--rw-rw-r--   0 holl      (1001) holl      (1001)      108 2023-03-13 10:22:43.000000 phiflow-2.3.2/phi/vis/_matplotlib/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    23769 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/vis/_matplotlib/_matplotlib_plots.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     7426 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/vis/_matplotlib/_scalars.py
--rw-rw-r--   0 holl      (1001) holl      (1001)      793 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/vis/_plot_util.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     7184 2022-08-29 12:54:06.000000 phiflow-2.3.2/phi/vis/_user_namespace.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    10673 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/vis/_viewer.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    26967 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/vis/_vis.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    17042 2023-03-28 12:16:42.000000 phiflow-2.3.2/phi/vis/_vis_base.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-03-28 12:17:10.581549 phiflow-2.3.2/phiflow.egg-info/
--rw-rw-r--   0 holl      (1001) holl      (1001)     2290 2023-03-28 12:17:10.000000 phiflow-2.3.2/phiflow.egg-info/PKG-INFO
--rw-rw-r--   0 holl      (1001) holl      (1001)     2333 2023-03-28 12:17:10.000000 phiflow-2.3.2/phiflow.egg-info/SOURCES.txt
--rw-rw-r--   0 holl      (1001) holl      (1001)        1 2023-03-28 12:17:10.000000 phiflow-2.3.2/phiflow.egg-info/dependency_links.txt
--rw-rw-r--   0 holl      (1001) holl      (1001)       30 2023-03-28 12:17:10.000000 phiflow-2.3.2/phiflow.egg-info/requires.txt
--rw-rw-r--   0 holl      (1001) holl      (1001)        4 2023-03-28 12:17:10.000000 phiflow-2.3.2/phiflow.egg-info/top_level.txt
--rw-rw-r--   0 holl      (1001) holl      (1001)       79 2023-03-28 12:17:10.581549 phiflow-2.3.2/setup.cfg
--rw-rw-r--   0 holl      (1001) holl      (1001)     7119 2023-03-13 10:22:43.000000 phiflow-2.3.2/setup.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.781157 phiflow-2.3.3/
+-rw-rw-r--   0 holl      (1001) holl      (1001)     1085 2022-01-28 11:41:32.000000 phiflow-2.3.3/LICENSE.txt
+-rw-rw-r--   0 holl      (1001) holl      (1001)       95 2022-08-29 12:54:06.000000 phiflow-2.3.3/MANIFEST.in
+-rw-rw-r--   0 holl      (1001) holl      (1001)     2290 2023-04-13 11:47:15.781157 phiflow-2.3.3/PKG-INFO
+-rw-rw-r--   0 holl      (1001) holl      (1001)     8330 2023-04-13 11:46:51.000000 phiflow-2.3.3/README.md
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.769157 phiflow-2.3.3/phi/
+-rw-rw-r--   0 holl      (1001) holl      (1001)        5 2023-04-13 11:46:55.000000 phiflow-2.3.3/phi/VERSION
+-rw-rw-r--   0 holl      (1001) holl      (1001)     1944 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     8988 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/_troubleshoot.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.773157 phiflow-2.3.3/phi/field/
+-rw-rw-r--   0 holl      (1001) holl      (1001)     2349 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/field/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     2486 2023-04-11 10:15:31.000000 phiflow-2.3.3/phi/field/_angular_velocity.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     3553 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/field/_embed.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    17860 2023-04-13 11:46:55.000000 phiflow-2.3.3/phi/field/_field.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     5093 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/field/_field_io.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    40385 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/field/_field_math.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    33090 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/field/_grid.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     1554 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/field/_mask.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     2837 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/field/_noise.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    12374 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/field/_point_cloud.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    21224 2023-04-13 11:46:55.000000 phiflow-2.3.3/phi/field/_scene.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     1549 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/flow.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.773157 phiflow-2.3.3/phi/geom/
+-rw-rw-r--   0 holl      (1001) holl      (1001)      538 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/geom/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    21213 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/geom/_box.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    19879 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/geom/_geom.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     4410 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/geom/_sphere.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     3929 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/geom/_stack.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     7884 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/geom/_transform.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     3458 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/geom/_union.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.773157 phiflow-2.3.3/phi/jax/
+-rw-rw-r--   0 holl      (1001) holl      (1001)      463 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/jax/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    20030 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/jax/_jax_backend.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)      907 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/jax/flow.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.773157 phiflow-2.3.3/phi/jax/stax/
+-rw-rw-r--   0 holl      (1001) holl      (1001)        0 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/jax/stax/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)      795 2023-03-30 12:42:58.000000 phiflow-2.3.3/phi/jax/stax/flow.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    46153 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/jax/stax/nets.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.773157 phiflow-2.3.3/phi/math/
+-rw-rw-r--   0 holl      (1001) holl      (1001)     4221 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     3842 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/math/_fit.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    56756 2023-04-13 11:46:55.000000 phiflow-2.3.3/phi/math/_functional.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    35805 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/_magic_ops.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    32322 2023-03-30 12:42:58.000000 phiflow-2.3.3/phi/math/_nd.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)   109536 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/_ops.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    33258 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/_optimize.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    73037 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/_shape.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    37387 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/_sparse.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)   109308 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/_tensors.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    18437 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/_trace.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/math/backend/
+-rw-rw-r--   0 holl      (1001) holl      (1001)      787 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/math/backend/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    58953 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/backend/_backend.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     6140 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/math/backend/_dtype.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    22293 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/math/backend/_linalg.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     9054 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/math/backend/_minimize.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    21102 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/backend/_numpy_backend.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    22448 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/math/backend/_profile.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    59061 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/extrapolation.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    31605 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/magic.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    15528 2022-08-30 18:09:37.000000 phiflow-2.3.3/phi/net.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/physics/
+-rw-rw-r--   0 holl      (1001) holl      (1001)      480 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/physics/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    18206 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/physics/_boundaries.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     8446 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/physics/advect.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     4795 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/physics/diffuse.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    15513 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/physics/fluid.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/tf/
+-rw-rw-r--   0 holl      (1001) holl      (1001)     1224 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/tf/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     4228 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/tf/_compile_cuda.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     2085 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/tf/_profiling.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    29887 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/tf/_tf_backend.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     3280 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/tf/_tf_cuda_resample.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.769157 phiflow-2.3.3/phi/tf/cuda/
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/tf/cuda/build/
+-rw-rw-r--   0 holl      (1001) holl      (1001)   888280 2022-08-08 09:28:29.000000 phiflow-2.3.3/phi/tf/cuda/build/resample.cu.o
+-rw-rw-r--   0 holl      (1001) holl      (1001)     1175 2023-03-30 12:42:58.000000 phiflow-2.3.3/phi/tf/flow.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    34671 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/tf/nets.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/torch/
+-rw-rw-r--   0 holl      (1001) holl      (1001)      498 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/torch/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    55629 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/torch/_torch_backend.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     1145 2023-03-30 12:42:58.000000 phiflow-2.3.3/phi/torch/flow.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    39365 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/torch/nets.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/vis/
+-rw-rw-r--   0 holl      (1001) holl      (1001)     1089 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/__init__.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/vis/_console/
+-rw-rw-r--   0 holl      (1001) holl      (1001)       36 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_console/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     6865 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_console/_console_gui.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     3140 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/vis/_console/_console_plot.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     2360 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_console/_console_util.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/vis/_dash/
+-rw-rw-r--   0 holl      (1001) holl      (1001)        0 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_dash/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    21970 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_dash/_plotly_plots.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     7826 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/vis/_dash/board.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     4222 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_dash/colormaps.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     2954 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_dash/dash_app.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     7143 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/vis/_dash/dash_gui.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     2075 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_dash/info.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     1228 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_dash/log.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     5359 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/vis/_dash/model_controls.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     3462 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_dash/player_controls.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     2710 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/vis/_dash/viewer.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     5890 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/vis/_dash/viewsettings.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     3016 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_log.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/vis/_matplotlib/
+-rw-rw-r--   0 holl      (1001) holl      (1001)      108 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/vis/_matplotlib/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    23769 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_matplotlib/_matplotlib_plots.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     7426 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_matplotlib/_scalars.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)      793 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_plot_util.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     7184 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/vis/_user_namespace.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    10673 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_viewer.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    26967 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_vis.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    17042 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_vis_base.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.781157 phiflow-2.3.3/phiflow.egg-info/
+-rw-rw-r--   0 holl      (1001) holl      (1001)     2290 2023-04-13 11:47:15.000000 phiflow-2.3.3/phiflow.egg-info/PKG-INFO
+-rw-rw-r--   0 holl      (1001) holl      (1001)     2333 2023-04-13 11:47:15.000000 phiflow-2.3.3/phiflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 holl      (1001) holl      (1001)        1 2023-04-13 11:47:15.000000 phiflow-2.3.3/phiflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 holl      (1001) holl      (1001)       30 2023-04-13 11:47:15.000000 phiflow-2.3.3/phiflow.egg-info/requires.txt
+-rw-rw-r--   0 holl      (1001) holl      (1001)        4 2023-04-13 11:47:15.000000 phiflow-2.3.3/phiflow.egg-info/top_level.txt
+-rw-rw-r--   0 holl      (1001) holl      (1001)       79 2023-04-13 11:47:15.781157 phiflow-2.3.3/setup.cfg
+-rw-rw-r--   0 holl      (1001) holl      (1001)     7119 2023-03-13 10:22:43.000000 phiflow-2.3.3/setup.py
```

### Comparing `phiflow-2.3.2/LICENSE.txt` & `phiflow-2.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/PKG-INFO` & `phiflow-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: phiflow
-Version: 2.3.2
+Version: 2.3.3
 Summary: Differentiable PDE solving framework for machine learning
 Home-page: https://github.com/tum-pbs/PhiFlow
-Download-URL: https://github.com/tum-pbs/PhiFlow/archive/2.3.2.tar.gz
+Download-URL: https://github.com/tum-pbs/PhiFlow/archive/2.3.3.tar.gz
 Author: Philipp Holl
 Author-email: philipp.holl@tum.de
 License: MIT
 Keywords: Differentiable,Simulation,Fluid,Machine Learning,Deep Learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `phiflow-2.3.2/README.md` & `phiflow-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/__init__.py` & `phiflow-2.3.3/phi/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/_troubleshoot.py` & `phiflow-2.3.3/phi/_troubleshoot.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/field/__init__.py` & `phiflow-2.3.3/phi/field/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/field/_angular_velocity.py` & `phiflow-2.3.3/phi/field/_angular_velocity.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/field/_embed.py` & `phiflow-2.3.3/phi/field/_embed.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/field/_field.py` & `phiflow-2.3.3/phi/field/_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,17 +286,17 @@
         if isinstance(other, Field):
             other_values = reduce_sample(other, self._elements)
             values = operator(self._values, other_values)
             extrapolation_ = operator(self._extrapolation, other.extrapolation)
             return self.with_values(values).with_extrapolation(extrapolation_)
         else:
             if isinstance(other, (tuple, list)) and len(other) == self.spatial_rank:
-                other = math.tensor(other, self.points.shape['vector'])
+                other = math.wrap(other, self.points.shape['vector'])
             else:
-                other = math.tensor(other)
+                other = math.wrap(other)
             values = operator(self._values, other)
             return self.with_values(values)
 
 
 def sample(field: Field or Geometry,
            geometry: Geometry or SampledField or Tensor,
            **kwargs) -> math.Tensor:
```

### Comparing `phiflow-2.3.2/phi/field/_field_io.py` & `phiflow-2.3.3/phi/field/_field_io.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/field/_field_math.py` & `phiflow-2.3.3/phi/field/_field_math.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/field/_grid.py` & `phiflow-2.3.3/phi/field/_grid.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/field/_mask.py` & `phiflow-2.3.3/phi/field/_mask.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/field/_noise.py` & `phiflow-2.3.3/phi/field/_noise.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/field/_point_cloud.py` & `phiflow-2.3.3/phi/field/_point_cloud.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/field/_scene.py` & `phiflow-2.3.3/phi/field/_scene.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,15 @@
         self._init_properties()
         if update:
             self._properties.update(update)
         self._properties.update(kw_updates)
         for key, value in self._properties.items():
             if isinstance(value, (np.int64, np.int32)):
                 value = int(value)
-            elif isinstance(value, (np.float32, np.float64, np.float16, np.float128)):
+            elif isinstance(value, (np.float16, np.float32, np.float64, np.float16)) or (hasattr(np, 'float128') and isinstance(value, np.float128)):
                 value = float(value)
             self._properties[key] = value
         self._write_properties()
 
     def _get_properties(self, index: dict):
         result = dict(self._properties)
         tensor_names = []
```

### Comparing `phiflow-2.3.2/phi/flow.py` & `phiflow-2.3.3/phi/flow.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/geom/__init__.py` & `phiflow-2.3.3/phi/geom/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/geom/_box.py` & `phiflow-2.3.3/phi/geom/_box.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/geom/_geom.py` & `phiflow-2.3.3/phi/geom/_geom.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/geom/_sphere.py` & `phiflow-2.3.3/phi/geom/_sphere.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/geom/_stack.py` & `phiflow-2.3.3/phi/geom/_stack.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/geom/_transform.py` & `phiflow-2.3.3/phi/geom/_transform.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/geom/_union.py` & `phiflow-2.3.3/phi/geom/_union.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/jax/_jax_backend.py` & `phiflow-2.3.3/phi/jax/_jax_backend.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/jax/flow.py` & `phiflow-2.3.3/phi/jax/flow.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/jax/stax/flow.py` & `phiflow-2.3.3/phi/jax/stax/flow.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/jax/stax/nets.py` & `phiflow-2.3.3/phi/jax/stax/nets.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/__init__.py` & `phiflow-2.3.3/phi/math/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/_fit.py` & `phiflow-2.3.3/phi/math/_fit.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/_functional.py` & `phiflow-2.3.3/phi/math/_functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     def __init__(self, f: Callable, auxiliary_args: Set[str], forget_traces: bool):
         self.f = f
         self.f_params = function_parameters(f)
         self.auxiliary_args = auxiliary_args
         self.forget_traces = forget_traces
         self.traces: Dict[SignatureKey, Callable] = {}
         self.recorded_mappings: Dict[SignatureKey, SignatureKey] = {}
-        self.grad_jit = GradientFunction(f.f, f.wrt, f.get_output, f.is_f_scalar, jit=True) if isinstance(f, GradientFunction) else None
+        self.grad_jit = GradientFunction(f.f, self.f_params, f.wrt, f.get_output, f.is_f_scalar, jit=True) if isinstance(f, GradientFunction) else None
 
     def _jit_compile(self, in_key: SignatureKey):
         PHI_LOGGER.debug(f"Φ-jit: '{f_name(self.f)}' called with new key. shapes={[s.volume for s in in_key.shapes]}, args={in_key.tree}")
 
         def jit_f_native(*natives):
             PHI_LOGGER.debug(f"Φ-jit: Tracing '{f_name(self.f)}'")
             in_tensors = assemble_tensors(natives, in_key.specs)
```

### Comparing `phiflow-2.3.2/phi/math/_magic_ops.py` & `phiflow-2.3.3/phi/math/_magic_ops.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/_nd.py` & `phiflow-2.3.3/phi/math/_nd.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/_ops.py` & `phiflow-2.3.3/phi/math/_ops.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/_optimize.py` & `phiflow-2.3.3/phi/math/_optimize.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/_shape.py` & `phiflow-2.3.3/phi/math/_shape.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/_sparse.py` & `phiflow-2.3.3/phi/math/_sparse.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/_tensors.py` & `phiflow-2.3.3/phi/math/_tensors.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/_trace.py` & `phiflow-2.3.3/phi/math/_trace.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/backend/__init__.py` & `phiflow-2.3.3/phi/math/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/backend/_backend.py` & `phiflow-2.3.3/phi/math/backend/_backend.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/backend/_dtype.py` & `phiflow-2.3.3/phi/math/backend/_dtype.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/backend/_linalg.py` & `phiflow-2.3.3/phi/math/backend/_linalg.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/backend/_minimize.py` & `phiflow-2.3.3/phi/math/backend/_minimize.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/backend/_numpy_backend.py` & `phiflow-2.3.3/phi/math/backend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/backend/_profile.py` & `phiflow-2.3.3/phi/math/backend/_profile.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/extrapolation.py` & `phiflow-2.3.3/phi/math/extrapolation.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/math/magic.py` & `phiflow-2.3.3/phi/math/magic.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/net.py` & `phiflow-2.3.3/phi/net.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/physics/_boundaries.py` & `phiflow-2.3.3/phi/physics/_boundaries.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/physics/advect.py` & `phiflow-2.3.3/phi/physics/advect.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/physics/diffuse.py` & `phiflow-2.3.3/phi/physics/diffuse.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/physics/fluid.py` & `phiflow-2.3.3/phi/physics/fluid.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/tf/__init__.py` & `phiflow-2.3.3/phi/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/tf/_compile_cuda.py` & `phiflow-2.3.3/phi/tf/_compile_cuda.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/tf/_profiling.py` & `phiflow-2.3.3/phi/tf/_profiling.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/tf/_tf_backend.py` & `phiflow-2.3.3/phi/tf/_tf_backend.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/tf/_tf_cuda_resample.py` & `phiflow-2.3.3/phi/tf/_tf_cuda_resample.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/tf/cuda/build/resample.cu.o` & `phiflow-2.3.3/phi/tf/cuda/build/resample.cu.o`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/tf/flow.py` & `phiflow-2.3.3/phi/tf/flow.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/tf/nets.py` & `phiflow-2.3.3/phi/tf/nets.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/torch/_torch_backend.py` & `phiflow-2.3.3/phi/torch/_torch_backend.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/torch/flow.py` & `phiflow-2.3.3/phi/torch/flow.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/torch/nets.py` & `phiflow-2.3.3/phi/torch/nets.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/__init__.py` & `phiflow-2.3.3/phi/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_console/_console_gui.py` & `phiflow-2.3.3/phi/vis/_console/_console_gui.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_console/_console_plot.py` & `phiflow-2.3.3/phi/vis/_console/_console_plot.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_console/_console_util.py` & `phiflow-2.3.3/phi/vis/_console/_console_util.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_dash/_plotly_plots.py` & `phiflow-2.3.3/phi/vis/_dash/_plotly_plots.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_dash/board.py` & `phiflow-2.3.3/phi/vis/_dash/board.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_dash/colormaps.py` & `phiflow-2.3.3/phi/vis/_dash/colormaps.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_dash/dash_app.py` & `phiflow-2.3.3/phi/vis/_dash/dash_app.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_dash/dash_gui.py` & `phiflow-2.3.3/phi/vis/_dash/dash_gui.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_dash/info.py` & `phiflow-2.3.3/phi/vis/_dash/info.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_dash/log.py` & `phiflow-2.3.3/phi/vis/_dash/log.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_dash/model_controls.py` & `phiflow-2.3.3/phi/vis/_dash/model_controls.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_dash/player_controls.py` & `phiflow-2.3.3/phi/vis/_dash/player_controls.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_dash/viewer.py` & `phiflow-2.3.3/phi/vis/_dash/viewer.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_dash/viewsettings.py` & `phiflow-2.3.3/phi/vis/_dash/viewsettings.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_log.py` & `phiflow-2.3.3/phi/vis/_log.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_matplotlib/_matplotlib_plots.py` & `phiflow-2.3.3/phi/vis/_matplotlib/_matplotlib_plots.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_matplotlib/_scalars.py` & `phiflow-2.3.3/phi/vis/_matplotlib/_scalars.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_plot_util.py` & `phiflow-2.3.3/phi/vis/_plot_util.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_user_namespace.py` & `phiflow-2.3.3/phi/vis/_user_namespace.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_viewer.py` & `phiflow-2.3.3/phi/vis/_viewer.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_vis.py` & `phiflow-2.3.3/phi/vis/_vis.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phi/vis/_vis_base.py` & `phiflow-2.3.3/phi/vis/_vis_base.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/phiflow.egg-info/PKG-INFO` & `phiflow-2.3.3/phiflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: phiflow
-Version: 2.3.2
+Version: 2.3.3
 Summary: Differentiable PDE solving framework for machine learning
 Home-page: https://github.com/tum-pbs/PhiFlow
-Download-URL: https://github.com/tum-pbs/PhiFlow/archive/2.3.2.tar.gz
+Download-URL: https://github.com/tum-pbs/PhiFlow/archive/2.3.3.tar.gz
 Author: Philipp Holl
 Author-email: philipp.holl@tum.de
 License: MIT
 Keywords: Differentiable,Simulation,Fluid,Machine Learning,Deep Learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `phiflow-2.3.2/phiflow.egg-info/SOURCES.txt` & `phiflow-2.3.3/phiflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.2/setup.py` & `phiflow-2.3.3/setup.py`

 * *Files identical despite different names*

