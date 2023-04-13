# Comparing `tmp/vmngclient-0.8.1.tar.gz` & `tmp/vmngclient-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmngclient-0.8.1.tar", max compression
+gzip compressed data, was "vmngclient-0.8.2.tar", max compression
```

## Comparing `vmngclient-0.8.1.tar` & `vmngclient-0.8.2.tar`

### file list

```diff
@@ -1,91 +1,96 @@
--rw-r--r--   0        0        0     2953 2023-03-29 18:35:07.100481 vmngclient-0.8.1/README.md
--rw-r--r--   0        0        0      807 2023-03-29 18:35:07.104481 vmngclient-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2259 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/__init__.py
--rw-r--r--   0        0        0     6010 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/admin_tech_api.py
--rw-r--r--   0        0        0     8671 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/administration.py
--rw-r--r--   0        0        0     6253 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/alarms_api.py
--rw-r--r--   0        0        0     1374 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/api_containter.py
--rw-r--r--   0        0        0    11371 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/basic_api.py
--rw-r--r--   0        0        0     6508 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/device_action_api.py
--rw-r--r--   0        0        0     1651 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/logs_api.py
--rw-r--r--   0        0        0     5881 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/mtt_aaa_api.py
--rw-r--r--   0        0        0     4040 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/omp_api.py
--rw-r--r--   0        0        0     5432 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/packet_capture_api.py
--rw-r--r--   0        0        0     4116 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/partition_manager_api.py
--rw-r--r--   0        0        0     8646 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/software_action_api.py
--rw-r--r--   0        0        0     5412 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/speedtest_api.py
--rw-r--r--   0        0        0     5345 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/task_status_api.py
--rw-r--r--   0        0        0    21722 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/template_api.py
--rw-r--r--   0        0        0     1476 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/__init__.py
--rw-r--r--   0        0        0     7176 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/cli_template.py
--rw-r--r--   0        0        0     2109 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/device_template/device_template.py
--rw-r--r--   0        0        0      476 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/device_template/device_template_payload.json.j2
--rw-r--r--   0        0        0     1224 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/feature_template.py
--rw-r--r--   0        0        0     3118 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/feature_template_field.py
--rw-r--r--   0        0        0      615 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/feature_template_payload.py
--rw-r--r--   0        0        0     2441 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/models/cisco_aaa_model.py
--rw-r--r--   0        0        0     2160 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/aaa/aaa_model.py
--rw-r--r--   0        0        0    11178 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2
--rw-r--r--   0        0        0     1041 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2
--rw-r--r--   0        0        0     4264 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2
--rw-r--r--   0        0        0     3735 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2
--rw-r--r--   0        0        0     1999 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/aaa/feature/user.json.j2
--rw-r--r--   0        0        0      419 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_system/cisco_system_model.py
--rw-r--r--   0        0        0     6752 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2
--rw-r--r--   0        0        0     2430 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
--rw-r--r--   0        0        0     4529 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
--rw-r--r--   0        0        0     1843 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2
--rw-r--r--   0        0        0     2123 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
--rw-r--r--   0        0        0     2098 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
--rw-r--r--   0        0        0      627 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
--rw-r--r--   0        0        0     2665 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py
--rw-r--r--   0        0        0     8179 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2
--rw-r--r--   0        0        0     9926 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2
--rw-r--r--   0        0        0     7057 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/tenant/tenant.json.j2
--rw-r--r--   0        0        0     1701 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/templates/payloads/tenant/tenant_model.py
--rw-r--r--   0        0        0     1119 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/tenant_api.py
--rw-r--r--   0        0        0     4837 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/tenant_backup_restore_api.py
--rw-r--r--   0        0        0    10925 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/api/versions_utils.py
--rw-r--r--   0        0        0    19658 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/dataclasses.py
--rw-r--r--   0        0        0     1243 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/exceptions.py
--rw-r--r--   0        0        0      672 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/logging.conf
--rw-r--r--   0        0        0     5570 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/response.py
--rw-r--r--   0        0        0    11671 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/session.py
--rw-r--r--   0        0        0     7877 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/tests/test_admin_tech_api.py
--rw-r--r--   0        0        0    12255 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/tests/test_administration.py
--rw-r--r--   0        0        0    11034 2023-03-29 18:35:07.104481 vmngclient-0.8.1/vmngclient/tests/test_alarms_api.py
--rw-r--r--   0        0        0     4460 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_creation_tools.py
--rw-r--r--   0        0        0     3878 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_device_action_api.py
--rw-r--r--   0        0        0    25969 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_devices_api.py
--rw-r--r--   0        0        0      836 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_feature_template_field.py
--rw-r--r--   0        0        0     1485 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_logs_api.py
--rw-r--r--   0        0        0    11146 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_mtt_aaa_api.py
--rw-r--r--   0        0        0    16398 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_omp_api.py
--rw-r--r--   0        0        0     5153 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_packet_capture.py
--rw-r--r--   0        0        0     4772 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_partition_manager_api.py
--rw-r--r--   0        0        0     2947 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_response.py
--rw-r--r--   0        0        0     4753 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_session.py
--rw-r--r--   0        0        0     3753 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_software_action_api.py
--rw-r--r--   0        0        0     6005 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_speed_test_api.py
--rw-r--r--   0        0        0     3124 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_task_status_api.py
--rw-r--r--   0        0        0     8234 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_templates.py
--rw-r--r--   0        0        0     3625 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_tenant_backup_restore_api.py
--rw-r--r--   0        0        0     8432 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_typed_list.py
--rw-r--r--   0        0        0     5333 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_version_utils.py
--rw-r--r--   0        0        0     3132 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/tests/test_vmanage_auth.py
--rw-r--r--   0        0        0     7218 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/typed_list.py
--rw-r--r--   0        0        0        0 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/utils/__init__.py
--rw-r--r--   0        0        0      190 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/utils/alarm_status.py
--rw-r--r--   0        0        0      196 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/utils/certificate_status.py
--rw-r--r--   0        0        0       97 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/utils/config_status.py
--rw-r--r--   0        0        0     4677 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/utils/creation_tools.py
--rw-r--r--   0        0        0     2261 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/utils/device_model.py
--rw-r--r--   0        0        0      472 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/utils/operation_status.py
--rw-r--r--   0        0        0      139 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/utils/personality.py
--rw-r--r--   0        0        0      115 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/utils/reachability.py
--rw-r--r--   0        0        0       92 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/utils/template_type.py
--rw-r--r--   0        0        0      102 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/utils/validate_status.py
--rw-r--r--   0        0        0     4977 2023-03-29 18:35:07.108481 vmngclient-0.8.1/vmngclient/vmanage_auth.py
--rw-r--r--   0        0        0     4749 1970-01-01 00:00:00.000000 vmngclient-0.8.1/setup.py
--rw-r--r--   0        0        0     4099 1970-01-01 00:00:00.000000 vmngclient-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     2748 2023-04-13 09:36:23.756716 vmngclient-0.8.2/README.md
+-rw-r--r--   0        0        0      807 2023-04-13 09:36:23.756716 vmngclient-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     2259 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/__init__.py
+-rw-r--r--   0        0        0     6010 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/admin_tech_api.py
+-rw-r--r--   0        0        0     8671 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/administration.py
+-rw-r--r--   0        0        0     6253 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/alarms_api.py
+-rw-r--r--   0        0        0     1829 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/api_containter.py
+-rw-r--r--   0        0        0    11371 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/basic_api.py
+-rw-r--r--   0        0        0     2742 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/dashboard_api.py
+-rw-r--r--   0        0        0     6508 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/device_action_api.py
+-rw-r--r--   0        0        0     1651 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/logs_api.py
+-rw-r--r--   0        0        0     5881 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/mtt_aaa_api.py
+-rw-r--r--   0        0        0     4040 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/omp_api.py
+-rw-r--r--   0        0        0     5432 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/packet_capture_api.py
+-rw-r--r--   0        0        0     4945 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/partition_manager_api.py
+-rw-r--r--   0        0        0     2041 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/resource_pool_api.py
+-rw-r--r--   0        0        0     7330 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/software_action_api.py
+-rw-r--r--   0        0        0     5412 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/speedtest_api.py
+-rw-r--r--   0        0        0     9546 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/task_status_api.py
+-rw-r--r--   0        0        0    21616 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/template_api.py
+-rw-r--r--   0        0        0     1476 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/__init__.py
+-rw-r--r--   0        0        0     7176 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/cli_template.py
+-rw-r--r--   0        0        0     2109 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/device_template/device_template.py
+-rw-r--r--   0        0        0      476 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/device_template/device_template_payload.json.j2
+-rw-r--r--   0        0        0     1224 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/feature_template.py
+-rw-r--r--   0        0        0     3118 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/feature_template_field.py
+-rw-r--r--   0        0        0      615 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/feature_template_payload.py
+-rw-r--r--   0        0        0     2441 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/models/cisco_aaa_model.py
+-rw-r--r--   0        0        0     2160 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/aaa_model.py
+-rw-r--r--   0        0        0    11178 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2
+-rw-r--r--   0        0        0     1041 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2
+-rw-r--r--   0        0        0     4264 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2
+-rw-r--r--   0        0        0     3735 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2
+-rw-r--r--   0        0        0     1999 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/user.json.j2
+-rw-r--r--   0        0        0      419 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_system/cisco_system_model.py
+-rw-r--r--   0        0        0     6752 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2
+-rw-r--r--   0        0        0     2430 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
+-rw-r--r--   0        0        0     4529 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
+-rw-r--r--   0        0        0     1843 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2
+-rw-r--r--   0        0        0     2123 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
+-rw-r--r--   0        0        0     2098 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
+-rw-r--r--   0        0        0      627 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
+-rw-r--r--   0        0        0     2665 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py
+-rw-r--r--   0        0        0     8179 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2
+-rw-r--r--   0        0        0     9926 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2
+-rw-r--r--   0        0        0     7057 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/tenant/tenant.json.j2
+-rw-r--r--   0        0        0     1701 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/tenant/tenant_model.py
+-rw-r--r--   0        0        0     1119 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/tenant_api.py
+-rw-r--r--   0        0        0     4953 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/tenant_backup_restore_api.py
+-rw-r--r--   0        0        0    10790 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/versions_utils.py
+-rw-r--r--   0        0        0    19969 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/dataclasses.py
+-rw-r--r--   0        0        0     1634 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/exceptions.py
+-rw-r--r--   0        0        0      672 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/logging.conf
+-rw-r--r--   0        0        0     5615 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/response.py
+-rw-r--r--   0        0        0    11671 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/session.py
+-rw-r--r--   0        0        0     7877 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_admin_tech_api.py
+-rw-r--r--   0        0        0    12255 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_administration.py
+-rw-r--r--   0        0        0    11034 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_alarms_api.py
+-rw-r--r--   0        0        0     8053 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_cli_template.py
+-rw-r--r--   0        0        0     4460 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_creation_tools.py
+-rw-r--r--   0        0        0     3878 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_device_action_api.py
+-rw-r--r--   0        0        0    25969 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_devices_api.py
+-rw-r--r--   0        0        0      836 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_feature_template_field.py
+-rw-r--r--   0        0        0     1485 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_logs_api.py
+-rw-r--r--   0        0        0    11146 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_mtt_aaa_api.py
+-rw-r--r--   0        0        0    16398 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_omp_api.py
+-rw-r--r--   0        0        0     5153 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_packet_capture.py
+-rw-r--r--   0        0        0     4967 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_partition_manager_api.py
+-rw-r--r--   0        0        0     2947 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_response.py
+-rw-r--r--   0        0        0     4753 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_session.py
+-rw-r--r--   0        0        0     3774 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_software_action_api.py
+-rw-r--r--   0        0        0     6005 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_speed_test_api.py
+-rw-r--r--   0        0        0     5042 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_task_status_api.py
+-rw-r--r--   0        0        0     8686 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_templates.py
+-rw-r--r--   0        0        0     3625 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     8432 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_typed_list.py
+-rw-r--r--   0        0        0     5170 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_version_utils.py
+-rw-r--r--   0        0        0     3132 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_vmanage_auth.py
+-rw-r--r--   0        0        0     7357 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/typed_list.py
+-rw-r--r--   0        0        0        0 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/__init__.py
+-rw-r--r--   0        0        0      190 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/alarm_status.py
+-rw-r--r--   0        0        0      196 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/certificate_status.py
+-rw-r--r--   0        0        0       97 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/config_status.py
+-rw-r--r--   0        0        0     4677 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/creation_tools.py
+-rw-r--r--   0        0        0     1233 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/dashboard.py
+-rw-r--r--   0        0        0     2261 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/device_model.py
+-rw-r--r--   0        0        0      472 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/operation_status.py
+-rw-r--r--   0        0        0      139 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/personality.py
+-rw-r--r--   0        0        0      115 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/reachability.py
+-rw-r--r--   0        0        0       92 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/template_type.py
+-rw-r--r--   0        0        0     1944 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/upgrades_helper.py
+-rw-r--r--   0        0        0      102 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/validate_status.py
+-rw-r--r--   0        0        0     4977 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/vmanage_auth.py
+-rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 vmngclient-0.8.2/setup.py
+-rw-r--r--   0        0        0     3894 1970-01-01 00:00:00.000000 vmngclient-0.8.2/PKG-INFO
```

### Comparing `vmngclient-0.8.1/README.md` & `vmngclient-0.8.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -53,28 +53,27 @@
 </details>
 
 <details>
     <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>
 
 ```python
 # Prepare devices list
-vsmarts = [device for device in DevicesAPI(session).devices
-            if device .personality == Personality.VSMART]
-software_image = "viptela-20.7.2-x86_64.tar.gz"
+vsmarts = session.api.devices.get().filter(personality = Personality.VSMART)
+image = "viptela-20.7.2-x86_64.tar.gz"
 
 # Upload image
 session.api.repository.upload_image(software_image)
 
-# Upgrade
-software_action = SoftwareActionAPI(session, DeviceCategory.VEDGES)
-software_action_id = software_action.upgrade_software(vsmarts,
-    InstallSpecHelper.CEDGE.value, reboot = False, sync = True, software_image=software_image)
+# Install software
+
+install_task = session.api.software.install(devices = vsmarts,
+    image= image)
 
 # Check action status
-wait_for_completed(session, software_action_id, 3000)
+install_task.wait_for_completed()
 ```
 
 </details>
 
 <details>
     <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>
```

### Comparing `vmngclient-0.8.1/pyproject.toml` & `vmngclient-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vmngclient"
-version = "0.8.1"
+version = "0.8.2"
 description = "Universal vManage API"
 authors = ["kagorski <kagorski@cisco.com>"]
 readme = "README.md"
 repository = "https://github.com/CiscoDevNet/vManage-client"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `vmngclient-0.8.1/vmngclient/__init__.py` & `vmngclient-0.8.2/vmngclient/__init__.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/admin_tech_api.py` & `vmngclient-0.8.2/vmngclient/api/admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/administration.py` & `vmngclient-0.8.2/vmngclient/api/administration.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/alarms_api.py` & `vmngclient-0.8.2/vmngclient/api/alarms_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/api_containter.py` & `vmngclient-0.8.2/vmngclient/api/api_containter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from vmngclient.api.admin_tech_api import AdminTechAPI
 from vmngclient.api.alarms_api import AlarmsAPI
 from vmngclient.api.basic_api import DevicesAPI, DeviceStateAPI
+from vmngclient.api.dashboard_api import DashboardAPI
 from vmngclient.api.logs_api import LogsAPI
 from vmngclient.api.omp_api import OmpAPI
 from vmngclient.api.packet_capture_api import PacketCaptureAPI
+from vmngclient.api.partition_manager_api import PartitionManagerAPI
+from vmngclient.api.resource_pool_api import ResourcePoolAPI
+from vmngclient.api.software_action_api import SoftwareActionAPI
 from vmngclient.api.speedtest_api import SpeedtestAPI
 from vmngclient.api.template_api import TemplatesAPI
 from vmngclient.api.tenant_api import TenantsAPI
 from vmngclient.api.tenant_backup_restore_api import TenantBackupRestoreAPI
 from vmngclient.api.versions_utils import RepositoryAPI
 
 if TYPE_CHECKING:
@@ -19,16 +23,20 @@
 
 
 class APIContainter:
     def __init__(self, session: vManageSession):
         self.tenants = TenantsAPI(session)
         self.admin_tech = AdminTechAPI(session)
         self.alarms = AlarmsAPI(session)
+        self.dashboard = DashboardAPI(session)
         self.devices = DevicesAPI(session)
         self.device_state = DeviceStateAPI(session)
         self.logs = LogsAPI(session)
         self.omp = OmpAPI(session)
         self.packet_capture = PacketCaptureAPI(session)
         self.speedtest = SpeedtestAPI(session)
         self.templates = TemplatesAPI(session)
         self.tenant_backup = TenantBackupRestoreAPI(session)
         self.repository = RepositoryAPI(session)
+        self.resource_pool = ResourcePoolAPI(session)
+        self.software = SoftwareActionAPI(session)
+        self.partition = PartitionManagerAPI(session)
```

### Comparing `vmngclient-0.8.1/vmngclient/api/basic_api.py` & `vmngclient-0.8.2/vmngclient/api/basic_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/device_action_api.py` & `vmngclient-0.8.2/vmngclient/api/device_action_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/logs_api.py` & `vmngclient-0.8.2/vmngclient/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/mtt_aaa_api.py` & `vmngclient-0.8.2/vmngclient/api/mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/omp_api.py` & `vmngclient-0.8.2/vmngclient/api/omp_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/packet_capture_api.py` & `vmngclient-0.8.2/vmngclient/api/packet_capture_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/software_action_api.py` & `vmngclient-0.8.2/vmngclient/api/software_action_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,144 +1,103 @@
 from __future__ import annotations
 
 import logging
-from enum import Enum
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, cast
 
-from attr import define  # type: ignore
-
-from vmngclient.api.versions_utils import DeviceCategory, DeviceVersions, RepositoryAPI
+from vmngclient.api.task_status_api import Task
+from vmngclient.api.versions_utils import DeviceVersions, RepositoryAPI
 from vmngclient.dataclasses import Device
 from vmngclient.exceptions import VersionDeclarationError  # type: ignore
 from vmngclient.typed_list import DataSequence
 from vmngclient.utils.creation_tools import asdict
 from vmngclient.utils.personality import Personality
+from vmngclient.utils.upgrades_helper import get_install_specification, validate_personality_homogeneity
 
 logger = logging.getLogger(__name__)
 
 
 if TYPE_CHECKING:
     from vmngclient.session import vManageSession
 
 
-class Family(Enum):
-    VEDGE = "vedge"
-    VMANAGE = "vmanage"
-
-
-class VersionType(Enum):
-    VMANAGE = "vmanage"
-
-
-class DeviceType(Enum):
-    CONTROLLER = "controller"
-    VEDGE = "vedge"
-    VMANAGE = "vmanage"
-
-
-class DeviceClass(Enum):
-    VEDGE = "vedge"
-    VMANAGE = "vmanage"
-    VSMART = "vsmart"
-    VBOND = "vbond"
-    CEDGE = "cedge"
-
-
-@define
-class InstallSpecification:
-
-    family: Family
-    version_type: VersionType
-    device_type: DeviceType
-
-
-class InstallSpecHelper(Enum):
-
-    VMANAGE = InstallSpecification(Family.VMANAGE, VersionType.VMANAGE, DeviceType.VMANAGE)
-    VSMART = InstallSpecification(Family.VEDGE, VersionType.VMANAGE, DeviceType.CONTROLLER)
-    VBOND = InstallSpecification(Family.VEDGE, VersionType.VMANAGE, DeviceType.CONTROLLER)
-    VEDGE = InstallSpecification(Family.VEDGE, VersionType.VMANAGE, DeviceType.VEDGE)
-
-
 class SoftwareActionAPI:
     """
     API methods for software actions. All methods
     are exececutable on all device categories.
 
     Usage example:
     # Create session
     session = create_vManageSession(...)
 
     # Prepare devices list
-    devices = [device for device in DevicesAPI(session).devices
-                if device .personality == Personality.VSMART]
+    devices = session.api.devices.get()
+    vsmarts = devices.filter(personality=Personality.VSMART)
     software_image = "viptela-20.7.2-x86_64.tar.gz"
 
     # Upgrade
-    devices_payload = DeviceVersions(session, DeviceCategory.CONTROLLERS).get_devices_current_version(devices)
-    software_action = SoftwareActionAPI(session, DeviceCategory.VEDGES)
-    software_action_id = software_action.upgrade_software(devices_payload,
-        InstallSpecHelper.CEDGE.value, reboot = False, sync = True, software_image=software_image)
+    upgrade_id = SoftwareActionAPI(session).install(devices = vmanages,
+    software_image=software_image)
 
-    # Check action status
-    wait_for_completed(session, software_action_id, 3000)
+    # Check upgrade status
+    TaskAPI(session, software_action_id).wait_for_completed()
     """
 
-    def __init__(self, session: vManageSession, device_category: DeviceCategory) -> None:
+    def __init__(self, session: vManageSession) -> None:
 
         self.session = session
         self.repository = RepositoryAPI(self.session)
-        self.device_versions = DeviceVersions(self.session, device_category)
+        self.device_versions = DeviceVersions(self.session)
 
-    def activate_software(
+    def activate(
         self,
         devices: DataSequence[Device],
-        device_type: DeviceType,
         version_to_activate: Optional[str] = "",
-        software_image: Optional[str] = "",
-    ) -> str:
+        image: Optional[str] = "",
+    ) -> Task:
         """
         Set chosen version as current version
 
         Args:
             devices (List[Device]): For those devices software will be activated
             version_to_activate (Optional[str]): version to be set as current version
             software_image (Optional[str]): path to software image
 
             Notice: Have to pass one of those arguments (version_to_activate,
             software_image)
 
         Returns:
             str: Activate software action id
         """
-        if software_image and not version_to_activate:
-            version = cast(str, self.repository.get_image_version(software_image))
-        elif version_to_activate and not software_image:
+        validate_personality_homogeneity(devices)
+        if image and not version_to_activate:
+            version = cast(str, self.repository.get_image_version(image))
+        elif version_to_activate and not image:
             version = cast(str, version_to_activate)
         else:
             raise VersionDeclarationError("You can not provide software_image and image version at the same time!")
+
         url = "/dataservice/device/action/changepartition"
         payload = {
             "action": "changepartition",
             "devices": [
                 asdict(device) for device in self.device_versions.get_device_available(version, devices)  # type: ignore
             ],
-            "deviceType": device_type.value,
+            "deviceType": get_install_specification(devices.first()).device_type.value,
         }
         activate = dict(self.session.post(url, json=payload).json())
-        return activate["id"]
+        return Task(self.session, activate["id"])
 
-    def upgrade_software(
+    def install(
         self,
         devices: DataSequence[Device],
-        reboot: bool,
+        reboot: bool = False,
         sync: bool = True,
-        software_image: Optional[str] = "",
+        image: Optional[str] = "",
         image_version: Optional[str] = "",
-    ) -> str:
+    ) -> Task:
         """
         Method to install new software
 
         Args:
             devices (List[Device]): For those devices software will be activated
             install_spec (InstallSpecification): specification of devices
             on which the action is to be performed
@@ -152,68 +111,63 @@
 
         Raises:
             ValueError: Raise error if downgrade in certain cases
 
         Returns:
             str: action id
         """
-        if software_image and not image_version:
-            version = cast(str, self.repository.get_image_version(software_image))
-        elif image_version and not software_image:
+        validate_personality_homogeneity(devices)
+        if image and not image_version:
+            version = cast(str, self.repository.get_image_version(image))
+        elif image_version and not image:
             version = cast(str, image_version)
         else:
             raise VersionDeclarationError("You can not provide software_image and image version at the same time")
-
-        specification_container = {
-            Personality.VMANAGE: InstallSpecHelper.VMANAGE.value,
-            Personality.VBOND: InstallSpecHelper.VBOND.value,
-            Personality.VSMART: InstallSpecHelper.VSMART.value,
-            Personality.EDGE: InstallSpecHelper.VEDGE.value,
-        }
-
-        personality = devices[0].personality
-        install_spec = specification_container[personality]
+        install_specification = get_install_specification(devices.first())
 
         url = "/dataservice/device/action/install"
         payload: Dict[str, Any] = {
             "action": "install",
             "input": {
                 "vEdgeVPN": 0,
                 "vSmartVPN": 0,
-                "family": install_spec.family.value,
+                "family": install_specification.family.value,
                 "version": version,
-                "versionType": install_spec.version_type.value,
+                "versionType": install_specification.version_type.value,
                 "reboot": reboot,
                 "sync": sync,
             },
             "devices": [
                 {"deviceId": device.deviceId, "deviceIP": device.deviceIP}
                 for device in self.device_versions.get_device_list(devices)
             ],  # type: ignore
-            "deviceType": install_spec.device_type.value,
+            "deviceType": install_specification.device_type.value,
         }
-        if personality in (Personality.VMANAGE, Personality.EDGE):  # block downgrade for edges and vmanages
-            self._downgrade_check(payload["devices"], payload["input"]["version"], install_spec.family.value)
+        if devices.first().personality in (
+            Personality.VMANAGE,
+            Personality.EDGE,
+        ):  # block downgrade for edges and vmanages
+            self._downgrade_check(payload["devices"], payload["input"]["version"], install_specification.family.value)
         upgrade = dict(self.session.post(url, json=payload).json())
-        return upgrade["id"]
+        return Task(self.session, upgrade["id"])
 
     def _downgrade_check(self, payload_devices: List[dict], version_to_upgrade: str, family: str) -> None:
         """
         Check if upgrade operation is not actually a downgrade opeartion.
         If so, in some cases action is being blocked.
 
         Args:
             version_to_upgrade (str): version to upgrade
             devices_category (DeviceCategory): devices category
 
         Returns:
             List[str]: list of devices with no permission to downgrade
         """
         incorrect_devices = []
-        devices_versions_repo = self.repository.get_devices_versions_repository(self.device_versions.device_category)
+        devices_versions_repo = self.repository.get_devices_versions_repository()
         for device in payload_devices:
             dev_current_version = str(devices_versions_repo[device["deviceId"]].current_version)
             splited_version_to_upgrade = version_to_upgrade.split(".")
             for priority, label in enumerate(dev_current_version.split("-")[0].split(".")):
                 try:
                     label = int(label)  # type: ignore
                     version = int(splited_version_to_upgrade[priority])
```

### Comparing `vmngclient-0.8.1/vmngclient/api/speedtest_api.py` & `vmngclient-0.8.2/vmngclient/api/speedtest_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/template_api.py` & `vmngclient-0.8.2/vmngclient/api/template_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 import json
 import logging
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Optional, Type, overload
 
 from requests.exceptions import HTTPError
 
-from vmngclient.api.task_status_api import wait_for_completed
+from vmngclient.api.task_status_api import Task
 from vmngclient.api.templates.cli_template import CLITemplate
 from vmngclient.api.templates.device_template.device_template import (
     DeviceSpecificValue,
     DeviceTemplate,
     GeneralTemplate,
 )
 from vmngclient.api.templates.feature_template import FeatureTemplate
 from vmngclient.api.templates.feature_template_field import FeatureTemplateField, get_path_dict
 from vmngclient.api.templates.feature_template_payload import FeatureTemplatePayload
 from vmngclient.api.templates.models.cisco_aaa_model import CiscoAAAModel
 from vmngclient.dataclasses import Device, DeviceTemplateInfo, FeatureTemplateInfo, TemplateInfo
 from vmngclient.exceptions import AlreadyExistsError, AttachedError, TemplateNotFoundError
 from vmngclient.typed_list import DataSequence
-from vmngclient.utils.operation_status import OperationStatus
 from vmngclient.utils.template_type import TemplateType
 
 if TYPE_CHECKING:
     from vmngclient.session import vManageSession
 
 logger = logging.getLogger(__name__)
 
@@ -148,19 +147,19 @@
 
         if invalid:
             raise TypeError()
 
         endpoint = "/dataservice/template/device/config/attachfeature"
         logger.info(f"Attaching a template: {name} to the device: {device.hostname}.")
         response = self.session.post(url=endpoint, json=payload).json()
-        task = wait_for_completed(session=self.session, action_id=response["id"])
-        if task.status == OperationStatus.SUCCESS.value:
+        task = Task(session=self.session, task_id=response["id"]).wait_for_completed()
+        if task.result:
             return True
         logger.warning(f"Failed to attach tempate: {name} to the device: {device.hostname}.")
-        logger.warning(f"Task activity information: {task.activity}")
+        logger.warning(f"Task activity information: {task.sub_tasks_data[0].activity}")
         return False
 
     def _attach_cli(self, name: str, device: Device, is_edited: bool = False) -> bool:
         """
 
         Args:
             name (str): Template name to attached.
@@ -197,19 +196,19 @@
             ]
         }
         if is_edited:
             payload["deviceTemplateList"][0]["isEdited"] = True  # type: ignore
         endpoint = "/dataservice/template/device/config/attachcli"
         logger.info(f"Attaching a template: {name} to the device: {device.hostname}.")
         response = self.session.post(url=endpoint, json=payload).json()
-        task = wait_for_completed(session=self.session, action_id=response["id"])
-        if task.status == OperationStatus.SUCCESS.value:
+        task = Task(session=self.session, task_id=response["id"]).wait_for_completed()
+        if task.result:
             return True
         logger.warning(f"Failed to attach tempate: {name} to the device: {device.hostname}.")
-        logger.warning(f"Task activity information: {task.activity}")
+        logger.warning(f"Task activity information: {task.sub_tasks_data[0].activity}")
         return False
 
     def deatach(self, device: Device) -> bool:
         """
         Deatach it`s the same to change device mode to CLI mode.
 
         Args:
@@ -221,19 +220,19 @@
         payload = {
             "deviceType": device.personality.value,
             "devices": [{"deviceId": device.uuid, "deviceIP": device.id}],
         }
         endpoint = "/dataservice/template/config/device/mode/cli"
         logger.info(f"Changing mode to cli mode for {device.hostname}.")
         response = self.session.post(url=endpoint, json=payload).json()
-        task = wait_for_completed(session=self.session, action_id=response["id"])
-        if task.status == OperationStatus.SUCCESS.value:
+        task = Task(session=self.session, task_id=response["id"]).wait_for_completed()
+        if task.result:
             return True
         logger.warning(f"Failed to change to cli mode for device: {device.hostname}.")
-        logger.warning(f"Task activity information: {task.activity}")
+        logger.warning(f"Task activity information: {task.sub_tasks_data[0].activity}")
         return False
 
     @overload
     def delete(self, template: Type[DeviceTemplate], name: str) -> bool:  # type: ignore
         ...
 
     @overload
```

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/__init__.py` & `vmngclient-0.8.2/vmngclient/api/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/cli_template.py` & `vmngclient-0.8.2/vmngclient/api/templates/cli_template.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/device_template/device_template.py` & `vmngclient-0.8.2/vmngclient/api/templates/device_template/device_template.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/feature_template.py` & `vmngclient-0.8.2/vmngclient/api/templates/feature_template.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/feature_template_field.py` & `vmngclient-0.8.2/vmngclient/api/templates/feature_template_field.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/feature_template_payload.py` & `vmngclient-0.8.2/vmngclient/api/templates/feature_template_payload.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/models/cisco_aaa_model.py` & `vmngclient-0.8.2/vmngclient/api/templates/models/cisco_aaa_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/aaa/aaa_model.py` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/aaa_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/aaa/feature/user.json.j2` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/user.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/tenant/tenant.json.j2` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/tenant/tenant.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/templates/payloads/tenant/tenant_model.py` & `vmngclient-0.8.2/vmngclient/api/templates/payloads/tenant/tenant_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/tenant_api.py` & `vmngclient-0.8.2/vmngclient/api/tenant_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/api/tenant_backup_restore_api.py` & `vmngclient-0.8.2/vmngclient/api/tenant_backup_restore_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from __future__ import annotations
 
 import logging
 import re
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional
 
-from vmngclient.api.task_status_api import TaskStatus, wait_for_completed
+from vmngclient.api.task_status_api import SubTaskData, Task
 
 if TYPE_CHECKING:
     from vmngclient.session import vManageSession
 
 logger = logging.getLogger(__name__)
 
 
@@ -70,16 +70,16 @@
         Returns:
             str: filename of exported tenant backup file stored on vManage
 
         Example usage:
             fileName = ProviderBackupRestore.export()
         """
         response = self.session.get_json("/dataservice/tenantbackup/export")
-        status = wait_for_completed(self.session, response["processId"], timeout)
-        string = re.search("""file location: (.*)""", status.activity[-1])
+        status = Task(self.session, response["processId"]).wait_for_completed(timeout_seconds=timeout)
+        string = re.search("""file location: (.*)""", status.sub_tasks_data[0].activity[-1])
         assert string, "File location not found."
         return string.group(1)
 
     def delete(self, file: str) -> List[str]:
         """Delete tenant backup file
 
         Args:
@@ -124,15 +124,15 @@
             file = f"/dataservice/tenantbackup/download/{tenant_id}/{file}"
 
         download_dir = download_dir if download_dir else Path.cwd()
         download = download_dir / Path(file).name
         self.session.get_file(file, download)
         return download
 
-    def import_file(self, file: Path, timeout: int = 300) -> TaskStatus:
+    def import_file(self, file: Path, timeout: int = 300) -> SubTaskData:
         """Upload the file for tenant import to the DB and poll for Success
 
         Args:
             file: The path of the file to be upladed
             timeout: Max polling time for task (default: 300 seconds)
 
         Returns:
@@ -141,8 +141,12 @@
         Example usage:
              status = ProviderBackupRestore.import_file(file)
         """
 
         url = "/dataservice/tenantbackup/import"
         files = {"file": (file.name, open(str(file), "rb"))}
         response = self.session.post(url, data={}, files=files)
-        return wait_for_completed(self.session, response.json()["processId"], timeout)
+        return (
+            Task(self.session, response.json()["processId"])
+            .wait_for_completed(timeout_seconds=timeout)
+            .sub_tasks_data[0]
+        )
```

### Comparing `vmngclient-0.8.1/vmngclient/api/versions_utils.py` & `vmngclient-0.8.2/vmngclient/api/versions_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import logging
-from enum import Enum
 from pathlib import PurePath
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 from attr import define, field  # type: ignore
 from clint.textui.progress import Bar as ProgressBar  # type: ignore
 from requests_toolbelt.multipart.encoder import MultipartEncoder, MultipartEncoderMonitor  # type: ignore
 
@@ -16,19 +15,14 @@
 
 if TYPE_CHECKING:
     from vmngclient.session import vManageSession
 
 logger = logging.getLogger(__name__)
 
 
-class DeviceCategory(Enum):
-    CONTROLLERS = "controllers"
-    VEDGES = "vedges"
-
-
 @define
 class DeviceSoftwareRepository(DataclassBase):
     installed_versions: List[str] = field(default=None)
     available_versions: List[str] = field(default=None, metadata={FIELD_NAME: "availableVersions"})
     current_version: str = field(default=None, metadata={FIELD_NAME: "version"})
     default_version: str = field(default=None, metadata={FIELD_NAME: "defaultVersion"})
     device_id: str = field(default=None, metadata={FIELD_NAME: "uuid"})
@@ -75,28 +69,30 @@
         Returns:
             list: software images list
         """
         url = "/dataservice/device/action/software/images?imageType=software"
         software_images = list(self.session.get_data(url))
         return software_images
 
-    def get_devices_versions_repository(self, device_category: DeviceCategory) -> Dict[str, DeviceSoftwareRepository]:
+    def get_devices_versions_repository(self) -> Dict[str, DeviceSoftwareRepository]:
         """
         Create DeviceSoftwareRepository dataclass,
         which cointains information about all possible version types for certain devices
 
         Returns:
             Dict[str, DeviceSoftwareRepository]: Dictionary containing all versions
             information
         """
 
-        url = f"/dataservice/system/device/{device_category.value}"
-        devices_versions_info = self.session.get_data(url)
+        url = "/dataservice/system/device/controllers"
+        controllers_versions_info = self.session.get_data(url)
+        url = "/dataservice/system/device/vedges"
+        edges_versions_info = self.session.get_data(url)
         devices_versions_repository = {}
-        for device in devices_versions_info:
+        for device in controllers_versions_info + edges_versions_info:
             device_all_versions = create_dataclass(DeviceSoftwareRepository, device)
             device_all_versions.installed_versions = [version for version in device_all_versions.available_versions]
             device_all_versions.installed_versions.append(device_all_versions.current_version)
             devices_versions_repository[device_all_versions.device_id] = device_all_versions
         return devices_versions_repository
 
     def get_image_version(self, software_image: str) -> Union[str, None]:
@@ -171,17 +167,16 @@
 
 
 class DeviceVersions:
     """
     Methods to prepare devices list for payload
     """
 
-    def __init__(self, session: vManageSession, device_category: DeviceCategory):
+    def __init__(self, session: vManageSession):
         self.repository = RepositoryAPI(session)
-        self.device_category = device_category
 
     def _get_device_list_in(
         self, version_to_set_up: str, devices: DataSequence[Device], version_type: str
     ) -> DataSequence[DeviceVersionPayload]:
         """
         Create devices payload list included requested version, if requested version
         is in specified version type
@@ -193,15 +188,15 @@
 
         Returns:
             list : list of devices
         """
         devices_payload = DataSequence(
             DeviceVersionPayload, [DeviceVersionPayload(device.uuid, device.id) for device in devices]  # type: ignore
         )
-        all_dev_versions = self.repository.get_devices_versions_repository(self.device_category)
+        all_dev_versions = self.repository.get_devices_versions_repository()
         for device in devices_payload:
             device_versions = getattr(all_dev_versions[device.deviceId], version_type)
             try:
                 for version in device_versions:
                     if version_to_set_up in version:
                         device.version = version
                         break
@@ -258,15 +253,15 @@
 
         Returns:
             list : list of devices
         """
         devices_payload = DataSequence(
             DeviceVersionPayload, [DeviceVersionPayload(device.uuid, device.id) for device in devices]  # type: ignore
         )
-        all_dev_versions = self.repository.get_devices_versions_repository(self.device_category)
+        all_dev_versions = self.repository.get_devices_versions_repository()
         for device in devices_payload:
             device.version = getattr(all_dev_versions[device.deviceId], version_type)
         return devices_payload
 
     def get_devices_current_version(self, devices: DataSequence[Device]) -> DataSequence[DeviceVersionPayload]:
         """
         Create devices payload list included current software version key
```

### Comparing `vmngclient-0.8.1/vmngclient/dataclasses.py` & `vmngclient-0.8.2/vmngclient/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -474,7 +474,16 @@
     servers: List[TacacsServer] = field(factory=list, metadata={FIELD_NAME: "server"})
 
 
 @define
 class SoftwareInstallTimeout(DataclassBase):
     download_timeout_min: int = field(converter=str, metadata={FIELD_NAME: "downloadTimeoutInMin"})
     activate_timeout_min: int = field(converter=str, metadata={FIELD_NAME: "activateTimeoutInMin"})
+
+
+@define
+class ResourcePoolData(DataclassBase):
+    """Endpoint: /resourcepool/resource/vpn"""
+
+    tenant_id: str = field(metadata={FIELD_NAME: "tenantId"})
+    tenant_vpn: int = field(metadata={FIELD_NAME: "tenantVpn"})
+    device_vpn: Optional[int] = field(default=None, metadata={FIELD_NAME: "deviceVpn"})
```

### Comparing `vmngclient-0.8.1/vmngclient/exceptions.py` & `vmngclient-0.8.2/vmngclient/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,7 +43,23 @@
         self.message = f"Template: {name} - wrong template type."
 
 
 class AlreadyExistsError(Exception):
     """Raised when an entity that we attempted to create already exists."""
 
     pass
+
+
+class EmptyTaskResponseError(Exception):
+    """Raised if task is registred by vManage, but reponse content is empty"""
+
+    pass
+
+
+class TaskNotRegisteredError(Exception):
+    """Raised if task_id is generated, but it's not registere in vManage"""
+
+    pass
+
+
+class MultiplePersonalityError(Exception):
+    """Raised if Device DataSequnce contains devices with multiples personalities"""
```

### Comparing `vmngclient-0.8.1/vmngclient/logging.conf` & `vmngclient-0.8.2/vmngclient/logging.conf`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/response.py` & `vmngclient-0.8.2/vmngclient/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,18 @@
             "status": response.status_code,
             "reason": response.reason,
             "elapsed-seconds": round(float(response.elapsed.microseconds) / 1000000, 3),
             "headers": dict(response.headers.items()),
         }
         try:
             json = response.json()
-            json.pop("header", None)
+
+            if isinstance(json, dict):
+                json.pop("header", None)
+
             response_debug.update({"json": json})
         except JSONDecodeError:
             if response.encoding is not None:
                 if len(response.text) <= 1024:
                     response_debug.update({"text": response.text})
                 else:
                     response_debug.update({"text(trimmed)": response.text[:1024]})
```

### Comparing `vmngclient-0.8.1/vmngclient/session.py` & `vmngclient-0.8.2/vmngclient/session.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_admin_tech_api.py` & `vmngclient-0.8.2/vmngclient/tests/test_admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_administration.py` & `vmngclient-0.8.2/vmngclient/tests/test_administration.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_alarms_api.py` & `vmngclient-0.8.2/vmngclient/tests/test_alarms_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_creation_tools.py` & `vmngclient-0.8.2/vmngclient/tests/test_creation_tools.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_device_action_api.py` & `vmngclient-0.8.2/vmngclient/tests/test_device_action_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_devices_api.py` & `vmngclient-0.8.2/vmngclient/tests/test_devices_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_feature_template_field.py` & `vmngclient-0.8.2/vmngclient/tests/test_feature_template_field.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_logs_api.py` & `vmngclient-0.8.2/vmngclient/tests/test_logs_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_mtt_aaa_api.py` & `vmngclient-0.8.2/vmngclient/tests/test_mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_omp_api.py` & `vmngclient-0.8.2/vmngclient/tests/test_omp_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_packet_capture.py` & `vmngclient-0.8.2/vmngclient/tests/test_packet_capture.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_partition_manager_api.py` & `vmngclient-0.8.2/vmngclient/tests/test_partition_manager_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 import unittest
 from unittest.mock import Mock, patch
 
 from vmngclient.api.partition_manager_api import PartitionManagerAPI
-from vmngclient.api.software_action_api import DeviceType
-from vmngclient.api.versions_utils import (
-    DeviceCategory,
-    DeviceSoftwareRepository,
-    DeviceVersionPayload,
-    DeviceVersions,
-    RepositoryAPI,
-)
+from vmngclient.api.versions_utils import DeviceSoftwareRepository, DeviceVersionPayload, DeviceVersions, RepositoryAPI
 from vmngclient.dataclasses import Device
+from vmngclient.typed_list import DataSequence
 
 
 class TestPartitionManagerAPI(unittest.TestCase):
     def setUp(self):
-        self.device = Device(
-            personality="vedge",
-            uuid="mock_uuid",
-            id="mock_ip",
-            hostname="mock_host",
-            reachability="reachable",
-            local_system_ip="mock_ip",
-            status="normal",
-            memUsage=1.0,
-            connected_vManages=["192.168.0.1"],
-            model="vedge-cloud",
+        self.device = DataSequence(
+            Device,
+            [
+                Device(
+                    personality="vedge",
+                    uuid="mock_uuid",
+                    id="mock_ip",
+                    hostname="mock_host",
+                    reachability="reachable",
+                    local_system_ip="mock_ip",
+                    status="normal",
+                    memUsage=1.0,
+                    connected_vManages=["192.168.0.1"],
+                    model="vedge-cloud",
+                )
+            ],
         )
         self.DeviceSoftwareRepository_obj = {
             "mock_uuid": DeviceSoftwareRepository(
                 ["ver1", "ver2", "curr_ver"],
                 ["ver1", "ver2"],
                 "curr_ver",
                 "def_ver",
                 "mock_uuid",
             ),
         }
 
         self.mock_devices = [{"deviceId": "mock_uuid", "deviceIP": "mock_ip", "version": "ver1"}]
-        self.mock_device_version_payload = [DeviceVersionPayload("mock_uuid", "mock_ip", "ver1")]
+        self.mock_device_version_payload = DataSequence(
+            DeviceVersionPayload, [DeviceVersionPayload("mock_uuid", "mock_ip", "ver1")]
+        )
         mock_session = Mock()
         self.mock_repository_object = RepositoryAPI(mock_session)
-        self.mock_device_versions = DeviceVersions(self.mock_repository_object, DeviceCategory.CONTROLLERS)
-        self.mock_partition_manager_obj = PartitionManagerAPI(
-            mock_session, DeviceCategory.CONTROLLERS, DeviceType.CONTROLLER
-        )
+        self.mock_device_versions = DeviceVersions(self.mock_repository_object)
+        self.mock_partition_manager_obj = PartitionManagerAPI(mock_session)
 
-    @patch.object(DeviceVersions, "get_device_available")
-    def test_remove_partition_if_force_true(self, mock_get_device_list):
+    @patch("vmngclient.utils.upgrades_helper.get_install_specification")
+    @patch.object(DeviceVersions, "get_devices_available_versions")
+    def test_remove_partition_if_force_true(self, mock_get_device_list, mock_get_spec):
         # Prepare mock data
         mock_get_device_list.return_value = Mock()
         mock_devices = Mock()
         mock_devices.return_value = self.mock_devices
         mock_get_device_list.return_value = self.mock_device_version_payload
         self.mock_repository_object.devices = self.mock_devices
         self.mock_repository_object.session.post.return_value.json.return_value = {"id": "mock_action_id"}
 
         # Assert
-        answer = self.mock_partition_manager_obj.remove_partition(self.mock_device_version_payload, True)
+        answer = self.mock_partition_manager_obj.remove_partition(self.device, force=True).task_id
         self.assertEqual(answer, "mock_action_id")
 
     @patch.object(PartitionManagerAPI, "_check_remove_partition_possibility")
-    @patch.object(DeviceVersions, "get_device_available")
+    @patch.object(DeviceVersions, "get_devices_available_versions")
     def test_remove_partition_not_raise_error_force_false(self, mock_get_device_list, mock_check_remove):
         # Prepare mock data
         mock_get_device_list.return_value = self.mock_device_version_payload
         mock_check_remove.return_value = []
         self.mock_repository_object.devices = self.mock_devices
         self.mock_repository_object.session.post.return_value.json.return_value = {"id": "mock_action_id"}
 
         # Assert
-        answer = self.mock_partition_manager_obj.remove_partition(self.mock_device_version_payload, False)
+        answer = self.mock_partition_manager_obj.remove_partition(self.device, force=False).task_id
         self.assertEqual(answer, "mock_action_id", "action ids not equal")
 
     @patch.object(RepositoryAPI, "get_devices_versions_repository")
     def test_check_remove_partition_possibility_if_version_incorrect(self, mock_get_devices_versions_repository):
         # Prepare mock data
         mock_get_devices_versions_repository.return_value = self.DeviceSoftwareRepository_obj
         mock_devices = [{"deviceId": "mock_uuid", "deviceIP": "mock_ip", "version": "curr_ver"}]
@@ -88,17 +88,18 @@
         mock_get_devices_versions_repository.return_value = self.DeviceSoftwareRepository_obj
         mock_devices = [{"deviceId": "mock_uuid", "deviceIP": "mock_ip", "version": "any_ver"}]
 
         # Assert
         answer = self.mock_partition_manager_obj._check_remove_partition_possibility(mock_devices)
         self.assertEqual(answer, None, "lists are not equal")
 
+    @patch.object(DeviceVersions, "get_devices_current_version")
     @patch("vmngclient.session.vManageSession")
-    def test_set_default_partition(self, mock_session):
+    def test_set_default_partition(self, mock_session, mock_get_devices):
         # Arrange
-        mock_partition_manager = PartitionManagerAPI(mock_session, DeviceCategory.CONTROLLERS, DeviceType.CONTROLLER)
+        mock_partition_manager = PartitionManagerAPI(mock_session)
         mock_partition_manager.session.post.return_value.json.return_value = {"id": "id_1"}
         # Act
-        answer = mock_partition_manager.set_default_partition(self.mock_device_version_payload)
+        answer = mock_partition_manager.set_default_partition(self.device).task_id
 
         # Assert
         self.assertEqual(answer, "id_1")
```

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_response.py` & `vmngclient-0.8.2/vmngclient/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_session.py` & `vmngclient-0.8.2/vmngclient/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_software_action_api.py` & `vmngclient-0.8.2/vmngclient/tests/test_software_action_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import unittest
 from unittest.mock import Mock, patch
 
-from vmngclient.api.software_action_api import Family, InstallSpecHelper, SoftwareActionAPI
-from vmngclient.api.versions_utils import DeviceCategory, DeviceSoftwareRepository, DeviceVersions, RepositoryAPI
+from vmngclient.api.software_action_api import SoftwareActionAPI
+from vmngclient.api.versions_utils import DeviceSoftwareRepository, DeviceVersions, RepositoryAPI
 from vmngclient.dataclasses import Device
+from vmngclient.typed_list import DataSequence
+from vmngclient.utils.upgrades_helper import Family, InstallSpecHelper
 
 
 class TestSoftwareAcionAPI(unittest.TestCase):
     def setUp(self):
         self.device = Device(
             personality="vedge",
             uuid="mock_uuid",
@@ -31,32 +33,32 @@
         }
 
         self.mock_devices = [{"deviceId": "mock_uuid", "deviceIP": "mock_ip", "version": "ver1"}]
         self.install_spec = InstallSpecHelper.VMANAGE.value
 
         mock_session = Mock()
         self.mock_repository_object = RepositoryAPI(mock_session)
-        self.mock_device_versions = DeviceVersions(self.mock_repository_object, DeviceCategory.CONTROLLERS)
-        self.mock_software_action_obj = SoftwareActionAPI(mock_session, DeviceCategory.VEDGES)
+        self.mock_device_versions = DeviceVersions(self.mock_repository_object)
+        self.mock_software_action_obj = SoftwareActionAPI(mock_session)
 
     @patch("vmngclient.session.vManageSession")
     @patch.object(SoftwareActionAPI, "_downgrade_check")
     @patch.object(RepositoryAPI, "get_image_version")
     def test_upgrade_software_if_downgrade_check_is_none(
         self, mock_get_image_version, mock_downgrade_check, mock_session
     ):
 
         # Prepare mock data
         mock_downgrade_check.return_value = False
         self.mock_repository_object.session.post.return_value.json.return_value = {"id": "mock_action_id"}
         mock_session.post.return_value = {"id": "mock_action_id"}
 
         # Assert
-        answer = self.mock_software_action_obj.upgrade_software([self.device], True, True, "path")
-        self.assertEqual(answer, "mock_action_id", "action ids not equal")
+        answer = self.mock_software_action_obj.install(DataSequence(Device, [self.device]), True, True, "path").task_id
+        self.assertEqual(answer, "mock_action_id")
 
     @patch.object(RepositoryAPI, "get_devices_versions_repository")
     def test_downgrade_check_no_incorrect_devices(self, mock_get_devices_versions_repository):
         # Preapre mock data
         upgrade_version = "20.9"
         mock_get_devices_versions_repository.return_value = self.DeviceSoftwareRepository_obj
         mock_devices = [{"deviceId": "mock_uuid", "deviceIP": "mock_ip", "version": upgrade_version}]
```

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_speed_test_api.py` & `vmngclient-0.8.2/vmngclient/tests/test_speed_test_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_templates.py` & `vmngclient-0.8.2/vmngclient/tests/test_templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from unittest.mock import patch
 
-from vmngclient.api.task_status_api import TaskStatus
+from vmngclient.api.task_status_api import SubTaskData, TaskResult
 from vmngclient.api.template_api import TemplatesAPI
 from vmngclient.api.templates.feature_template import FeatureTemplate
 from vmngclient.dataclasses import Device, FeatureTemplateInfo, TemplateInfo
 from vmngclient.typed_list import DataSequence
 from vmngclient.utils.creation_tools import create_dataclass
 from vmngclient.utils.personality import Personality
 from vmngclient.utils.reachability import Reachability
@@ -56,15 +56,29 @@
             reachability=Reachability.REACHABLE,
             local_system_ip="192.168.0.1",
             memUsage=1.0,
             connected_vManages=["192.168.0.1"],
             model="vedge-cloud",
             status="normal",
         )
-        self.task = TaskStatus("Success", "success", [])
+        sub_tasks_data = SubTaskData.parse_obj(
+            {
+                "status": "Success",
+                "statusId": "success",
+                "action": "",
+                "activity": [],
+                "currentActivity": "",
+                "actionConfig": "",
+                "order": 1,
+                "uuid": "",
+                "host-name": "",
+                "site-id": "",
+            }
+        )
+        self.task = TaskResult(result=True, sub_tasks_data=[sub_tasks_data])
 
     @patch("vmngclient.response.vManageResponse")
     @patch("vmngclient.session.vManageSession")
     def test_templates_success(self, mock_session, mocked_response):
 
         # Arrange
         mock_session.get.return_value = mocked_response
```

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_tenant_backup_restore_api.py` & `vmngclient-0.8.2/vmngclient/tests/test_tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_typed_list.py` & `vmngclient-0.8.2/vmngclient/tests/test_typed_list.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_version_utils.py` & `vmngclient-0.8.2/vmngclient/tests/test_version_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 import unittest
 from unittest.mock import Mock, patch
 
-from vmngclient.api.versions_utils import (
-    DeviceCategory,
-    DeviceSoftwareRepository,
-    DeviceVersionPayload,
-    DeviceVersions,
-    RepositoryAPI,
-)
+from vmngclient.api.versions_utils import DeviceSoftwareRepository, DeviceVersionPayload, DeviceVersions, RepositoryAPI
 from vmngclient.dataclasses import Device
 from vmngclient.typed_list import DataSequence
 
 
 class TestRepositoryAPI(unittest.TestCase):
     def setUp(self):
         self.device = Device(
@@ -66,29 +60,29 @@
                 "defaultVersion": "def_ver",
                 "uuid": "mock_uuid",
             }
         ]
         mock_session.get_data.return_value = api_mock_response
         mock_repository_object = RepositoryAPI(mock_session)
 
-        answer = mock_repository_object.get_devices_versions_repository(DeviceCategory.CONTROLLERS)
+        answer = mock_repository_object.get_devices_versions_repository()
 
         self.assertEqual(
             answer["mock_uuid"],
             self.DeviceSoftwareRepository_obj["mock_uuid"],
             "DeviceSoftwareRepository object created uncorrectly",
         )
 
     @patch.object(RepositoryAPI, "get_devices_versions_repository")
     def test_get_device_available(self, mock_get_devices_versions_repository):
         # Prepare mock data
         mock_get_devices_versions_repository.return_value = Mock()
         mock_session = Mock()
         mock_repository_object = RepositoryAPI(mock_session)
-        mock_device_versions = DeviceVersions(mock_repository_object, DeviceCategory.CONTROLLERS.value)
+        mock_device_versions = DeviceVersions(mock_repository_object)
         mock_get_devices_versions_repository.return_value = self.DeviceSoftwareRepository_obj
         answer = mock_device_versions.get_device_available("ver1", [self.device])
         expected_result = DataSequence(DeviceVersionPayload, [DeviceVersionPayload("mock_uuid", "mock_ip", "ver1")])
 
         # Assert
         self.assertEqual(
             answer,
@@ -98,15 +92,15 @@
 
     @patch.object(RepositoryAPI, "get_devices_versions_repository")
     def test_get_device_list_if_in_installed(self, mock_get_devices_versions_repository):
         # Prepare mock data
         mock_get_devices_versions_repository.return_value = Mock()
         mock_session = Mock()
         mock_repository_object = RepositoryAPI(mock_session)
-        mock_device_versions = DeviceVersions(mock_repository_object, DeviceCategory.CONTROLLERS.value)
+        mock_device_versions = DeviceVersions(mock_repository_object)
         mock_get_devices_versions_repository.return_value = self.DeviceSoftwareRepository_obj
         answer = mock_device_versions.get_device_list_in_installed("ver1", [self.device])
         expected_result = DataSequence(DeviceVersionPayload, [DeviceVersionPayload("mock_uuid", "mock_ip", "ver1")])
 
         # Assert
         self.assertEqual(
             answer,
@@ -117,13 +111,13 @@
     @patch.object(RepositoryAPI, "get_devices_versions_repository")
     def test_get_devices_current_version(self, mock_get_devices_versions_repository):
         # Arrange
         mock_session = Mock()
         mock_get_devices_versions_repository.return_value = Mock()
         mock_get_devices_versions_repository.return_value = self.DeviceSoftwareRepository_obj
         mock_repository_object = RepositoryAPI(mock_session)
-        mock_device_versions = DeviceVersions(mock_repository_object, DeviceCategory.CONTROLLERS)
+        mock_device_versions = DeviceVersions(mock_repository_object)
         # Act
         answer = mock_device_versions.get_devices_current_version([self.device])
         # Answer
         proper_answer = DataSequence(DeviceVersionPayload, [DeviceVersionPayload("mock_uuid", "mock_ip", "curr_ver")])
         self.assertEqual(answer, proper_answer)
```

### Comparing `vmngclient-0.8.1/vmngclient/tests/test_vmanage_auth.py` & `vmngclient-0.8.2/vmngclient/tests/test_vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/typed_list.py` & `vmngclient-0.8.2/vmngclient/typed_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 from typing import Any, Generic, Iterable, MutableSequence, Type, TypeVar, overload
 
+from pydantic import BaseModel  # type: ignore
+
 from vmngclient.exceptions import InvalidOperationError
 from vmngclient.utils.creation_tools import AttrsInstance
 
 T = TypeVar("T")
 D = TypeVar("D")
 
 
@@ -136,16 +138,18 @@
         ...
 
     @overload
     def __init__(self, _type: Type[T], _iterable: Iterable[T], /) -> None:
         ...
 
     def __init__(self, _type, _iterable=None, /):
-        if not isinstance(_type, AttrsInstance):
-            raise TypeError(f"Expected {AttrsInstance.__name__} item type, got {_type.__name__}.")
+        if not isinstance(_type, AttrsInstance) and not issubclass(_type, BaseModel):
+            raise TypeError(
+                f"Expected {AttrsInstance.__name__} or {BaseModel.__name__} item type, got {_type.__name__}."
+            )
 
         super().__init__(_type, _iterable)
 
     def __eq__(self, __o: object) -> bool:
         if isinstance(__o, DataSequence):
             if len(self) != len(__o):
                 return False
```

### Comparing `vmngclient-0.8.1/vmngclient/utils/creation_tools.py` & `vmngclient-0.8.2/vmngclient/utils/creation_tools.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/utils/device_model.py` & `vmngclient-0.8.2/vmngclient/utils/device_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/vmngclient/vmanage_auth.py` & `vmngclient-0.8.2/vmngclient/vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.1/setup.py` & `vmngclient-0.8.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,17 +35,17 @@
  'python-dateutil>=2.8.2,<3.0.0',
  'requests-toolbelt>=0.10.1,<0.11.0',
  'requests>=2.27.1,<3.0.0',
  'tenacity>=8.1.0,<9.0.0']
 
 setup_kwargs = {
     'name': 'vmngclient',
-    'version': '0.8.1',
+    'version': '0.8.2',
     'description': 'Universal vManage API',
-    'long_description': '# vManage-client\n[![Python3.8](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8)](https://www.python.org/)\n\nvManage client is a package for creating simple and parallel automatic requests via official vManageAPI. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any vManage.\n\n## Installation\n```console\npip install vmngclient\n```\n\n## Session usage example\nOur session is an extension to `requests.Session` designed to make it easier to communicate via API calls with vManage. We provide ready to use authenticetion, you have to simply provide the vmanage url, username and password as as if you were doing it through a GUI. \n```python\nfrom vmngclient.session import create_vManageSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\nsession = create_vManageSession(url=url, username=username, password=password)\n\nsession.get("/dataservice/device")\n```\n\n## API usage examples\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nadmintech.download(admin_tech_file)\nadmintech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\nvsmarts = [device for device in DevicesAPI(session).devices\n            if device .personality == Personality.VSMART]\nsoftware_image = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(software_image)\n\n# Upgrade\nsoftware_action = SoftwareActionAPI(session, DeviceCategory.VEDGES)\nsoftware_action_id = software_action.upgrade_software(vsmarts,\n    InstallSpecHelper.CEDGE.value, reboot = False, sync = True, software_image=software_image)\n\n# Check action status\nwait_for_completed(session, software_action_id, 3000)\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\n\n```python\nalarms = session.api.alarms.get()\n```\n\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts:\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## [Contributing, bug reporting and feature requests](https://github.com/CiscoDevNet/vManage-client/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/CiscoDevNet/vManage-client/issues), or directly via mail on vmngclient@cisco.com.\n',
+    'long_description': '# vManage-client\n[![Python3.8](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8)](https://www.python.org/)\n\nvManage client is a package for creating simple and parallel automatic requests via official vManageAPI. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any vManage.\n\n## Installation\n```console\npip install vmngclient\n```\n\n## Session usage example\nOur session is an extension to `requests.Session` designed to make it easier to communicate via API calls with vManage. We provide ready to use authenticetion, you have to simply provide the vmanage url, username and password as as if you were doing it through a GUI. \n```python\nfrom vmngclient.session import create_vManageSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\nsession = create_vManageSession(url=url, username=username, password=password)\n\nsession.get("/dataservice/device")\n```\n\n## API usage examples\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nadmintech.download(admin_tech_file)\nadmintech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\nvsmarts = session.api.devices.get().filter(personality = Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(software_image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices = vsmarts,\n    image= image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\n\n```python\nalarms = session.api.alarms.get()\n```\n\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts:\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## [Contributing, bug reporting and feature requests](https://github.com/CiscoDevNet/vManage-client/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/CiscoDevNet/vManage-client/issues), or directly via mail on vmngclient@cisco.com.\n',
     'author': 'kagorski',
     'author_email': 'kagorski@cisco.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/CiscoDevNet/vManage-client',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `vmngclient-0.8.1/PKG-INFO` & `vmngclient-0.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmngclient
-Version: 0.8.1
+Version: 0.8.2
 Summary: Universal vManage API
 Home-page: https://github.com/CiscoDevNet/vManage-client
 Author: kagorski
 Author-email: kagorski@cisco.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -82,28 +82,27 @@
 </details>
 
 <details>
     <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>
 
 ```python
 # Prepare devices list
-vsmarts = [device for device in DevicesAPI(session).devices
-            if device .personality == Personality.VSMART]
-software_image = "viptela-20.7.2-x86_64.tar.gz"
+vsmarts = session.api.devices.get().filter(personality = Personality.VSMART)
+image = "viptela-20.7.2-x86_64.tar.gz"
 
 # Upload image
 session.api.repository.upload_image(software_image)
 
-# Upgrade
-software_action = SoftwareActionAPI(session, DeviceCategory.VEDGES)
-software_action_id = software_action.upgrade_software(vsmarts,
-    InstallSpecHelper.CEDGE.value, reboot = False, sync = True, software_image=software_image)
+# Install software
+
+install_task = session.api.software.install(devices = vsmarts,
+    image= image)
 
 # Check action status
-wait_for_completed(session, software_action_id, 3000)
+install_task.wait_for_completed()
 ```
 
 </details>
 
 <details>
     <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>
```

