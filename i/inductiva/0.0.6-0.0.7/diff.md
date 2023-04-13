# Comparing `tmp/inductiva-0.0.6.tar.gz` & `tmp/inductiva-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inductiva-0.0.6.tar", last modified: Tue Apr 11 15:58:03 2023, max compression
+gzip compressed data, was "inductiva-0.0.7.tar", last modified: Thu Apr 13 17:01:24 2023, max compression
```

## Comparing `inductiva-0.0.6.tar` & `inductiva-0.0.7.tar`

### file list

```diff
@@ -1,135 +1,140 @@
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.137819 inductiva-0.0.6/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       43 2023-03-29 15:57:40.000000 inductiva-0.0.6/MANIFEST.in
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      579 2023-04-11 15:58:03.137819 inductiva-0.0.6/PKG-INFO
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      205 2023-03-29 15:57:40.000000 inductiva-0.0.6/README.md
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.125819 inductiva-0.0.6/inductiva/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      363 2023-04-03 08:49:49.000000 inductiva-0.0.6/inductiva/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.125819 inductiva-0.0.6/inductiva/api/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      122 2023-04-03 08:49:49.000000 inductiva-0.0.6/inductiva/api/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    13457 2023-04-10 16:30:57.000000 inductiva-0.0.6/inductiva/api/methods.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.125819 inductiva-0.0.6/inductiva/client/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      805 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    60856 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/api_client.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/apis/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      214 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1421 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/path_to_api.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/apis/paths/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      243 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      112 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/admin_user.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      137 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/admin_user_username_tasks.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      114 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/task_submit.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      126 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/task_task_id_input.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      124 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/task_task_id_kill.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/task_task_id_output.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/paths/task_task_id_status.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      400 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/tag_to_api.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/apis/tags/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/tags/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      622 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/tags/admin_api.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      916 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/apis/tags/tasks_api.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    16615 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/configuration.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4590 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/exceptions.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/model/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      350 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2759 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/body_upload_task_input.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3636 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/http_validation_error.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4386 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/new_user.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4682 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/queue_status.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3628 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/task_request.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6465 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/task_status.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7930 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/model/validation_error.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/models/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      843 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/models/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/paths/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      617 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/paths/admin_user/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      311 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/admin_user/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12303 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/admin_user/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/paths/admin_user_username_tasks/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      341 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/admin_user_username_tasks/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10351 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/admin_user_username_tasks/get.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/paths/task_submit/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      313 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_submit/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12455 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_submit/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/paths/task_task_id_input/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      327 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_input/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    15178 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_input/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/paths/task_task_id_kill/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      325 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_kill/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10501 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_kill/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.129819 inductiva-0.0.6/inductiva/client/paths/task_task_id_output/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_output/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10463 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_output/get.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/client/paths/task_task_id_status/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_status/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10400 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/paths/task_task_id_status/get.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    11962 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/rest.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)   103899 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/client/schemas.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/core/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      120 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/core/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/core/cupy/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       85 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/core/cupy/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      379 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/core/cupy/linalg.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      586 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/core/math.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/core/slepc/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       64 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/core/slepc/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      491 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/core/slepc/linalg.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      333 2023-04-10 14:10:43.000000 inductiva-0.0.6/inductiva/core/test.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      102 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/exceptions.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/fluids/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      411 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2579 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/_output_post_processing.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1002 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/fluid_types.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/fluids/post_processing/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/post_processing/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     5931 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/post_processing/splishsplash.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/fluids/scenarios/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      110 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/fluids/scenarios/dam_break/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/dam_break/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2341 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/scenarios/dam_break/dam_break.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       78 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6904 2023-04-10 16:28:58.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/fluid_block.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4230 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1350 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      700 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/unit_box.obj
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      182 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8165 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1914 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     9161 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6444 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2507 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/fluids/shapes.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/fluids/simulators/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      203 2023-04-03 08:49:49.000000 inductiva-0.0.6/inductiva/fluids/simulators/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1121 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/simulators/dualsphysics.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1286 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/simulators/openfoam.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1084 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/simulators/splishsplash.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1065 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/fluids/simulators/swash.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      995 2023-04-11 15:37:20.000000 inductiva-0.0.6/inductiva/fluids/simulators/xbeach.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1760 2023-04-11 14:04:20.000000 inductiva-0.0.6/inductiva/scenarios.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.133819 inductiva-0.0.6/inductiva/simulation/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       76 2023-04-03 08:49:49.000000 inductiva-0.0.6/inductiva/simulation/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1938 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/simulation/simulator.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      142 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/types.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.137819 inductiva-0.0.6/inductiva/utils/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/utils/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8337 2023-04-03 08:49:49.000000 inductiva-0.0.6/inductiva/utils/data.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      919 2023-04-11 14:04:20.000000 inductiva-0.0.6/inductiva/utils/files.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      783 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/utils/files_test.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1720 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/utils/flags.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1672 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/utils/meta.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      272 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/utils/misc.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      750 2023-04-10 14:10:51.000000 inductiva-0.0.6/inductiva/utils/misc_test.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      509 2023-03-29 15:57:40.000000 inductiva-0.0.6/inductiva/utils/templates.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10104 2023-04-03 08:49:49.000000 inductiva-0.0.6/inductiva/utils/visualization.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-11 15:58:03.125819 inductiva-0.0.6/inductiva.egg-info/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      579 2023-04-11 15:58:03.000000 inductiva-0.0.6/inductiva.egg-info/PKG-INFO
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4014 2023-04-11 15:58:03.000000 inductiva-0.0.6/inductiva.egg-info/SOURCES.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        1 2023-04-11 15:58:03.000000 inductiva-0.0.6/inductiva.egg-info/dependency_links.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      175 2023-04-11 15:58:03.000000 inductiva-0.0.6/inductiva.egg-info/requires.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       10 2023-04-11 15:58:03.000000 inductiva-0.0.6/inductiva.egg-info/top_level.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       87 2023-04-03 08:49:49.000000 inductiva-0.0.6/pyproject.toml
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      779 2023-04-11 15:58:03.137819 inductiva-0.0.6/setup.cfg
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       56 2023-04-03 08:49:49.000000 inductiva-0.0.6/setup.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.164712 inductiva-0.0.7/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       43 2023-03-29 15:57:40.000000 inductiva-0.0.7/MANIFEST.in
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3570 2023-04-13 17:01:24.164712 inductiva-0.0.7/PKG-INFO
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3196 2023-04-12 11:44:25.000000 inductiva-0.0.7/README.md
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      387 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/api/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      122 2023-04-03 08:49:49.000000 inductiva-0.0.7/inductiva/api/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    13042 2023-04-13 14:14:35.000000 inductiva-0.0.7/inductiva/api/methods.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      805 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    60856 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/api_client.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/apis/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      214 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1421 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/path_to_api.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/apis/paths/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      243 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      112 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/admin_user.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      137 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/admin_user_username_tasks.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      114 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/task_submit.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      126 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/task_task_id_input.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      124 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/task_task_id_kill.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/task_task_id_output.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/task_task_id_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      400 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/tag_to_api.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/apis/tags/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/tags/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      622 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/tags/admin_api.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      916 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/tags/tasks_api.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    16615 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/configuration.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4590 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/exceptions.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/model/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      350 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2759 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/body_upload_task_input.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3636 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/http_validation_error.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4386 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/new_user.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4682 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/queue_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3628 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/task_request.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6465 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/task_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7930 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/validation_error.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/models/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      843 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/models/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      617 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/admin_user/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      311 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/admin_user/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12303 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/admin_user/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/admin_user_username_tasks/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      341 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/admin_user_username_tasks/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10351 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/admin_user_username_tasks/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/task_submit/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      313 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_submit/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12455 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_submit/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/task_task_id_input/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      327 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_input/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    15178 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_input/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/task_task_id_kill/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      325 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_kill/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10501 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_kill/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/task_task_id_output/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_output/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10463 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_output/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/task_task_id_status/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_status/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10400 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_status/get.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    11962 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/rest.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)   103899 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/schemas.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/core/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      120 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/core/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/core/cupy/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       85 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/core/cupy/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      379 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/core/cupy/linalg.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      586 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/core/math.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/core/slepc/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       64 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/core/slepc/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      491 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/core/slepc/linalg.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      333 2023-04-13 16:55:23.000000 inductiva-0.0.7/inductiva/core/test.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      102 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/exceptions.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/fluids/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      432 2023-04-13 16:55:27.000000 inductiva-0.0.7/inductiva/fluids/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1002 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/fluid_types.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/fluids/post_processing/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/post_processing/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     5247 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/fluids/post_processing/splishsplash.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/fluids/scenarios/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      250 2023-04-13 16:55:27.000000 inductiva-0.0.7/inductiva/fluids/scenarios/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1610 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/fluids/scenarios/_post_processing.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/fluids/scenarios/dam_break/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/scenarios/dam_break/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2678 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/fluids/scenarios/dam_break/dam_break.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       78 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7087 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/fluid_block.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4230 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1350 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      700 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/unit_box.obj
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      182 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8165 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1914 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     9161 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6444 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2507 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/shapes.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/fluids/simulators/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      203 2023-04-03 08:49:49.000000 inductiva-0.0.7/inductiva/fluids/simulators/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1121 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/fluids/simulators/dualsphysics.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1288 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/fluids/simulators/openfoam.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1084 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/fluids/simulators/splishsplash.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1065 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/fluids/simulators/swash.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      995 2023-04-11 15:37:20.000000 inductiva-0.0.7/inductiva/fluids/simulators/xbeach.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/molecules/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/molecules/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/molecules/simulators/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       71 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/molecules/simulators/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1312 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/molecules/simulators/gromacs.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1760 2023-04-11 14:04:20.000000 inductiva-0.0.7/inductiva/scenarios.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/simulation/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       76 2023-04-03 08:49:49.000000 inductiva-0.0.7/inductiva/simulation/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1938 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/simulation/simulator.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      142 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/types.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.164712 inductiva-0.0.7/inductiva/utils/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/utils/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8337 2023-04-03 08:49:49.000000 inductiva-0.0.7/inductiva/utils/data.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2167 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/utils/files.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      783 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/utils/files_test.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1720 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/utils/flags.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1672 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/utils/meta.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      272 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/utils/misc.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      750 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/utils/misc_test.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      509 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/utils/templates.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    14282 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/utils/visualization.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva.egg-info/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3570 2023-04-13 17:01:24.000000 inductiva-0.0.7/inductiva.egg-info/PKG-INFO
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4134 2023-04-13 17:01:24.000000 inductiva-0.0.7/inductiva.egg-info/SOURCES.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        1 2023-04-13 17:01:24.000000 inductiva-0.0.7/inductiva.egg-info/dependency_links.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      175 2023-04-13 17:01:24.000000 inductiva-0.0.7/inductiva.egg-info/requires.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       10 2023-04-13 17:01:24.000000 inductiva-0.0.7/inductiva.egg-info/top_level.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       87 2023-04-03 08:49:49.000000 inductiva-0.0.7/pyproject.toml
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      779 2023-04-13 17:01:24.164712 inductiva-0.0.7/setup.cfg
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       56 2023-04-03 08:49:49.000000 inductiva-0.0.7/setup.py
```

### Comparing `inductiva-0.0.6/inductiva/api/methods.py` & `inductiva-0.0.7/inductiva/api/methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,35 +116,23 @@
     logging.debug("Blocking until task is finished ...")
     return block_until_status_is(api_instance, task_id, {"success", "failed"})
 
 
 def kill_task(api_instance: TasksApi, task_id: str):
     """Kill a task that is executing remotely.
 
-    The function sends a Kill request to the API and then polls until the
-    status of the task is killed.
-    TODO: should polling be done here? Or should the API endpoint make sure
-    that the task is killed instead of the client having to wait for
-    confirmation?
+    The function sends a kill request to the API.
 
     Args:
         api_instance: Instance of TasksApi used to send necessary requests.
         task_id: ID of the task to kill.
-
-    Returns:
-        Returns info related to the task, containing two fields,
-        "id" and "status".
-    """
+   """
     logging.debug("Sending kill task request ...")
-    _ = api_instance.kill_task(path_params={"task_id": task_id},)
-
-    logging.debug("Blocking until task is killed ...")
-    out = block_until_status_is(api_instance, task_id, {"killed"})
+    api_instance.kill_task(path_params={"task_id": task_id},)
     logging.info("Task terminated.")
-    return out
 
 
 def block_until_status_is(api_instance: TasksApi,
                           task_id,
                           desired_status,
                           sleep_secs=0.5):
     """Block until the status of a task becomes the desired status.
@@ -168,21 +156,19 @@
                 )
 
             status = api_response.body["status"]
             logging.debug("Task status is %s", status)
         except ApiException as e:
             raise e
 
-        if status == prev_status:
-            continue
-
-        if status == "submitted":
-            logging.info("Waiting for resources...")
+        if status != prev_status:
+            if status == "submitted":
+                logging.info("Waiting for resources...")
 
-        prev_status = status
+            prev_status = status
 
         # If status reaches the desired status, then stop polling
         if status in desired_status:
             break
 
         time.sleep(sleep_secs)
 
@@ -389,17 +375,19 @@
         raise RuntimeError(f"Expected result to be a Path, got {type(result)}")
 
     return result
 
 
 async def follow_task(task_id: str) -> str:
     parsed_url = urlparse(inductiva.api_url)
-    url = f"ws://{parsed_url.hostname}:{parsed_url.port}/ \
-        task/{task_id}/logs/tail"
+    url = \
+        f"ws://{parsed_url.hostname}:{parsed_url.port}/" \
+        f"task/{task_id}/logs/tail"
 
+    logging.debug("Following task logs at %s", url)
     async with websockets.connect(url) as ws:
         while True:
             message = await ws.recv()
             parsed_message = json.loads(message)
 
             if parsed_message["type"] == "update":
                 status = parsed_message["content"]
```

### Comparing `inductiva-0.0.6/inductiva/client/__init__.py` & `inductiva-0.0.7/inductiva/client/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/api_client.py` & `inductiva-0.0.7/inductiva/client/api_client.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/apis/path_to_api.py` & `inductiva-0.0.7/inductiva/client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/apis/tags/admin_api.py` & `inductiva-0.0.7/inductiva/client/apis/tags/admin_api.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/apis/tags/tasks_api.py` & `inductiva-0.0.7/inductiva/client/apis/tags/tasks_api.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/configuration.py` & `inductiva-0.0.7/inductiva/client/configuration.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/exceptions.py` & `inductiva-0.0.7/inductiva/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/model/body_upload_task_input.py` & `inductiva-0.0.7/inductiva/client/model/body_upload_task_input.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/model/http_validation_error.py` & `inductiva-0.0.7/inductiva/client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/model/new_user.py` & `inductiva-0.0.7/inductiva/client/model/new_user.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/model/queue_status.py` & `inductiva-0.0.7/inductiva/client/model/queue_status.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/model/task_request.py` & `inductiva-0.0.7/inductiva/client/model/task_request.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/model/task_status.py` & `inductiva-0.0.7/inductiva/client/model/task_status.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/model/validation_error.py` & `inductiva-0.0.7/inductiva/client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/models/__init__.py` & `inductiva-0.0.7/inductiva/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/paths/__init__.py` & `inductiva-0.0.7/inductiva/client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/paths/admin_user/post.py` & `inductiva-0.0.7/inductiva/client/paths/admin_user/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/paths/admin_user_username_tasks/get.py` & `inductiva-0.0.7/inductiva/client/paths/admin_user_username_tasks/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/paths/task_submit/post.py` & `inductiva-0.0.7/inductiva/client/paths/task_submit/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/paths/task_task_id_input/post.py` & `inductiva-0.0.7/inductiva/client/paths/task_task_id_input/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/paths/task_task_id_kill/post.py` & `inductiva-0.0.7/inductiva/client/paths/task_task_id_kill/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/paths/task_task_id_output/get.py` & `inductiva-0.0.7/inductiva/client/paths/task_task_id_output/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/paths/task_task_id_status/get.py` & `inductiva-0.0.7/inductiva/client/paths/task_task_id_status/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/rest.py` & `inductiva-0.0.7/inductiva/client/rest.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/client/schemas.py` & `inductiva-0.0.7/inductiva/client/schemas.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/core/math.py` & `inductiva-0.0.7/inductiva/core/math.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/fluids/fluid_types.py` & `inductiva-0.0.7/inductiva/fluids/fluid_types.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/fluids/post_processing/splishsplash.py` & `inductiva-0.0.7/inductiva/fluids/post_processing/splishsplash.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,36 +7,15 @@
 
 import numpy as np
 from tqdm import tqdm
 import vtk
 from vtk.util.numpy_support import vtk_to_numpy as _vtk_data_to_numpy
 import xarray as xr
 
-
-def get_sorted_vtk_files(data_dir: str):
-    """Returns a list of sorted vtk files in a directory."""
-
-    if not os.path.exists(data_dir):
-        raise IOError(f"Directory '{data_dir}' does not exist.")
-
-    # Get a list of the files in the data directory.
-    files = os.scandir(data_dir)
-
-    # The files must have .vtk extension.
-    files = [file for file in files if pathlib.Path(file.path).suffix == ".vtk"]
-
-    # Sort the files to be read according to [file_key].
-    def get_alphanum_key(file):
-        file_name = pathlib.Path(file.path).stem
-        file_name_splits = file_name.split("_")
-        file_key = file_name_splits[-1]
-        return int(file_key)
-
-    files = sorted(files, key=get_alphanum_key)
-    return files
+from inductiva.utils.files import get_sorted_files
 
 
 def convert_vtk_data_dir_to_netcdf(
     data_dir: str,
     output_time_step: float,
     netcdf_data_dir: str,
 ):
@@ -44,15 +23,15 @@
 
     Args:
         data_dir: Data directory.
         output_time_step: Time step between output files, in seconds.
         netcdf_data_dir: Directory to store files in netcdf format.
     """
 
-    files = get_sorted_vtk_files(data_dir)
+    files = get_sorted_files(data_dir, ".vtk")
 
     if not os.path.exists(netcdf_data_dir):
         os.makedirs(netcdf_data_dir)
 
     logging.info("Converting vtk files to netcdf format...")
     for file_key, file in tqdm(enumerate(files), total=len(files)):
         time = file_key * output_time_step
```

### Comparing `inductiva-0.0.6/inductiva/fluids/scenarios/dam_break/dam_break.py` & `inductiva-0.0.7/inductiva/fluids/scenarios/dam_break/dam_break.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Describes the physical scenarios and runs its simulation via API."""
 from typing import List, Literal, Optional
 from enum import Enum
 from dataclasses import dataclass
 
 from inductiva.simulation import Simulator
+from inductiva.fluids.simulators import DualSPHysics
 from inductiva.fluids.scenarios.fluid_block import FluidBlock
 from inductiva.fluids.fluid_types import FluidType
 from inductiva.fluids.fluid_types import WATER
 from inductiva.types import Path
 
+from inductiva.fluids.scenarios._post_processing import SPHSimulationOutput
+
 
 @dataclass
 class ParticleRadius(Enum):
     """Sets particle radius according to resolution."""
     HIGH = 0.008
     MEDIUM = 0.012
     LOW = 0.02
@@ -44,17 +47,17 @@
                          kinematic_viscosity=fluid.kinematic_viscosity,
                          dimensions=dimensions,
                          position=position)
 
     # pylint: disable=arguments-renamed
     def simulate(
         self,
-        simulator: Simulator,
+        simulator: Simulator = DualSPHysics(),
         output_dir: Optional[Path] = None,
-        device: Literal["cpu", "gpu"] = "cpu",
+        device: Literal["cpu", "gpu"] = "gpu",
         resolution: Literal["high", "medium", "low"] = "medium",
         simulation_time: float = 1,
     ):
         """Simulates the scenario.
         
         Args:
             simulator: Simulator to use.
@@ -62,14 +65,14 @@
             device: Device in which to run the simulation.
             resolution: Resolution of the simulation.
             simulation_time: Simulation time, in seconds.
         """
 
         particle_radius = ParticleRadius[resolution.upper()].value
 
-        return super().simulate(
-            simulator,
-            output_dir=output_dir,
-            device=device,
-            particle_radius=particle_radius,
-            simulation_time=simulation_time,
-        )
+        sim_output_path = super().simulate(simulator=simulator,
+                                           output_dir=output_dir,
+                                           device=device,
+                                           particle_radius=particle_radius,
+                                           simulation_time=simulation_time)
+
+        return SPHSimulationOutput(sim_output_path.sim_output_dir)
```

### Comparing `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/fluid_block.py` & `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/fluid_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from inductiva.types import Path
 from inductiva.scenarios import Scenario
 from inductiva.simulation import Simulator
 from inductiva.fluids.fluid_types import FluidType
 from inductiva.fluids.simulators import SPlisHSPlasH
 from inductiva.fluids.simulators import DualSPHysics
 from inductiva.utils.templates import replace_params_in_template
+from inductiva.fluids.scenarios._post_processing import SPHSimulationOutput
 
 TANK_DIMENSIONS = [1, 1, 1]
 
 SPLISHSPLASH_TEMPLATE_FILENAME = "fluid_block_template.splishsplash.json.jinja"
 SPLISHSPLASH_CONFIG_FILENAME = "fluid_block.json"
 UNIT_BOX_MESH_FILENAME = "unit_box.obj"
 
@@ -59,23 +60,23 @@
         if inital_velocity is None:
             self.initial_velocity = [0, 0, 0]
         else:
             self.initial_velocity = inital_velocity
 
     def simulate(
         self,
-        simulator: Simulator,
+        simulator: Simulator = DualSPHysics(),
         output_dir: Optional[Path] = None,
-        device: Literal["cpu", "gpu"] = "cpu",
+        device: Literal["cpu", "gpu"] = "gpu",
         particle_radius: float = 0.02,
         simulation_time: float = 1,
         adaptive_time_step: bool = True,
         particle_sorting: bool = True,
         time_step: float = 0.001,
-        output_time_step: float = 0.02,
+        output_time_step: float = 1 / 60,
     ):
         """Simulates the scenario.
         
         Args:
             simulator: Simulator to use.
             output_dir: Directory to store the simulation output.
             device: Device in which to run the simulation.
@@ -103,15 +104,15 @@
 
         # TODO: Add any kind of post-processing here, e.g. convert files?
         # convert_vtk_data_dir_to_netcdf(
         #     data_dir=os.path.join(output_path, "vtk"),
         #     output_time_step=SPLISHSPLASH_OUTPUT_TIM_STEP,
         #     netcdf_data_dir=os.path.join(output_path, "netcdf"))
 
-        return output_path
+        return SPHSimulationOutput(output_path)
 
 
 @FluidBlock.get_config_filename.register
 def _(cls, simulator: SPlisHSPlasH):  # pylint: disable=unused-argument
     """Returns the configuration filename for SPlisHSPlasH."""
     return SPLISHSPLASH_CONFIG_FILENAME
 
@@ -138,15 +139,17 @@
             "time_step": self.time_step,
             "particle_radius": self.particle_radius,
             "data_export_rate": 1 / self.output_time_step,
             "tank_filename": UNIT_BOX_MESH_FILENAME,
             "tank_dimensions": TANK_DIMENSIONS,
             "fluid_filename": UNIT_BOX_MESH_FILENAME,
             "fluid": self.fluid,
-            "fluid_position": [fluid_margin] * 3,
+            "fluid_position": [
+                position + fluid_margin for position in self.position
+            ],
             "fluid_dimensions": [
                 dimension - 2 * fluid_margin for dimension in self.dimensions
             ],
             "fluid_velocity": self.initial_velocity,
             "particle_sorting": self.particle_sorting,
             "adaptive_time_step": self.adaptive_time_step,
         },
```

### Comparing `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja` & `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja` & `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_block/unit_box.obj` & `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/unit_box.obj`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py` & `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja` & `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py` & `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py` & `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/fluids/shapes.py` & `inductiva-0.0.7/inductiva/fluids/shapes.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/fluids/simulators/dualsphysics.py` & `inductiva-0.0.7/inductiva/fluids/simulators/dualsphysics.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/fluids/simulators/openfoam.py` & `inductiva-0.0.7/inductiva/fluids/simulators/openfoam.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def api_method_name(self) -> str:
         return "fvm.openfoam.run_simulation"
 
     def run(
         self,
         input_dir: types.Path,
         output_dir: Optional[types.Path] = None,
-        openfoam_solver: str = "isoFoam",
+        openfoam_solver: str = "interFoam",
         n_cores=1,
         track_logs: bool = False,
     ) -> pathlib.Path:
         """Run the simulation.
 
         Args:
             n_cores: Number of MPI cores to use for the simulation.
```

### Comparing `inductiva-0.0.6/inductiva/fluids/simulators/splishsplash.py` & `inductiva-0.0.7/inductiva/fluids/simulators/splishsplash.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/fluids/simulators/swash.py` & `inductiva-0.0.7/inductiva/fluids/simulators/swash.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/fluids/simulators/xbeach.py` & `inductiva-0.0.7/inductiva/fluids/simulators/xbeach.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/scenarios.py` & `inductiva-0.0.7/inductiva/scenarios.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/simulation/simulator.py` & `inductiva-0.0.7/inductiva/simulation/simulator.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/utils/data.py` & `inductiva-0.0.7/inductiva/utils/data.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/utils/files_test.py` & `inductiva-0.0.7/inductiva/utils/files_test.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/utils/flags.py` & `inductiva-0.0.7/inductiva/utils/flags.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/utils/meta.py` & `inductiva-0.0.7/inductiva/utils/meta.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva/utils/misc_test.py` & `inductiva-0.0.7/inductiva/utils/misc_test.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.6/inductiva.egg-info/SOURCES.txt` & `inductiva-0.0.7/inductiva.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -62,20 +62,20 @@
 inductiva/core/math.py
 inductiva/core/test.py
 inductiva/core/cupy/__init__.py
 inductiva/core/cupy/linalg.py
 inductiva/core/slepc/__init__.py
 inductiva/core/slepc/linalg.py
 inductiva/fluids/__init__.py
-inductiva/fluids/_output_post_processing.py
 inductiva/fluids/fluid_types.py
 inductiva/fluids/shapes.py
 inductiva/fluids/post_processing/__init__.py
 inductiva/fluids/post_processing/splishsplash.py
 inductiva/fluids/scenarios/__init__.py
+inductiva/fluids/scenarios/_post_processing.py
 inductiva/fluids/scenarios/dam_break/__init__.py
 inductiva/fluids/scenarios/dam_break/dam_break.py
 inductiva/fluids/scenarios/fluid_block/__init__.py
 inductiva/fluids/scenarios/fluid_block/fluid_block.py
 inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja
 inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja
 inductiva/fluids/scenarios/fluid_block/unit_box.obj
@@ -86,14 +86,17 @@
 inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py
 inductiva/fluids/simulators/__init__.py
 inductiva/fluids/simulators/dualsphysics.py
 inductiva/fluids/simulators/openfoam.py
 inductiva/fluids/simulators/splishsplash.py
 inductiva/fluids/simulators/swash.py
 inductiva/fluids/simulators/xbeach.py
+inductiva/molecules/__init__.py
+inductiva/molecules/simulators/__init__.py
+inductiva/molecules/simulators/gromacs.py
 inductiva/simulation/__init__.py
 inductiva/simulation/simulator.py
 inductiva/utils/__init__.py
 inductiva/utils/data.py
 inductiva/utils/files.py
 inductiva/utils/files_test.py
 inductiva/utils/flags.py
```

### Comparing `inductiva-0.0.6/setup.cfg` & `inductiva-0.0.7/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = inductiva
-version = 0.0.6
+version = 0.0.7
 description = Python client for the Inductiva API
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Inductiva Research Labs
 author_email = contact@inductiva.ai
 url = https://github.com/inductiva/inductiva
 classifiers = 
@@ -26,15 +26,15 @@
 	numpy
 	scipy
 	matplotlib
 	xarray
 	gmsh
 	meshio
 	vtk
-	imageio
+	pyvista
 	imageio-ffmpeg
 	ipython
 	websockets
 
 [options.package_data]
 * = *.obj, *.jinja
```

