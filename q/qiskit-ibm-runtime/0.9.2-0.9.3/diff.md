# Comparing `tmp/qiskit-ibm-runtime-0.9.2.tar.gz` & `tmp/qiskit-ibm-runtime-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-ibm-runtime-0.9.2.tar", last modified: Thu Mar 30 17:21:57 2023, max compression
+gzip compressed data, was "qiskit-ibm-runtime-0.9.3.tar", last modified: Thu Apr 13 17:22:39 2023, max compression
```

## Comparing `qiskit-ibm-runtime-0.9.2.tar` & `qiskit-ibm-runtime-0.9.3.tar`

### file list

```diff
@@ -1,171 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.991030 qiskit-ibm-runtime-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-03-30 17:21:57.991030 qiskit-ibm-runtime-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.975030 qiskit-ibm-runtime-0.9.2/program_source/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/program_source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.975030 qiskit-ibm-runtime-0.9.2/program_source/circuit_runner/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/program_source/circuit_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/program_source/circuit_runner/circuit_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.975030 qiskit-ibm-runtime-0.9.2/program_source/hello_world/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/program_source/hello_world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/program_source/hello_world/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/program_source/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.975030 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.979030 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/accounts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/accounts/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/accounts/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.979030 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/client_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.979030 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/clients/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/clients/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/clients/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/clients/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/clients/runtime_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/clients/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.979030 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/cloud_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/program_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/runtime_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.979030 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/utils/data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/backendreservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    16513 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/hub_group_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/ibm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/ibm_qubit_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.983030 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/environment_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/execution_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/resilience_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/simulator_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/transpilation_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.983030 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/program/
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/program/program_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/program/program_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/program/result_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/program/user_messenger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.983030 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/proxies/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/proxies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/proxies/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    60418 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qiskit_runtime_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.983030 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.983030 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/binary_io/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/binary_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38998 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/binary_io/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/binary_io/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/binary_io/value.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/type_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    22479 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/runtime_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/runtime_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/runtime_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/runtime_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    14624 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.983030 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/backend_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/backend_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/estimator_result_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/hgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/runner_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/sampler_result_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.979030 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-03-30 17:21:57.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-03-30 17:21:57.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 17:21:57.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 17:21:57.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-30 17:21:57.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-30 17:21:57.000000 qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-30 17:21:57.991030 qiskit-ibm-runtime-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.987030 qiskit-ibm-runtime-0.9.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.987030 qiskit-ibm-runtime-0.9.2/test/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/e2e/test_tutorials.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/ibm_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.987030 qiskit-ibm-runtime-0.9.2/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/integration/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/integration/test_auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/integration/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/integration/test_backend_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/integration/test_basic_server_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/integration/test_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/integration/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/integration/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/integration/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)    11712 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/integration/test_proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/integration/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/integration/test_retrieve_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/integration/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/integration/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.991030 qiskit-ibm-runtime-0.9.2/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:21:57.991030 qiskit-ibm-runtime-0.9.2/test/unit/mock/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/mock/fake_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/mock/fake_quantum_auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18158 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/mock/fake_runtime_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/mock/fake_runtime_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/mock/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/mock/proxy_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/mock/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/mock/ws_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    39762 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/test_backend_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/test_client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/test_data_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/test_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    27773 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/test_ibm_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/test_job_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/test_programs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/test_runtime_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/unit/test_utils_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-03-30 17:21:48.000000 qiskit-ibm-runtime-0.9.2/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.164676 qiskit-ibm-runtime-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-04-13 17:22:39.164676 qiskit-ibm-runtime-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.144676 qiskit-ibm-runtime-0.9.3/program_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/program_source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.144676 qiskit-ibm-runtime-0.9.3/program_source/circuit_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/program_source/circuit_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/program_source/circuit_runner/circuit_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.144676 qiskit-ibm-runtime-0.9.3/program_source/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/program_source/hello_world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/program_source/hello_world/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/program_source/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.144676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.148676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.148676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/client_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.148676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/runtime_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.148676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/cloud_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/program_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/runtime_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.152676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/utils/data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/backendreservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17990 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/hub_group_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23941 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/ibm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/ibm_qubit_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.152676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/environment_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/execution_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/resilience_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/simulator_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/transpilation_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.152676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/program_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/program_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/result_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/user_messenger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.152676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/proxies/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/proxies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/proxies/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63935 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qiskit_runtime_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.152676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.156676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38998 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/type_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22526 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.156676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/backend_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/backend_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/estimator_result_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/hgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/runner_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/sampler_result_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.144676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-04-13 17:22:39.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-04-13 17:22:39.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:22:39.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:22:39.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-13 17:22:39.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 17:22:39.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-13 17:22:39.164676 qiskit-ibm-runtime-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.156676 qiskit-ibm-runtime-0.9.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.156676 qiskit-ibm-runtime-0.9.3/test/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/e2e/test_tutorials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/ibm_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.160676 qiskit-ibm-runtime-0.9.3/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_backend_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_basic_server_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_retrieve_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.160676 qiskit-ibm-runtime-0.9.3/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.164676 qiskit-ibm-runtime-0.9.3/test/unit/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/fake_api_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/fake_quantum_auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17945 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/fake_runtime_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/fake_runtime_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/proxy_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/ws_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39797 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_backend_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_data_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36753 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_ibm_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_job_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_programs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_runtime_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_runtime_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_utils_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/utils.py
```

### Comparing `qiskit-ibm-runtime-0.9.2/LICENSE.txt` & `qiskit-ibm-runtime-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/PKG-INFO` & `qiskit-ibm-runtime-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-runtime
-Version: 0.9.2
+Version: 0.9.3
 Summary: IBM Quantum client for Qiskit Runtime.
 Home-page: https://github.com/Qiskit/qiskit-ibm-runtime
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-runtime/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-runtime-0.9.2/README.md` & `qiskit-ibm-runtime-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/program_source/__init__.py` & `qiskit-ibm-runtime-0.9.3/program_source/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/program_source/circuit_runner/__init__.py` & `qiskit-ibm-runtime-0.9.3/program_source/circuit_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/program_source/circuit_runner/circuit_runner.py` & `qiskit-ibm-runtime-0.9.3/program_source/circuit_runner/circuit_runner.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/program_source/hello_world/__init__.py` & `qiskit-ibm-runtime-0.9.3/program_source/hello_world/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/program_source/hello_world/hello_world.py` & `qiskit-ibm-runtime-0.9.3/program_source/hello_world/hello_world.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/__init__.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/accounts/__init__.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/accounts/account.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/accounts/exceptions.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/accounts/management.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/management.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/accounts/storage.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/storage.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/__init__.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/auth.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/client_parameters.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/client_parameters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/clients/__init__.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/clients/auth.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/clients/backend.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/clients/base.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/clients/runtime.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/runtime.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/clients/runtime_ws.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/runtime_ws.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/clients/version.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/exceptions.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/__init__.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/backend.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/base.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/cloud_backend.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/cloud_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/program.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/program.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/program_job.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/program_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/root.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/root.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/runtime.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/runtime.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/runtime_session.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/runtime_session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/utils/__init__.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/rest/utils/data_mapper.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/utils/data_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/api/session.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,21 @@
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Session customized for IBM Quantum access."""
 
+import inspect
 import os
 import re
 import logging
+import sys
 from typing import Dict, Optional, Any, Tuple, Union
+from pathlib import PurePath
 import pkg_resources
 
 from requests import Session, RequestException, Response
 from requests.adapters import HTTPAdapter
 from requests.auth import AuthBase
 from urllib3.util.retry import Retry
 
@@ -47,28 +50,39 @@
 # the `/devices/v/1` endpoint.
 # Capture groups: (/backends/)(<device_name>)(</optional rest of the url>)
 RE_BACKENDS_ENDPOINT = re.compile(r"^(.*/backends/)([^/}]{2,})(.*)$", re.IGNORECASE)
 
 
 def _get_client_header() -> str:
     """Return the client version."""
-    try:
-        client_header = "qiskit/" + pkg_resources.get_distribution("qiskit").version
-        return client_header
-    except Exception:  # pylint: disable=broad-except
-        pass
 
-    qiskit_pkgs = ["qiskit-terra", "qiskit-aer", "qiskit-ignis", "qiskit-aqua"]
-    pkg_versions = {"qiskit-ibm-runtime": ibm_runtime_version}
+    qiskit_pkgs = [
+        "qiskit_terra",
+        "qiskit_aer",
+        "qiskit_experiments",
+        "qiskit_nature",
+        "qiskit_machine_learning",
+        "qiskit_optimization",
+        "qiskit_finance",
+    ]
+
+    pkg_versions = {"qiskit_ibm_runtime": f"qiskit_ibm_runtime-{ibm_runtime_version}"}
     for pkg_name in qiskit_pkgs:
         try:
-            pkg_versions[pkg_name] = pkg_resources.get_distribution(pkg_name).version
+            version_info = (
+                f"{pkg_name}-{pkg_resources.get_distribution(pkg_name).version}"
+            )
+
+            if pkg_name in sys.modules:
+                version_info += "*"
+
+            pkg_versions[pkg_name] = version_info
         except Exception:  # pylint: disable=broad-except
             pass
-    return ",".join(pkg_versions.keys()) + "/" + ",".join(pkg_versions.values())
+    return f"qiskit-version-2/{','.join(pkg_versions.values())}"
 
 
 CLIENT_APPLICATION = _get_client_header()
 
 
 class PostForcelistRetry(Retry):
     """Custom ``urllib3.Retry`` class that performs retry on ``POST`` errors in the force list.
@@ -162,15 +176,15 @@
             auth: Authentication handler.
             timeout: Timeout for the requests, in the form of (connection_timeout,
                 total_timeout).
         """
         super().__init__()
 
         self.base_url = base_url
-
+        self.custom_header: Optional[str] = None
         self._initialize_retry(retries_total, retries_connect, backoff_factor)
         self._initialize_session_parameters(verify, proxies or {}, auth)
         self._timeout = timeout
 
     def __del__(self) -> None:
         """RetrySession destructor. Closes the session."""
         try:
@@ -206,25 +220,17 @@
         """Set the session parameters and attributes.
 
         Args:
             verify: Whether to enable SSL verification.
             proxies: Proxy URLs mapped by protocol.
             auth: Authentication handler.
         """
-        client_app_header = CLIENT_APPLICATION
-
-        # Append custom header to the end if specified
-        custom_header = os.getenv(CUSTOM_HEADER_ENV_VAR) or os.getenv(
+        self.custom_header = os.getenv(CUSTOM_HEADER_ENV_VAR) or os.getenv(
             QE_PROVIDER_HEADER_ENV_VAR
         )
-        if custom_header:
-            client_app_header += "/" + custom_header
-
-        self.headers.update({"X-Qx-Client-Application": client_app_header})
-
         self.auth = auth
         self.proxies = proxies or {}
         self.verify = verify
 
     def request(  # type: ignore[override]
         self, method: str, url: str, bare: bool = False, **kwargs: Any
     ) -> Response:
@@ -257,17 +263,46 @@
         else:
             final_url = self.base_url + url
 
         # Add a timeout to the connection for non-proxy connections.
         if not self.proxies and "timeout" not in kwargs:
             kwargs.update({"timeout": self._timeout})
 
-        headers = self.headers.copy()
+        headers = self.headers.copy()  # type: ignore
         headers.update(kwargs.pop("headers", {}))
 
+        # Set default caller
+        headers.update({"X-Qx-Client-Application": f"{CLIENT_APPLICATION}/qiskit"})
+
+        # Use PurePath in order to support arbitrary path formats
+        callers = {PurePath("qiskit/"), "qiskit_"}
+
+        stack = inspect.stack()
+        stack.reverse()
+
+        found_caller = False
+        for frame in stack:
+            frame_path = str(PurePath(frame.filename))
+            for caller in callers:
+                if str(caller) in frame_path:
+                    caller_str = str(caller) + frame_path.split(str(caller), 1)[-1]
+                    sanitized_caller_str = caller_str.replace("/", "~")
+                    headers.update(
+                        {
+                            "X-Qx-Client-Application": f"{CLIENT_APPLICATION}/{sanitized_caller_str}"
+                        }
+                    )
+                    found_caller = True
+                    break  # break out of the inner loop
+            if found_caller:
+                break  # break out of the outer loop
+
+        self.headers = headers
+        self._set_custom_header()
+
         try:
             self._log_request_info(final_url, method, kwargs)
             response = super().request(method, final_url, headers=headers, **kwargs)
             response.raise_for_status()
         except RequestException as ex:
             # Wrap the requests exceptions into a IBM Q custom one, for
             # compatibility.
@@ -369,12 +404,22 @@
         if "objectstorage" in endpoint_url:
             return False
         if "bookings" in endpoint_url:
             return False
 
         return True
 
+    def _set_custom_header(self) -> None:
+        """Set custom header."""
+        headers = self.headers.copy()  # type: ignore
+        if self.custom_header:
+            current = headers["X-Qx-Client-Application"]
+            headers.update(
+                {"X-Qx-Client-Application": f"{current}/{self.custom_header}"}
+            )
+            self.headers = headers
+
     def __getstate__(self) -> Dict:
         """Overwrite Session's getstate to include all attributes."""
         state = super().__getstate__()  # type: ignore
         state.update(self.__dict__)
         return state
```

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/backendreservation.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/backendreservation.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/constants.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/estimator.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/estimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Estimator primitive."""
 
 from __future__ import annotations
+import os
 import copy
 from typing import Iterable, Optional, Dict, Sequence, Any, Union
 import logging
 from dataclasses import asdict
 
 from qiskit.circuit import QuantumCircuit, Parameter
 from qiskit.quantum_info import SparsePauliOp
@@ -301,28 +302,35 @@
             "observables": observables,
             "observable_indices": list(range(len(observables))),
             "parameters": [circ.parameters for circ in circuits],
             "parameter_values": parameter_values,
         }
 
         combined = Options._merge_options(self._options, kwargs.get("_user_kwargs", {}))
+
+        backend_obj: Optional[IBMBackend] = None
         if self._session.backend():
             backend_obj = self._session.service.backend(self._session.backend())
             combined = set_default_error_levels(
                 combined,
                 backend_obj,
                 Options._DEFAULT_OPTIMIZATION_LEVEL,
                 Options._DEFAULT_RESILIENCE_LEVEL,
             )
         else:
             combined["optimization_level"] = Options._DEFAULT_OPTIMIZATION_LEVEL
             combined["resilience_level"] = Options._DEFAULT_RESILIENCE_LEVEL
         logger.info("Submitting job using options %s", combined)
+        self._validate_options(combined)
         inputs.update(Options._get_program_inputs(combined))
 
+        if backend_obj and combined["transpilation"]["skip_transpilation"]:
+            for circ in circuits:
+                backend_obj.check_faulty(circ)
+
         return self._session.run(
             program_id=self._PROGRAM_ID,
             inputs=inputs,
             options=Options._get_runtime_options(combined),
             callback=combined.get("environment", {}).get("callback", None),
             result_decoder=DEFAULT_DECODERS.get(self._PROGRAM_ID),
         )
@@ -363,14 +371,16 @@
             "parameters": self._initial_inputs["parameters"],
             "observables": self._initial_inputs["observables"],
             "circuit_indices": circuits,
             "parameter_values": parameter_values,
             "observable_indices": observables,
         }
         combined = Options._merge_options(self._options, run_options)
+
+        self._validate_options(combined)
         inputs.update(Options._get_program_inputs(combined))
 
         return self._session.run(
             program_id=self._PROGRAM_ID,
             inputs=inputs,
             options=Options._get_runtime_options(combined),
             result_decoder=DEFAULT_DECODERS.get(self._PROGRAM_ID),
@@ -408,7 +418,34 @@
     def set_options(self, **fields: Any) -> None:
         """Set options values for the estimator.
 
         Args:
             **fields: The fields to update the options
         """
         self._options = Options._merge_options(self._options, fields)
+
+    def _validate_options(self, options: dict) -> None:
+        """Validate that program inputs (options) are valid
+        Raises:
+            ValueError: if resilience_level is out of the allowed range.
+            ValueError: if resilience_level==3, backend is simulator and no coupling map
+        """
+        if os.getenv("QISKIT_RUNTIME_SKIP_OPTIONS_VALIDATION"):
+            return
+
+        if not options.get("resilience_level") in list(
+            range(Options._MAX_RESILIENCE_LEVEL_ESTIMATOR + 1)
+        ):
+            raise ValueError(
+                f"resilience_level can only take the values "
+                f"{list(range(Options._MAX_RESILIENCE_LEVEL_ESTIMATOR + 1))} in Estimator"
+            )
+
+        if options.get("resilience_level") == 3 and self._session.backend() in [
+            b.name for b in self._session.service.backends(simulator=True)
+        ]:
+            if not options.get("simulator").get("coupling_map"):
+                raise ValueError(
+                    "When the backend is a simulator and resilience_level == 3,"
+                    "a coupling map is required."
+                )
+        Options.validate_options(options)
```

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/exceptions.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/hub_group_project.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/hub_group_project.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,23 +9,20 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """A hub, group and project in an IBM Quantum account."""
 
 import logging
-from collections import OrderedDict
-from typing import Any, Dict, Optional
+from typing import Any, List
 
 from qiskit_ibm_runtime import (  # pylint: disable=unused-import
     ibm_backend,
     qiskit_runtime_service,
 )
-
-from .utils.backend_decoder import configuration_from_server_data
 from .api.client_parameters import ClientParameters
 from .api.clients import RuntimeClient
 from .utils.hgp import from_instance_format
 
 logger = logging.getLogger(__name__)
 
 
@@ -43,64 +40,50 @@
         Args:
             client_params: Parameters used for server connection.
             instance: Hub/group/project.
         """
         self._service = service
         self._runtime_client = RuntimeClient(client_params)
         # Initialize the internal list of backends.
-        self._backends: Dict[str, "ibm_backend.IBMBackend"] = {}
+        # self._backends: Dict[str, "ibm_backend.IBMBackend"] = {}
+        self._backends: List[str] = []
         self._hub, self._group, self._project = from_instance_format(instance)
 
     @property
-    def backends(self) -> Dict[str, "ibm_backend.IBMBackend"]:
-        """Gets the backends for the hub/group/project, if not loaded.
+    def backends(self) -> List[str]:
+        """Gets the backends for the hub/group/project.
 
         Returns:
-            Dict[str, IBMBackend]: the backends
+            A list of backend names.
         """
         if not self._backends:
             self._backends = self._discover_remote_backends()
         return self._backends
 
     @backends.setter
-    def backends(self, value: Dict[str, "ibm_backend.IBMBackend"]) -> None:
+    def backends(self, value: List[str]) -> None:
         """Sets the value for the hub/group/project's backends.
 
         Args:
             value: the backends
         """
         self._backends = value
 
-    def _discover_remote_backends(self) -> Dict[str, "ibm_backend.IBMBackend"]:
+    def _discover_remote_backends(self) -> List[str]:
         """Return the remote backends available for this hub/group/project.
 
         Returns:
-            A dict of the remote backend instances, keyed by backend name.
+            A list of backends.
         """
-        ret = OrderedDict()
         backends = self._runtime_client.list_backends(self.name)
-        if backends:
-            for backend in backends:
-                raw_config = self._runtime_client.backend_configuration(backend)
-                config = configuration_from_server_data(
-                    raw_config=raw_config, instance=self.name
-                )
-                if not config:
-                    continue
-                ret[config.backend_name] = ibm_backend.IBMBackend(
-                    instance=self.name,
-                    configuration=config,
-                    service=self._service,
-                    api_client=self._runtime_client,
-                )
-        return ret
-
-    def backend(self, name: str) -> Optional["ibm_backend.IBMBackend"]:
-        """Get backend by name."""
-        return self._backends.get(name, None)
+        return backends or []
+
+    def has_backend(self, name: str) -> bool:
+        """Determine if the hgp can access the backend."""
+        return name in self._backends
 
     @property
     def name(self) -> str:
         """Returns the unique id.
 
         Returns:
             An ID uniquely represents this h/g/p.
```

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/ibm_backend.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/ibm_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 """Module for interfacing with an IBM Quantum Backend."""
 
 import logging
 
 from typing import Iterable, Union, Optional, Any, List
 from datetime import datetime as python_datetime
 
+from qiskit import QuantumCircuit
 from qiskit.qobj.utils import MeasLevel, MeasReturnType
 from qiskit.providers.backend import BackendV2 as Backend
 from qiskit.providers.options import Options
 from qiskit.providers.models import (
     BackendStatus,
     BackendProperties,
     PulseDefaults,
@@ -498,14 +499,50 @@
     def run(self, *args: Any, **kwargs: Any) -> None:
         """Not supported method"""
         # pylint: disable=arguments-differ
         raise RuntimeError(
             "IBMBackend.run() is not supported in the Qiskit Runtime environment."
         )
 
+    def check_faulty(self, circuit: QuantumCircuit) -> None:
+        """Check if the input circuit uses faulty qubits or edges.
+
+        Args:
+            circuit: Circuit to check.
+
+        Raises:
+            ValueError: If an instruction operating on a faulty qubit or edge is found.
+        """
+        if not self.properties():
+            return
+
+        faulty_qubits = self.properties().faulty_qubits()
+        faulty_gates = self.properties().faulty_gates()
+        faulty_edges = [
+            tuple(gate.qubits) for gate in faulty_gates if len(gate.qubits) > 1
+        ]
+
+        for instr in circuit.data:
+            if instr.operation.name == "barrier":
+                continue
+            qubit_indices = tuple(circuit.find_bit(x).index for x in instr.qubits)
+
+            for circ_qubit in qubit_indices:
+                if circ_qubit in faulty_qubits:
+                    raise ValueError(
+                        f"Circuit {circuit.name} contains instruction "
+                        f"{instr} operating on a faulty qubit {circ_qubit}."
+                    )
+
+            if len(qubit_indices) == 2 and qubit_indices in faulty_edges:
+                raise ValueError(
+                    f"Circuit {circuit.name} contains instruction "
+                    f"{instr} operating on a faulty edge {qubit_indices}"
+                )
+
 
 class IBMRetiredBackend(IBMBackend):
     """Backend class interfacing with an IBM Quantum device no longer available."""
 
     def __init__(
         self,
         configuration: Union[QasmBackendConfiguration, PulseBackendConfiguration],
```

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/ibm_qubit_properties.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/ibm_qubit_properties.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/__init__.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/environment_options.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/environment_options.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/execution_options.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/execution_options.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/options.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,18 @@
             :class:`SimulatorOptions` for all available options.
     """
 
     # Defaults for optimization_level and for resilience_level will be assigned
     # in Sampler/Estimator
     _DEFAULT_OPTIMIZATION_LEVEL = 3
     _DEFAULT_RESILIENCE_LEVEL = 1
+    _MAX_OPTIMIZATION_LEVEL = 3
+    _MAX_RESILIENCE_LEVEL_ESTIMATOR = 3
+    _MAX_RESILIENCE_LEVEL_SAMPLER = 1
+
     optimization_level: Optional[int] = None
     resilience_level: Optional[int] = None
     max_execution_time: Optional[int] = None
     transpilation: Union[TranspilationOptions, Dict] = field(
         default_factory=TranspilationOptions
     )
     resilience: Union[ResilienceOptions, Dict] = field(
@@ -102,14 +106,15 @@
     simulator: Union[SimulatorOptions, Dict] = field(default_factory=SimulatorOptions)
 
     _obj_fields: ClassVar[dict] = {
         "transpilation": TranspilationOptions,
         "execution": ExecutionOptions,
         "environment": EnvironmentOptions,
         "simulator": SimulatorOptions,
+        "resilience": ResilienceOptions,
     }
 
     @staticmethod
     def _get_program_inputs(options: dict) -> dict:
         """Convert the input options to program compatible inputs.
 
         Returns:
@@ -152,14 +157,29 @@
                 warnings.warn(
                     f"Key '{key}' is an unrecognized option. It may be ignored."
                 )
                 inputs[key] = options[key]
         return inputs
 
     @staticmethod
+    def validate_options(options: dict) -> None:
+        """Validate that program inputs (options) are valid
+        Raises:
+            ValueError: if optimization_level is out of the allowed range.
+        """
+        if not options.get("optimization_level") in list(
+            range(Options._MAX_OPTIMIZATION_LEVEL + 1)
+        ):
+            raise ValueError(
+                f"optimization_level can only take the values "
+                f"{list(range(Options._MAX_OPTIMIZATION_LEVEL + 1))}"
+            )
+        ResilienceOptions.validate_resilience_options(options.get("resilience"))
+
+    @staticmethod
     def _get_runtime_options(options: dict) -> dict:
         """Extract runtime options.
 
         Returns:
             Runtime options.
         """
         environment = options.get("environment") or {}
```

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/simulator_options.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/simulator_options.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/transpilation_options.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/transpilation_options.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/options/utils.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/program/__init__.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/program/program_backend.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/program_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/program/program_template.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/program_template.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/program/result_decoder.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/result_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/program/user_messenger.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/user_messenger.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/proxies/__init__.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/proxies/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/proxies/configuration.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/proxies/configuration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qiskit_runtime_service.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qiskit_runtime_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 from collections import OrderedDict
 from typing import Dict, Callable, Optional, Union, List, Any, Type, Sequence
 
 from qiskit.providers.backend import BackendV1 as Backend
 from qiskit.providers.provider import ProviderV1 as Provider
 from qiskit.providers.exceptions import QiskitBackendNotFoundError
 from qiskit.providers.providerutils import filter_backends
+from qiskit.providers.models import (
+    PulseBackendConfiguration,
+    QasmBackendConfiguration,
+)
 
 from qiskit_ibm_runtime import ibm_backend
 from .accounts import AccountManager, Account, AccountType, ChannelType
 from .proxies import ProxyConfiguration
 from .api.clients import AuthClient, VersionClient
 from .api.clients.runtime import RuntimeClient
 from .api.exceptions import RequestsApiError
@@ -45,14 +49,15 @@
 from .runtime_program import RuntimeProgram, ParameterNamespace
 from .runtime_session import RuntimeSession  # pylint: disable=cyclic-import
 from .utils import RuntimeDecoder, to_base64_string, to_python_identifier
 from .utils.backend_decoder import configuration_from_server_data
 from .utils.hgp import to_instance_format, from_instance_format
 from .api.client_parameters import ClientParameters
 from .runtime_options import RuntimeOptions
+from .ibm_backend import IBMBackend
 from .utils.deprecation import (
     deprecate_function,
     deprecate_arguments,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -202,14 +207,15 @@
             proxies=self._account.proxies,
             verify=self._account.verify,
         )
 
         self._channel = self._account.channel
         self._programs: Dict[str, RuntimeProgram] = {}
         self._backends: Dict[str, "ibm_backend.IBMBackend"] = {}
+        self._backend_configs: Dict[str, Any] = {}
 
         if self._channel == "ibm_cloud":
             self._api_client = RuntimeClient(self._client_params)
             # TODO: We can make the backend discovery lazy
             self._backends = self._discover_cloud_backends()
             return
         else:
@@ -218,17 +224,17 @@
             self._client_params.url = auth_client.current_service_urls()["services"][
                 "runtime"
             ]
             self._client_params.token = auth_client.current_access_token()
             self._api_client = RuntimeClient(self._client_params)
             self._hgps = self._initialize_hgps(auth_client)
             for hgp in self._hgps.values():
-                for backend_name, backend in hgp.backends.items():
+                for backend_name in hgp.backends:
                     if backend_name not in self._backends:
-                        self._backends[backend_name] = backend
+                        self._backends[backend_name] = None
 
         # TODO - it'd be nice to allow some kind of autocomplete, but `service.ibmq_foo`
         # just seems wrong since backends are not runtime service instances.
         # self._discover_backends()
 
     @staticmethod
     def _auth_warning() -> None:
@@ -486,26 +492,26 @@
         if instance:
             _ = from_instance_format(instance)  # Verify format
             if instance not in self._hgps:
                 raise IBMInputValueError(
                     f"Hub/group/project {instance} "
                     "could not be found for this account."
                 )
-            if backend_name and not self._hgps[instance].backend(backend_name):
+            if backend_name and not self._hgps[instance].has_backend(backend_name):
                 raise QiskitBackendNotFoundError(
                     f"Backend {backend_name} cannot be found in "
                     f"hub/group/project {instance}"
                 )
             return self._hgps[instance]
 
         if not backend_name:
             return list(self._hgps.values())[0]
 
         for hgp in self._hgps.values():
-            if hgp.backend(backend_name):
+            if hgp.has_backend(backend_name):
                 return hgp
 
         error_message = (
             f"Backend {backend_name} cannot be found in any "
             f"hub/group/project for this account."
         )
         if not isinstance(backend_name, str):
@@ -566,21 +572,53 @@
                 <https://qiskit.org/documentation/apidoc/providers_models.html>
 
         Returns:
             The list of available backends that match the filter.
 
         Raises:
             IBMInputValueError: If an input is invalid.
+            QiskitBackendNotFoundError: If the backend is not in any instance.
         """
         # TODO filter out input_allowed not having runtime
+        backends: List[IBMBackend] = []
         if self._channel == "ibm_quantum":
-            if instance:
-                backends = list(self._get_hgp(instance=instance).backends.values())
+            if name:
+                if name not in self._backends:
+                    raise QiskitBackendNotFoundError("No backend matches the criteria.")
+                if (
+                    not self._backends[name]
+                    or instance != self._backends[name]._instance
+                ):
+                    self._set_backend_config(name)
+                    self._backends[name] = self._create_backend_obj(
+                        self._backend_configs[name],
+                        instance,
+                    )
+                backends.append(self._backends[name])
+            elif instance:
+                hgp = self._get_hgp(instance=instance)
+                for backend_name in hgp.backends:
+                    if (
+                        not self._backends[backend_name]
+                        or instance != self._backends[backend_name]._instance
+                    ):
+                        self._set_backend_config(backend_name, instance)
+                        self._backends[backend_name] = self._create_backend_obj(
+                            self._backend_configs[backend_name], instance
+                        )
+                    backends.append(self._backends[backend_name])
             else:
-                backends = list(self._backends.values())
+                for backend_name, backend_config in self._backends.items():
+                    if not backend_config:
+                        self._set_backend_config(backend_name)
+                        self._backends[backend_name] = self._create_backend_obj(
+                            self._backend_configs[backend_name]
+                        )
+                    backends.append(self._backends[backend_name])
+
         else:
             if instance:
                 raise IBMInputValueError(
                     "The 'instance' keyword is only supported for ``ibm_quantum`` runtime."
                 )
             backends = list(self._backends.values())
 
@@ -588,14 +626,62 @@
             kwargs["backend_name"] = name
         if min_num_qubits:
             backends = list(
                 filter(lambda b: b.configuration().n_qubits >= min_num_qubits, backends)
             )
         return filter_backends(backends, filters=filters, **kwargs)
 
+    def _set_backend_config(
+        self, backend_name: str, instance: Optional[str] = None
+    ) -> None:
+        """Retrieve backend configuration and add to backend_configs.
+        Args:
+            backend_name: backend name that will be returned.
+            instance: the current h/g/p.
+        """
+        if backend_name not in self._backend_configs:
+            raw_config = self._api_client.backend_configuration(backend_name)
+            config = configuration_from_server_data(
+                raw_config=raw_config, instance=instance
+            )
+            self._backend_configs[backend_name] = config
+
+    def _create_backend_obj(
+        self,
+        config: Union[QasmBackendConfiguration, PulseBackendConfiguration],
+        instance: Optional[str] = None,
+    ) -> IBMBackend:
+        """Given a backend configuration return the backend object.
+        Args:
+            config: backend configuration.
+            instance: the current h/g/p.
+        Returns:
+            A backend object.
+        Raises:
+            QiskitBackendNotFoundError: if the backend is not in the hgp passed in.
+        """
+        if not instance:
+            for hgp in list(self._hgps.values()):
+                if config.backend_name in hgp.backends:
+                    instance = to_instance_format(hgp._hub, hgp._group, hgp._project)
+                    break
+
+        elif config.backend_name not in self._get_hgp(instance=instance).backends:
+            raise QiskitBackendNotFoundError(
+                f"Backend {config.backend_name} is not in "
+                f"{instance}: please try a different hub/group/project."
+            )
+
+        return ibm_backend.IBMBackend(
+            instance=instance,
+            configuration=config,
+            service=self,
+            api_client=self._api_client,
+        )
+
     def active_account(self) -> Optional[Dict[str, str]]:
         """Return the IBM Quantum account currently in use for the session.
 
         Returns:
             A dictionary with information about the account currently in the session.
         """
         return self._account.to_saved_format()
@@ -980,22 +1066,20 @@
         # If using params object, extract as dictionary
         if isinstance(inputs, ParameterNamespace):
             inputs.validate()
             inputs = vars(inputs)
 
         qrt_options.validate(channel=self.channel)
 
-        backend = None
         hgp_name = None
         if self._channel == "ibm_quantum":
             # Find the right hgp
             hgp = self._get_hgp(
                 instance=qrt_options.instance, backend_name=qrt_options.backend
             )
-            backend = hgp.backend(qrt_options.backend)
             hgp_name = hgp.name
 
         try:
             response = self._api_client.program_run(
                 program_id=program_id,
                 backend_name=qrt_options.backend,
                 params=inputs,
@@ -1011,16 +1095,15 @@
         except RequestsApiError as ex:
             if ex.status_code == 404:
                 raise RuntimeProgramNotFound(
                     f"Program not found: {ex.message}"
                 ) from None
             raise IBMRuntimeError(f"Failed to run program: {ex}") from None
 
-        if not backend:
-            backend = self.backend(name=response["backend"])
+        backend = self.backend(name=response["backend"], instance=hgp_name)
 
         job = RuntimeJob(
             backend=backend,
             api_client=self._api_client,
             client_params=self._client_params,
             job_id=response["id"],
             program_id=program_id,
```

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/__init__.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/binary_io/__init__.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/binary_io/circuits.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/circuits.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/binary_io/schedules.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/schedules.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/binary_io/value.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/value.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/common.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/common.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/exceptions.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/formats.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/formats.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/interface.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/interface.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/qpy/type_keys.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/type_keys.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/runtime_job.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,22 +162,23 @@
 
     def _download_external_result(self, response: Any) -> Any:
         """Download result from external URL.
 
         Args:
             response: Response to check for url keyword, if available, download result from given URL
         """
-        if "url" in response:
+        try:
             result_url_json = json.loads(response)
             if "url" in result_url_json:
                 url = result_url_json["url"]
                 result_response = requests.get(url)
-                response = result_response.content
-
-        return response
+                return result_response.content
+            return response
+        except json.JSONDecodeError:
+            return response
 
     def interim_results(self, decoder: Optional[Type[ResultDecoder]] = None) -> Any:
         """Return the interim results of the job.
 
         Args:
             decoder: A :class:`ResultDecoder` subclass used to decode interim results.
```

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/runtime_options.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_options.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/runtime_program.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_program.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/runtime_session.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/sampler.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Sampler primitive."""
 
 from __future__ import annotations
+import os
 from typing import Dict, Iterable, Optional, Sequence, Any, Union
 import copy
 import logging
 from dataclasses import asdict
 
 from qiskit.circuit import QuantumCircuit, Parameter
 from qiskit.providers.options import Options as TerraOptions
@@ -255,28 +256,35 @@
         inputs = {
             "circuits": circuits,
             "parameters": [circ.parameters for circ in circuits],
             "circuit_indices": list(range(len(circuits))),
             "parameter_values": parameter_values,
         }
         combined = Options._merge_options(self._options, kwargs.get("_user_kwargs", {}))
+
+        backend_obj: Optional[IBMBackend] = None
         if self._session.backend():
             backend_obj = self._session.service.backend(self._session.backend())
             combined = set_default_error_levels(
                 combined,
                 backend_obj,
                 Options._DEFAULT_OPTIMIZATION_LEVEL,
                 Options._DEFAULT_RESILIENCE_LEVEL,
             )
         else:
             combined["optimization_level"] = Options._DEFAULT_OPTIMIZATION_LEVEL
             combined["resilience_level"] = Options._DEFAULT_RESILIENCE_LEVEL
         logger.info("Submitting job using options %s", combined)
+        Sampler._validate_options(combined)
         inputs.update(Options._get_program_inputs(combined))
 
+        if backend_obj and combined["transpilation"]["skip_transpilation"]:
+            for circ in circuits:
+                backend_obj.check_faulty(circ)
+
         return self._session.run(
             program_id=self._PROGRAM_ID,
             inputs=inputs,
             options=Options._get_runtime_options(combined),
             callback=combined.get("environment", {}).get("callback", None),
             result_decoder=DEFAULT_DECODERS.get(self._PROGRAM_ID),
         )
@@ -314,15 +322,15 @@
         inputs = {
             "circuits": self._initial_inputs["circuits"],
             "parameters": self._initial_inputs["parameters"],
             "circuit_indices": circuits,
             "parameter_values": parameter_values,
         }
         combined = Options._merge_options(self._options, run_options)
-
+        Sampler._validate_options(combined)
         inputs.update(Options._get_program_inputs(combined))
 
         raw_result = self._session.run(
             program_id=self._PROGRAM_ID,
             inputs=inputs,
             options=Options._get_runtime_options(combined),
         ).result()
@@ -360,7 +368,26 @@
     def set_options(self, **fields: Any) -> None:
         """Set options values for the sampler.
 
         Args:
             **fields: The fields to update the options
         """
         self._options = Options._merge_options(self._options, fields)
+
+    @staticmethod
+    def _validate_options(options: dict) -> None:
+        """Validate that program inputs (options) are valid
+        Raises:
+            ValueError: if resilience_level is out of the allowed range.
+        """
+        if os.getenv("QISKIT_RUNTIME_SKIP_OPTIONS_VALIDATION"):
+            return
+
+        if options.get("resilience_level") and not options.get("resilience_level") in [
+            0,
+            1,
+        ]:
+            raise ValueError(
+                f"resilience_level can only take the values "
+                f"{list(range(Options._MAX_RESILIENCE_LEVEL_SAMPLER + 1))} in Sampler"
+            )
+        Options.validate_options(options)
```

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/session.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/__init__.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/backend_converter.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/backend_converter.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/backend_decoder.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/backend_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/converters.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/converters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/deprecation.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/estimator_result_decoder.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/estimator_result_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/hgp.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/hgp.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/json.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/json.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/runner_result.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/runner_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/sampler_result_decoder.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/sampler_result_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/utils/utils.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime/version.py` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime.egg-info/PKG-INFO` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-runtime
-Version: 0.9.2
+Version: 0.9.3
 Summary: IBM Quantum client for Qiskit Runtime.
 Home-page: https://github.com/Qiskit/qiskit-ibm-runtime
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-runtime/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-runtime-0.9.2/qiskit_ibm_runtime.egg-info/SOURCES.txt` & `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -129,20 +129,21 @@
 test/unit/test_estimator.py
 test/unit/test_ibm_primitives.py
 test/unit/test_job_retrieval.py
 test/unit/test_jobs.py
 test/unit/test_logger.py
 test/unit/test_options.py
 test/unit/test_programs.py
+test/unit/test_runtime_client.py
 test/unit/test_runtime_ws.py
 test/unit/test_sampler.py
 test/unit/test_session.py
 test/unit/test_utils_converters.py
 test/unit/mock/__init__.py
-test/unit/mock/fake_account_client.py
+test/unit/mock/fake_api_backend.py
 test/unit/mock/fake_quantum_auth_client.py
 test/unit/mock/fake_runtime_client.py
 test/unit/mock/fake_runtime_service.py
 test/unit/mock/http_server.py
 test/unit/mock/proxy_server.py
 test/unit/mock/ws_handler.py
 test/unit/mock/ws_server.py
```

### Comparing `qiskit-ibm-runtime-0.9.2/setup.py` & `qiskit-ibm-runtime-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/__init__.py` & `qiskit-ibm-runtime-0.9.3/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/account.py` & `qiskit-ibm-runtime-0.9.3/test/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/decorators.py` & `qiskit-ibm-runtime-0.9.3/test/decorators.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/e2e/test_tutorials.py` & `qiskit-ibm-runtime-0.9.3/test/e2e/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/ibm_test_case.py` & `qiskit-ibm-runtime-0.9.3/test/ibm_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/integration/test_account.py` & `qiskit-ibm-runtime-0.9.3/test/integration/test_account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/integration/test_auth_client.py` & `qiskit-ibm-runtime-0.9.3/test/integration/test_auth_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/integration/test_backend.py` & `qiskit-ibm-runtime-0.9.3/test/integration/test_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/integration/test_backend_serialization.py` & `qiskit-ibm-runtime-0.9.3/test/integration/test_backend_serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/integration/test_basic_server_paths.py` & `qiskit-ibm-runtime-0.9.3/test/integration/test_basic_server_paths.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/integration/test_estimator.py` & `qiskit-ibm-runtime-0.9.3/test/integration/test_estimator.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/integration/test_job.py` & `qiskit-ibm-runtime-0.9.3/test/integration/test_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/integration/test_options.py` & `qiskit-ibm-runtime-0.9.3/test/integration/test_options.py`

 * *Files 13% similar despite different names*

```diff
@@ -94,7 +94,22 @@
 
                     estimator = Estimator(options=opt)
                     job2 = estimator.run(circ, observables=obs)
                     with self.assertRaises(RuntimeJobFailureError):
                         job2.result()
                     # TODO: Re-enable when ntc-1651 is fixed
                     # self.assertIn("TranspilerError", err.exception.message)
+
+    @run_integration_test
+    def test_unsupported_input_combinations(self, service):
+        """Test that when resilience_level==3, and backend is a simulator,
+        a coupling map is required."""
+        circ = QuantumCircuit(1)
+        obs = SparsePauliOp.from_list([("I", 1)])
+        options = Options()
+        options.resilience_level = 3
+        backend = service.backends(simulator=True)[0]
+        with Session(service=service, backend=backend) as session:
+            with self.assertRaises(ValueError) as exc:
+                inst = Estimator(session=session, options=options)
+                inst.run(circ, observables=obs)
+            self.assertIn("a coupling map is required.", str(exc.exception))
```

### Comparing `qiskit-ibm-runtime-0.9.2/test/integration/test_program.py` & `qiskit-ibm-runtime-0.9.3/test/integration/test_program.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/integration/test_proxies.py` & `qiskit-ibm-runtime-0.9.3/test/integration/test_proxies.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             token=dependencies.token,
             url=dependencies.url,
             proxies={"urls": VALID_PROXIES},
         )
         service.programs(limit=1)
 
         auth_line = pproxy_desired_access_log_line(dependencies.url)
-        api_line = list(service._hgps.values())[0]._api_client._session.base_url
+        api_line = list(service._hgps.values())[0]._runtime_client._session.base_url
         api_line = pproxy_desired_access_log_line(api_line)
         self.proxy_process.terminate()  # kill to be able of reading the output
         proxy_output = self.proxy_process.stdout.read().decode("utf-8")
 
         # Check if the authentication call went through proxy.
         self.assertIn(auth_line, proxy_output)
         # Check if the API call (querying providers list) went through proxy.
@@ -105,15 +105,15 @@
             url=dependencies.url,
             proxies={"urls": VALID_PROXIES},
         )
 
         self.proxy_process.terminate()  # kill to be able of reading the output
 
         auth_line = pproxy_desired_access_log_line(dependencies.url)
-        api_line = list(service._hgps.values())[0]._api_client._session.base_url
+        api_line = list(service._hgps.values())[0]._runtime_client._session.base_url
         api_line = pproxy_desired_access_log_line(api_line)
         proxy_output = self.proxy_process.stdout.read().decode("utf-8")
 
         # Check if the authentication call went through proxy.
         self.assertIn(auth_line, proxy_output)
         # Check if the API call (querying providers list) went through proxy.
         self.assertIn(api_line, proxy_output)
```

### Comparing `qiskit-ibm-runtime-0.9.2/test/integration/test_results.py` & `qiskit-ibm-runtime-0.9.3/test/integration/test_results.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/integration/test_retrieve_job.py` & `qiskit-ibm-runtime-0.9.3/test/integration/test_retrieve_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/integration/test_sampler.py` & `qiskit-ibm-runtime-0.9.3/test/integration/test_sampler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/integration/test_session.py` & `qiskit-ibm-runtime-0.9.3/test/integration/test_session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/program.py` & `qiskit-ibm-runtime-0.9.3/test/program.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/serialization.py` & `qiskit-ibm-runtime-0.9.3/test/serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/templates.py` & `qiskit-ibm-runtime-0.9.3/test/templates.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/mock/fake_quantum_auth_client.py` & `qiskit-ibm-runtime-0.9.3/test/unit/mock/fake_quantum_auth_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/mock/fake_runtime_client.py` & `qiskit-ibm-runtime-0.9.3/test/unit/mock/fake_runtime_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,33 +14,21 @@
 
 import base64
 import json
 import time
 import uuid
 from datetime import timezone, datetime as python_datetime
 from concurrent.futures import ThreadPoolExecutor
-from functools import wraps
 from typing import Optional, Dict, Any, List
 
 from qiskit_ibm_runtime.api.exceptions import RequestsApiError
 from qiskit_ibm_runtime.utils import RuntimeEncoder
 from qiskit_ibm_runtime.utils.hgp import from_instance_format
-from .fake_account_client import BaseFakeAccountClient
 
-
-def cloud_only(func):
-    """Decorator that runs a test using only ibm_cloud services."""
-
-    @wraps(func)
-    def _wrapper(self, *args, **kwargs):
-        if self._channel != "ibm_cloud":
-            raise ValueError(f"Method {func} called by an ibm_quantum client!")
-        return func(self, *args, **kwargs)
-
-    return _wrapper
+from .fake_api_backend import FakeApiBackend, FakeApiBackendSpecs
 
 
 class BaseFakeProgram:
     """Base class for faking a program."""
 
     def __init__(
         self,
@@ -258,29 +246,42 @@
         if self._status == "COMPLETED":
             self._result = json.dumps("foo")
 
 
 class BaseFakeRuntimeClient:
     """Base class for faking the runtime client."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(
+        self,
+        job_classes=None,
+        final_status=None,
+        job_kwargs=None,
+        backend_client=None,
+        channel="ibm_quantum",
+        num_backends=2,
+        backend_specs=None,
+    ):
         """Initialize a fake runtime client."""
         # pylint: disable=unused-argument
-        test_options = kwargs.pop("test_options", {})
         self._programs = {}
         self._jobs = {}
-        self._job_classes = test_options.get("job_classes", [])
-        self._final_status = test_options.get("final_status")
-        self._job_kwargs = test_options.get("job_kwargs", {})
-        self._backend_client = test_options.get(
-            "backend_client", BaseFakeAccountClient()
-        )
-        self._channel = test_options.get("channel", "ibm_quantum")
+        self._job_classes = job_classes or []
+        self._final_status = final_status
+        self._job_kwargs = job_kwargs or {}
+        self._channel = channel
         self.session_time = 0
 
+        # Setup the available backends
+        if not backend_specs:
+            backend_specs = [
+                FakeApiBackendSpecs(backend_name=f"backend{idx}")
+                for idx in range(num_backends)
+            ]
+        self._backends = [FakeApiBackend(specs) for specs in backend_specs]
+
     def set_job_classes(self, classes):
         """Set job classes to use."""
         if not isinstance(classes, list):
             classes = [classes]
         self._job_classes = classes
 
     def set_final_status(self, final_status):
@@ -513,41 +514,36 @@
 
     def _get_job(self, job_id):
         """Get job."""
         if job_id not in self._jobs:
             raise RequestsApiError("Job not found", status_code=404)
         return self._jobs[job_id]
 
-    @cloud_only
-    def list_backends(self):
-        """Return IBM Cloud backends"""
-        self._check_cloud_only()
-        return self._backend_client.backend_names
+    def list_backends(self, hgp: Optional[str] = None) -> List[str]:
+        """Return IBM backends available for this service instance."""
+        return [back.name for back in self._backends if back.has_access(hgp)]
 
-    @cloud_only
     def backend_configuration(self, backend_name: str) -> Dict[str, Any]:
-        """Return the configuration of the IBM Cloud backend."""
-        return self._backend_client.backend_configuration(backend_name)
+        """Return the configuration a backend."""
+        return self._find_backend(backend_name).configuration
 
-    @cloud_only
     def backend_status(self, backend_name: str) -> Dict[str, Any]:
-        """Return the status of the IBM Cloud backend."""
-        return self._backend_client.backend_status(backend_name)
+        """Return the status of a backend."""
+        return self._find_backend(backend_name).status
 
-    @cloud_only
     def backend_properties(
         self, backend_name: str, datetime: Any = None
     ) -> Dict[str, Any]:
-        """Return the properties of the IBM Cloud backend."""
+        """Return the properties of a backend."""
         if datetime:
-            raise NotImplementedError("'datetime' is not supported with cloud runtime.")
-        return self._backend_client.backend_properties(backend_name)
+            raise NotImplementedError("'datetime' is not supported.")
+        return self._find_backend(backend_name).properties
 
-    @cloud_only
     def backend_pulse_defaults(self, backend_name: str) -> Dict[str, Any]:
-        """Return the pulse defaults of the IBM Cloud backend."""
-        return self._backend_client.backend_pulse_defaults(backend_name)
+        """Return the pulse defaults of a backend."""
+        return self._find_backend(backend_name).defaults
 
-    @cloud_only
-    def _check_cloud_only(self):
-        if self._channel != "ibm_cloud":
-            raise ValueError("A backend method is called by an ibm_quantum client!")
+    def _find_backend(self, backend_name):
+        for back in self._backends:
+            if back.name == backend_name:
+                return back
+        raise ValueError(f"Backend {backend_name} not found")
```

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/mock/http_server.py` & `qiskit-ibm-runtime-0.9.3/test/unit/mock/http_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/mock/proxy_server.py` & `qiskit-ibm-runtime-0.9.3/test/unit/mock/proxy_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/mock/ws_handler.py` & `qiskit-ibm-runtime-0.9.3/test/unit/mock/ws_handler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/mock/ws_server.py` & `qiskit-ibm-runtime-0.9.3/test/unit/mock/ws_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/test_account.py` & `qiskit-ibm-runtime-0.9.3/test/unit/test_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -922,14 +922,15 @@
         name = "foo"
         instance = uuid.uuid4().hex
         with temporary_account_config_file(name=name, instance="stored-instance"):
             service = FakeRuntimeService(name=name, instance=instance)
         self.assertTrue(service._account)
         self.assertEqual(service._account.instance, instance)
 
+    @no_envs(["QISKIT_IBM_TOKEN"])
     def test_enable_account_by_qiskitrc(self):
         """Test initializing account by a qiskitrc file."""
         token = "token-x"
         proxies = {"urls": {"https": "localhost:8080"}}
         str_contents = f"""
         [ibmq]
         token = {token}
```

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/test_backend_retrieval.py` & `qiskit-ibm-runtime-0.9.3/test/unit/test_backend_retrieval.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Backends Filtering Test."""
 
+import uuid
+
 from qiskit.providers.exceptions import QiskitBackendNotFoundError
 from qiskit.providers.fake_provider import FakeLima
 
-from .mock.fake_account_client import BaseFakeAccountClient
 from .mock.fake_runtime_service import FakeRuntimeService
+from .mock.fake_api_backend import FakeApiBackendSpecs
 from ..ibm_test_case import IBMTestCase
 from ..decorators import run_quantum_and_cloud_fake
 
 
 class TestBackendFilters(IBMTestCase):
     """Qiskit Backend Filtering Tests."""
 
@@ -47,23 +49,23 @@
         service = FakeRuntimeService(channel="ibm_quantum", token="my_token")
         for hgp in FakeRuntimeService.DEFAULT_HGPS:
             with self.subTest(hgp=hgp):
                 backends = service.backends(instance=hgp)
                 backend_name = [back.name for back in backends]
                 self.assertEqual(len(backend_name), 2)
                 for back in backends:
-                    self.assertEqual(back._api_client.hgp, hgp)
+                    self.assertEqual(back._instance, hgp)
 
     def test_filter_config_properties(self):
         """Test filtering by configuration properties."""
         n_qubits = 5
         fake_backends = [
-            self._get_specs(n_qubits=n_qubits, local=False),
-            self._get_specs(n_qubits=n_qubits * 2, local=False),
-            self._get_specs(n_qubits=n_qubits, local=True),
+            self._get_fake_backend_specs(n_qubits=n_qubits, local=False),
+            self._get_fake_backend_specs(n_qubits=n_qubits * 2, local=False),
+            self._get_fake_backend_specs(n_qubits=n_qubits, local=True),
         ]
 
         services = self._get_services(fake_backends)
         for service in services:
             with self.subTest(service=service.channel):
                 filtered_backends = service.backends(n_qubits=n_qubits, local=False)
                 self.assertTrue(len(filtered_backends), 1)
@@ -71,18 +73,18 @@
                     n_qubits, filtered_backends[0].configuration().n_qubits
                 )
                 self.assertFalse(filtered_backends[0].configuration().local)
 
     def test_filter_status_dict(self):
         """Test filtering by dictionary of mixed status/configuration properties."""
         fake_backends = [
-            self._get_specs(operational=True, simulator=True),
-            self._get_specs(operational=True, simulator=True),
-            self._get_specs(operational=True, simulator=False),
-            self._get_specs(operational=False, simulator=False),
+            self._get_fake_backend_specs(operational=True, simulator=True),
+            self._get_fake_backend_specs(operational=True, simulator=True),
+            self._get_fake_backend_specs(operational=True, simulator=False),
+            self._get_fake_backend_specs(operational=False, simulator=False),
         ]
 
         services = self._get_services(fake_backends)
         for service in services:
             with self.subTest(service=service.channel):
                 filtered_backends = service.backends(
                     operational=True,  # from status
@@ -93,17 +95,17 @@
                     self.assertTrue(backend.status().operational)
                     self.assertTrue(backend.configuration().simulator)
 
     def test_filter_config_callable(self):
         """Test filtering by lambda function on configuration properties."""
         n_qubits = 5
         fake_backends = [
-            self._get_specs(n_qubits=n_qubits),
-            self._get_specs(n_qubits=n_qubits * 2),
-            self._get_specs(n_qubits=n_qubits - 1),
+            self._get_fake_backend_specs(n_qubits=n_qubits),
+            self._get_fake_backend_specs(n_qubits=n_qubits * 2),
+            self._get_fake_backend_specs(n_qubits=n_qubits - 1),
         ]
 
         services = self._get_services(fake_backends)
         for service in services:
             with self.subTest(service=service.channel):
                 filtered_backends = service.backends(
                     filters=lambda x: (x.configuration().n_qubits >= 5)
@@ -112,128 +114,138 @@
                 for backend in filtered_backends:
                     self.assertGreaterEqual(backend.configuration().n_qubits, n_qubits)
 
     def test_filter_least_busy(self):
         """Test filtering by least busy function."""
         default_stat = {"pending_jobs": 1, "operational": True, "status_msg": "active"}
         fake_backends = [
-            self._get_specs(
+            self._get_fake_backend_specs(
                 **{**default_stat, "backend_name": "bingo", "pending_jobs": 5}
             ),
-            self._get_specs(**{**default_stat, "pending_jobs": 7}),
-            self._get_specs(**{**default_stat, "operational": False}),
-            self._get_specs(**{**default_stat, "status_msg": "internal"}),
+            self._get_fake_backend_specs(**{**default_stat, "pending_jobs": 7}),
+            self._get_fake_backend_specs(**{**default_stat, "operational": False}),
+            self._get_fake_backend_specs(**{**default_stat, "status_msg": "internal"}),
         ]
 
         services = self._get_services(fake_backends)
         for service in services:
             with self.subTest(service=service.channel):
                 backend = service.least_busy()
                 self.assertEqual(backend.name, "bingo")
 
     def test_filter_min_num_qubits(self):
         """Test filtering by minimum number of qubits."""
         n_qubits = 5
         fake_backends = [
-            self._get_specs(n_qubits=n_qubits),
-            self._get_specs(n_qubits=n_qubits * 2),
-            self._get_specs(n_qubits=n_qubits - 1),
+            self._get_fake_backend_specs(n_qubits=n_qubits),
+            self._get_fake_backend_specs(n_qubits=n_qubits * 2),
+            self._get_fake_backend_specs(n_qubits=n_qubits - 1),
         ]
 
         services = self._get_services(fake_backends)
         for service in services:
             with self.subTest(service=service.channel):
                 filtered_backends = service.backends(min_num_qubits=n_qubits)
                 self.assertTrue(len(filtered_backends), 2)
                 for backend in filtered_backends:
                     self.assertGreaterEqual(backend.configuration().n_qubits, n_qubits)
 
     def test_filter_by_hgp(self):
         """Test filtering by hub/group/project."""
         num_backends = 3
-        test_options = {
-            "account_client": BaseFakeAccountClient(num_backends=num_backends),
-            "num_hgps": 2,
-        }
+        hgp_name = "hub0/group0/project0"
+        hgp_backend_specs = [
+            self._get_fake_backend_specs(hgps=[hgp_name]) for _ in range(num_backends)
+        ]
+        all_backend_specs = hgp_backend_specs + [
+            self._get_fake_backend_specs(hgps=["hub1/group1/project1"])
+        ]
         ibm_quantum_service = FakeRuntimeService(
             channel="ibm_quantum",
             token="my_token",
             instance="h/g/p",
-            test_options=test_options,
+            num_hgps=2,
+            backend_specs=all_backend_specs,
         )
         backends = ibm_quantum_service.backends(instance="hub0/group0/project0")
         self.assertEqual(len(backends), num_backends)
-
-    def _get_specs(self, **kwargs):
-        """Get the backend specs to pass to the fake account client."""
-        specs = {"configuration": {}, "status": {}}
+        right_names = {spec.backend_name for spec in hgp_backend_specs}
+        got_names = {back.name for back in backends}
+        self.assertEqual(right_names, got_names)
+
+    def _get_fake_backend_specs(self, hgps=None, **kwargs):
+        """Get the backend specs to pass to the fake client."""
+        config = {}
+        status = {}
         status_keys = FakeLima().status().to_dict()
         status_keys.pop("backend_name")  # name is in both config and status
         status_keys = list(status_keys.keys())
         for key, val in kwargs.items():
             if key in status_keys:
-                specs["status"][key] = val
+                status[key] = val
             else:
-                specs["configuration"][key] = val
-        return specs
+                config[key] = val
+        name = config.get("backend_name", uuid.uuid4().hex)
+        return FakeApiBackendSpecs(
+            backend_name=name, configuration=config, status=status, hgps=hgps
+        )
 
-    def _get_services(self, fake_backends):
+    def _get_services(self, fake_backend_specs):
         """Get both ibm_cloud and ibm_quantum services initialized with fake backends."""
-        test_options = {"account_client": BaseFakeAccountClient(specs=fake_backends)}
         ibm_quantum_service = FakeRuntimeService(
             channel="ibm_quantum",
             token="my_token",
             instance="h/g/p",
-            test_options=test_options,
+            backend_specs=fake_backend_specs,
         )
         cloud_service = FakeRuntimeService(
             channel="ibm_cloud",
             token="my_token",
             instance="my_instance",
-            test_options=test_options,
+            backend_specs=fake_backend_specs,
         )
         return [ibm_quantum_service, cloud_service]
 
 
 class TestGetBackend(IBMTestCase):
     """Test getting a backend via ibm_quantum api."""
 
     def test_get_common_backend(self):
         """Test getting a backend that is in default and non-default hgp."""
         service = FakeRuntimeService(channel="ibm_quantum", token="my_token")
         backend = service.backend(FakeRuntimeService.DEFAULT_COMMON_BACKEND)
-        self.assertEqual(backend._api_client.hgp, list(service._hgps.keys())[0])
+        self.assertEqual(backend._instance, list(service._hgps.keys())[0])
 
     def test_get_unique_backend_default_hgp(self):
         """Test getting a backend in the default hgp."""
         service = FakeRuntimeService(channel="ibm_quantum", token="my_token")
         backend_name = FakeRuntimeService.DEFAULT_UNIQUE_BACKEND_PREFIX + "0"
         backend = service.backend(backend_name)
-        self.assertEqual(backend._api_client.hgp, list(service._hgps.keys())[0])
+        self.assertEqual(backend._instance, list(service._hgps.keys())[0])
 
     def test_get_unique_backend_non_default_hgp(self):
         """Test getting a backend in the non default hgp."""
         service = FakeRuntimeService(channel="ibm_quantum", token="my_token")
         backend_name = FakeRuntimeService.DEFAULT_UNIQUE_BACKEND_PREFIX + "1"
         backend = service.backend(backend_name)
-        self.assertEqual(backend._api_client.hgp, list(service._hgps.keys())[1])
+        self.assertEqual(backend._instance, list(service._hgps.keys())[1])
 
     def test_get_phantom_backend(self):
         """Test getting a phantom backend."""
         service = FakeRuntimeService(channel="ibm_quantum", token="my_token")
         with self.assertRaises(QiskitBackendNotFoundError):
             service.backend("phantom")
 
     def test_get_backend_by_hgp(self):
         """Test getting a backend by hgp."""
         hgp = FakeRuntimeService.DEFAULT_HGPS[1]
         backend_name = FakeRuntimeService.DEFAULT_COMMON_BACKEND
         service = FakeRuntimeService(channel="ibm_quantum", token="my_token")
         backend = service.backend(backend_name, instance=hgp)
-        self.assertEqual(backend._api_client.hgp, hgp)
+        self.assertEqual(backend._instance, hgp)
 
     def test_get_backend_by_bad_hgp(self):
         """Test getting a backend not in hgp."""
         hgp = FakeRuntimeService.DEFAULT_HGPS[1]
         backend_name = FakeRuntimeService.DEFAULT_UNIQUE_BACKEND_PREFIX + "0"
         service = FakeRuntimeService(channel="ibm_quantum", token="my_token")
         with self.assertRaises(QiskitBackendNotFoundError):
```

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/test_client_parameters.py` & `qiskit-ibm-runtime-0.9.3/test/unit/test_client_parameters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/test_data_serialization.py` & `qiskit-ibm-runtime-0.9.3/test/unit/test_data_serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/test_estimator.py` & `qiskit-ibm-runtime-0.9.3/test/unit/test_estimator.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 """Tests for estimator class."""
 
 import unittest
 import json
 from unittest.mock import patch
 
+from qiskit import QuantumCircuit
 from qiskit.circuit.library import RealAmplitudes
 from qiskit.quantum_info import SparsePauliOp
 from qiskit.primitives.utils import _circuit_key
 
 from qiskit_ibm_runtime.utils.json import RuntimeEncoder
 from qiskit_ibm_runtime.utils.utils import _hash
 from qiskit_ibm_runtime import Estimator, Session
@@ -78,7 +79,25 @@
 
             with patch.object(estimator._session, "run") as mock_run:
                 estimator.run([psi4, psi1], [H2, H1], [[1] * 8, [1] * 6])
                 _, kwargs = mock_run.call_args
                 inputs = kwargs["inputs"]
                 self.assertDictEqual(inputs["circuits"], {psi4_id: psi4})
                 self.assertEqual(inputs["circuit_ids"], [psi4_id, psi1_id])
+
+    def test_unsupported_values_for_estimator_options(self):
+        """Test exception when options levels are not supported."""
+        options_bad = [
+            {"resilience_level": 4, "optimization_level": 3},
+            {"optimization_level": 4, "resilience_level": 3},
+        ]
+        with Session(
+            service=FakeRuntimeService(channel="ibm_quantum", token="abc"),
+            backend="common_backend",
+        ) as session:
+            circuit = QuantumCircuit(1, 1)
+            obs = SparsePauliOp.from_list([("I", 1)])
+            for bad_opt in options_bad:
+                inst = Estimator(session=session)
+                with self.assertRaises(ValueError) as exc:
+                    _ = inst.run(circuit, observables=obs, **bad_opt)
+                self.assertIn(list(bad_opt.keys())[0], str(exc.exception))
```

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/test_job_retrieval.py` & `qiskit-ibm-runtime-0.9.3/test/unit/test_job_retrieval.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/test_jobs.py` & `qiskit-ibm-runtime-0.9.3/test/unit/test_jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,47 +88,45 @@
         self.assertTrue(job.backend())
 
     def test_run_program_default_hgp_backend(self):
         """Test running a program with a backend in default hgp."""
         service = FakeRuntimeService(channel="ibm_quantum", token="my_token")
         backend = FakeRuntimeService.DEFAULT_COMMON_BACKEND
         default_hgp = list(service._hgps.values())[0]
-        self.assertIn(backend, default_hgp.backends.keys())
+        self.assertIn(backend, default_hgp.backends)
         job = run_program(service=service, backend_name=backend)
         self.assertEqual(job.backend().name, backend)
-        self.assertEqual(
-            job.backend()._api_client.hgp, FakeRuntimeService.DEFAULT_HGPS[0]
-        )
+        self.assertEqual(job.backend()._instance, FakeRuntimeService.DEFAULT_HGPS[0])
 
     def test_run_program_non_default_hgp_backend(self):
         """Test running a program with a backend in non-default hgp."""
         service = FakeRuntimeService(channel="ibm_quantum", token="my_token")
         backend = FakeRuntimeService.DEFAULT_UNIQUE_BACKEND_PREFIX + "1"
         default_hgp = list(service._hgps.values())[0]
-        self.assertNotIn(backend, default_hgp.backends.keys())
+        self.assertNotIn(backend, default_hgp.backends)
         job = run_program(service=service, backend_name=backend)
         self.assertEqual(job.backend().name, backend)
 
     def test_run_program_by_hgp_backend(self):
         """Test running a program with both backend and hgp."""
         service = FakeRuntimeService(channel="ibm_quantum", token="my_token")
         backend = FakeRuntimeService.DEFAULT_COMMON_BACKEND
         non_default_hgp = list(service._hgps.keys())[1]
         job = run_program(
             service=service, backend_name=backend, instance=non_default_hgp
         )
         self.assertEqual(job.backend().name, backend)
-        self.assertEqual(job.backend()._api_client.hgp, non_default_hgp)
+        self.assertEqual(job.backend()._instance, non_default_hgp)
 
     def test_run_program_by_hgp_bad_backend(self):
         """Test running a program with backend not in hgp."""
         service = FakeRuntimeService(channel="ibm_quantum", token="my_token")
         backend = FakeRuntimeService.DEFAULT_UNIQUE_BACKEND_PREFIX + "1"
         default_hgp = list(service._hgps.values())[0]
-        self.assertNotIn(backend, default_hgp.backends.keys())
+        self.assertNotIn(backend, default_hgp.backends)
         with self.assertRaises(QiskitBackendNotFoundError):
             _ = run_program(
                 service=service, backend_name=backend, instance=default_hgp.name
             )
 
     def test_run_program_by_phantom_hgp(self):
         """Test running a program with a phantom hgp."""
```

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/test_logger.py` & `qiskit-ibm-runtime-0.9.3/test/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/test_options.py` & `qiskit-ibm-runtime-0.9.3/test/unit/test_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,16 @@
             {"resilience_level": 9},
             {"simulator": {"seed_simulator": 42}},
             {"resilience_level": 8, "environment": {"log_level": "WARNING"}},
             {
                 "transpilation": {"initial_layout": [1, 2], "layout_method": "trivial"},
                 "execution": {"shots": 100},
             },
+            {"resilience": {"noise_amplifier": "GlobalFoldingAmplifier"}},
+            {"environment": {"log_level": "ERROR"}},
         ]
 
         for opts_dict in options_dicts:
             with self.subTest(opts_dict=opts_dict):
                 options = asdict(Options(**opts_dict))
                 self.assertTrue(
                     dict_paritally_equal(options, opts_dict),
```

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/test_programs.py` & `qiskit-ibm-runtime-0.9.3/test/unit/test_programs.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/test_runtime_ws.py` & `qiskit-ibm-runtime-0.9.3/test/unit/test_runtime_ws.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/test_sampler.py` & `qiskit-ibm-runtime-0.9.3/test/unit/test_sampler.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 """Tests for sampler class."""
 
 import json
 from unittest.mock import patch
 import unittest
 
+from qiskit.circuit import QuantumCircuit
 from qiskit.circuit.library import RealAmplitudes
 from qiskit.primitives.utils import _circuit_key
 
 from qiskit_ibm_runtime.utils.json import RuntimeEncoder
 from qiskit_ibm_runtime.utils.utils import _hash
 from qiskit_ibm_runtime import Sampler, Session
 
@@ -75,7 +76,24 @@
 
             with patch.object(sampler._session, "run") as mock_run:
                 sampler.run([pqc4, pqc], [[1] * 8, [1] * 6])
                 _, kwargs = mock_run.call_args
                 inputs = kwargs["inputs"]
                 self.assertDictEqual(inputs["circuits"], {pqc4_id: pqc4})
                 self.assertEqual(inputs["circuit_ids"], [pqc4_id, pqc_id])
+
+    def test_unsupported_values_for_sampler_options(self):
+        """Test exception when options levels are not supported."""
+        options_bad = [
+            {"resilience_level": 2, "optimization_level": 3},
+            {"optimization_level": 4, "resilience_level": 1},
+        ]
+        with Session(
+            service=FakeRuntimeService(channel="ibm_quantum", token="abc"),
+            backend="common_backend",
+        ) as session:
+            circuit = QuantumCircuit(1, 1)
+            for bad_opt in options_bad:
+                inst = Sampler(session=session)
+                with self.assertRaises(ValueError) as exc:
+                    _ = inst.run(circuit, **bad_opt)
+                self.assertIn(list(bad_opt.keys())[0], str(exc.exception))
```

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/test_session.py` & `qiskit-ibm-runtime-0.9.3/test/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/unit/test_utils_converters.py` & `qiskit-ibm-runtime-0.9.3/test/unit/test_utils_converters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.2/test/utils.py` & `qiskit-ibm-runtime-0.9.3/test/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,19 +13,22 @@
 """General utility functions for testing."""
 
 import os
 import logging
 import time
 import unittest
 from unittest import mock
-from typing import Dict
+from typing import Dict, Optional
+from datetime import datetime
 
 from qiskit.circuit import QuantumCircuit
 from qiskit.providers.jobstatus import JOB_FINAL_STATES, JobStatus
 from qiskit.providers.exceptions import QiskitBackendNotFoundError
+from qiskit.providers.models import BackendStatus, BackendProperties
+from qiskit.providers.backend import Backend
 from qiskit_ibm_runtime.hub_group_project import HubGroupProject
 from qiskit_ibm_runtime import QiskitRuntimeService
 from qiskit_ibm_runtime.ibm_backend import IBMBackend
 from qiskit_ibm_runtime.runtime_job import RuntimeJob
 from qiskit_ibm_runtime.exceptions import RuntimeInvalidStateError
 
 
@@ -190,7 +193,61 @@
         if key not in dict2:
             return False
         if isinstance(val, dict):
             if not dict_keys_equal(val, dict2[key]):
                 return False
 
     return True
+
+
+def create_faulty_backend(
+    model_backend: Backend,
+    faulty_qubit: Optional[int] = None,
+    faulty_edge: Optional[tuple] = None,
+) -> IBMBackend:
+    """Create an IBMBackend that has faulty qubits and/or edges.
+
+    Args:
+        model_backend: Fake backend to model after.
+        faulty_qubit: Faulty qubit.
+        faulty_edge: Faulty edge, a tuple of (gate, qubits)
+
+    Returns:
+        An IBMBackend with faulty qubits/edges.
+    """
+
+    properties = model_backend.properties().to_dict()
+
+    if faulty_qubit:
+        properties["qubits"][faulty_qubit].append(
+            {"date": datetime.now(), "name": "operational", "unit": "", "value": 0}
+        )
+
+    if faulty_edge:
+        gate, qubits = faulty_edge
+        for gate_obj in properties["gates"]:
+            if gate_obj["gate"] == gate and gate_obj["qubits"] == qubits:
+                gate_obj["parameters"].append(
+                    {
+                        "date": datetime.now(),
+                        "name": "operational",
+                        "unit": "",
+                        "value": 0,
+                    }
+                )
+
+    out_backend = IBMBackend(
+        configuration=model_backend.configuration(),
+        service=mock.MagicMock(),
+        api_client=None,
+        instance=None,
+    )
+
+    out_backend.status = lambda: BackendStatus(  # type: ignore[assignment]
+        backend_name="foo",
+        backend_version="1.0",
+        operational=True,
+        pending_jobs=0,
+        status_msg="",
+    )
+    out_backend.properties = lambda: BackendProperties.from_dict(properties)  # type: ignore
+    return out_backend
```

