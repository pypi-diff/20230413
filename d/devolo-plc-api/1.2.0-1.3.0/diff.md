# Comparing `tmp/devolo_plc_api-1.2.0.tar.gz` & `tmp/devolo_plc_api-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devolo_plc_api-1.2.0.tar", last modified: Fri Feb 17 12:26:10 2023, max compression
+gzip compressed data, was "devolo_plc_api-1.3.0.tar", last modified: Thu Apr 13 13:15:23 2023, max compression
```

## Comparing `devolo_plc_api-1.2.0.tar` & `devolo_plc_api-1.3.0.tar`

### file list

```diff
@@ -1,99 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.134261 devolo_plc_api-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.126260 devolo_plc_api-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.126260 devolo_plc_api-1.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.126260 devolo_plc_api-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/.github/workflows/convert_todos_to_issues.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44988 2023-02-17 12:26:10.134261 devolo_plc_api-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.126260 devolo_plc_api-1.2.0/devolo_plc_api/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.126260 devolo_plc_api-1.2.0/devolo_plc_api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/clients/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.130261 devolo_plc_api-1.2.0/devolo_plc_api/device_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11865 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device_api/deviceapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device_api/deviceapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device_api/factoryreset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device_api/factoryreset_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device_api/ledsettings_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device_api/ledsettings_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device_api/restart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device_api/restart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device_api/support_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device_api/support_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device_api/updatefirmware_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device_api/updatefirmware_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device_api/wifinetwork_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/device_api/wifinetwork_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.130261 devolo_plc_api-1.2.0/devolo_plc_api/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/exceptions/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/exceptions/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.130261 devolo_plc_api-1.2.0/devolo_plc_api/network/
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.130261 devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/identifydevice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/pairdevice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/plcnetapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/plcnetapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.130261 devolo_plc_api-1.2.0/devolo_plc_api/zeroconf/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/devolo_plc_api/zeroconf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.126260 devolo_plc_api-1.2.0/devolo_plc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44988 2023-02-17 12:26:10.000000 devolo_plc_api-1.2.0/devolo_plc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-02-17 12:26:10.000000 devolo_plc_api-1.2.0/devolo_plc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 12:26:10.000000 devolo_plc_api-1.2.0/devolo_plc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-17 12:26:10.000000 devolo_plc_api-1.2.0/devolo_plc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-17 12:26:10.000000 devolo_plc_api-1.2.0/devolo_plc_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.130261 devolo_plc_api-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/example_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/example_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.130261 devolo_plc_api-1.2.0/script/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4250 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/script/stubgen.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 12:26:10.134261 devolo_plc_api-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.134261 devolo_plc_api-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.134261 devolo_plc_api-1.2.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/fixtures/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/fixtures/device_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/fixtures/plcnet_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/fixtures/protobuf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.134261 devolo_plc_api-1.2.0/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/mocks/mock_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/mocks/mock_zeroconf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:26:10.134261 devolo_plc_api-1.2.0/tests/stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/stubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/stubs/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/stubs/zeroconf.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/test_data.json
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    15151 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/test_deviceapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/test_plcnetapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-02-17 12:25:48.000000 devolo_plc_api-1.2.0/tests/test_profobuf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.237554 devolo_plc_api-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.225554 devolo_plc_api-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.225554 devolo_plc_api-1.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.225554 devolo_plc_api-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.github/workflows/convert_todos_to_issues.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44988 2023-04-13 13:15:23.237554 devolo_plc_api-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.225554 devolo_plc_api-1.3.0/devolo_plc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.225554 devolo_plc_api-1.3.0/devolo_plc_api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/clients/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.229554 devolo_plc_api-1.3.0/devolo_plc_api/device_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12415 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/deviceapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/deviceapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/factoryreset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/factoryreset_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/ledsettings_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/ledsettings_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/multiap_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/multiap_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/restart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/restart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/support_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/support_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/updatefirmware_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/updatefirmware_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/wifinetwork_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/wifinetwork_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.229554 devolo_plc_api-1.3.0/devolo_plc_api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/exceptions/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/exceptions/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.229554 devolo_plc_api-1.3.0/devolo_plc_api/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.233554 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/identifydevice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/pairdevice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/plcnetapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/plcnetapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.233554 devolo_plc_api-1.3.0/devolo_plc_api/zeroconf/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/zeroconf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.225554 devolo_plc_api-1.3.0/devolo_plc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44988 2023-04-13 13:15:23.000000 devolo_plc_api-1.3.0/devolo_plc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-13 13:15:23.000000 devolo_plc_api-1.3.0/devolo_plc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:15:23.000000 devolo_plc_api-1.3.0/devolo_plc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-13 13:15:23.000000 devolo_plc_api-1.3.0/devolo_plc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 13:15:23.000000 devolo_plc_api-1.3.0/devolo_plc_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.233554 devolo_plc_api-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/example_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/example_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.233554 devolo_plc_api-1.3.0/script/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4250 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/script/stubgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 13:15:23.237554 devolo_plc_api-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.233554 devolo_plc_api-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.237554 devolo_plc_api-1.3.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/fixtures/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/fixtures/device_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/fixtures/plcnet_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/fixtures/protobuf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.237554 devolo_plc_api-1.3.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/mocks/mock_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/mocks/mock_zeroconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.237554 devolo_plc_api-1.3.0/tests/stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/stubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/stubs/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/stubs/zeroconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/test_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/test_deviceapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/test_plcnetapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/test_profobuf.py
```

### Comparing `devolo_plc_api-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `devolo_plc_api-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `devolo_plc_api-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/.github/workflows/pythonpackage.yml` & `devolo_plc_api-1.3.0/.github/workflows/pythonpackage.yml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 jobs:
 
   format:
     name: Check formatting
     runs-on: ubuntu-latest
     steps:
     - name: Checkout sources
-      uses: actions/checkout@v3.3.0
+      uses: actions/checkout@v3.5.0
     - name: Set up Python
       uses: actions/setup-python@v4.5.0
       with:
         python-version: "3.8"
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
@@ -22,15 +22,15 @@
       uses: pre-commit/action@v3.0.0
 
   lint:
     name: Lint
     runs-on: ubuntu-latest
     steps:
     - name: Checkout sources
-      uses: actions/checkout@v3.3.0
+      uses: actions/checkout@v3.5.0
     - name: Set up Python
       uses: actions/setup-python@v4.5.0
       with:
         python-version: "3.8"
     - name: Lint with ruff
       run: |
         python -m pip install --upgrade pip
@@ -47,15 +47,15 @@
     name: Test with Python ${{ matrix.python-version }}
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
     - name: Checkout sources
-      uses: actions/checkout@v3.3.0
+      uses: actions/checkout@v3.5.0
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4.5.0
       with:
         python-version: ${{ matrix.python-version }}
         check-latest: true
     - name: Install dependencies
       run: |
@@ -72,15 +72,15 @@
 
   coverage:
     name: Upload coverage
     runs-on: ubuntu-latest
     needs: test
     steps:
     - name: Checkout sources
-      uses: actions/checkout@v3.3.0
+      uses: actions/checkout@v3.5.0
     - name: Set up Python
       uses: actions/setup-python@v4.5.0
       with:
         python-version: "3.8"
     - name: Download coverage
       uses: actions/download-artifact@v3.0.2
       with:
```

### Comparing `devolo_plc_api-1.2.0/.github/workflows/pythonpublish.yml` & `devolo_plc_api-1.3.0/.github/workflows/pythonpublish.yml`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   release:
     types: [created]
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3.3.0
+    - uses: actions/checkout@v3.5.0
     - name: Set up Python
       uses: actions/setup-python@v4.5.0
       with:
         python-version: "3.8"
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
```

### Comparing `devolo_plc_api-1.2.0/.gitignore` & `devolo_plc_api-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/.pre-commit-config.yaml` & `devolo_plc_api-1.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/LICENSE` & `devolo_plc_api-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/PKG-INFO` & `devolo_plc_api-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devolo_plc_api
-Version: 1.2.0
+Version: 1.3.0
 Summary: devolo PLC devices in Python
 Author-email: Markus Bong <m.bong@famabo.de>, Guido Schmitz <guido.schmitz@fedaix.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `devolo_plc_api-1.2.0/README.md` & `devolo_plc_api-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/clients/protobuf.py` & `devolo_plc_api-1.3.0/devolo_plc_api/clients/protobuf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Google Protobuf client."""
 from __future__ import annotations
 
 import asyncio
-import hashlib
 import logging
 from abc import ABC, abstractmethod
+from hashlib import sha256
 from http import HTTPStatus
 from typing import Any, Callable
 
 from httpx import (
     AsyncClient,
     ConnectError,
     ConnectTimeout,
@@ -41,15 +41,16 @@
         self._user: str
         self._version: str
 
     def __getattr__(self, attr: str) -> Callable[..., Any]:
         """Catch attempts to call methods synchronously."""
 
         def method(*args: Any, **kwargs: Any) -> Any:
-            return asyncio.run(getattr(self, async_method)(*args, **kwargs))
+            loop = asyncio.get_event_loop()
+            return loop.run_until_complete(getattr(self, async_method)(*args, **kwargs))
 
         async_method = f"async_{attr}"
         if hasattr(self.__class__, async_method):
             return method
         raise AttributeError(f"{self.__class__.__name__} object has no attribute {attr}")  # noqa: EM102, TRY003
 
     @property
@@ -76,15 +77,15 @@
                 method,
                 url,
                 auth=DigestAuth(self._user, self.password),
                 content=content,
                 timeout=timeout,
             )
             if response.status_code == HTTPStatus.UNAUTHORIZED:
-                self.password = hashlib.sha256(self.password.encode("utf-8")).hexdigest()
+                self.password = sha256(self.password.encode("utf-8")).hexdigest()
                 response = await self._session.request(
                     method,
                     url,
                     auth=DigestAuth(self._user, self.password),
                     content=content,
                     timeout=timeout,
                 )
```

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device.py` & `devolo_plc_api-1.3.0/devolo_plc_api/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Representation of your devolo device."""
 from __future__ import annotations
 
 import asyncio
-import ipaddress
 import logging
-import struct
 from contextlib import suppress
 from datetime import date
+from ipaddress import ip_address
+from struct import unpack_from
 from types import TracebackType
 
-import httpx
+from httpx import AsyncClient
 from zeroconf import DNSQuestionType, ServiceInfo, ServiceStateChange, Zeroconf
 from zeroconf.asyncio import AsyncServiceBrowser, AsyncServiceInfo, AsyncZeroconf
 
 from .device_api import SERVICE_TYPE as DEVICEAPI, DeviceApi
 from .exceptions.device import DeviceNotFound
 from .plcnet_api import DEVICES_WITHOUT_PLCNET, SERVICE_TYPE as PLCNETAPI, PlcNetApi
 from .zeroconf import ZeroconfServiceInfo
@@ -50,19 +50,19 @@
         self._background_tasks: set[asyncio.Task] = set()
         self._browser: dict[str, AsyncServiceBrowser] = {}
         self._connected = False
         self._info: dict[str, ZeroconfServiceInfo] = {PLCNETAPI: ZeroconfServiceInfo(), DEVICEAPI: ZeroconfServiceInfo()}
         self._logger = logging.getLogger(f"{self.__class__.__module__}.{self.__class__.__name__}")
         self._multicast = False
         self._password = ""
-        self._session_instance: httpx.AsyncClient | None = None
+        self._session_instance: AsyncClient | None = None
         self._zeroconf_instance = zeroconf_instance
         logging.captureWarnings(True)
 
-        self._session: httpx.AsyncClient
+        self._session: AsyncClient
         self._zeroconf: AsyncZeroconf
 
     def __del__(self) -> None:
         """Warn user, if the connection was not properly closed."""
         if self._connected and self._session_instance is None:
             self._logger.warning("Please disconnect properly from the device.")
 
@@ -92,15 +92,15 @@
     @property
     def firmware_version(self) -> str:
         """Firmware version currently installed."""
         return self._info[DEVICEAPI].properties.get("FirmwareVersion", "")
 
     @property
     def hostname(self) -> str:
-        """mDNS hostname of the device."""
+        """mDNS hostname of the device."""  # noqa: D403
         return self._info[DEVICEAPI].hostname
 
     @property
     def password(self) -> str:
         """The currently set device password."""
         return self._password
 
@@ -109,51 +109,54 @@
         """Change the currently set device password."""
         self._password = password
         if self.device:
             self.device.password = password
         if self.plcnet:
             self.plcnet.password = password
 
-    async def async_connect(self, session_instance: httpx.AsyncClient | None = None) -> None:
+    async def async_connect(self, session_instance: AsyncClient | None = None) -> None:
         """
         Connect to a device asynchronous.
 
         :param: session_instance: Session client instance to be potentially reused.
         """
         self._session_instance = session_instance
-        self._session = self._session_instance or httpx.AsyncClient()
+        self._session = self._session_instance or AsyncClient()
         if not self._zeroconf_instance:
             self._zeroconf = AsyncZeroconf()
         elif isinstance(self._zeroconf_instance, Zeroconf):
             self._zeroconf = AsyncZeroconf(zc=self._zeroconf_instance)
         else:
             self._zeroconf = self._zeroconf_instance
         await asyncio.gather(self._get_device_info(), self._get_plcnet_info())
         if not self.device and not self.plcnet:
             raise DeviceNotFound(self.ip)
         self._connected = True
 
     def connect(self) -> None:
         """Connect to a device synchronous."""
-        asyncio.run(self.async_connect())
+        loop = asyncio.new_event_loop()
+        loop.run_until_complete(self.async_connect())
 
     async def async_disconnect(self) -> None:
         """Disconnect from a device asynchronous."""
         if self._connected:
             for browser in self._browser.values():
                 await browser.async_cancel()
             if not self._zeroconf_instance:
                 await self._zeroconf.async_close()
             if not self._session_instance:
                 await self._session.aclose()
             self._connected = False
 
     def disconnect(self) -> None:
         """Disconnect from a device synchronous."""
-        asyncio.run(self.async_disconnect())
+        loop = asyncio.get_event_loop()
+        loop.run_until_complete(self.async_disconnect())
+        loop.close()
 
     async def _get_device_info(self) -> None:
         """Get information from the devolo Device API."""
         service_type = DEVICEAPI
         await self._get_zeroconf_info(service_type=service_type)
         if not self._info[service_type].properties:
             await self._retry_zeroconf_info(service_type=service_type)
@@ -214,15 +217,15 @@
     async def _get_service_info(self, zeroconf: Zeroconf, service_type: str, name: str) -> None:
         """Get service information, if IP matches."""
         service_info = AsyncServiceInfo(service_type, name)
         question_type = DNSQuestionType.QM if self._multicast else DNSQuestionType.QU
         with suppress(RuntimeError):
             await service_info.async_request(zeroconf, timeout=1000, question_type=question_type)
 
-        if not service_info.addresses or str(ipaddress.ip_address(service_info.addresses[0])) != self.ip:
+        if not service_info.addresses or str(ip_address(service_info.addresses[0])) != self.ip:
             return  # No need to continue, if there are no relevant service information
 
         self._logger.debug("Updating service info of %s for %s", service_type, service_info.server_key)
         if info := self.info_from_service(service_info):
             self._info[service_type] = info
 
     @staticmethod
@@ -231,18 +234,18 @@
         properties = {}
         if not service_info.addresses:
             return None  # No need to continue, if there is no IP address to contact the device
 
         total_length = len(service_info.text)
         offset = 0
         while offset < total_length:
-            (parsed_length,) = struct.unpack_from("!B", service_info.text, offset)
+            (parsed_length,) = unpack_from("!B", service_info.text, offset)
             key_value = service_info.text[offset + 1 : offset + 1 + parsed_length].decode("UTF-8").split("=")
             properties[key_value[0]] = key_value[1]
             offset += parsed_length + 1
 
         return ZeroconfServiceInfo(
             address=service_info.addresses[0],
-            hostname=service_info.server,
+            hostname=service_info.server or "",
             port=service_info.port,
             properties=properties,
         )
```

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device_api/__init__.py` & `devolo_plc_api-1.3.0/devolo_plc_api/device_api/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The devolo device API."""
 import re
 
 from .deviceapi import DeviceApi
+from .multiap_pb2 import WifiMultiApGetResponse
 from .support_pb2 import SupportInfoDump
 from .updatefirmware_pb2 import UpdateFirmwareCheck
 from .wifinetwork_pb2 import (
     WIFI_BAND_2G,
     WIFI_BAND_5G,
     WIFI_VAP_GUEST_AP,
     WIFI_VAP_MAIN_AP,
@@ -29,14 +30,15 @@
 __all__ = [
     "ConnectedStationInfo",
     "DeviceApi",
     "NeighborAPInfo",
     "RepeatedAPInfo",
     "SupportInfoItem",
     "WifiGuestAccessGet",
+    "WifiMultiApGetResponse",
     "CONFIGLAYER_FORMAT",
     "SERVICE_TYPE",
     "UPDATE_AVAILABLE",
     "UPDATE_NOT_AVAILABLE",
     "WIFI_BAND_2G",
     "WIFI_BAND_5G",
     "WIFI_VAP_GUEST_AP",
```

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device_api/deviceapi.py` & `devolo_plc_api-1.3.0/devolo_plc_api/device_api/deviceapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from devolo_plc_api.clients import Protobuf
 from devolo_plc_api.exceptions.feature import FeatureNotSupported
 from devolo_plc_api.zeroconf import ZeroconfServiceInfo
 
 from .factoryreset_pb2 import FactoryResetStart
 from .ledsettings_pb2 import LedSettingsGet, LedSettingsSet, LedSettingsSetResponse
+from .multiap_pb2 import WifiMultiApGetResponse
 from .restart_pb2 import RestartResponse, UptimeGetResponse
 from .support_pb2 import SupportInfoDump, SupportInfoDumpResponse
 from .updatefirmware_pb2 import UpdateFirmwareCheck, UpdateFirmwareStart
 from .wifinetwork_pb2 import (
     WifiConnectedStationsGet,
     WifiGuestAccessGet,
     WifiGuestAccessSet,
@@ -101,14 +102,27 @@
         led_setting = LedSettingsSet()
         led_setting.state = led_setting.LED_ON if enable else led_setting.LED_OFF
         query = await self._async_post("LedSettingsSet", content=led_setting.SerializeToString())
         response = LedSettingsSetResponse()
         response.ParseFromString(await query.aread())
         return response.result == response.SUCCESS
 
+    @_feature("multiap")
+    async def async_get_wifi_multi_ap(self) -> WifiMultiApGetResponse:
+        """
+        Get MultiAP details asynchronously. This feature only works on devices, that announce the multiap feature.
+
+        return: MultiAP details
+        """
+        self._logger.debug("Getting MultiAP details.")
+        query = await self._async_get("WifiMultiApGet")
+        response = WifiMultiApGetResponse()
+        response.ParseFromString(await query.aread())
+        return response
+
     @_feature("repeater0")
     async def async_get_wifi_repeated_access_points(self) -> list[WifiRepeatedAPsGet.RepeatedAPInfo]:
         """
         Get repeated wifi access point asynchronously. This feature only works on repeater devices, that announce the
         repeater0 feature.
 
         :return: Repeated access points in the neighborhood including connection rate data
```

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device_api/deviceapi.pyi` & `devolo_plc_api-1.3.0/devolo_plc_api/device_api/deviceapi.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 @generated by stubgen.  Do not edit manually!
 isort:skip_file
 """
 from __future__ import annotations
+from .multiap_pb2 import WifiMultiApGetResponse
 from .support_pb2 import SupportInfoDump
 from .updatefirmware_pb2 import UpdateFirmwareCheck
 from .wifinetwork_pb2 import WifiConnectedStationsGet, WifiGuestAccessGet, WifiNeighborAPsGet, WifiRepeatedAPsGet
 from devolo_plc_api.clients import Protobuf
 from devolo_plc_api.zeroconf import ZeroconfServiceInfo as ZeroconfServiceInfo
 from httpx import AsyncClient as AsyncClient
 
 class DeviceApi(Protobuf):
     features: list[str]
     password: str
     def __init__(self, ip: str, session: AsyncClient, info: ZeroconfServiceInfo) -> None: ...
     async def async_get_led_setting(self) -> bool: ...
     async def async_set_led_setting(self, enable: bool) -> bool: ...
+    async def async_get_wifi_multi_ap(self) -> WifiMultiApGetResponse: ...
     async def async_get_wifi_repeated_access_points(self) -> list[WifiRepeatedAPsGet.RepeatedAPInfo]: ...
     async def async_start_wps_clone(self) -> bool: ...
     async def async_factory_reset(self) -> bool: ...
     async def async_restart(self) -> bool: ...
     async def async_uptime(self) -> int: ...
     async def async_get_support_info(self) -> SupportInfoDump: ...
     async def async_check_firmware_available(self) -> UpdateFirmwareCheck: ...
@@ -27,14 +29,15 @@
     async def async_get_wifi_connected_station(self) -> list[WifiConnectedStationsGet.ConnectedStationInfo]: ...
     async def async_get_wifi_guest_access(self) -> WifiGuestAccessGet: ...
     async def async_set_wifi_guest_access(self, enable: bool, duration: int = ...) -> bool: ...
     async def async_get_wifi_neighbor_access_points(self) -> list[WifiNeighborAPsGet.NeighborAPInfo]: ...
     async def async_start_wps(self) -> bool: ...
     def get_led_setting(self) -> bool: ...
     def set_led_setting(self, enable: bool) -> bool: ...
+    def get_wifi_multi_ap(self) -> WifiMultiApGetResponse: ...
     def get_wifi_repeated_access_points(self) -> list[WifiRepeatedAPsGet.RepeatedAPInfo]: ...
     def start_wps_clone(self) -> bool: ...
     def factory_reset(self) -> bool: ...
     def restart(self) -> bool: ...
     def uptime(self) -> int: ...
     def get_support_info(self) -> SupportInfoDump: ...
     def check_firmware_available(self) -> UpdateFirmwareCheck: ...
```

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device_api/factoryreset_pb2.py` & `devolo_plc_api-1.3.0/devolo_plc_api/device_api/factoryreset_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device_api/factoryreset_pb2.pyi` & `devolo_plc_api-1.3.0/devolo_plc_api/device_api/factoryreset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device_api/ledsettings_pb2.py` & `devolo_plc_api-1.3.0/devolo_plc_api/device_api/ledsettings_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device_api/ledsettings_pb2.pyi` & `devolo_plc_api-1.3.0/devolo_plc_api/device_api/ledsettings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device_api/restart_pb2.py` & `devolo_plc_api-1.3.0/devolo_plc_api/device_api/restart_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device_api/restart_pb2.pyi` & `devolo_plc_api-1.3.0/devolo_plc_api/device_api/restart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device_api/support_pb2.py` & `devolo_plc_api-1.3.0/devolo_plc_api/device_api/support_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device_api/support_pb2.pyi` & `devolo_plc_api-1.3.0/devolo_plc_api/device_api/support_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device_api/updatefirmware_pb2.py` & `devolo_plc_api-1.3.0/devolo_plc_api/device_api/updatefirmware_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device_api/updatefirmware_pb2.pyi` & `devolo_plc_api-1.3.0/devolo_plc_api/device_api/updatefirmware_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device_api/wifinetwork_pb2.py` & `devolo_plc_api-1.3.0/devolo_plc_api/device_api/wifinetwork_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/device_api/wifinetwork_pb2.pyi` & `devolo_plc_api-1.3.0/devolo_plc_api/device_api/wifinetwork_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/exceptions/device.py` & `devolo_plc_api-1.3.0/devolo_plc_api/exceptions/device.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/network/__init__.py` & `devolo_plc_api-1.3.0/devolo_plc_api/network/__init__.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/__init__.py` & `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/__init__.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py` & `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi` & `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/identifydevice_pb2.py` & `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/identifydevice_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi` & `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/pairdevice_pb2.py` & `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/pairdevice_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi` & `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/plcnetapi.py` & `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/plcnetapi.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/plcnetapi.pyi` & `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/plcnetapi.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py` & `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi` & `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api.egg-info/PKG-INFO` & `devolo_plc_api-1.3.0/devolo_plc_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devolo-plc-api
-Version: 1.2.0
+Version: 1.3.0
 Summary: devolo PLC devices in Python
 Author-email: Markus Bong <m.bong@famabo.de>, Guido Schmitz <guido.schmitz@fedaix.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `devolo_plc_api-1.2.0/devolo_plc_api.egg-info/SOURCES.txt` & `devolo_plc_api-1.3.0/devolo_plc_api.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 devolo_plc_api/device_api/__init__.py
 devolo_plc_api/device_api/deviceapi.py
 devolo_plc_api/device_api/deviceapi.pyi
 devolo_plc_api/device_api/factoryreset_pb2.py
 devolo_plc_api/device_api/factoryreset_pb2.pyi
 devolo_plc_api/device_api/ledsettings_pb2.py
 devolo_plc_api/device_api/ledsettings_pb2.pyi
+devolo_plc_api/device_api/multiap_pb2.py
+devolo_plc_api/device_api/multiap_pb2.pyi
 devolo_plc_api/device_api/restart_pb2.py
 devolo_plc_api/device_api/restart_pb2.pyi
 devolo_plc_api/device_api/support_pb2.py
 devolo_plc_api/device_api/support_pb2.pyi
 devolo_plc_api/device_api/updatefirmware_pb2.py
 devolo_plc_api/device_api/updatefirmware_pb2.pyi
 devolo_plc_api/device_api/wifinetwork_pb2.py
```

### Comparing `devolo_plc_api-1.2.0/docs/CHANGELOG.md` & `devolo_plc_api-1.3.0/docs/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [v1.3.0] - 2023/04/13
+
+### Added
+
+- Get MultiAP information from the device
+
+### Fixed
+
+- The event loop got closed to early when disconnecting from a device synchronously.
+
 ## [v1.2.0] - 2023/02/17
 
 ### Added
 
 - Support for devices with password protected PLCNET API
 
 ## [v1.1.0] - 2023/01/24
```

### Comparing `devolo_plc_api-1.2.0/docs/CODE_OF_CONDUCT.md` & `devolo_plc_api-1.3.0/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/docs/CONTRIBUTING.md` & `devolo_plc_api-1.3.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/example_async.py` & `devolo_plc_api-1.3.0/example_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,20 @@
         # Get LED settings of the device. The state might be LED_ON or LED_OFF.
         print("LED is on" if await dpa.device.async_get_led_setting() else "LED if off")
 
         # Set LED settings of the device. Set enable to True to them turn on, to False to turn them off.
         # If the state was changed successfully, True is returned, otherwise False.
         print("success" if await dpa.device.async_set_led_setting(enable=True) else "failed")
 
+        # Get MultiAP details. If the device is not aware of a mesh controller or doesn't know its IP, it is left empty.
+        multi_ap = await dpa.device.async_get_wifi_multi_ap()
+        print(multi_ap.enabled)  # True
+        print(multi_ap.controller_id)  # "AA:BB:CC:DD:EE:FF"
+        print(multi_ap.controller_ip)  # "192.0.2.1"
+
         # Factory reset the device. If the reset will happen shortly, True is returned, otherwise False.
         print("success" if await dpa.device.async_factory_reset() else "failed")
 
         # Restart the device. If the restart will happen shortly, True is returned, otherwise False.
         print("success" if await dpa.device.async_restart() else "failed")
 
         # Get uptime of the device. This value can only be used as a strict monotonically increasing number and therefore has no unit.
```

### Comparing `devolo_plc_api-1.2.0/example_sync.py` & `devolo_plc_api-1.3.0/example_sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,20 @@
         # Get LED settings of the device. The state might be LED_ON or LED_OFF.
         print("LED is on" if dpa.device.get_led_setting() else "LED if off")
 
         # Set LED settings of the device. Set enable to True to them turn on, to False to turn them off.
         # If the state was changed successfully, True is returned, otherwise False.
         print("success" if dpa.device.set_led_setting(enable=True) else "failed")
 
+        # Get MultiAP details. If the device is not aware of a mesh controller or doesn't know its IP, it is left empty.
+        multi_ap = dpa.device.get_wifi_multi_ap()
+        print(multi_ap.enabled)  # True
+        print(multi_ap.controller_id)  # "AA:BB:CC:DD:EE:FF"
+        print(multi_ap.controller_ip)  # "192.0.2.1"
+
         # Factory reset the device. If the reset will happen shortly, True is returned, otherwise False.
         print("success" if dpa.device.factory_reset() else "failed")
 
         # Restart the device. If the restart will happen shortly, True is returned, otherwise False.
         print("success" if dpa.device.restart() else "failed")
 
         # Get uptime of the device. This value can only be used as a strict monotonically increasing number and therefore has no unit.
```

### Comparing `devolo_plc_api-1.2.0/pyproject.toml` & `devolo_plc_api-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/script/stubgen.py` & `devolo_plc_api-1.3.0/script/stubgen.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/tests/__init__.py` & `devolo_plc_api-1.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/tests/conftest.py` & `devolo_plc_api-1.3.0/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,21 +38,17 @@
     else:
         yield None
 
 
 @pytest.fixture()
 def block_communication() -> Generator[None, None, None]:
     """Block external communication."""
-    with patch("devolo_plc_api.device.AsyncZeroconf", AsyncMock), patch(
-        "devolo_plc_api.device.httpx.AsyncClient", AsyncMock
-    ), patch("devolo_plc_api.device.AsyncServiceBrowser", MockServiceBrowser), patch(
-        "devolo_plc_api.device.AsyncServiceInfo"
-    ), patch(
-        "devolo_plc_api.network.Zeroconf"
-    ), patch(
+    with patch("devolo_plc_api.device.AsyncZeroconf", AsyncMock), patch("devolo_plc_api.device.AsyncClient", AsyncMock), patch(
+        "devolo_plc_api.device.AsyncServiceBrowser", MockServiceBrowser
+    ), patch("devolo_plc_api.device.AsyncServiceInfo"), patch("devolo_plc_api.network.Zeroconf"), patch(
         "devolo_plc_api.network.ServiceBrowser", MockServiceBrowser
     ):
         yield
 
 
 @pytest.fixture()
 def event_loop() -> Generator[asyncio.events.AbstractEventLoop, None, None]:
```

### Comparing `devolo_plc_api-1.2.0/tests/fixtures/device.py` & `devolo_plc_api-1.3.0/tests/fixtures/device.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/tests/fixtures/device_api.py` & `devolo_plc_api-1.3.0/tests/fixtures/device_api.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/tests/fixtures/plcnet_api.py` & `devolo_plc_api-1.3.0/tests/fixtures/plcnet_api.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/tests/mocks/mock_zeroconf.py` & `devolo_plc_api-1.3.0/tests/mocks/mock_zeroconf.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/tests/stubs/protobuf.py` & `devolo_plc_api-1.3.0/tests/stubs/protobuf.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/tests/stubs/zeroconf.py` & `devolo_plc_api-1.3.0/tests/stubs/zeroconf.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/tests/test_data.json` & `devolo_plc_api-1.3.0/tests/test_data.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'ip'": "'192.0.2.1'"}*

```diff
@@ -20,9 +20,9 @@
                 "PlcMacAddress": "AABBCCDDEEFF",
                 "PlcTechnology": "hpav",
                 "Version": "v0"
             }
         }
     },
     "hostname": "device.local",
-    "ip": "192.168.0.10"
+    "ip": "192.0.2.1"
 }
```

### Comparing `devolo_plc_api-1.2.0/tests/test_device.py` & `devolo_plc_api-1.3.0/tests/test_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
     @pytest.mark.asyncio()
     @pytest.mark.usefixtures("mock_get_device_info", "mock_service_browser")
     async def test__get_service_info_alien(self, mock_info_from_service: Mock):
         """Test ignoring alien information discovered via mDNS."""
         with patch("devolo_plc_api.device.AsyncServiceInfo", StubAsyncServiceInfo), patch(
             "devolo_plc_api.device.PlcNetApi"
         ), pytest.raises(DeviceNotFound):
-            mock_device = Device(ip="192.168.0.11")
+            mock_device = Device(ip="192.0.2.2")
             await mock_device.async_connect()
             assert StubAsyncServiceInfo.async_request.call_count == 1
             assert mock_info_from_service.call_count == 0
 
     def test_info_from_service_no_address(self, mock_device: Device):
         """Test ignoring information received for an other address."""
         service_info = Mock()
```

### Comparing `devolo_plc_api-1.2.0/tests/test_deviceapi.py` & `devolo_plc_api-1.3.0/tests/test_deviceapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import pytest
 from pytest_httpx import HTTPXMock
 
 from devolo_plc_api.device_api import ConnectedStationInfo, DeviceApi, NeighborAPInfo, RepeatedAPInfo, SupportInfoItem
 from devolo_plc_api.device_api.factoryreset_pb2 import FactoryResetStart
 from devolo_plc_api.device_api.ledsettings_pb2 import LedSettingsGet, LedSettingsSetResponse
+from devolo_plc_api.device_api.multiap_pb2 import WifiMultiApGetResponse
 from devolo_plc_api.device_api.restart_pb2 import RestartResponse, UptimeGetResponse
 from devolo_plc_api.device_api.support_pb2 import SupportInfoDump, SupportInfoDumpResponse
 from devolo_plc_api.device_api.updatefirmware_pb2 import UpdateFirmwareCheck, UpdateFirmwareStart
 from devolo_plc_api.device_api.wifinetwork_pb2 import (
     WifiConnectedStationsGet,
     WifiGuestAccessGet,
     WifiGuestAccessSetResponse,
@@ -64,14 +65,31 @@
     def test_set_led_setting(self, device_api: DeviceApi, httpx_mock: HTTPXMock):
         """Test setting LED settings synchronously."""
         led_setting_set = LedSettingsSetResponse()
         httpx_mock.add_response(content=led_setting_set.SerializeToString())
         assert device_api.set_led_setting(True)
 
     @pytest.mark.asyncio()
+    @pytest.mark.parametrize("feature", ["multiap"])
+    async def test_async_get_wifi_multi_ap(self, device_api: DeviceApi, httpx_mock: HTTPXMock):
+        """Test setting LED settings asynchronously."""
+        multi_ap_details = WifiMultiApGetResponse(enabled=True)
+        httpx_mock.add_response(content=multi_ap_details.SerializeToString())
+        details = await device_api.async_get_wifi_multi_ap()
+        assert details.enabled
+
+    @pytest.mark.parametrize("feature", ["multiap"])
+    def test_get_wifi_multi_ap(self, device_api: DeviceApi, httpx_mock: HTTPXMock):
+        """Test setting LED settings synchronously."""
+        multi_ap_details = WifiMultiApGetResponse(enabled=True)
+        httpx_mock.add_response(content=multi_ap_details.SerializeToString())
+        details = device_api.get_wifi_multi_ap()
+        assert details.enabled
+
+    @pytest.mark.asyncio()
     @pytest.mark.parametrize("feature", ["repeater0"])
     async def test_async_get_wifi_repeated_access_points(
         self, device_api: DeviceApi, httpx_mock: HTTPXMock, repeated_ap: RepeatedAPInfo
     ):
         """Test getting AP settings asynchronously."""
         wifi_repeated_accesspoints_get = WifiRepeatedAPsGet(repeated_aps=[repeated_ap])
         httpx_mock.add_response(content=wifi_repeated_accesspoints_get.SerializeToString())
```

### Comparing `devolo_plc_api-1.2.0/tests/test_network.py` & `devolo_plc_api-1.3.0/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/tests/test_plcnetapi.py` & `devolo_plc_api-1.3.0/tests/test_plcnetapi.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.2.0/tests/test_profobuf.py` & `devolo_plc_api-1.3.0/tests/test_profobuf.py`

 * *Files identical despite different names*

