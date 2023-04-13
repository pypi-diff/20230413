# Comparing `tmp/extremecloudiq-api-23.2.0.4.tar.gz` & `tmp/extremecloudiq-api-23.2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/var/lib/jenkins/workspace/Build-Promotions/UploadtoPyPi/dist/tmpcnmjwwo8/extremecloudiq-api-23.2.0.4.tar", last modified: Thu Apr 13 17:11:36 2023, max compression
+gzip compressed data, was "/var/lib/jenkins/workspace/Build-Promotions/UploadtoPyPi/dist/tmp8w6fh7ih/extremecloudiq-api-23.2.1.4.tar", last modified: Thu Apr 13 17:12:33 2023, max compression
```

## Comparing `extremecloudiq-api-23.2.0.4.tar` & `extremecloudiq-api-23.2.1.4.tar`

### file list

```diff
@@ -1,742 +1,778 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:11:36.000000 extremecloudiq-api-23.2.0.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:11:36.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:11:36.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/
--rw-r--r--   0 root         (0) root         (0)     1588 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32862 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/account_api.py
--rw-r--r--   0 root         (0) root         (0)    16606 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/alert_api.py
--rw-r--r--   0 root         (0) root         (0)    24695 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/application_api.py
--rw-r--r--   0 root         (0) root         (0)    11074 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/authentication_api.py
--rw-r--r--   0 root         (0) root         (0)    26154 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/authorization_api.py
--rw-r--r--   0 root         (0) root         (0)    28878 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/client_api.py
--rw-r--r--   0 root         (0) root         (0)   171864 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/configuration___authentication_api.py
--rw-r--r--   0 root         (0) root         (0)    34019 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/configuration___basic_api.py
--rw-r--r--   0 root         (0) root         (0)     7035 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/configuration___certificate_api.py
--rw-r--r--   0 root         (0) root         (0)    16187 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/configuration___deployment_api.py
--rw-r--r--   0 root         (0) root         (0)   292852 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/configuration___policy_api.py
--rw-r--r--   0 root         (0) root         (0)   133457 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/configuration___user_management_api.py
--rw-r--r--   0 root         (0) root         (0)    18543 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/copilot___anomalies_api.py
--rw-r--r--   0 root         (0) root         (0)    96668 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/copilot___connectivity_experience_api.py
--rw-r--r--   0 root         (0) root         (0)   235486 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/device_api.py
--rw-r--r--   0 root         (0) root         (0)    56014 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/hiq_api.py
--rw-r--r--   0 root         (0) root         (0)    67517 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/location_api.py
--rw-r--r--   0 root         (0) root         (0)    44748 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/log_api.py
--rw-r--r--   0 root         (0) root         (0)    49086 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/network_policy_api.py
--rw-r--r--   0 root         (0) root         (0)    15844 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/notification_api.py
--rw-r--r--   0 root         (0) root         (0)    16818 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/operation_api.py
--rw-r--r--   0 root         (0) root         (0)    59447 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api/user_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:11:36.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/
--rw-r--r--   0 root         (0) root         (0)    28570 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3761 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/inline_object.py
--rw-r--r--   0 root         (0) root         (0)     7332 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)     7548 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     7116 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     7197 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     7170 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     7467 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     7143 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     7413 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     7683 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     7521 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     7332 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     7062 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     7143 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     7197 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)     7170 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     7521 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     7305 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)     7521 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)     7521 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     7251 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     7332 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     7305 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     7467 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     7386 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     7143 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     7089 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     7089 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_user.py
--rw-r--r--   0 root         (0) root         (0)     7224 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     7413 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)    14243 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_account.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_account_mode.py
--rw-r--r--   0 root         (0) root         (0)     2909 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_account_type.py
--rw-r--r--   0 root         (0) root         (0)    30788 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)    21693 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     2937 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py
--rw-r--r--   0 root         (0) root         (0)    10199 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     2986 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_alert_category.py
--rw-r--r--   0 root         (0) root         (0)     2913 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_alert_group_query.py
--rw-r--r--   0 root         (0) root         (0)     2884 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_alert_severity.py
--rw-r--r--   0 root         (0) root         (0)     5055 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_alert_source.py
--rw-r--r--   0 root         (0) root         (0)     2859 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_alert_source_type.py
--rw-r--r--   0 root         (0) root         (0)    11941 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_anomaly_device_entity.py
--rw-r--r--   0 root         (0) root         (0)     4637 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py
--rw-r--r--   0 root         (0) root         (0)    12034 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     2874 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_anomaly_severity.py
--rw-r--r--   0 root         (0) root         (0)     2899 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_anomaly_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     3113 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_anomaly_type.py
--rw-r--r--   0 root         (0) root         (0)    11006 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_api_token_info.py
--rw-r--r--   0 root         (0) root         (0)    11340 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_application_detection_protocol.py
--rw-r--r--   0 root         (0) root         (0)     5032 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_application_detection_rule.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_application_detection_type.py
--rw-r--r--   0 root         (0) root         (0)     2879 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_application_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     7296 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_application_top_clients_usage.py
--rw-r--r--   0 root         (0) root         (0)     4721 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_assign_devices_country_code_request.py
--rw-r--r--   0 root         (0) root         (0)     4787 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_assign_devices_location_request.py
--rw-r--r--   0 root         (0) root         (0)     4917 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_assign_devices_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     9991 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     2992 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_audit_log_category.py
--rw-r--r--   0 root         (0) root         (0)    15660 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     8802 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_building.py
--rw-r--r--   0 root         (0) root         (0)     9739 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     2844 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_certificate_type.py
--rw-r--r--   0 root         (0) root         (0)    10480 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_change_devices_ibeacon_request.py
--rw-r--r--   0 root         (0) root         (0)     5520 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_change_devices_os_mode_request.py
--rw-r--r--   0 root         (0) root         (0)     4512 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_check_permission_request.py
--rw-r--r--   0 root         (0) root         (0)     4715 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_check_permission_response.py
--rw-r--r--   0 root         (0) root         (0)    10384 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_classification.py
--rw-r--r--   0 root         (0) root         (0)     9146 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     3030 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_classification_type.py
--rw-r--r--   0 root         (0) root         (0)     5159 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_cli_output.py
--rw-r--r--   0 root         (0) root         (0)     3849 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_cli_response_code.py
--rw-r--r--   0 root         (0) root         (0)    36438 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     4736 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_client_field.py
--rw-r--r--   0 root         (0) root         (0)     5121 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_client_summary.py
--rw-r--r--   0 root         (0) root         (0)     4155 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_client_usage.py
--rw-r--r--   0 root         (0) root         (0)     2980 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_client_view.py
--rw-r--r--   0 root         (0) root         (0)    13089 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     8577 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     2937 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_connectivity_experience_view_type.py
--rw-r--r--   0 root         (0) root         (0)     2907 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     3006 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     8601 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_copilot_wired_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)    10452 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)     8903 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_country_code.py
--rw-r--r--   0 root         (0) root         (0)     5500 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_building_request.py
--rw-r--r--   0 root         (0) root         (0)     6857 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     5894 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     5416 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)    13024 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)    11802 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)    11599 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_floor_request.py
--rw-r--r--   0 root         (0) root         (0)    32292 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     3786 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)    19020 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     4576 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_location_request.py
--rw-r--r--   0 root         (0) root         (0)     5395 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     4469 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_organization_request.py
--rw-r--r--   0 root         (0) root         (0)    18199 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     5564 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_radius_client.py
--rw-r--r--   0 root         (0) root         (0)    15073 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     5735 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)    13169 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)     7342 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)    15879 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     4740 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     6656 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_user_request.py
--rw-r--r--   0 root         (0) root         (0)     5112 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     7192 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     6670 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_webhook_subscription_request.py
--rw-r--r--   0 root         (0) root         (0)     6440 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     6706 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     4292 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_data_point.py
--rw-r--r--   0 root         (0) root         (0)     7368 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_date_time_type.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_date_time_unit_type.py
--rw-r--r--   0 root         (0) root         (0)     3706 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_default_device_password.py
--rw-r--r--   0 root         (0) root         (0)     3766 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     4587 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_delivery_settings.py
--rw-r--r--   0 root         (0) root         (0)     3661 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_dell_devices.py
--rw-r--r--   0 root         (0) root         (0)     5048 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_deployment_overview.py
--rw-r--r--   0 root         (0) root         (0)     6472 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_deployment_policy.py
--rw-r--r--   0 root         (0) root         (0)     4442 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_deployment_request.py
--rw-r--r--   0 root         (0) root         (0)     3464 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_deployment_response.py
--rw-r--r--   0 root         (0) root         (0)     8691 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_deployment_status.py
--rw-r--r--   0 root         (0) root         (0)    28834 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     2965 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_admin_state.py
--rw-r--r--   0 root         (0) root         (0)     8198 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     5362 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_cpu_memory_usage.py
--rw-r--r--   0 root         (0) root         (0)     4262 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_field.py
--rw-r--r--   0 root         (0) root         (0)     3376 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_filter.py
--rw-r--r--   0 root         (0) root         (0)     3236 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_function.py
--rw-r--r--   0 root         (0) root         (0)     9175 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_ibeacon.py
--rw-r--r--   0 root         (0) root         (0)     5439 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_level_ssid.py
--rw-r--r--   0 root         (0) root         (0)     4957 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)    14406 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_location.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_location_assignment.py
--rw-r--r--   0 root         (0) root         (0)     2838 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     5418 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_stats.py
--rw-r--r--   0 root         (0) root         (0)     2890 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_type.py
--rw-r--r--   0 root         (0) root         (0)     2956 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_view.py
--rw-r--r--   0 root         (0) root         (0)     8665 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)    13080 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_email_template.py
--rw-r--r--   0 root         (0) root         (0)    19288 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_entitlement_type.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_error.py
--rw-r--r--   0 root         (0) root         (0)     3521 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_exos_devices.py
--rw-r--r--   0 root         (0) root         (0)     2918 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_expiration_action_type.py
--rw-r--r--   0 root         (0) root         (0)     8372 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_expiration_settings.py
--rw-r--r--   0 root         (0) root         (0)     3011 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_expiration_type.py
--rw-r--r--   0 root         (0) root         (0)     9135 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_external_account.py
--rw-r--r--   0 root         (0) root         (0)    13975 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     8094 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)    15642 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_external_user_directory.py
--rw-r--r--   0 root         (0) root         (0)     5339 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_external_user_directory_entry.py
--rw-r--r--   0 root         (0) root         (0)     2938 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_external_user_directory_type.py
--rw-r--r--   0 root         (0) root         (0)     3545 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_extreme_devices.py
--rw-r--r--   0 root         (0) root         (0)     6249 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_firmware_activate_option.py
--rw-r--r--   0 root         (0) root         (0)     5507 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_firmware_upgrade_policy.py
--rw-r--r--   0 root         (0) root         (0)     6362 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_flap_count_entity.py
--rw-r--r--   0 root         (0) root         (0)    15299 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_floor.py
--rw-r--r--   0 root         (0) root         (0)     3089 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_forensic_bucket.py
--rw-r--r--   0 root         (0) root         (0)     5813 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_generate_api_token_request.py
--rw-r--r--   0 root         (0) root         (0)     9829 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_generate_api_token_response.py
--rw-r--r--   0 root         (0) root         (0)     6336 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_get_port_assignment_details_response.py
--rw-r--r--   0 root         (0) root         (0)     5581 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_grant_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)     5021 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_hiq_context.py
--rw-r--r--   0 root         (0) root         (0)     3580 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_hiq_status.py
--rw-r--r--   0 root         (0) root         (0)     5920 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_init_key_based_pcg_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     4703 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_initialize_location_request.py
--rw-r--r--   0 root         (0) root         (0)     9687 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)    34396 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     3013 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     3180 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py
--rw-r--r--   0 root         (0) root         (0)    10730 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_key_based_pcg.py
--rw-r--r--   0 root         (0) root         (0)     9190 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_key_based_pcg_user.py
--rw-r--r--   0 root         (0) root         (0)     5806 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py
--rw-r--r--   0 root         (0) root         (0)     7343 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_l3_address_profile.py
--rw-r--r--   0 root         (0) root         (0)     2890 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_l3_address_type.py
--rw-r--r--   0 root         (0) root         (0)     2854 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ldap_protocol_type.py
--rw-r--r--   0 root         (0) root         (0)    18839 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     2921 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ldap_server_verification_mode.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_license_mode.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_license_status.py
--rw-r--r--   0 root         (0) root         (0)    11042 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_location.py
--rw-r--r--   0 root         (0) root         (0)     4025 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_location_legend.py
--rw-r--r--   0 root         (0) root         (0)     2874 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_location_type.py
--rw-r--r--   0 root         (0) root         (0)     4525 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_login_request.py
--rw-r--r--   0 root         (0) root         (0)     5818 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_login_response.py
--rw-r--r--   0 root         (0) root         (0)     2853 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_measurement_unit.py
--rw-r--r--   0 root         (0) root         (0)     9804 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     3084 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_network_policy_field.py
--rw-r--r--   0 root         (0) root         (0)     3377 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_network_policy_type.py
--rw-r--r--   0 root         (0) root         (0)     2858 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_network_policy_view.py
--rw-r--r--   0 root         (0) root         (0)     6078 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_onboard_device_request.py
--rw-r--r--   0 root         (0) root         (0)     5597 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py
--rw-r--r--   0 root         (0) root         (0)    12063 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_operation_metadata.py
--rw-r--r--   0 root         (0) root         (0)     6798 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_operation_object.py
--rw-r--r--   0 root         (0) root         (0)     3009 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_operation_status.py
--rw-r--r--   0 root         (0) root         (0)     8614 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_organization.py
--rw-r--r--   0 root         (0) root         (0)     2869 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_organization_type.py
--rw-r--r--   0 root         (0) root         (0)     3135 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_password_character_type.py
--rw-r--r--   0 root         (0) root         (0)     2865 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_password_db_location.py
--rw-r--r--   0 root         (0) root         (0)    10247 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_password_settings.py
--rw-r--r--   0 root         (0) root         (0)     2841 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_password_type.py
--rw-r--r--   0 root         (0) root         (0)     3937 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_assign_ports_request.py
--rw-r--r--   0 root         (0) root         (0)     6201 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_assign_ports_response.py
--rw-r--r--   0 root         (0) root         (0)     6696 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_port_assignment.py
--rw-r--r--   0 root         (0) root         (0)    10512 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_port_assignment_entry.py
--rw-r--r--   0 root         (0) root         (0)     9628 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py
--rw-r--r--   0 root         (0) root         (0)     9870 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py
--rw-r--r--   0 root         (0) root         (0)    11649 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py
--rw-r--r--   0 root         (0) root         (0)     2842 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_type.py
--rw-r--r--   0 root         (0) root         (0)     5441 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_permission.py
--rw-r--r--   0 root         (0) root         (0)     4632 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_poe_flapping_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     7189 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_post_expiration_action.py
--rw-r--r--   0 root         (0) root         (0)     2938 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_psk_generation_method.py
--rw-r--r--   0 root         (0) root         (0)     2985 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radio_mode.py
--rw-r--r--   0 root         (0) root         (0)    24026 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     6103 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_client.py
--rw-r--r--   0 root         (0) root         (0)    17440 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_client_object_entry.py
--rw-r--r--   0 root         (0) root         (0)     3058 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_client_object_type.py
--rw-r--r--   0 root         (0) root         (0)    13996 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     2907 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_proxy_format_type.py
--rw-r--r--   0 root         (0) root         (0)     6300 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     2923 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_server_type.py
--rw-r--r--   0 root         (0) root         (0)     3812 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_regenerate_end_user_password_response.py
--rw-r--r--   0 root         (0) root         (0)     3200 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rf_environment_type.py
--rw-r--r--   0 root         (0) root         (0)    31139 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rp_channel_selection.py
--rw-r--r--   0 root         (0) root         (0)    11298 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     8919 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rp_miscellaneous_settings.py
--rw-r--r--   0 root         (0) root         (0)    12893 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rp_neighborhood_analysis.py
--rw-r--r--   0 root         (0) root         (0)    50567 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rp_radio_usage_optimization.py
--rw-r--r--   0 root         (0) root         (0)     8500 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rp_sensor_scan_settings.py
--rw-r--r--   0 root         (0) root         (0)    12157 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rp_wmm_qos_settings.py
--rw-r--r--   0 root         (0) root         (0)     4444 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_send_cli_request.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_send_cli_response.py
--rw-r--r--   0 root         (0) root         (0)     2911 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_server_role.py
--rw-r--r--   0 root         (0) root         (0)     9305 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py
--rw-r--r--   0 root         (0) root         (0)    13068 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py
--rw-r--r--   0 root         (0) root         (0)    10196 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py
--rw-r--r--   0 root         (0) root         (0)    14920 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py
--rw-r--r--   0 root         (0) root         (0)    11002 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     2916 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_sms_log_status.py
--rw-r--r--   0 root         (0) root         (0)    10606 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_sms_template.py
--rw-r--r--   0 root         (0) root         (0)     2850 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_sort_order.py
--rw-r--r--   0 root         (0) root         (0)     9632 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     2971 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     2992 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_dot1x_key_management.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_key_type.py
--rw-r--r--   0 root         (0) root         (0)     2928 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_ppsk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_psk_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     2960 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_psk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     2850 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_sae_group.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_wep_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     2921 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_wep_default_key.py
--rw-r--r--   0 root         (0) root         (0)     2888 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_wep_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     2879 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_wep_key_management.py
--rw-r--r--   0 root         (0) root         (0)     3176 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_subscription_data_type.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_subscription_message_type.py
--rw-r--r--   0 root         (0) root         (0)     2880 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_subscription_status.py
--rw-r--r--   0 root         (0) root         (0)     6384 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_top_applications_usage.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_trend_indicator.py
--rw-r--r--   0 root         (0) root         (0)     5030 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_building_request.py
--rw-r--r--   0 root         (0) root         (0)     6859 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     5906 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     5262 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)     6260 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)    10732 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)    10501 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)    13896 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_user.py
--rw-r--r--   0 root         (0) root         (0)     4393 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)    10458 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_floor_request.py
--rw-r--r--   0 root         (0) root         (0)    29854 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     3786 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)    16311 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     4263 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_location_request.py
--rw-r--r--   0 root         (0) root         (0)     5087 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)    18045 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_radius_client.py
--rw-r--r--   0 root         (0) root         (0)    13978 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6534 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)    11162 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)    31686 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_rp_channel_selection_request.py
--rw-r--r--   0 root         (0) root         (0)     7033 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     5656 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py
--rw-r--r--   0 root         (0) root         (0)    10883 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py
--rw-r--r--   0 root         (0) root         (0)    58065 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py
--rw-r--r--   0 root         (0) root         (0)     5907 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py
--rw-r--r--   0 root         (0) root         (0)    11171 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py
--rw-r--r--   0 root         (0) root         (0)    15879 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     4421 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     6177 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_user_request.py
--rw-r--r--   0 root         (0) root         (0)     5112 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     7192 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)    19133 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     3137 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_user_role.py
--rw-r--r--   0 root         (0) root         (0)     7243 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_valid_daily_settings.py
--rw-r--r--   0 root         (0) root         (0)     5799 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_valid_during_date_settings.py
--rw-r--r--   0 root         (0) root         (0)     6383 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_valid_for_time_period_settings.py
--rw-r--r--   0 root         (0) root         (0)     7741 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_valid_time_period_after_first_login.py
--rw-r--r--   0 root         (0) root         (0)     5242 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py
--rw-r--r--   0 root         (0) root         (0)     2925 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_valid_time_period_after_type.py
--rw-r--r--   0 root         (0) root         (0)     7920 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_viq.py
--rw-r--r--   0 root         (0) root         (0)    13203 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_viq_license.py
--rw-r--r--   0 root         (0) root         (0)     8961 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_vlan_object_classified_entry.py
--rw-r--r--   0 root         (0) root         (0)    10998 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_vlan_profile_filter.py
--rw-r--r--   0 root         (0) root         (0)     3521 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_voss_devices.py
--rw-r--r--   0 root         (0) root         (0)    11214 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_webhook_subscription.py
--rw-r--r--   0 root         (0) root         (0)     3682 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wing_devices.py
--rw-r--r--   0 root         (0) root         (0)     8402 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)     7173 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wired_hardware_entity.py
--rw-r--r--   0 root         (0) root         (0)     3853 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wired_hardware_response.py
--rw-r--r--   0 root         (0) root         (0)     4583 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wired_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)     2827 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wired_view_type.py
--rw-r--r--   0 root         (0) root         (0)     7144 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_apps_response.py
--rw-r--r--   0 root         (0) root         (0)     4027 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py
--rw-r--r--   0 root         (0) root         (0)     8513 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_event_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_if_name.py
--rw-r--r--   0 root         (0) root         (0)     9193 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_performance_entity.py
--rw-r--r--   0 root         (0) root         (0)     5556 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_performance_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     5774 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)    13565 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py
--rw-r--r--   0 root         (0) root         (0)     3957 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_time_to_connect_response.py
--rw-r--r--   0 root         (0) root         (0)     2865 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_views_list_type.py
--rw-r--r--   0 root         (0) root         (0)     3834 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_views_type_response.py
--rw-r--r--   0 root         (0) root         (0)    30510 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26259 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/api_client.py
--rw-r--r--   0 root         (0) root         (0)    12883 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/configuration.py
--rw-r--r--   0 root         (0) root         (0)     3801 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    12333 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/extremecloudiq/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:11:36.000000 extremecloudiq-api-23.2.0.4/extremecloudiq_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      375 2023-04-13 17:11:36.000000 extremecloudiq-api-23.2.0.4/extremecloudiq_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    32720 2023-04-13 17:11:36.000000 extremecloudiq-api-23.2.0.4/extremecloudiq_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 17:11:36.000000 extremecloudiq-api-23.2.0.4/extremecloudiq_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-04-13 17:11:36.000000 extremecloudiq-api-23.2.0.4/extremecloudiq_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-13 17:11:36.000000 extremecloudiq-api-23.2.0.4/extremecloudiq_api.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:11:36.000000 extremecloudiq-api-23.2.0.4/test/
--rw-r--r--   0 root         (0) root         (0)     1912 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/test/test_account_api.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/test/test_alert_api.py
--rw-r--r--   0 root         (0) root         (0)     1294 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/test/test_application_api.py
--rw-r--r--   0 root         (0) root         (0)     1077 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/test/test_authentication_api.py
--rw-r--r--   0 root         (0) root         (0)     1572 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/test/test_authorization_api.py
--rw-r--r--   0 root         (0) root         (0)     1325 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/test/test_client_api.py
--rw-r--r--   0 root         (0) root         (0)     6221 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/test/test_configuration___authentication_api.py
--rw-r--r--   0 root         (0) root         (0)     1736 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/test/test_configuration___basic_api.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/test/test_configuration___certificate_api.py
--rw-r--r--   0 root         (0) root         (0)     1339 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/test/test_configuration___deployment_api.py
--rw-r--r--   0 root         (0) root         (0)     9450 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/test/test_configuration___policy_api.py
--rw-r--r--   0 root         (0) root         (0)     4801 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/test/test_configuration___user_management_api.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/test/test_copilot___anomalies_api.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/test/test_copilot___connectivity_experience_api.py
--rw-r--r--   0 root         (0) root         (0)     7736 2023-02-16 12:13:08.000000 extremecloudiq-api-23.2.0.4/test/test_device_api.py
--rw-r--r--   0 root         (0) root         (0)     2467 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/test/test_hiq_api.py
--rw-r--r--   0 root         (0) root         (0)     1449 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_inline_object.py
--rw-r--r--   0 root         (0) root         (0)     2472 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/test/test_location_api.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/test/test_log_api.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/test/test_network_policy_api.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/test/test_notification_api.py
--rw-r--r--   0 root         (0) root         (0)     1250 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/test/test_operation_api.py
--rw-r--r--   0 root         (0) root         (0)     3344 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)     3019 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     2487 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     2681 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     2491 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     2301 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     3024 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     4077 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     2599 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     2484 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     3559 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     2120 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     2110 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)     4635 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     2793 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     2320 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     3042 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     3197 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     2459 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     2210 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     2549 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_user.py
--rw-r--r--   0 root         (0) root         (0)     6281 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     4284 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     2200 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_paged_xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/test/test_user_api.py
--rw-r--r--   0 root         (0) root         (0)     2380 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_account.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_account_mode.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_account_type.py
--rw-r--r--   0 root         (0) root         (0)     2669 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)     2647 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     1681 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_active_directory_server_base_dn_fetch_mode.py
--rw-r--r--   0 root         (0) root         (0)     2160 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     1418 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_alert_category.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_alert_group_query.py
--rw-r--r--   0 root         (0) root         (0)     1418 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_alert_severity.py
--rw-r--r--   0 root         (0) root         (0)     1505 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_alert_source.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_alert_source_type.py
--rw-r--r--   0 root         (0) root         (0)     1883 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_anomaly_device_entity.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_anomaly_devices_by_location_response.py
--rw-r--r--   0 root         (0) root         (0)     1920 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_anomaly_severity.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_anomaly_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_anomaly_type.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_api_token_info.py
--rw-r--r--   0 root         (0) root         (0)     2371 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     1585 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_application_detection_protocol.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_application_detection_rule.py
--rw-r--r--   0 root         (0) root         (0)     1541 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_application_detection_type.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_application_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_application_top_clients_usage.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_assign_devices_country_code_request.py
--rw-r--r--   0 root         (0) root         (0)     2523 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_assign_devices_location_request.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_assign_devices_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     1957 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_audit_log_category.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_building.py
--rw-r--r--   0 root         (0) root         (0)     2141 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_certificate_type.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_change_devices_ibeacon_request.py
--rw-r--r--   0 root         (0) root         (0)     1793 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_change_devices_os_mode_request.py
--rw-r--r--   0 root         (0) root         (0)     1633 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_check_permission_request.py
--rw-r--r--   0 root         (0) root         (0)     2176 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_check_permission_response.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_classification.py
--rw-r--r--   0 root         (0) root         (0)     2711 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     1473 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_classification_type.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_cli_output.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_cli_response_code.py
--rw-r--r--   0 root         (0) root         (0)     3521 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_client_field.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_client_summary.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_client_usage.py
--rw-r--r--   0 root         (0) root         (0)     1385 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_client_view.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     2261 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     1609 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_connectivity_experience_view_type.py
--rw-r--r--   0 root         (0) root         (0)     1578 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_copilot_events_wired_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_copilot_events_wireless_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     2607 2023-02-16 12:13:05.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     1578 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_copilot_wired_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)     2218 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_copilot_wireless_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_country_code.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_building_request.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     2398 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     1769 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     2099 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_floor_request.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     2499 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_location_request.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     1637 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_organization_request.py
--rw-r--r--   0 root         (0) root         (0)     2040 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_radius_client.py
--rw-r--r--   0 root         (0) root         (0)     2939 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     3015 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)     1816 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     8503 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     2002 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_create_webhook_subscription_request.py
--rw-r--r--   0 root         (0) root         (0)     1594 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     1848 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     1469 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_data_point.py
--rw-r--r--   0 root         (0) root         (0)     1734 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_date_time_type.py
--rw-r--r--   0 root         (0) root         (0)     1455 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_date_time_unit_type.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_default_device_password.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_delete_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_delivery_settings.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_dell_devices.py
--rw-r--r--   0 root         (0) root         (0)     1631 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_deployment_overview.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_deployment_policy.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_deployment_request.py
--rw-r--r--   0 root         (0) root         (0)     1505 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_deployment_response.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_deployment_status.py
--rw-r--r--   0 root         (0) root         (0)     3107 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device_admin_state.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device_cpu_memory_usage.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device_field.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device_filter.py
--rw-r--r--   0 root         (0) root         (0)     1429 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device_function.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device_ibeacon.py
--rw-r--r--   0 root         (0) root         (0)     1565 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device_level_ssid.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)     2366 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device_location.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device_location_assignment.py
--rw-r--r--   0 root         (0) root         (0)     1526 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device_stats.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1385 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device_type.py
--rw-r--r--   0 root         (0) root         (0)     1385 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_device_view.py
--rw-r--r--   0 root         (0) root         (0)     1645 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)     2314 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_email_template.py
--rw-r--r--   0 root         (0) root         (0)     2673 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_entitlement_type.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_error.py
--rw-r--r--   0 root         (0) root         (0)     1537 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_exos_devices.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_expiration_action_type.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_expiration_settings.py
--rw-r--r--   0 root         (0) root         (0)     1429 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_expiration_type.py
--rw-r--r--   0 root         (0) root         (0)     2173 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_external_account.py
--rw-r--r--   0 root         (0) root         (0)     2482 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)     2716 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_external_user_directory.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_external_user_directory_entry.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_external_user_directory_type.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_extreme_devices.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_firmware_activate_option.py
--rw-r--r--   0 root         (0) root         (0)     1704 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_firmware_upgrade_policy.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_flap_count_entity.py
--rw-r--r--   0 root         (0) root         (0)     2504 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_floor.py
--rw-r--r--   0 root         (0) root         (0)     1429 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_forensic_bucket.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_generate_api_token_request.py
--rw-r--r--   0 root         (0) root         (0)     2271 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_generate_api_token_response.py
--rw-r--r--   0 root         (0) root         (0)     5132 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_get_port_assignment_details_response.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_grant_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1625 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_hiq_context.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_hiq_status.py
--rw-r--r--   0 root         (0) root         (0)     2359 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_init_key_based_pcg_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_initialize_location_request.py
--rw-r--r--   0 root         (0) root         (0)     2241 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)     5512 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     1721 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_internal_radius_server_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     1778 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_internal_radius_server_authentication_method_group.py
--rw-r--r--   0 root         (0) root         (0)     2744 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_key_based_pcg.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_key_based_pcg_user.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_key_based_pcg_user_base_info.py
--rw-r--r--   0 root         (0) root         (0)     2084 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_l3_address_profile.py
--rw-r--r--   0 root         (0) root         (0)     1420 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_l3_address_type.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_ldap_protocol_type.py
--rw-r--r--   0 root         (0) root         (0)     2488 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     1565 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_ldap_server_verification_mode.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_license_mode.py
--rw-r--r--   0 root         (0) root         (0)     1418 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_license_status.py
--rw-r--r--   0 root         (0) root         (0)     3474 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_location.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_location_legend.py
--rw-r--r--   0 root         (0) root         (0)     1407 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_location_type.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_login_request.py
--rw-r--r--   0 root         (0) root         (0)     1625 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_login_response.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_measurement_unit.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_network_policy_field.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_network_policy_type.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_network_policy_view.py
--rw-r--r--   0 root         (0) root         (0)     2356 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_onboard_device_request.py
--rw-r--r--   0 root         (0) root         (0)     1837 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_onboard_key_based_pcg_request.py
--rw-r--r--   0 root         (0) root         (0)     2381 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_operation_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3238 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_operation_object.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_operation_status.py
--rw-r--r--   0 root         (0) root         (0)     2074 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_organization.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_organization_type.py
--rw-r--r--   0 root         (0) root         (0)     1508 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_password_character_type.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_password_db_location.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_password_settings.py
--rw-r--r--   0 root         (0) root         (0)     1407 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_password_type.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_assign_ports_request.py
--rw-r--r--   0 root         (0) root         (0)     2956 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_assign_ports_response.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_port_assignment.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_port_assignment_entry.py
--rw-r--r--   0 root         (0) root         (0)     4618 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_port_assignment_entry_detail.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_port_assignment_entry_device_meta.py
--rw-r--r--   0 root         (0) root         (0)     2576 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py
--rw-r--r--   0 root         (0) root         (0)     1352 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_type.py
--rw-r--r--   0 root         (0) root         (0)     1574 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_permission.py
--rw-r--r--   0 root         (0) root         (0)     1910 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_poe_flapping_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1687 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_post_expiration_action.py
--rw-r--r--   0 root         (0) root         (0)     1486 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_psk_generation_method.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_radio_mode.py
--rw-r--r--   0 root         (0) root         (0)     2681 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     1550 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_radius_client.py
--rw-r--r--   0 root         (0) root         (0)     3277 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     1805 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_radius_client_object_entry.py
--rw-r--r--   0 root         (0) root         (0)     1521 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_radius_client_object_type.py
--rw-r--r--   0 root         (0) root         (0)     2806 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_radius_proxy_format_type.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_radius_server_type.py
--rw-r--r--   0 root         (0) root         (0)     1707 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_regenerate_end_user_password_response.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_rf_environment_type.py
--rw-r--r--   0 root         (0) root         (0)     2986 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_rp_channel_selection.py
--rw-r--r--   0 root         (0) root         (0)     2178 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     2833 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_rp_miscellaneous_settings.py
--rw-r--r--   0 root         (0) root         (0)     2306 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_rp_neighborhood_analysis.py
--rw-r--r--   0 root         (0) root         (0)     4357 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_rp_radio_usage_optimization.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_rp_sensor_scan_settings.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_rp_wmm_qos_settings.py
--rw-r--r--   0 root         (0) root         (0)     1911 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_send_cli_request.py
--rw-r--r--   0 root         (0) root         (0)     1778 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_send_cli_response.py
--rw-r--r--   0 root         (0) root         (0)     1385 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_server_role.py
--rw-r--r--   0 root         (0) root         (0)     1956 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_set_ssid_mode_dot1x_request.py
--rw-r--r--   0 root         (0) root         (0)     2169 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_set_ssid_mode_ppsk_request.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-02-16 12:13:06.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_set_ssid_mode_psk_request.py
--rw-r--r--   0 root         (0) root         (0)     2031 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_set_ssid_mode_wep_request.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_sms_log_status.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_sms_template.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_sort_order.py
--rw-r--r--   0 root         (0) root         (0)     2071 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_dot1x_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     1521 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_dot1x_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_key_type.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_ppsk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_psk_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_psk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_sae_group.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_wep_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_wep_default_key.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_wep_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_wep_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_subscription_data_type.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_subscription_message_type.py
--rw-r--r--   0 root         (0) root         (0)     1473 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_subscription_status.py
--rw-r--r--   0 root         (0) root         (0)     1639 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_top_applications_usage.py
--rw-r--r--   0 root         (0) root         (0)     1429 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_trend_indicator.py
--rw-r--r--   0 root         (0) root         (0)     1600 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_building_request.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     2398 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1953 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)     2035 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1830 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_floor_request.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     2077 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     1568 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_location_request.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1618 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_radius_client.py
--rw-r--r--   0 root         (0) root         (0)     2306 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)     2646 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_rp_channel_selection_request.py
--rw-r--r--   0 root         (0) root         (0)     1759 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1756 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_rp_miscellaneous_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_rp_neighborhood_analysis_request.py
--rw-r--r--   0 root         (0) root         (0)     3371 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_rp_radio_usage_optimization_request.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_rp_sensor_scan_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_rp_wmm_qos_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     8503 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1609 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1616 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_update_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     2295 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_user.py
--rw-r--r--   0 root         (0) root         (0)     9059 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     4351 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_user_role.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_valid_daily_settings.py
--rw-r--r--   0 root         (0) root         (0)     2484 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_viq.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_valid_during_date_settings.py
--rw-r--r--   0 root         (0) root         (0)     2275 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_valid_for_time_period_settings.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_valid_time_period_after_first_login.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_valid_time_period_after_id_creation.py
--rw-r--r--   0 root         (0) root         (0)     1545 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_valid_time_period_after_type.py
--rw-r--r--   0 root         (0) root         (0)     2374 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_viq_license.py
--rw-r--r--   0 root         (0) root         (0)     3275 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_vlan_object_classified_entry.py
--rw-r--r--   0 root         (0) root         (0)     3940 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_vlan_profile_filter.py
--rw-r--r--   0 root         (0) root         (0)     1537 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_voss_devices.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_webhook_subscription.py
--rw-r--r--   0 root         (0) root         (0)     1565 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wing_devices.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)     1697 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wired_hardware_entity.py
--rw-r--r--   0 root         (0) root         (0)     1884 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wired_hardware_response.py
--rw-r--r--   0 root         (0) root         (0)     1627 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wired_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)     1420 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wired_view_type.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_apps_response.py
--rw-r--r--   0 root         (0) root         (0)     2438 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_connectivity_performance_response.py
--rw-r--r--   0 root         (0) root         (0)     1809 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_event_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     1431 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_if_name.py
--rw-r--r--   0 root         (0) root         (0)     2065 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_performance_entity.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_performance_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)     2043 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_time_to_connect_entity.py
--rw-r--r--   0 root         (0) root         (0)     2296 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_time_to_connect_response.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_views_list_type.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-02-16 12:13:07.000000 extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_views_type_response.py
--rw-r--r--   0 root         (0) root         (0)    63680 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/README.md
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-13 17:11:36.000000 extremecloudiq-api-23.2.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1123 2023-02-16 12:13:09.000000 extremecloudiq-api-23.2.0.4/setup.py
--rw-r--r--   0 root         (0) root         (0)      375 2023-04-13 17:11:36.000000 extremecloudiq-api-23.2.0.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:12:33.000000 extremecloudiq-api-23.2.1.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:12:33.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:12:33.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-04-07 00:03:30.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32862 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/account_api.py
+-rw-r--r--   0 root         (0) root         (0)    16606 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/alert_api.py
+-rw-r--r--   0 root         (0) root         (0)    24695 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/application_api.py
+-rw-r--r--   0 root         (0) root         (0)    11074 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)    26154 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/authorization_api.py
+-rw-r--r--   0 root         (0) root         (0)    47956 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/client_api.py
+-rw-r--r--   0 root         (0) root         (0)   171864 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/configuration___authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)    34019 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/configuration___basic_api.py
+-rw-r--r--   0 root         (0) root         (0)     7035 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/configuration___certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)    16187 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/configuration___deployment_api.py
+-rw-r--r--   0 root         (0) root         (0)   292852 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/configuration___policy_api.py
+-rw-r--r--   0 root         (0) root         (0)   133457 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/configuration___user_management_api.py
+-rw-r--r--   0 root         (0) root         (0)    45168 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/copilot___anomalies_api.py
+-rw-r--r--   0 root         (0) root         (0)    96668 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/copilot___connectivity_experience_api.py
+-rw-r--r--   0 root         (0) root         (0)   253764 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/device_api.py
+-rw-r--r--   0 root         (0) root         (0)    56014 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/hiq_api.py
+-rw-r--r--   0 root         (0) root         (0)    67517 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/location_api.py
+-rw-r--r--   0 root         (0) root         (0)    45123 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/log_api.py
+-rw-r--r--   0 root         (0) root         (0)    49086 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/network_policy_api.py
+-rw-r--r--   0 root         (0) root         (0)    15844 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/notification_api.py
+-rw-r--r--   0 root         (0) root         (0)    16818 2023-04-07 00:03:30.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/operation_api.py
+-rw-r--r--   0 root         (0) root         (0)    59447 2023-04-07 00:03:30.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api/user_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:12:33.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/
+-rw-r--r--   0 root         (0) root         (0)    30265 2023-04-07 00:03:30.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3761 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/inline_object.py
+-rw-r--r--   0 root         (0) root         (0)     7332 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)     7548 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     7116 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     7197 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     7170 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     7143 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     7413 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     7683 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     7521 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     7332 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     7143 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     7197 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)     7170 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     7521 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     7305 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)     7521 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)     7521 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     7251 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     7332 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     7305 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     7386 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7143 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     7089 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     7089 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7413 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)    14243 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_account.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_account_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2909 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_account_type.py
+-rw-r--r--   0 root         (0) root         (0)    30788 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)    21693 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py
+-rw-r--r--   0 root         (0) root         (0)    10199 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     2986 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_alert_category.py
+-rw-r--r--   0 root         (0) root         (0)     2913 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_alert_group_query.py
+-rw-r--r--   0 root         (0) root         (0)     2884 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_alert_severity.py
+-rw-r--r--   0 root         (0) root         (0)     5055 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_alert_source.py
+-rw-r--r--   0 root         (0) root         (0)     2859 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_alert_source_type.py
+-rw-r--r--   0 root         (0) root         (0)    10206 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_anomalies_count_vo_entity.py
+-rw-r--r--   0 root         (0) root         (0)    11941 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_anomaly_device_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4637 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py
+-rw-r--r--   0 root         (0) root         (0)    12034 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_anomaly_severity.py
+-rw-r--r--   0 root         (0) root         (0)     2899 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_anomaly_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_anomaly_type.py
+-rw-r--r--   0 root         (0) root         (0)    11006 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_api_token_info.py
+-rw-r--r--   0 root         (0) root         (0)    11340 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_application_detection_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     5032 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_application_detection_rule.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_application_detection_type.py
+-rw-r--r--   0 root         (0) root         (0)     2879 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_application_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     7296 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_application_top_clients_usage.py
+-rw-r--r--   0 root         (0) root         (0)     4721 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_assign_devices_country_code_request.py
+-rw-r--r--   0 root         (0) root         (0)     4787 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_assign_devices_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     4917 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_assign_devices_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     5033 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_assurance_scans_overview_response.py
+-rw-r--r--   0 root         (0) root         (0)     9991 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     2992 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_audit_log_category.py
+-rw-r--r--   0 root         (0) root         (0)    15660 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     5199 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_bounce_device_port_data.py
+-rw-r--r--   0 root         (0) root         (0)     4359 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_bounce_device_port_operation_result.py
+-rw-r--r--   0 root         (0) root         (0)     5672 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_bounce_device_port_request.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_bounce_device_port_response.py
+-rw-r--r--   0 root         (0) root         (0)     8802 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_building.py
+-rw-r--r--   0 root         (0) root         (0)     9739 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_certificate_type.py
+-rw-r--r--   0 root         (0) root         (0)    10480 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_change_devices_ibeacon_request.py
+-rw-r--r--   0 root         (0) root         (0)     5520 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_change_devices_os_mode_request.py
+-rw-r--r--   0 root         (0) root         (0)     4512 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_check_permission_request.py
+-rw-r--r--   0 root         (0) root         (0)     4715 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_check_permission_response.py
+-rw-r--r--   0 root         (0) root         (0)    10384 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_classification.py
+-rw-r--r--   0 root         (0) root         (0)     9146 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     3030 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_classification_type.py
+-rw-r--r--   0 root         (0) root         (0)     5159 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_cli_output.py
+-rw-r--r--   0 root         (0) root         (0)     3849 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_cli_response_code.py
+-rw-r--r--   0 root         (0) root         (0)    36438 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     4736 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_client_field.py
+-rw-r--r--   0 root         (0) root         (0)     3459 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_client_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     5121 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_client_summary.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_client_usage.py
+-rw-r--r--   0 root         (0) root         (0)     2980 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_client_view.py
+-rw-r--r--   0 root         (0) root         (0)    13089 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     8577 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_connectivity_experience_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     8903 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_country_code.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     3006 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     8601 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_copilot_wired_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)    10452 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)     5500 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     6857 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     5416 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)    13024 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    11802 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)    11599 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)    32292 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     3786 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)    19020 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     4576 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     4469 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_organization_request.py
+-rw-r--r--   0 root         (0) root         (0)    18199 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     5564 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)    15073 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     5735 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)    13169 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)     7342 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)    15879 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     4740 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     7691 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     5112 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     7192 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_webhook_subscription_request.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     6706 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     4292 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     7368 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_date_time_type.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_date_time_unit_type.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_default_device_password.py
+-rw-r--r--   0 root         (0) root         (0)     3766 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     4587 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_delivery_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3661 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_dell_devices.py
+-rw-r--r--   0 root         (0) root         (0)     5048 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_deployment_overview.py
+-rw-r--r--   0 root         (0) root         (0)     6912 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_deployment_policy.py
+-rw-r--r--   0 root         (0) root         (0)     4442 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_deployment_request.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_deployment_response.py
+-rw-r--r--   0 root         (0) root         (0)     8691 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)    29776 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_admin_state.py
+-rw-r--r--   0 root         (0) root         (0)     8198 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     5362 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_cpu_memory_usage.py
+-rw-r--r--   0 root         (0) root         (0)     4313 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_field.py
+-rw-r--r--   0 root         (0) root         (0)     3376 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_function.py
+-rw-r--r--   0 root         (0) root         (0)     9175 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_ibeacon.py
+-rw-r--r--   0 root         (0) root         (0)    11914 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_installation_report.py
+-rw-r--r--   0 root         (0) root         (0)     5439 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_level_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     4957 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_lldp_cdp_info.py
+-rw-r--r--   0 root         (0) root         (0)    14406 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_location.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_location_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     2838 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     5418 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_stats.py
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_type.py
+-rw-r--r--   0 root         (0) root         (0)     2956 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_view.py
+-rw-r--r--   0 root         (0) root         (0)    29252 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_wifi_interface.py
+-rw-r--r--   0 root         (0) root         (0)     4432 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_dfs_channel_changes_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4606 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_dfs_channel_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     5837 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     4872 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     5411 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_duplex_data_rate_entity.py
+-rw-r--r--   0 root         (0) root         (0)     8665 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)    13080 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_email_template.py
+-rw-r--r--   0 root         (0) root         (0)    19288 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_entitlement_type.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_error.py
+-rw-r--r--   0 root         (0) root         (0)     3521 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_exos_devices.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_expiration_action_type.py
+-rw-r--r--   0 root         (0) root         (0)     8372 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_expiration_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3011 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_expiration_type.py
+-rw-r--r--   0 root         (0) root         (0)     9135 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_external_account.py
+-rw-r--r--   0 root         (0) root         (0)    13975 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)    15642 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_external_user_directory.py
+-rw-r--r--   0 root         (0) root         (0)     5339 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_external_user_directory_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_external_user_directory_type.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_extreme_devices.py
+-rw-r--r--   0 root         (0) root         (0)     6249 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_firmware_activate_option.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_firmware_upgrade_policy.py
+-rw-r--r--   0 root         (0) root         (0)     6362 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_flap_count_entity.py
+-rw-r--r--   0 root         (0) root         (0)    15299 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_floor.py
+-rw-r--r--   0 root         (0) root         (0)     3089 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_forensic_bucket.py
+-rw-r--r--   0 root         (0) root         (0)     5813 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_generate_api_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     9829 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_generate_api_token_response.py
+-rw-r--r--   0 root         (0) root         (0)     6336 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_get_port_assignment_details_response.py
+-rw-r--r--   0 root         (0) root         (0)     6608 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_grant_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     5021 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_hiq_context.py
+-rw-r--r--   0 root         (0) root         (0)     3580 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_hiq_status.py
+-rw-r--r--   0 root         (0) root         (0)     5920 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_init_key_based_pcg_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     4703 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_initialize_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     9687 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)    34396 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     3180 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py
+-rw-r--r--   0 root         (0) root         (0)    10730 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_key_based_pcg.py
+-rw-r--r--   0 root         (0) root         (0)     9190 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_key_based_pcg_user.py
+-rw-r--r--   0 root         (0) root         (0)     5806 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py
+-rw-r--r--   0 root         (0) root         (0)     7343 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_l3_address_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_l3_address_type.py
+-rw-r--r--   0 root         (0) root         (0)     2854 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ldap_protocol_type.py
+-rw-r--r--   0 root         (0) root         (0)    18839 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ldap_server_verification_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_license_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_license_status.py
+-rw-r--r--   0 root         (0) root         (0)    11042 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_location.py
+-rw-r--r--   0 root         (0) root         (0)     4025 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_location_legend.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_location_type.py
+-rw-r--r--   0 root         (0) root         (0)     4525 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_login_request.py
+-rw-r--r--   0 root         (0) root         (0)     5818 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_login_response.py
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_measurement_unit.py
+-rw-r--r--   0 root         (0) root         (0)     9804 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_network_policy_field.py
+-rw-r--r--   0 root         (0) root         (0)     3377 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_network_policy_type.py
+-rw-r--r--   0 root         (0) root         (0)     2858 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_network_policy_view.py
+-rw-r--r--   0 root         (0) root         (0)     6078 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_onboard_device_request.py
+-rw-r--r--   0 root         (0) root         (0)     5597 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py
+-rw-r--r--   0 root         (0) root         (0)    12063 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_operation_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     6798 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_operation_object.py
+-rw-r--r--   0 root         (0) root         (0)     3009 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_operation_status.py
+-rw-r--r--   0 root         (0) root         (0)     8614 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_organization.py
+-rw-r--r--   0 root         (0) root         (0)     2869 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_organization_type.py
+-rw-r--r--   0 root         (0) root         (0)     3135 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_password_character_type.py
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_password_db_location.py
+-rw-r--r--   0 root         (0) root         (0)    10247 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_password_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2841 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_password_type.py
+-rw-r--r--   0 root         (0) root         (0)     3937 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_assign_ports_request.py
+-rw-r--r--   0 root         (0) root         (0)     6201 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_assign_ports_response.py
+-rw-r--r--   0 root         (0) root         (0)     6696 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_port_assignment.py
+-rw-r--r--   0 root         (0) root         (0)    10512 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_port_assignment_entry.py
+-rw-r--r--   0 root         (0) root         (0)     9628 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py
+-rw-r--r--   0 root         (0) root         (0)     9870 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py
+-rw-r--r--   0 root         (0) root         (0)    11649 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_type.py
+-rw-r--r--   0 root         (0) root         (0)     5441 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4632 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_poe_flapping_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     4001 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_port_efficiency_speed_duplex_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     4010 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_port_efficiency_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     7189 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_post_expiration_action.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_psk_generation_method.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radio_mode.py
+-rw-r--r--   0 root         (0) root         (0)    24026 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     6103 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)    17440 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_client_object_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3058 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_client_object_type.py
+-rw-r--r--   0 root         (0) root         (0)    13996 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_proxy_format_type.py
+-rw-r--r--   0 root         (0) root         (0)     6300 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_server_type.py
+-rw-r--r--   0 root         (0) root         (0)     3812 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_regenerate_end_user_password_response.py
+-rw-r--r--   0 root         (0) root         (0)     3200 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rf_environment_type.py
+-rw-r--r--   0 root         (0) root         (0)    31139 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rp_channel_selection.py
+-rw-r--r--   0 root         (0) root         (0)    11298 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     8919 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rp_miscellaneous_settings.py
+-rw-r--r--   0 root         (0) root         (0)    12893 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rp_neighborhood_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    50567 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rp_radio_usage_optimization.py
+-rw-r--r--   0 root         (0) root         (0)     8500 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rp_sensor_scan_settings.py
+-rw-r--r--   0 root         (0) root         (0)    12157 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rp_wmm_qos_settings.py
+-rw-r--r--   0 root         (0) root         (0)     4444 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_send_cli_request.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_send_cli_response.py
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_server_role.py
+-rw-r--r--   0 root         (0) root         (0)     9305 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py
+-rw-r--r--   0 root         (0) root         (0)    13068 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py
+-rw-r--r--   0 root         (0) root         (0)    10196 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py
+-rw-r--r--   0 root         (0) root         (0)    14920 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py
+-rw-r--r--   0 root         (0) root         (0)    11002 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     2916 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_sms_log_status.py
+-rw-r--r--   0 root         (0) root         (0)    10606 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_sms_template.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_sort_order.py
+-rw-r--r--   0 root         (0) root         (0)     5339 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_speed_duplex_entity.py
+-rw-r--r--   0 root         (0) root         (0)     9632 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     2992 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_dot1x_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_key_type.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_ppsk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_psk_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_psk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_sae_group.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_wep_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_wep_default_key.py
+-rw-r--r--   0 root         (0) root         (0)     2888 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_wep_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     2879 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_wep_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     3176 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_subscription_data_type.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_subscription_message_type.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_subscription_status.py
+-rw-r--r--   0 root         (0) root         (0)     6384 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_top_applications_usage.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_trend_indicator.py
+-rw-r--r--   0 root         (0) root         (0)     5030 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     6859 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     5906 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     5262 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     6260 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)    10732 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    10501 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     5312 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    10458 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)    29854 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     3786 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)    16311 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     4263 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     5087 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)    18045 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)    13978 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6534 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)    11162 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)    31686 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_rp_channel_selection_request.py
+-rw-r--r--   0 root         (0) root         (0)     7033 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     5656 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)    10883 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py
+-rw-r--r--   0 root         (0) root         (0)    58065 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py
+-rw-r--r--   0 root         (0) root         (0)     5907 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)    11171 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)    15879 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     4421 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     6940 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     5112 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     7192 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)    14729 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)    19133 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_user_role.py
+-rw-r--r--   0 root         (0) root         (0)     7243 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_valid_daily_settings.py
+-rw-r--r--   0 root         (0) root         (0)     5799 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_valid_during_date_settings.py
+-rw-r--r--   0 root         (0) root         (0)     6383 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_valid_for_time_period_settings.py
+-rw-r--r--   0 root         (0) root         (0)     7741 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_valid_time_period_after_first_login.py
+-rw-r--r--   0 root         (0) root         (0)     5242 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py
+-rw-r--r--   0 root         (0) root         (0)     2925 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_valid_time_period_after_type.py
+-rw-r--r--   0 root         (0) root         (0)     7920 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_viq.py
+-rw-r--r--   0 root         (0) root         (0)    13203 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_viq_license.py
+-rw-r--r--   0 root         (0) root         (0)     8961 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_vlan_object_classified_entry.py
+-rw-r--r--   0 root         (0) root         (0)    10998 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_vlan_profile_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3521 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_voss_devices.py
+-rw-r--r--   0 root         (0) root         (0)    11214 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_webhook_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     3682 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wing_devices.py
+-rw-r--r--   0 root         (0) root         (0)     8402 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)     7173 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wired_hardware_entity.py
+-rw-r--r--   0 root         (0) root         (0)     3853 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wired_hardware_response.py
+-rw-r--r--   0 root         (0) root         (0)     4583 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wired_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wired_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_apps_response.py
+-rw-r--r--   0 root         (0) root         (0)     4027 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py
+-rw-r--r--   0 root         (0) root         (0)     8513 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_event_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_if_name.py
+-rw-r--r--   0 root         (0) root         (0)     9193 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_performance_entity.py
+-rw-r--r--   0 root         (0) root         (0)     5556 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_performance_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     5774 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)    13565 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py
+-rw-r--r--   0 root         (0) root         (0)     3957 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_time_to_connect_response.py
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_views_list_type.py
+-rw-r--r--   0 root         (0) root         (0)     3834 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_views_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    32205 2023-04-07 00:03:30.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26259 2023-04-07 00:03:30.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    12883 2023-04-07 00:03:30.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2023-04-07 00:03:30.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12333 2023-04-07 00:03:30.000000 extremecloudiq-api-23.2.1.4/extremecloudiq/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:12:33.000000 extremecloudiq-api-23.2.1.4/extremecloudiq_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      375 2023-04-13 17:12:33.000000 extremecloudiq-api-23.2.1.4/extremecloudiq_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    34560 2023-04-13 17:12:33.000000 extremecloudiq-api-23.2.1.4/extremecloudiq_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 17:12:33.000000 extremecloudiq-api-23.2.1.4/extremecloudiq_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-13 17:12:33.000000 extremecloudiq-api-23.2.1.4/extremecloudiq_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-13 17:12:33.000000 extremecloudiq-api-23.2.1.4/extremecloudiq_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:12:33.000000 extremecloudiq-api-23.2.1.4/test/
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_account_api.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_alert_api.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_application_api.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_authorization_api.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_client_api.py
+-rw-r--r--   0 root         (0) root         (0)     6221 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_configuration___authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_configuration___basic_api.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_configuration___certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_configuration___deployment_api.py
+-rw-r--r--   0 root         (0) root         (0)     9450 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_configuration___policy_api.py
+-rw-r--r--   0 root         (0) root         (0)     4801 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_configuration___user_management_api.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_copilot___anomalies_api.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_copilot___connectivity_experience_api.py
+-rw-r--r--   0 root         (0) root         (0)     8298 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_device_api.py
+-rw-r--r--   0 root         (0) root         (0)     2467 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_hiq_api.py
+-rw-r--r--   0 root         (0) root         (0)     1449 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_inline_object.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_location_api.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_log_api.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_network_policy_api.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-04-07 00:03:29.000000 extremecloudiq-api-23.2.1.4/test/test_notification_api.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2023-04-07 00:03:30.000000 extremecloudiq-api-23.2.1.4/test/test_operation_api.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)     3019 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     2681 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     2491 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     3024 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     4077 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     2599 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     3937 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3042 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     3197 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     2653 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)     6281 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     4284 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2200 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_paged_xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-04-07 00:03:30.000000 extremecloudiq-api-23.2.1.4/test/test_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_account.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_account_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_account_type.py
+-rw-r--r--   0 root         (0) root         (0)     2669 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_active_directory_server_base_dn_fetch_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_alert_category.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_alert_group_query.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_alert_severity.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_alert_source.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_alert_source_type.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_anomalies_count_vo_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_anomaly_device_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_anomaly_devices_by_location_response.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_anomaly_severity.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_anomaly_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_anomaly_type.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_api_token_info.py
+-rw-r--r--   0 root         (0) root         (0)     2371 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_application_detection_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_application_detection_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_application_detection_type.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_application_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_application_top_clients_usage.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_assign_devices_country_code_request.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_assign_devices_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_assign_devices_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     2182 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_assurance_scans_overview_response.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_audit_log_category.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_bounce_device_port_data.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_bounce_device_port_operation_result.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_bounce_device_port_request.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_bounce_device_port_response.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_building.py
+-rw-r--r--   0 root         (0) root         (0)     2141 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_certificate_type.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_change_devices_ibeacon_request.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_change_devices_os_mode_request.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_check_permission_request.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_check_permission_response.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_classification.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_classification_type.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_cli_output.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_cli_response_code.py
+-rw-r--r--   0 root         (0) root         (0)     3521 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_client_field.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_client_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_client_summary.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_client_usage.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_client_view.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     1609 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_connectivity_experience_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_copilot_events_wired_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_copilot_events_wireless_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_copilot_wired_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_copilot_wireless_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_country_code.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-04-07 00:03:26.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     2099 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_organization_request.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     8503 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_create_webhook_subscription_request.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_date_time_type.py
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_date_time_unit_type.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_default_device_password.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_delete_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_delivery_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_dell_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_deployment_overview.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_deployment_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_deployment_request.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_deployment_response.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_admin_state.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_cpu_memory_usage.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_field.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_function.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_ibeacon.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_installation_report.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_level_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_lldp_cdp_info.py
+-rw-r--r--   0 root         (0) root         (0)     2366 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_location.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_location_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_type.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_view.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_device_wifi_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_dfs_channel_changes_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_dfs_channel_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_dfs_recurence_channel_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_dfs_recurence_count_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_duplex_data_rate_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_email_template.py
+-rw-r--r--   0 root         (0) root         (0)     2673 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_entitlement_type.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_error.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_exos_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_expiration_action_type.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_expiration_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_expiration_type.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_external_account.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_external_user_directory.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_external_user_directory_entry.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_external_user_directory_type.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_extreme_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_firmware_activate_option.py
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_firmware_upgrade_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_flap_count_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_floor.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_forensic_bucket.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_generate_api_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_generate_api_token_response.py
+-rw-r--r--   0 root         (0) root         (0)     5132 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_get_port_assignment_details_response.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_grant_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_hiq_context.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_hiq_status.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_init_key_based_pcg_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_initialize_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)     5512 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     1721 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_internal_radius_server_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     1778 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_internal_radius_server_authentication_method_group.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_key_based_pcg.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_key_based_pcg_user.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_key_based_pcg_user_base_info.py
+-rw-r--r--   0 root         (0) root         (0)     2084 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_l3_address_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_l3_address_type.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_ldap_protocol_type.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_ldap_server_verification_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_license_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_license_status.py
+-rw-r--r--   0 root         (0) root         (0)     3474 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_location.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_location_legend.py
+-rw-r--r--   0 root         (0) root         (0)     1407 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_location_type.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_login_request.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_login_response.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_measurement_unit.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_network_policy_field.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_network_policy_type.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_network_policy_view.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_onboard_device_request.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_onboard_key_based_pcg_request.py
+-rw-r--r--   0 root         (0) root         (0)     2381 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_operation_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3238 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_operation_object.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_operation_status.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_organization.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_organization_type.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_password_character_type.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_password_db_location.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_password_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1407 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_password_type.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_assign_ports_request.py
+-rw-r--r--   0 root         (0) root         (0)     2956 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_assign_ports_response.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_port_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_port_assignment_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4618 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_port_assignment_entry_detail.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_port_assignment_entry_device_meta.py
+-rw-r--r--   0 root         (0) root         (0)     2576 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_type.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_permission.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_poe_flapping_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_port_efficiency_speed_duplex_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_port_efficiency_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_post_expiration_action.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_psk_generation_method.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_radio_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2681 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)     3277 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     1805 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_radius_client_object_entry.py
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_radius_client_object_type.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_radius_proxy_format_type.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_radius_server_type.py
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_regenerate_end_user_password_response.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_rf_environment_type.py
+-rw-r--r--   0 root         (0) root         (0)     2986 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_rp_channel_selection.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2833 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_rp_miscellaneous_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2306 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_rp_neighborhood_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     4357 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_rp_radio_usage_optimization.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_rp_sensor_scan_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_rp_wmm_qos_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_send_cli_request.py
+-rw-r--r--   0 root         (0) root         (0)     1778 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_send_cli_response.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_server_role.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_set_ssid_mode_dot1x_request.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_set_ssid_mode_ppsk_request.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_set_ssid_mode_psk_request.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_set_ssid_mode_wep_request.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-04-07 00:03:27.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_sms_log_status.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_sms_template.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_sort_order.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_speed_duplex_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_dot1x_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_dot1x_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_key_type.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_ppsk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_psk_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_psk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_sae_group.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_wep_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_wep_default_key.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_wep_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_wep_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_subscription_data_type.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_subscription_message_type.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_subscription_status.py
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_top_applications_usage.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_trend_indicator.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     1568 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)     2306 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)     2646 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_rp_channel_selection_request.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_rp_miscellaneous_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_rp_neighborhood_analysis_request.py
+-rw-r--r--   0 root         (0) root         (0)     3371 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_rp_radio_usage_optimization_request.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_rp_sensor_scan_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_rp_wmm_qos_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     8503 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1609 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_update_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     9059 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     4351 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_user_role.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_valid_daily_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_valid_during_date_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_valid_for_time_period_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_valid_time_period_after_first_login.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_valid_time_period_after_id_creation.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_valid_time_period_after_type.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_viq.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_viq_license.py
+-rw-r--r--   0 root         (0) root         (0)     3275 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_vlan_object_classified_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3940 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_vlan_profile_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_voss_devices.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_webhook_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wing_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wired_hardware_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wired_hardware_response.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wired_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wired_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_apps_response.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_connectivity_performance_response.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_event_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1431 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_if_name.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_performance_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_performance_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_time_to_connect_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_time_to_connect_response.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_views_list_type.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-04-07 00:03:28.000000 extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_views_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    66662 2023-04-07 00:03:30.000000 extremecloudiq-api-23.2.1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-13 17:12:33.000000 extremecloudiq-api-23.2.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-04-07 00:03:30.000000 extremecloudiq-api-23.2.1.4/setup.py
+-rw-r--r--   0 root         (0) root         (0)      375 2023-04-13 17:12:33.000000 extremecloudiq-api-23.2.1.4/PKG-INFO
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/__init__.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/__init__.py`

 * *Files identical despite different names*

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/account_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/account_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/alert_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/alert_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/application_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/application_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/authentication_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/authorization_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/authorization_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/client_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/configuration___basic_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -21,122 +21,228 @@
 from extremecloudiq.api_client import ApiClient
 from extremecloudiq.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ClientApi(object):
+class ConfigurationBasicApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def get_client(self, id, **kwargs):  # noqa: E501
-        """Get client info  # noqa: E501
+    def create_vlan_profile(self, xiq_create_vlan_profile_request, **kwargs):  # noqa: E501
+        """Create VLAN profile  # noqa: E501
 
-        Get client detailed information.  # noqa: E501
+        Create a new VLAN profile.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_client(id, async_req=True)
+        >>> thread = api.create_vlan_profile(xiq_create_vlan_profile_request, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param int id: The client ID (required)
-        :param list[XiqClientView] views: The views to return client fields (Check fields for each view at XiqClientView schema)
-        :param list[XiqClientField] fields: The client fields to return
+        :param XiqCreateVlanProfileRequest xiq_create_vlan_profile_request: The payload to create new VLAN profile (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: XiqClient
+        :return: XiqVlanProfile
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_client_with_http_info(id, **kwargs)  # noqa: E501
+        return self.create_vlan_profile_with_http_info(xiq_create_vlan_profile_request, **kwargs)  # noqa: E501
 
-    def get_client_with_http_info(self, id, **kwargs):  # noqa: E501
-        """Get client info  # noqa: E501
+    def create_vlan_profile_with_http_info(self, xiq_create_vlan_profile_request, **kwargs):  # noqa: E501
+        """Create VLAN profile  # noqa: E501
 
-        Get client detailed information.  # noqa: E501
+        Create a new VLAN profile.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_client_with_http_info(id, async_req=True)
+        >>> thread = api.create_vlan_profile_with_http_info(xiq_create_vlan_profile_request, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param int id: The client ID (required)
-        :param list[XiqClientView] views: The views to return client fields (Check fields for each view at XiqClientView schema)
-        :param list[XiqClientField] fields: The client fields to return
+        :param XiqCreateVlanProfileRequest xiq_create_vlan_profile_request: The payload to create new VLAN profile (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(XiqClient, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(XiqVlanProfile, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id',
-            'views',
-            'fields'
+            'xiq_create_vlan_profile_request'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_vlan_profile" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'xiq_create_vlan_profile_request' is set
+        if self.api_client.client_side_validation and ('xiq_create_vlan_profile_request' not in local_var_params or  # noqa: E501
+                                                        local_var_params['xiq_create_vlan_profile_request'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `xiq_create_vlan_profile_request` when calling `create_vlan_profile`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'xiq_create_vlan_profile_request' in local_var_params:
+            body_params = local_var_params['xiq_create_vlan_profile_request']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/vlan-profiles', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='XiqVlanProfile',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def delete_vlan_profile(self, id, **kwargs):  # noqa: E501
+        """Delete a VLAN profile  # noqa: E501
+
+        Delete a specific VLAN profile by ID.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_vlan_profile(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int id: The VLAN profile ID (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.delete_vlan_profile_with_http_info(id, **kwargs)  # noqa: E501
+
+    def delete_vlan_profile_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Delete a VLAN profile  # noqa: E501
+
+        Delete a specific VLAN profile by ID.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_vlan_profile_with_http_info(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int id: The VLAN profile ID (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_client" % key
+                    " to method delete_vlan_profile" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `get_client`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `delete_vlan_profile`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
-        if 'views' in local_var_params and local_var_params['views'] is not None:  # noqa: E501
-            query_params.append(('views', local_var_params['views']))  # noqa: E501
-            collection_formats['views'] = 'multi'  # noqa: E501
-        if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
-            query_params.append(('fields', local_var_params['fields']))  # noqa: E501
-            collection_formats['fields'] = 'multi'  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -144,267 +250,236 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['BearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/clients/{id}', 'GET',
+            '/vlan-profiles/{id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='XiqClient',  # noqa: E501
+            response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_client_summary(self, **kwargs):  # noqa: E501
-        """Get client summary metrics  # noqa: E501
+    def delete_vlan_profiles(self, xiq_vlan_profile_filter, **kwargs):  # noqa: E501
+        """[LRO] Delete VLAN profiles  # noqa: E501
 
-        Get number of connected wireless clients and number of detected wired clients.  # noqa: E501
+        Delete VLAN profiles.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_client_summary(async_req=True)
+        >>> thread = api.delete_vlan_profiles(xiq_vlan_profile_filter, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param list[int] location_ids: The location IDs
-        :param list[int] device_ids: The device IDs
-        :param list[int] vlans: The associate VLAN IDs
-        :param list[str] user_profile_names: The user profile names
-        :param list[str] ssids: The SSIDs
+        :param XiqVlanProfileFilter xiq_vlan_profile_filter: (required)
+        :param bool _async: Whether to enable async mode
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: XiqClientSummary
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_client_summary_with_http_info(**kwargs)  # noqa: E501
+        return self.delete_vlan_profiles_with_http_info(xiq_vlan_profile_filter, **kwargs)  # noqa: E501
 
-    def get_client_summary_with_http_info(self, **kwargs):  # noqa: E501
-        """Get client summary metrics  # noqa: E501
+    def delete_vlan_profiles_with_http_info(self, xiq_vlan_profile_filter, **kwargs):  # noqa: E501
+        """[LRO] Delete VLAN profiles  # noqa: E501
 
-        Get number of connected wireless clients and number of detected wired clients.  # noqa: E501
+        Delete VLAN profiles.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_client_summary_with_http_info(async_req=True)
+        >>> thread = api.delete_vlan_profiles_with_http_info(xiq_vlan_profile_filter, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param list[int] location_ids: The location IDs
-        :param list[int] device_ids: The device IDs
-        :param list[int] vlans: The associate VLAN IDs
-        :param list[str] user_profile_names: The user profile names
-        :param list[str] ssids: The SSIDs
+        :param XiqVlanProfileFilter xiq_vlan_profile_filter: (required)
+        :param bool _async: Whether to enable async mode
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(XiqClientSummary, status_code(int), headers(HTTPHeaderDict))
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'location_ids',
-            'device_ids',
-            'vlans',
-            'user_profile_names',
-            'ssids'
+            'xiq_vlan_profile_filter',
+            '_async'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_client_summary" % key
+                    " to method delete_vlan_profiles" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'xiq_vlan_profile_filter' is set
+        if self.api_client.client_side_validation and ('xiq_vlan_profile_filter' not in local_var_params or  # noqa: E501
+                                                        local_var_params['xiq_vlan_profile_filter'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `xiq_vlan_profile_filter` when calling `delete_vlan_profiles`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'location_ids' in local_var_params and local_var_params['location_ids'] is not None:  # noqa: E501
-            query_params.append(('locationIds', local_var_params['location_ids']))  # noqa: E501
-            collection_formats['locationIds'] = 'multi'  # noqa: E501
-        if 'device_ids' in local_var_params and local_var_params['device_ids'] is not None:  # noqa: E501
-            query_params.append(('deviceIds', local_var_params['device_ids']))  # noqa: E501
-            collection_formats['deviceIds'] = 'multi'  # noqa: E501
-        if 'vlans' in local_var_params and local_var_params['vlans'] is not None:  # noqa: E501
-            query_params.append(('vlans', local_var_params['vlans']))  # noqa: E501
-            collection_formats['vlans'] = 'multi'  # noqa: E501
-        if 'user_profile_names' in local_var_params and local_var_params['user_profile_names'] is not None:  # noqa: E501
-            query_params.append(('userProfileNames', local_var_params['user_profile_names']))  # noqa: E501
-            collection_formats['userProfileNames'] = 'multi'  # noqa: E501
-        if 'ssids' in local_var_params and local_var_params['ssids'] is not None:  # noqa: E501
-            query_params.append(('ssids', local_var_params['ssids']))  # noqa: E501
-            collection_formats['ssids'] = 'multi'  # noqa: E501
+        if '_async' in local_var_params and local_var_params['_async'] is not None:  # noqa: E501
+            query_params.append(('async', local_var_params['_async']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'xiq_vlan_profile_filter' in local_var_params:
+            body_params = local_var_params['xiq_vlan_profile_filter']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
         # Authentication setting
         auth_settings = ['BearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/clients/summary', 'GET',
+            '/vlan-profiles/:delete', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='XiqClientSummary',  # noqa: E501
+            response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_client_usage(self, client_ids, start_time, end_time, **kwargs):  # noqa: E501
-        """Get usage per client  # noqa: E501
+    def get_vlan_profile(self, id, **kwargs):  # noqa: E501
+        """Get a VLAN profile  # noqa: E501
 
-        Get the client usage.  # noqa: E501
+        Get a specific VLAN profile by ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_client_usage(client_ids, start_time, end_time, async_req=True)
+        >>> thread = api.get_vlan_profile(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param list[int] client_ids: The client IDs (required)
-        :param int start_time: The start time to query, epoch time in milliseconds since 1/1/1970 (required)
-        :param int end_time: The end time to query, epoch time in milliseconds since 1/1/1970 (required)
+        :param int id: The VLAN profile ID (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: list[XiqClientUsage]
+        :return: XiqVlanProfile
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_client_usage_with_http_info(client_ids, start_time, end_time, **kwargs)  # noqa: E501
+        return self.get_vlan_profile_with_http_info(id, **kwargs)  # noqa: E501
 
-    def get_client_usage_with_http_info(self, client_ids, start_time, end_time, **kwargs):  # noqa: E501
-        """Get usage per client  # noqa: E501
+    def get_vlan_profile_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Get a VLAN profile  # noqa: E501
 
-        Get the client usage.  # noqa: E501
+        Get a specific VLAN profile by ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_client_usage_with_http_info(client_ids, start_time, end_time, async_req=True)
+        >>> thread = api.get_vlan_profile_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param list[int] client_ids: The client IDs (required)
-        :param int start_time: The start time to query, epoch time in milliseconds since 1/1/1970 (required)
-        :param int end_time: The end time to query, epoch time in milliseconds since 1/1/1970 (required)
+        :param int id: The VLAN profile ID (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(list[XiqClientUsage], status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(XiqVlanProfile, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'client_ids',
-            'start_time',
-            'end_time'
+            'id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_client_usage" % key
+                    " to method get_vlan_profile" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'client_ids' is set
-        if self.api_client.client_side_validation and ('client_ids' not in local_var_params or  # noqa: E501
-                                                        local_var_params['client_ids'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `client_ids` when calling `get_client_usage`")  # noqa: E501
-        # verify the required parameter 'start_time' is set
-        if self.api_client.client_side_validation and ('start_time' not in local_var_params or  # noqa: E501
-                                                        local_var_params['start_time'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `start_time` when calling `get_client_usage`")  # noqa: E501
-        # verify the required parameter 'end_time' is set
-        if self.api_client.client_side_validation and ('end_time' not in local_var_params or  # noqa: E501
-                                                        local_var_params['end_time'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `end_time` when calling `get_client_usage`")  # noqa: E501
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `get_vlan_profile`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
-        if 'client_ids' in local_var_params and local_var_params['client_ids'] is not None:  # noqa: E501
-            query_params.append(('clientIds', local_var_params['client_ids']))  # noqa: E501
-            collection_formats['clientIds'] = 'multi'  # noqa: E501
-        if 'start_time' in local_var_params and local_var_params['start_time'] is not None:  # noqa: E501
-            query_params.append(('startTime', local_var_params['start_time']))  # noqa: E501
-        if 'end_time' in local_var_params and local_var_params['end_time'] is not None:  # noqa: E501
-            query_params.append(('endTime', local_var_params['end_time']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -412,162 +487,120 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['BearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/clients/usage', 'GET',
+            '/vlan-profiles/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='list[XiqClientUsage]',  # noqa: E501
+            response_type='XiqVlanProfile',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def list_active_clients(self, **kwargs):  # noqa: E501
-        """List active clients  # noqa: E501
+    def list_vlan_profiles(self, **kwargs):  # noqa: E501
+        """List VLAN profiles  # noqa: E501
 
-        List active clients with filters and pagination.  # noqa: E501
+        Get a page of VLAN profiles.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.list_active_clients(async_req=True)
+        >>> thread = api.list_vlan_profiles(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param list[int] location_ids: The location IDs
-        :param list[int] device_ids: The device IDs
-        :param list[int] vlans: The associate vlan IDs
-        :param list[str] user_profile_names: The user profile names
-        :param list[str] ssids: The SSIDs
         :param int page: Page number, min = 1
         :param int limit: Page Size, min = 1, max = 100
-        :param list[XiqClientView] views: The views to return client fields (Check fields for each view at XiqClientView schema)
-        :param list[XiqClientField] fields: The client fields to return
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: PagedXiqClient
+        :return: PagedXiqVlanProfile
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_active_clients_with_http_info(**kwargs)  # noqa: E501
+        return self.list_vlan_profiles_with_http_info(**kwargs)  # noqa: E501
 
-    def list_active_clients_with_http_info(self, **kwargs):  # noqa: E501
-        """List active clients  # noqa: E501
+    def list_vlan_profiles_with_http_info(self, **kwargs):  # noqa: E501
+        """List VLAN profiles  # noqa: E501
 
-        List active clients with filters and pagination.  # noqa: E501
+        Get a page of VLAN profiles.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.list_active_clients_with_http_info(async_req=True)
+        >>> thread = api.list_vlan_profiles_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param list[int] location_ids: The location IDs
-        :param list[int] device_ids: The device IDs
-        :param list[int] vlans: The associate vlan IDs
-        :param list[str] user_profile_names: The user profile names
-        :param list[str] ssids: The SSIDs
         :param int page: Page number, min = 1
         :param int limit: Page Size, min = 1, max = 100
-        :param list[XiqClientView] views: The views to return client fields (Check fields for each view at XiqClientView schema)
-        :param list[XiqClientField] fields: The client fields to return
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(PagedXiqClient, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(PagedXiqVlanProfile, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'location_ids',
-            'device_ids',
-            'vlans',
-            'user_profile_names',
-            'ssids',
             'page',
-            'limit',
-            'views',
-            'fields'
+            'limit'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_active_clients" % key
+                    " to method list_vlan_profiles" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
 
         if self.api_client.client_side_validation and 'page' in local_var_params and local_var_params['page'] < 1:  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `page` when calling `list_active_clients`, must be a value greater than or equal to `1`")  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `page` when calling `list_vlan_profiles`, must be a value greater than or equal to `1`")  # noqa: E501
         if self.api_client.client_side_validation and 'limit' in local_var_params and local_var_params['limit'] > 100:  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `limit` when calling `list_active_clients`, must be a value less than or equal to `100`")  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `limit` when calling `list_vlan_profiles`, must be a value less than or equal to `100`")  # noqa: E501
         if self.api_client.client_side_validation and 'limit' in local_var_params and local_var_params['limit'] < 1:  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `limit` when calling `list_active_clients`, must be a value greater than or equal to `1`")  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `limit` when calling `list_vlan_profiles`, must be a value greater than or equal to `1`")  # noqa: E501
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'location_ids' in local_var_params and local_var_params['location_ids'] is not None:  # noqa: E501
-            query_params.append(('locationIds', local_var_params['location_ids']))  # noqa: E501
-            collection_formats['locationIds'] = 'multi'  # noqa: E501
-        if 'device_ids' in local_var_params and local_var_params['device_ids'] is not None:  # noqa: E501
-            query_params.append(('deviceIds', local_var_params['device_ids']))  # noqa: E501
-            collection_formats['deviceIds'] = 'multi'  # noqa: E501
-        if 'vlans' in local_var_params and local_var_params['vlans'] is not None:  # noqa: E501
-            query_params.append(('vlans', local_var_params['vlans']))  # noqa: E501
-            collection_formats['vlans'] = 'multi'  # noqa: E501
-        if 'user_profile_names' in local_var_params and local_var_params['user_profile_names'] is not None:  # noqa: E501
-            query_params.append(('userProfileNames', local_var_params['user_profile_names']))  # noqa: E501
-            collection_formats['userProfileNames'] = 'multi'  # noqa: E501
-        if 'ssids' in local_var_params and local_var_params['ssids'] is not None:  # noqa: E501
-            query_params.append(('ssids', local_var_params['ssids']))  # noqa: E501
-            collection_formats['ssids'] = 'multi'  # noqa: E501
         if 'page' in local_var_params and local_var_params['page'] is not None:  # noqa: E501
             query_params.append(('page', local_var_params['page']))  # noqa: E501
         if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
             query_params.append(('limit', local_var_params['limit']))  # noqa: E501
-        if 'views' in local_var_params and local_var_params['views'] is not None:  # noqa: E501
-            query_params.append(('views', local_var_params['views']))  # noqa: E501
-            collection_formats['views'] = 'multi'  # noqa: E501
-        if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
-            query_params.append(('fields', local_var_params['fields']))  # noqa: E501
-            collection_formats['fields'] = 'multi'  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -575,21 +608,148 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['BearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/clients/active', 'GET',
+            '/vlan-profiles', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PagedXiqVlanProfile',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def update_vlan_profile(self, id, xiq_update_vlan_profile_request, **kwargs):  # noqa: E501
+        """Update a VLAN profile  # noqa: E501
+
+        Update a specific VLAN profile.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.update_vlan_profile(id, xiq_update_vlan_profile_request, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int id: The VLAN profile ID. (required)
+        :param XiqUpdateVlanProfileRequest xiq_update_vlan_profile_request: The payload to update VLAN profile (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: XiqVlanProfile
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.update_vlan_profile_with_http_info(id, xiq_update_vlan_profile_request, **kwargs)  # noqa: E501
+
+    def update_vlan_profile_with_http_info(self, id, xiq_update_vlan_profile_request, **kwargs):  # noqa: E501
+        """Update a VLAN profile  # noqa: E501
+
+        Update a specific VLAN profile.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.update_vlan_profile_with_http_info(id, xiq_update_vlan_profile_request, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int id: The VLAN profile ID. (required)
+        :param XiqUpdateVlanProfileRequest xiq_update_vlan_profile_request: The payload to update VLAN profile (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(XiqVlanProfile, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'id',
+            'xiq_update_vlan_profile_request'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_vlan_profile" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `update_vlan_profile`")  # noqa: E501
+        # verify the required parameter 'xiq_update_vlan_profile_request' is set
+        if self.api_client.client_side_validation and ('xiq_update_vlan_profile_request' not in local_var_params or  # noqa: E501
+                                                        local_var_params['xiq_update_vlan_profile_request'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `xiq_update_vlan_profile_request` when calling `update_vlan_profile`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'xiq_update_vlan_profile_request' in local_var_params:
+            body_params = local_var_params['xiq_update_vlan_profile_request']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/vlan-profiles/{id}', 'PATCH',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PagedXiqClient',  # noqa: E501
+            response_type='XiqVlanProfile',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/configuration___authentication_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/configuration___authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/configuration___certificate_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/configuration___certificate_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/configuration___deployment_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/configuration___deployment_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/configuration___policy_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/configuration___policy_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/configuration___user_management_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/configuration___user_management_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/copilot___anomalies_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/operation_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -21,109 +21,110 @@
 from extremecloudiq.api_client import ApiClient
 from extremecloudiq.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class CopilotAnomaliesApi(object):
+class OperationApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def get_devices_by_location(self, **kwargs):  # noqa: E501
-        """get_devices_by_location  # noqa: E501
+    def cancel_operation(self, operation_id, **kwargs):  # noqa: E501
+        """Cancel Long-Running Operation (LRO)  # noqa: E501
 
+        When the cancelable is true in operation metadata the clients are allowed to send a cancel request to ask the backend to cancel the operation. The server makes its best effort to cancel the operation, but success is not guaranteed.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_devices_by_location(async_req=True)
+        >>> thread = api.cancel_operation(operation_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param XiqAnomalyType anomaly_type: Anomaly type
-        :param int location_id: The location id
+        :param str operation_id: The operation ID (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: XiqAnomalyDevicesByLocationResponse
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_devices_by_location_with_http_info(**kwargs)  # noqa: E501
+        return self.cancel_operation_with_http_info(operation_id, **kwargs)  # noqa: E501
 
-    def get_devices_by_location_with_http_info(self, **kwargs):  # noqa: E501
-        """get_devices_by_location  # noqa: E501
+    def cancel_operation_with_http_info(self, operation_id, **kwargs):  # noqa: E501
+        """Cancel Long-Running Operation (LRO)  # noqa: E501
 
+        When the cancelable is true in operation metadata the clients are allowed to send a cancel request to ask the backend to cancel the operation. The server makes its best effort to cancel the operation, but success is not guaranteed.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_devices_by_location_with_http_info(async_req=True)
+        >>> thread = api.cancel_operation_with_http_info(operation_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param XiqAnomalyType anomaly_type: Anomaly type
-        :param int location_id: The location id
+        :param str operation_id: The operation ID (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(XiqAnomalyDevicesByLocationResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'anomaly_type',
-            'location_id'
+            'operation_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_devices_by_location" % key
+                    " to method cancel_operation" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'operation_id' is set
+        if self.api_client.client_side_validation and ('operation_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['operation_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `operation_id` when calling `cancel_operation`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'operation_id' in local_var_params:
+            path_params['operationId'] = local_var_params['operation_id']  # noqa: E501
 
         query_params = []
-        if 'anomaly_type' in local_var_params and local_var_params['anomaly_type'] is not None:  # noqa: E501
-            query_params.append(('anomalyType', local_var_params['anomaly_type']))  # noqa: E501
-        if 'location_id' in local_var_params and local_var_params['location_id'] is not None:  # noqa: E501
-            query_params.append(('locationId', local_var_params['location_id']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -131,116 +132,113 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['BearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/copilot/anomalies/devices-by-location', 'GET',
+            '/operations/{operationId}/:cancel', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='XiqAnomalyDevicesByLocationResponse',  # noqa: E501
+            response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_poe_flapping_stats(self, anomaly_id, **kwargs):  # noqa: E501
-        """get_poe_flapping_stats  # noqa: E501
+    def delete_operation(self, operation_id, **kwargs):  # noqa: E501
+        """Delete Long-Running Operation (LRO)  # noqa: E501
 
+        The Long-Running Operation (LRO) can be deleted when the operation is done or in PENDING status.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_poe_flapping_stats(anomaly_id, async_req=True)
+        >>> thread = api.delete_operation(operation_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str anomaly_id: The anomaly id (required)
-        :param int location_id: The location id
+        :param str operation_id: The operation ID (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: XiqPoeFlappingStatsResponse
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_poe_flapping_stats_with_http_info(anomaly_id, **kwargs)  # noqa: E501
+        return self.delete_operation_with_http_info(operation_id, **kwargs)  # noqa: E501
 
-    def get_poe_flapping_stats_with_http_info(self, anomaly_id, **kwargs):  # noqa: E501
-        """get_poe_flapping_stats  # noqa: E501
+    def delete_operation_with_http_info(self, operation_id, **kwargs):  # noqa: E501
+        """Delete Long-Running Operation (LRO)  # noqa: E501
 
+        The Long-Running Operation (LRO) can be deleted when the operation is done or in PENDING status.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_poe_flapping_stats_with_http_info(anomaly_id, async_req=True)
+        >>> thread = api.delete_operation_with_http_info(operation_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str anomaly_id: The anomaly id (required)
-        :param int location_id: The location id
+        :param str operation_id: The operation ID (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(XiqPoeFlappingStatsResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'anomaly_id',
-            'location_id'
+            'operation_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_poe_flapping_stats" % key
+                    " to method delete_operation" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'anomaly_id' is set
-        if self.api_client.client_side_validation and ('anomaly_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['anomaly_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `anomaly_id` when calling `get_poe_flapping_stats`")  # noqa: E501
+        # verify the required parameter 'operation_id' is set
+        if self.api_client.client_side_validation and ('operation_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['operation_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `operation_id` when calling `delete_operation`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'operation_id' in local_var_params:
+            path_params['operationId'] = local_var_params['operation_id']  # noqa: E501
 
         query_params = []
-        if 'anomaly_id' in local_var_params and local_var_params['anomaly_id'] is not None:  # noqa: E501
-            query_params.append(('anomalyId', local_var_params['anomaly_id']))  # noqa: E501
-        if 'location_id' in local_var_params and local_var_params['location_id'] is not None:  # noqa: E501
-            query_params.append(('locationId', local_var_params['location_id']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -248,138 +246,113 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['BearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/copilot/anomalies/poeflapping/stats', 'GET',
+            '/operations/{operationId}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='XiqPoeFlappingStatsResponse',  # noqa: E501
+            response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def list_anomaly_locations(self, **kwargs):  # noqa: E501
-        """list_anomaly_locations  # noqa: E501
+    def get_operation(self, operation_id, **kwargs):  # noqa: E501
+        """Get Long-Running Operation (LRO) status and result  # noqa: E501
 
+        Get the Long-Running Operation (LRO) status and result. The response will include either result or error if the operation is done.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.list_anomaly_locations(async_req=True)
+        >>> thread = api.get_operation(operation_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param XiqAnomalyType anomaly_type: Anomaly type
-        :param int page: Page number, min = 1
-        :param int limit: Number of Records, min = 1, max = 100
-        :param XiqAnomalySortField sort_field: sort by field
-        :param XiqSortOrder sort_order: The sorting order
-        :param bool exclude_muted: exclude muted
+        :param str operation_id: The operation ID (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: XiqCopilotPagedXiqAnomalyLocationEntity
+        :return: XiqOperationObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_anomaly_locations_with_http_info(**kwargs)  # noqa: E501
+        return self.get_operation_with_http_info(operation_id, **kwargs)  # noqa: E501
 
-    def list_anomaly_locations_with_http_info(self, **kwargs):  # noqa: E501
-        """list_anomaly_locations  # noqa: E501
+    def get_operation_with_http_info(self, operation_id, **kwargs):  # noqa: E501
+        """Get Long-Running Operation (LRO) status and result  # noqa: E501
 
+        Get the Long-Running Operation (LRO) status and result. The response will include either result or error if the operation is done.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.list_anomaly_locations_with_http_info(async_req=True)
+        >>> thread = api.get_operation_with_http_info(operation_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param XiqAnomalyType anomaly_type: Anomaly type
-        :param int page: Page number, min = 1
-        :param int limit: Number of Records, min = 1, max = 100
-        :param XiqAnomalySortField sort_field: sort by field
-        :param XiqSortOrder sort_order: The sorting order
-        :param bool exclude_muted: exclude muted
+        :param str operation_id: The operation ID (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(XiqCopilotPagedXiqAnomalyLocationEntity, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(XiqOperationObject, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'anomaly_type',
-            'page',
-            'limit',
-            'sort_field',
-            'sort_order',
-            'exclude_muted'
+            'operation_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_anomaly_locations" % key
+                    " to method get_operation" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'operation_id' is set
+        if self.api_client.client_side_validation and ('operation_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['operation_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `operation_id` when calling `get_operation`")  # noqa: E501
 
-        if self.api_client.client_side_validation and 'page' in local_var_params and local_var_params['page'] < 1:  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `page` when calling `list_anomaly_locations`, must be a value greater than or equal to `1`")  # noqa: E501
-        if self.api_client.client_side_validation and 'limit' in local_var_params and local_var_params['limit'] > 100:  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `limit` when calling `list_anomaly_locations`, must be a value less than or equal to `100`")  # noqa: E501
-        if self.api_client.client_side_validation and 'limit' in local_var_params and local_var_params['limit'] < 1:  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `limit` when calling `list_anomaly_locations`, must be a value greater than or equal to `1`")  # noqa: E501
         collection_formats = {}
 
         path_params = {}
+        if 'operation_id' in local_var_params:
+            path_params['operationId'] = local_var_params['operation_id']  # noqa: E501
 
         query_params = []
-        if 'anomaly_type' in local_var_params and local_var_params['anomaly_type'] is not None:  # noqa: E501
-            query_params.append(('anomalyType', local_var_params['anomaly_type']))  # noqa: E501
-        if 'page' in local_var_params and local_var_params['page'] is not None:  # noqa: E501
-            query_params.append(('page', local_var_params['page']))  # noqa: E501
-        if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
-            query_params.append(('limit', local_var_params['limit']))  # noqa: E501
-        if 'sort_field' in local_var_params and local_var_params['sort_field'] is not None:  # noqa: E501
-            query_params.append(('sortField', local_var_params['sort_field']))  # noqa: E501
-        if 'sort_order' in local_var_params and local_var_params['sort_order'] is not None:  # noqa: E501
-            query_params.append(('sortOrder', local_var_params['sort_order']))  # noqa: E501
-        if 'exclude_muted' in local_var_params and local_var_params['exclude_muted'] is not None:  # noqa: E501
-            query_params.append(('excludeMuted', local_var_params['exclude_muted']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -387,21 +360,21 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['BearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/copilot/anomalies/locations', 'GET',
+            '/operations/{operationId}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='XiqCopilotPagedXiqAnomalyLocationEntity',  # noqa: E501
+            response_type='XiqOperationObject',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/copilot___connectivity_experience_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/copilot___connectivity_experience_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/device_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/device_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -761,14 +761,141 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def bounce_device_port(self, id, xiq_bounce_device_port_request, **kwargs):  # noqa: E501
+        """Bounce port of a device (EXOS, VOSS and SR Switches  # noqa: E501
+
+        Bounce port for the given device id.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.bounce_device_port(id, xiq_bounce_device_port_request, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int id: The device id (required)
+        :param XiqBounceDevicePortRequest xiq_bounce_device_port_request: (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: XiqBounceDevicePortResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.bounce_device_port_with_http_info(id, xiq_bounce_device_port_request, **kwargs)  # noqa: E501
+
+    def bounce_device_port_with_http_info(self, id, xiq_bounce_device_port_request, **kwargs):  # noqa: E501
+        """Bounce port of a device (EXOS, VOSS and SR Switches  # noqa: E501
+
+        Bounce port for the given device id.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.bounce_device_port_with_http_info(id, xiq_bounce_device_port_request, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int id: The device id (required)
+        :param XiqBounceDevicePortRequest xiq_bounce_device_port_request: (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(XiqBounceDevicePortResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'id',
+            'xiq_bounce_device_port_request'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method bounce_device_port" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `bounce_device_port`")  # noqa: E501
+        # verify the required parameter 'xiq_bounce_device_port_request' is set
+        if self.api_client.client_side_validation and ('xiq_bounce_device_port_request' not in local_var_params or  # noqa: E501
+                                                        local_var_params['xiq_bounce_device_port_request'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `xiq_bounce_device_port_request` when calling `bounce_device_port`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'xiq_bounce_device_port_request' in local_var_params:
+            body_params = local_var_params['xiq_bounce_device_port_request']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/devices/{id}/bounce-port', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='XiqBounceDevicePortResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def change_device_description(self, id, body, **kwargs):  # noqa: E501
         """Change description for a device  # noqa: E501
 
         Change description for a specific device.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.change_device_description(id, body, async_req=True)
@@ -2903,14 +3030,260 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def get_device_wifi_interface(self, id, start_time, end_time, **kwargs):  # noqa: E501
+        """Get the device WiFi interfaces stats  # noqa: E501
+
+        Get the device WiFi interfaces stats by device ID.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_device_wifi_interface(id, start_time, end_time, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int id: The device ID (required)
+        :param int start_time: The start time for collecting the wifi interfaces stat (required)
+        :param int end_time: The end time for collecting the wifi interfaces stat (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: list[XiqDeviceWifiInterface]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_device_wifi_interface_with_http_info(id, start_time, end_time, **kwargs)  # noqa: E501
+
+    def get_device_wifi_interface_with_http_info(self, id, start_time, end_time, **kwargs):  # noqa: E501
+        """Get the device WiFi interfaces stats  # noqa: E501
+
+        Get the device WiFi interfaces stats by device ID.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_device_wifi_interface_with_http_info(id, start_time, end_time, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int id: The device ID (required)
+        :param int start_time: The start time for collecting the wifi interfaces stat (required)
+        :param int end_time: The end time for collecting the wifi interfaces stat (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(list[XiqDeviceWifiInterface], status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'id',
+            'start_time',
+            'end_time'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_device_wifi_interface" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `get_device_wifi_interface`")  # noqa: E501
+        # verify the required parameter 'start_time' is set
+        if self.api_client.client_side_validation and ('start_time' not in local_var_params or  # noqa: E501
+                                                        local_var_params['start_time'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `start_time` when calling `get_device_wifi_interface`")  # noqa: E501
+        # verify the required parameter 'end_time' is set
+        if self.api_client.client_side_validation and ('end_time' not in local_var_params or  # noqa: E501
+                                                        local_var_params['end_time'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `end_time` when calling `get_device_wifi_interface`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+
+        query_params = []
+        if 'start_time' in local_var_params and local_var_params['start_time'] is not None:  # noqa: E501
+            query_params.append(('startTime', local_var_params['start_time']))  # noqa: E501
+        if 'end_time' in local_var_params and local_var_params['end_time'] is not None:  # noqa: E501
+            query_params.append(('endTime', local_var_params['end_time']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/devices/{id}/interfaces/wifi', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[XiqDeviceWifiInterface]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_xiq_device_installation_report(self, id, **kwargs):  # noqa: E501
+        """Get device installation report  # noqa: E501
+
+        Get device installation report of a specific device.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_xiq_device_installation_report(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int id: The device ID (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: XiqDeviceInstallationReport
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_xiq_device_installation_report_with_http_info(id, **kwargs)  # noqa: E501
+
+    def get_xiq_device_installation_report_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Get device installation report  # noqa: E501
+
+        Get device installation report of a specific device.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_xiq_device_installation_report_with_http_info(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int id: The device ID (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(XiqDeviceInstallationReport, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_xiq_device_installation_report" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `get_xiq_device_installation_report`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/devices/{id}/installation-report', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='XiqDeviceInstallationReport',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def list_device_alarm(self, id, start_time, end_time, **kwargs):  # noqa: E501
         """List alarms for a device  # noqa: E501
 
         List alarms for a specific device.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_device_alarm(id, start_time, end_time, async_req=True)
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/hiq_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/hiq_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/location_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/location_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/log_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/log_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -190,14 +190,15 @@
         :param async_req bool: execute request asynchronously
         :param int page: Page number, min = 1
         :param int limit: Page Size, min = 1, max = 100
         :param list[XiqAuditLogCategory] categories: Audit category
         :param str username: The user login name
         :param int start_time: The start time to query, epoch time in milliseconds since 1/1/1970, default is 0 if not specified or is negative
         :param int end_time: The end time to query, epoch time in milliseconds since 1/1/1970, default is now if not specified or is negative
+        :param str keyword: The case-insensitive keyword to search in description
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -220,14 +221,15 @@
         :param async_req bool: execute request asynchronously
         :param int page: Page number, min = 1
         :param int limit: Page Size, min = 1, max = 100
         :param list[XiqAuditLogCategory] categories: Audit category
         :param str username: The user login name
         :param int start_time: The start time to query, epoch time in milliseconds since 1/1/1970, default is 0 if not specified or is negative
         :param int end_time: The end time to query, epoch time in milliseconds since 1/1/1970, default is now if not specified or is negative
+        :param str keyword: The case-insensitive keyword to search in description
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -242,15 +244,16 @@
 
         all_params = [
             'page',
             'limit',
             'categories',
             'username',
             'start_time',
-            'end_time'
+            'end_time',
+            'keyword'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -286,14 +289,16 @@
             collection_formats['categories'] = 'multi'  # noqa: E501
         if 'username' in local_var_params and local_var_params['username'] is not None:  # noqa: E501
             query_params.append(('username', local_var_params['username']))  # noqa: E501
         if 'start_time' in local_var_params and local_var_params['start_time'] is not None:  # noqa: E501
             query_params.append(('startTime', local_var_params['start_time']))  # noqa: E501
         if 'end_time' in local_var_params and local_var_params['end_time'] is not None:  # noqa: E501
             query_params.append(('endTime', local_var_params['end_time']))  # noqa: E501
+        if 'keyword' in local_var_params and local_var_params['keyword'] is not None:  # noqa: E501
+            query_params.append(('keyword', local_var_params['keyword']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/network_policy_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/network_policy_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/notification_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/notification_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api/user_api.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/__init__.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -59,14 +59,15 @@
 from extremecloudiq.models.xiq_active_directory_server_base_dn_fetch_mode import XiqActiveDirectoryServerBaseDnFetchMode
 from extremecloudiq.models.xiq_alert import XiqAlert
 from extremecloudiq.models.xiq_alert_category import XiqAlertCategory
 from extremecloudiq.models.xiq_alert_group_query import XiqAlertGroupQuery
 from extremecloudiq.models.xiq_alert_severity import XiqAlertSeverity
 from extremecloudiq.models.xiq_alert_source import XiqAlertSource
 from extremecloudiq.models.xiq_alert_source_type import XiqAlertSourceType
+from extremecloudiq.models.xiq_anomalies_count_vo_entity import XiqAnomaliesCountVoEntity
 from extremecloudiq.models.xiq_anomaly_device_entity import XiqAnomalyDeviceEntity
 from extremecloudiq.models.xiq_anomaly_devices_by_location_response import XiqAnomalyDevicesByLocationResponse
 from extremecloudiq.models.xiq_anomaly_location_entity import XiqAnomalyLocationEntity
 from extremecloudiq.models.xiq_anomaly_severity import XiqAnomalySeverity
 from extremecloudiq.models.xiq_anomaly_sort_field import XiqAnomalySortField
 from extremecloudiq.models.xiq_anomaly_type import XiqAnomalyType
 from extremecloudiq.models.xiq_api_token_info import XiqApiTokenInfo
@@ -75,31 +76,37 @@
 from extremecloudiq.models.xiq_application_detection_rule import XiqApplicationDetectionRule
 from extremecloudiq.models.xiq_application_detection_type import XiqApplicationDetectionType
 from extremecloudiq.models.xiq_application_sort_field import XiqApplicationSortField
 from extremecloudiq.models.xiq_application_top_clients_usage import XiqApplicationTopClientsUsage
 from extremecloudiq.models.xiq_assign_devices_country_code_request import XiqAssignDevicesCountryCodeRequest
 from extremecloudiq.models.xiq_assign_devices_location_request import XiqAssignDevicesLocationRequest
 from extremecloudiq.models.xiq_assign_devices_network_policy_request import XiqAssignDevicesNetworkPolicyRequest
+from extremecloudiq.models.xiq_assurance_scans_overview_response import XiqAssuranceScansOverviewResponse
 from extremecloudiq.models.xiq_audit_log import XiqAuditLog
 from extremecloudiq.models.xiq_audit_log_category import XiqAuditLogCategory
 from extremecloudiq.models.xiq_auth_log import XiqAuthLog
+from extremecloudiq.models.xiq_bounce_device_port_data import XiqBounceDevicePortData
+from extremecloudiq.models.xiq_bounce_device_port_operation_result import XiqBounceDevicePortOperationResult
+from extremecloudiq.models.xiq_bounce_device_port_request import XiqBounceDevicePortRequest
+from extremecloudiq.models.xiq_bounce_device_port_response import XiqBounceDevicePortResponse
 from extremecloudiq.models.xiq_building import XiqBuilding
 from extremecloudiq.models.xiq_certificate import XiqCertificate
 from extremecloudiq.models.xiq_certificate_type import XiqCertificateType
 from extremecloudiq.models.xiq_change_devices_ibeacon_request import XiqChangeDevicesIbeaconRequest
 from extremecloudiq.models.xiq_change_devices_os_mode_request import XiqChangeDevicesOsModeRequest
 from extremecloudiq.models.xiq_check_permission_request import XiqCheckPermissionRequest
 from extremecloudiq.models.xiq_check_permission_response import XiqCheckPermissionResponse
 from extremecloudiq.models.xiq_classification import XiqClassification
 from extremecloudiq.models.xiq_classification_rule import XiqClassificationRule
 from extremecloudiq.models.xiq_classification_type import XiqClassificationType
 from extremecloudiq.models.xiq_cli_output import XiqCliOutput
 from extremecloudiq.models.xiq_cli_response_code import XiqCliResponseCode
 from extremecloudiq.models.xiq_client import XiqClient
 from extremecloudiq.models.xiq_client_field import XiqClientField
+from extremecloudiq.models.xiq_client_sort_field import XiqClientSortField
 from extremecloudiq.models.xiq_client_summary import XiqClientSummary
 from extremecloudiq.models.xiq_client_usage import XiqClientUsage
 from extremecloudiq.models.xiq_client_view import XiqClientView
 from extremecloudiq.models.xiq_cloud_config_group import XiqCloudConfigGroup
 from extremecloudiq.models.xiq_connectivity_experience_data import XiqConnectivityExperienceData
 from extremecloudiq.models.xiq_connectivity_experience_view_type import XiqConnectivityExperienceViewType
 from extremecloudiq.models.xiq_copilot_events_wired_sort_field import XiqCopilotEventsWiredSortField
@@ -152,22 +159,30 @@
 from extremecloudiq.models.xiq_device_admin_state import XiqDeviceAdminState
 from extremecloudiq.models.xiq_device_alarm import XiqDeviceAlarm
 from extremecloudiq.models.xiq_device_cpu_memory_usage import XiqDeviceCpuMemoryUsage
 from extremecloudiq.models.xiq_device_field import XiqDeviceField
 from extremecloudiq.models.xiq_device_filter import XiqDeviceFilter
 from extremecloudiq.models.xiq_device_function import XiqDeviceFunction
 from extremecloudiq.models.xiq_device_ibeacon import XiqDeviceIbeacon
+from extremecloudiq.models.xiq_device_installation_report import XiqDeviceInstallationReport
 from extremecloudiq.models.xiq_device_level_ssid import XiqDeviceLevelSsid
 from extremecloudiq.models.xiq_device_level_ssid_status import XiqDeviceLevelSsidStatus
+from extremecloudiq.models.xiq_device_lldp_cdp_info import XiqDeviceLldpCdpInfo
 from extremecloudiq.models.xiq_device_location import XiqDeviceLocation
 from extremecloudiq.models.xiq_device_location_assignment import XiqDeviceLocationAssignment
 from extremecloudiq.models.xiq_device_sort_field import XiqDeviceSortField
 from extremecloudiq.models.xiq_device_stats import XiqDeviceStats
 from extremecloudiq.models.xiq_device_type import XiqDeviceType
 from extremecloudiq.models.xiq_device_view import XiqDeviceView
+from extremecloudiq.models.xiq_device_wifi_interface import XiqDeviceWifiInterface
+from extremecloudiq.models.xiq_dfs_channel_changes_entity import XiqDfsChannelChangesEntity
+from extremecloudiq.models.xiq_dfs_channel_stats_entity import XiqDfsChannelStatsEntity
+from extremecloudiq.models.xiq_dfs_recurence_channel_stats_response import XiqDfsRecurenceChannelStatsResponse
+from extremecloudiq.models.xiq_dfs_recurence_count_stats_response import XiqDfsRecurenceCountStatsResponse
+from extremecloudiq.models.xiq_duplex_data_rate_entity import XiqDuplexDataRateEntity
 from extremecloudiq.models.xiq_email_log import XiqEmailLog
 from extremecloudiq.models.xiq_email_template import XiqEmailTemplate
 from extremecloudiq.models.xiq_end_user import XiqEndUser
 from extremecloudiq.models.xiq_entitlement_type import XiqEntitlementType
 from extremecloudiq.models.xiq_error import XiqError
 from extremecloudiq.models.xiq_exos_devices import XiqExosDevices
 from extremecloudiq.models.xiq_expiration_action_type import XiqExpirationActionType
@@ -234,14 +249,16 @@
 from extremecloudiq.models.xiq_pcg_port_assignment_entry import XiqPcgPortAssignmentEntry
 from extremecloudiq.models.xiq_pcg_port_assignment_entry_detail import XiqPcgPortAssignmentEntryDetail
 from extremecloudiq.models.xiq_pcg_port_assignment_entry_device_meta import XiqPcgPortAssignmentEntryDeviceMeta
 from extremecloudiq.models.xiq_pcg_port_assignment_entry_eth_user_meta import XiqPcgPortAssignmentEntryEthUserMeta
 from extremecloudiq.models.xiq_pcg_type import XiqPcgType
 from extremecloudiq.models.xiq_permission import XiqPermission
 from extremecloudiq.models.xiq_poe_flapping_stats_response import XiqPoeFlappingStatsResponse
+from extremecloudiq.models.xiq_port_efficiency_speed_duplex_stats_response import XiqPortEfficiencySpeedDuplexStatsResponse
+from extremecloudiq.models.xiq_port_efficiency_stats_response import XiqPortEfficiencyStatsResponse
 from extremecloudiq.models.xiq_post_expiration_action import XiqPostExpirationAction
 from extremecloudiq.models.xiq_psk_generation_method import XiqPskGenerationMethod
 from extremecloudiq.models.xiq_radio_mode import XiqRadioMode
 from extremecloudiq.models.xiq_radio_profile import XiqRadioProfile
 from extremecloudiq.models.xiq_radius_client import XiqRadiusClient
 from extremecloudiq.models.xiq_radius_client_object import XiqRadiusClientObject
 from extremecloudiq.models.xiq_radius_client_object_entry import XiqRadiusClientObjectEntry
@@ -267,14 +284,15 @@
 from extremecloudiq.models.xiq_set_ssid_mode_psk_request import XiqSetSsidModePskRequest
 from extremecloudiq.models.xiq_set_ssid_mode_wep_request import XiqSetSsidModeWepRequest
 from extremecloudiq.models.xiq_sms_log import XiqSmsLog
 from extremecloudiq.models.xiq_sms_log_status import XiqSmsLogStatus
 from extremecloudiq.models.xiq_sms_template import XiqSmsTemplate
 from extremecloudiq.models.xiq_sort_field import XiqSortField
 from extremecloudiq.models.xiq_sort_order import XiqSortOrder
+from extremecloudiq.models.xiq_speed_duplex_entity import XiqSpeedDuplexEntity
 from extremecloudiq.models.xiq_ssid import XiqSsid
 from extremecloudiq.models.xiq_ssid_dot1x_encryption_method import XiqSsidDot1xEncryptionMethod
 from extremecloudiq.models.xiq_ssid_dot1x_key_management import XiqSsidDot1xKeyManagement
 from extremecloudiq.models.xiq_ssid_key_type import XiqSsidKeyType
 from extremecloudiq.models.xiq_ssid_ppsk_key_management import XiqSsidPpskKeyManagement
 from extremecloudiq.models.xiq_ssid_psk_encryption_method import XiqSsidPskEncryptionMethod
 from extremecloudiq.models.xiq_ssid_psk_key_management import XiqSsidPskKeyManagement
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/inline_object.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/inline_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_accounting_log.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_accounting_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_active_directory_server.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_active_directory_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_alert.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_alert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_application.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_application.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_audit_log.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_audit_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_auth_log.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_auth_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_certificate.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_certificate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_classification_rule.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_classification_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_client.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_cloud_config_group.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_cloud_config_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_connectivity_experience_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_copilot_wireless_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_credential_log.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_credential_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_cwp.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_cwp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_device.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_device_alarm.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_device_alarm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_email_log.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_email_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_end_user.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_end_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_external_radius_server.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_external_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_external_user.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_external_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_internal_radius_device.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_internal_radius_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_internal_radius_server.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_internal_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_ldap_server.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_ldap_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_network_policy.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_network_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_radio_profile.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_radio_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_radius_client_object.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_radius_client_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_radius_proxy.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_radius_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_sms_log.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_sms_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_ssid.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_ssid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_user.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_user_group.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_user_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_user_profile.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_user_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_vlan_profile.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_vlan_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/paged_xiq_wired_event_entity.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/paged_xiq_wired_event_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_account.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_account_mode.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_account_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_account_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_account_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_accounting_log.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_accounting_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_active_directory_server.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_active_directory_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_alert.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_alert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_alert_category.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_alert_category.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_alert_group_query.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_alert_group_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_alert_severity.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_alert_severity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_alert_source.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_alert_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_alert_source_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_alert_source_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_anomaly_device_entity.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_anomaly_device_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_anomaly_location_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_anomaly_severity.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_anomaly_severity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -25,19 +25,20 @@
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
+    NONE = "NONE"
     LOW = "LOW"
     MEDIUM = "MEDIUM"
     HIGH = "HIGH"
 
-    allowable_values = [LOW, MEDIUM, HIGH]  # noqa: E501
+    allowable_values = [NONE, LOW, MEDIUM, HIGH]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_anomaly_sort_field.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_anomaly_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_anomaly_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_anomaly_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -28,19 +28,19 @@
 
     """
     allowed enum values
     """
     POE_FLAPPING = "POE_FLAPPING"
     DFS_RECURRENCE = "DFS_RECURRENCE"
     MULTI_BROADCAST = "MULTI_BROADCAST"
-    UPLINK_EFFICIENCY = "UPLINK_EFFICIENCY"
+    PORT_EFFICIENCY = "PORT_EFFICIENCY"
     WIFI_CAPACITY = "WIFI_CAPACITY"
     WIFI_EFFICIENCY = "WIFI_EFFICIENCY"
 
-    allowable_values = [POE_FLAPPING, DFS_RECURRENCE, MULTI_BROADCAST, UPLINK_EFFICIENCY, WIFI_CAPACITY, WIFI_EFFICIENCY]  # noqa: E501
+    allowable_values = [POE_FLAPPING, DFS_RECURRENCE, MULTI_BROADCAST, PORT_EFFICIENCY, WIFI_CAPACITY, WIFI_EFFICIENCY]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_api_token_info.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_api_token_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_application.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_application.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_application_detection_protocol.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_application_detection_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_application_detection_rule.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_application_detection_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_application_detection_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_application_detection_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_application_sort_field.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_application_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_application_top_clients_usage.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_application_top_clients_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_assign_devices_country_code_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_assign_devices_country_code_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_assign_devices_location_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_assign_devices_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_assign_devices_network_policy_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_assign_devices_network_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_audit_log.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_audit_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_audit_log_category.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_audit_log_category.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_auth_log.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_auth_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_building.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_building.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_certificate.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_certificate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_certificate_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_certificate_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_change_devices_ibeacon_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_change_devices_ibeacon_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_change_devices_os_mode_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_change_devices_os_mode_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_check_permission_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_check_permission_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_check_permission_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_check_permission_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_classification.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_classification_rule.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_classification_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_classification_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_classification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_cli_output.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_cli_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_cli_response_code.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_cli_response_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_client.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_client_field.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_client_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_client_summary.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_client_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_client_usage.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_client_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_client_view.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_client_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_cloud_config_group.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_cloud_config_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_connectivity_experience_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_connectivity_experience_view_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_connectivity_experience_view_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_copilot_wired_events_score_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_copilot_wired_events_score_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_copilot_wireless_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_country_code.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_country_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_building_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_building_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_classification_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_classification_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_classification_rule_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_classification_rule_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_cloud_config_group_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_cloud_config_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_end_user_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_end_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_external_radius_server_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_external_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_floor_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_floor_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_internal_radius_server_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_internal_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_ldap_server_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_ldap_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_location_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_location_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_network_policy_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_network_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_organization_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_organization_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_radio_profile_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_radio_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_radius_client.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_radius_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_radius_client_object_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_radius_client_object_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_radius_proxy_realm.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_radius_proxy_realm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_radius_proxy_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_radius_proxy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_user_group_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_user_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_user_profile_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_user_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_user_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_user_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -33,41 +33,45 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'login_name': 'str',
         'display_name': 'str',
         'idle_timeout': 'int',
-        'user_role': 'XiqUserRole'
+        'user_role': 'XiqUserRole',
+        'location_ids': 'list[int]'
     }
 
     attribute_map = {
         'login_name': 'login_name',
         'display_name': 'display_name',
         'idle_timeout': 'idle_timeout',
-        'user_role': 'user_role'
+        'user_role': 'user_role',
+        'location_ids': 'location_ids'
     }
 
-    def __init__(self, login_name=None, display_name=None, idle_timeout=None, user_role=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, login_name=None, display_name=None, idle_timeout=None, user_role=None, location_ids=None, local_vars_configuration=None):  # noqa: E501
         """XiqCreateUserRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._login_name = None
         self._display_name = None
         self._idle_timeout = None
         self._user_role = None
+        self._location_ids = None
         self.discriminator = None
 
         self.login_name = login_name
         self.display_name = display_name
-        if idle_timeout is not None:
-            self.idle_timeout = idle_timeout
+        self.idle_timeout = idle_timeout
         self.user_role = user_role
+        if location_ids is not None:
+            self.location_ids = location_ids
 
     @property
     def login_name(self):
         """Gets the login_name of this XiqCreateUserRequest.  # noqa: E501
 
         Login name, i.e. username or login Email  # noqa: E501
 
@@ -90,55 +94,57 @@
 
         self._login_name = login_name
 
     @property
     def display_name(self):
         """Gets the display_name of this XiqCreateUserRequest.  # noqa: E501
 
-        The user name to displa  # noqa: E501
+        The user name to display  # noqa: E501
 
         :return: The display_name of this XiqCreateUserRequest.  # noqa: E501
         :rtype: str
         """
         return self._display_name
 
     @display_name.setter
     def display_name(self, display_name):
         """Sets the display_name of this XiqCreateUserRequest.
 
-        The user name to displa  # noqa: E501
+        The user name to display  # noqa: E501
 
         :param display_name: The display_name of this XiqCreateUserRequest.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
             raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
 
         self._display_name = display_name
 
     @property
     def idle_timeout(self):
         """Gets the idle_timeout of this XiqCreateUserRequest.  # noqa: E501
 
-        The idle timeout in minutes, the minimum value is 5 minutes and the maximum value is 4 hours  # noqa: E501
+        The idle timeout in minutes.  # noqa: E501
 
         :return: The idle_timeout of this XiqCreateUserRequest.  # noqa: E501
         :rtype: int
         """
         return self._idle_timeout
 
     @idle_timeout.setter
     def idle_timeout(self, idle_timeout):
         """Sets the idle_timeout of this XiqCreateUserRequest.
 
-        The idle timeout in minutes, the minimum value is 5 minutes and the maximum value is 4 hours  # noqa: E501
+        The idle timeout in minutes.  # noqa: E501
 
         :param idle_timeout: The idle_timeout of this XiqCreateUserRequest.  # noqa: E501
         :type: int
         """
+        if self.local_vars_configuration.client_side_validation and idle_timeout is None:  # noqa: E501
+            raise ValueError("Invalid value for `idle_timeout`, must not be `None`")  # noqa: E501
 
         self._idle_timeout = idle_timeout
 
     @property
     def user_role(self):
         """Gets the user_role of this XiqCreateUserRequest.  # noqa: E501
 
@@ -157,14 +163,37 @@
         :type: XiqUserRole
         """
         if self.local_vars_configuration.client_side_validation and user_role is None:  # noqa: E501
             raise ValueError("Invalid value for `user_role`, must not be `None`")  # noqa: E501
 
         self._user_role = user_role
 
+    @property
+    def location_ids(self):
+        """Gets the location_ids of this XiqCreateUserRequest.  # noqa: E501
+
+        The location IDs to assign. Null or empty list will assign Admin default locations.  # noqa: E501
+
+        :return: The location_ids of this XiqCreateUserRequest.  # noqa: E501
+        :rtype: list[int]
+        """
+        return self._location_ids
+
+    @location_ids.setter
+    def location_ids(self, location_ids):
+        """Sets the location_ids of this XiqCreateUserRequest.
+
+        The location IDs to assign. Null or empty list will assign Admin default locations.  # noqa: E501
+
+        :param location_ids: The location_ids of this XiqCreateUserRequest.  # noqa: E501
+        :type: list[int]
+        """
+
+        self._location_ids = location_ids
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_vlan_profile_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_vlan_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_create_webhook_subscription_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_create_webhook_subscription_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_credential_log.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_credential_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_cwp.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_cwp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_data_point.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_data_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_date_time_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_date_time_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_date_time_unit_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_date_time_unit_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_default_device_password.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_default_device_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_delivery_settings.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_delivery_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_dell_devices.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_dell_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_deployment_overview.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_deployment_overview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_deployment_policy.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_deployment_policy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -62,26 +62,26 @@
         if firmware_activate_option is not None:
             self.firmware_activate_option = firmware_activate_option
 
     @property
     def enable_complete_configuration_update(self):
         """Gets the enable_complete_configuration_update of this XiqDeploymentPolicy.  # noqa: E501
 
-        true if update complete configuration, otherwise update delta configuration  # noqa: E501
+        true if update complete configuration, otherwise update delta configuration. Note: ExtremeCloud IQ will neither upgrade device firmware nor reboot device for a delta configuration push. That means that the other parameters for firmware upgrade and activation are not required when this is false.  # noqa: E501
 
         :return: The enable_complete_configuration_update of this XiqDeploymentPolicy.  # noqa: E501
         :rtype: bool
         """
         return self._enable_complete_configuration_update
 
     @enable_complete_configuration_update.setter
     def enable_complete_configuration_update(self, enable_complete_configuration_update):
         """Sets the enable_complete_configuration_update of this XiqDeploymentPolicy.
 
-        true if update complete configuration, otherwise update delta configuration  # noqa: E501
+        true if update complete configuration, otherwise update delta configuration. Note: ExtremeCloud IQ will neither upgrade device firmware nor reboot device for a delta configuration push. That means that the other parameters for firmware upgrade and activation are not required when this is false.  # noqa: E501
 
         :param enable_complete_configuration_update: The enable_complete_configuration_update of this XiqDeploymentPolicy.  # noqa: E501
         :type: bool
         """
         if self.local_vars_configuration.client_side_validation and enable_complete_configuration_update is None:  # noqa: E501
             raise ValueError("Invalid value for `enable_complete_configuration_update`, must not be `None`")  # noqa: E501
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_deployment_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_deployment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_deployment_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_deployment_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_deployment_status.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_deployment_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -59,15 +59,16 @@
         'ipv6_netmask': 'int',
         'simulated': 'bool',
         'display_version': 'str',
         'active_clients': 'int',
         'location_id': 'int',
         'locations': 'list[XiqLocationLegend]',
         'country_code': 'int',
-        'description': 'str'
+        'description': 'str',
+        'lldp_cdp_infos': 'list[XiqDeviceLldpCdpInfo]'
     }
 
     attribute_map = {
         'id': 'id',
         'create_time': 'create_time',
         'update_time': 'update_time',
         'org_id': 'org_id',
@@ -92,18 +93,19 @@
         'ipv6_netmask': 'ipv6_netmask',
         'simulated': 'simulated',
         'display_version': 'display_version',
         'active_clients': 'active_clients',
         'location_id': 'location_id',
         'locations': 'locations',
         'country_code': 'country_code',
-        'description': 'description'
+        'description': 'description',
+        'lldp_cdp_infos': 'lldp_cdp_infos'
     }
 
-    def __init__(self, id=None, create_time=None, update_time=None, org_id=None, serial_number=None, service_tag=None, mac_address=None, device_function=None, product_type=None, hostname=None, ip_address=None, software_version=None, device_admin_state=None, connected=None, last_connect_time=None, network_policy_name=None, network_policy_id=None, primary_ntp_server_address=None, primary_dns_server_address=None, subnet_mask=None, default_gateway=None, ipv6_address=None, ipv6_netmask=None, simulated=None, display_version=None, active_clients=None, location_id=None, locations=None, country_code=None, description=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, create_time=None, update_time=None, org_id=None, serial_number=None, service_tag=None, mac_address=None, device_function=None, product_type=None, hostname=None, ip_address=None, software_version=None, device_admin_state=None, connected=None, last_connect_time=None, network_policy_name=None, network_policy_id=None, primary_ntp_server_address=None, primary_dns_server_address=None, subnet_mask=None, default_gateway=None, ipv6_address=None, ipv6_netmask=None, simulated=None, display_version=None, active_clients=None, location_id=None, locations=None, country_code=None, description=None, lldp_cdp_infos=None, local_vars_configuration=None):  # noqa: E501
         """XiqDevice - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._create_time = None
@@ -131,14 +133,15 @@
         self._simulated = None
         self._display_version = None
         self._active_clients = None
         self._location_id = None
         self._locations = None
         self._country_code = None
         self._description = None
+        self._lldp_cdp_infos = None
         self.discriminator = None
 
         self.id = id
         self.create_time = create_time
         self.update_time = update_time
         if org_id is not None:
             self.org_id = org_id
@@ -190,14 +193,16 @@
             self.location_id = location_id
         if locations is not None:
             self.locations = locations
         if country_code is not None:
             self.country_code = country_code
         if description is not None:
             self.description = description
+        if lldp_cdp_infos is not None:
+            self.lldp_cdp_infos = lldp_cdp_infos
 
     @property
     def id(self):
         """Gets the id of this XiqDevice.  # noqa: E501
 
         The unique identifier  # noqa: E501
 
@@ -883,14 +888,37 @@
 
         :param description: The description of this XiqDevice.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
+    @property
+    def lldp_cdp_infos(self):
+        """Gets the lldp_cdp_infos of this XiqDevice.  # noqa: E501
+
+        The device LLDP/CDP information  # noqa: E501
+
+        :return: The lldp_cdp_infos of this XiqDevice.  # noqa: E501
+        :rtype: list[XiqDeviceLldpCdpInfo]
+        """
+        return self._lldp_cdp_infos
+
+    @lldp_cdp_infos.setter
+    def lldp_cdp_infos(self, lldp_cdp_infos):
+        """Sets the lldp_cdp_infos of this XiqDevice.
+
+        The device LLDP/CDP information  # noqa: E501
+
+        :param lldp_cdp_infos: The lldp_cdp_infos of this XiqDevice.  # noqa: E501
+        :type: list[XiqDeviceLldpCdpInfo]
+        """
+
+        self._lldp_cdp_infos = lldp_cdp_infos
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_admin_state.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_admin_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_alarm.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_alarm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_cpu_memory_usage.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_cpu_memory_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_field.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -55,16 +55,17 @@
     SIMULATED = "SIMULATED"
     DISPLAY_VERSION = "DISPLAY_VERSION"
     ACTIVE_CLIENTS = "ACTIVE_CLIENTS"
     LOCATION_ID = "LOCATION_ID"
     LOCATIONS = "LOCATIONS"
     DESCRIPTION = "DESCRIPTION"
     COUNTRY_CODE = "COUNTRY_CODE"
+    LLDP_CDP_INFO = "LLDP_CDP_INFO"
 
-    allowable_values = [ID, CREATE_TIME, UPDATE_TIME, ORG_ID, SERIAL_NUMBER, SERVICE_TAG, MAC_ADDRESS, DEVICE_FUNCTION, PRODUCT_TYPE, HOSTNAME, IP_ADDRESS, SOFTWARE_VERSION, DEVICE_ADMIN_STATE, CONNECTED, LAST_CONNECT_TIME, NETWORK_POLICY_NAME, NETWORK_POLICY_ID, NTP_SERVER_ADDRESS, DNS_SERVER_ADDRESS, SUBNET_MASK, DEFAULT_GATEWAY, IPV6_ADDRESS, IPV6_NETMASK, SIMULATED, DISPLAY_VERSION, ACTIVE_CLIENTS, LOCATION_ID, LOCATIONS, DESCRIPTION, COUNTRY_CODE]  # noqa: E501
+    allowable_values = [ID, CREATE_TIME, UPDATE_TIME, ORG_ID, SERIAL_NUMBER, SERVICE_TAG, MAC_ADDRESS, DEVICE_FUNCTION, PRODUCT_TYPE, HOSTNAME, IP_ADDRESS, SOFTWARE_VERSION, DEVICE_ADMIN_STATE, CONNECTED, LAST_CONNECT_TIME, NETWORK_POLICY_NAME, NETWORK_POLICY_ID, NTP_SERVER_ADDRESS, DNS_SERVER_ADDRESS, SUBNET_MASK, DEFAULT_GATEWAY, IPV6_ADDRESS, IPV6_NETMASK, SIMULATED, DISPLAY_VERSION, ACTIVE_CLIENTS, LOCATION_ID, LOCATIONS, DESCRIPTION, COUNTRY_CODE, LLDP_CDP_INFO]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_filter.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_function.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_ibeacon.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_ibeacon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_level_ssid.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_level_ssid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_level_ssid_status.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_level_ssid_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_location.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_location_assignment.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_location_assignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_sort_field.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_stats.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_device_view.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_device_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_email_log.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_email_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_email_template.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_email_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_end_user.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_end_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_entitlement_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_entitlement_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_error.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_exos_devices.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_exos_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_expiration_action_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_expiration_action_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_expiration_settings.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_expiration_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_expiration_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_expiration_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_external_account.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_external_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_external_radius_server.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_external_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_external_user.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_external_user.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -35,47 +35,52 @@
     """
     openapi_types = {
         'id': 'int',
         'create_time': 'datetime',
         'update_time': 'datetime',
         'login_name': 'str',
         'user_role': 'XiqUserRole',
-        'org_id': 'int'
+        'org_id': 'int',
+        'location_ids': 'list[int]'
     }
 
     attribute_map = {
         'id': 'id',
         'create_time': 'create_time',
         'update_time': 'update_time',
         'login_name': 'login_name',
         'user_role': 'user_role',
-        'org_id': 'org_id'
+        'org_id': 'org_id',
+        'location_ids': 'location_ids'
     }
 
-    def __init__(self, id=None, create_time=None, update_time=None, login_name=None, user_role=None, org_id=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, create_time=None, update_time=None, login_name=None, user_role=None, org_id=None, location_ids=None, local_vars_configuration=None):  # noqa: E501
         """XiqExternalUser - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._create_time = None
         self._update_time = None
         self._login_name = None
         self._user_role = None
         self._org_id = None
+        self._location_ids = None
         self.discriminator = None
 
         self.id = id
         self.create_time = create_time
         self.update_time = update_time
         self.login_name = login_name
         self.user_role = user_role
         if org_id is not None:
             self.org_id = org_id
+        if location_ids is not None:
+            self.location_ids = location_ids
 
     @property
     def id(self):
         """Gets the id of this XiqExternalUser.  # noqa: E501
 
         The unique identifier  # noqa: E501
 
@@ -215,14 +220,37 @@
 
         :param org_id: The org_id of this XiqExternalUser.  # noqa: E501
         :type: int
         """
 
         self._org_id = org_id
 
+    @property
+    def location_ids(self):
+        """Gets the location_ids of this XiqExternalUser.  # noqa: E501
+
+        The assigned location IDs.  # noqa: E501
+
+        :return: The location_ids of this XiqExternalUser.  # noqa: E501
+        :rtype: list[int]
+        """
+        return self._location_ids
+
+    @location_ids.setter
+    def location_ids(self, location_ids):
+        """Sets the location_ids of this XiqExternalUser.
+
+        The assigned location IDs.  # noqa: E501
+
+        :param location_ids: The location_ids of this XiqExternalUser.  # noqa: E501
+        :type: list[int]
+        """
+
+        self._location_ids = location_ids
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_external_user_directory.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_external_user_directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_external_user_directory_entry.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_external_user_directory_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_external_user_directory_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_external_user_directory_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_extreme_devices.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_extreme_devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_firmware_activate_option.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_firmware_activate_option.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_firmware_upgrade_policy.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_firmware_upgrade_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_flap_count_entity.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_flap_count_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_floor.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_floor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_forensic_bucket.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_forensic_bucket.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_generate_api_token_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_generate_api_token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_generate_api_token_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_generate_api_token_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_get_port_assignment_details_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_get_port_assignment_details_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_grant_external_user_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_grant_external_user_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -32,38 +32,43 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'login_name': 'str',
         'user_role': 'XiqUserRole',
-        'org_id': 'int'
+        'org_id': 'int',
+        'location_ids': 'list[int]'
     }
 
     attribute_map = {
         'login_name': 'login_name',
         'user_role': 'user_role',
-        'org_id': 'org_id'
+        'org_id': 'org_id',
+        'location_ids': 'location_ids'
     }
 
-    def __init__(self, login_name=None, user_role=None, org_id=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, login_name=None, user_role=None, org_id=None, location_ids=None, local_vars_configuration=None):  # noqa: E501
         """XiqGrantExternalUserRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._login_name = None
         self._user_role = None
         self._org_id = None
+        self._location_ids = None
         self.discriminator = None
 
         self.login_name = login_name
         self.user_role = user_role
         if org_id is not None:
             self.org_id = org_id
+        if location_ids is not None:
+            self.location_ids = location_ids
 
     @property
     def login_name(self):
         """Gets the login_name of this XiqGrantExternalUserRequest.  # noqa: E501
 
         Login name, i.e. username or login Email  # noqa: E501
 
@@ -128,14 +133,37 @@
 
         :param org_id: The org_id of this XiqGrantExternalUserRequest.  # noqa: E501
         :type: int
         """
 
         self._org_id = org_id
 
+    @property
+    def location_ids(self):
+        """Gets the location_ids of this XiqGrantExternalUserRequest.  # noqa: E501
+
+        The location IDs to assign. Null or empty list will assign Admin default locations.  # noqa: E501
+
+        :return: The location_ids of this XiqGrantExternalUserRequest.  # noqa: E501
+        :rtype: list[int]
+        """
+        return self._location_ids
+
+    @location_ids.setter
+    def location_ids(self, location_ids):
+        """Sets the location_ids of this XiqGrantExternalUserRequest.
+
+        The location IDs to assign. Null or empty list will assign Admin default locations.  # noqa: E501
+
+        :param location_ids: The location_ids of this XiqGrantExternalUserRequest.  # noqa: E501
+        :type: list[int]
+        """
+
+        self._location_ids = location_ids
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_hiq_context.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_hiq_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_hiq_status.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_hiq_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_init_key_based_pcg_network_policy_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_init_key_based_pcg_network_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_initialize_location_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_initialize_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_internal_radius_device.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_internal_radius_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_internal_radius_server.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_internal_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_key_based_pcg.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_key_based_pcg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_key_based_pcg_user.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_key_based_pcg_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_l3_address_profile.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_l3_address_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_l3_address_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_l3_address_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ldap_protocol_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ldap_protocol_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ldap_server.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ldap_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ldap_server_verification_mode.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ldap_server_verification_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_license_mode.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_license_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_license_status.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_license_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_location.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_location_legend.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_location_legend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_location_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_location_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_login_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_login_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_login_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_login_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_measurement_unit.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_measurement_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_network_policy.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_network_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_network_policy_field.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_network_policy_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_network_policy_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_network_policy_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_network_policy_view.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_network_policy_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_onboard_device_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_onboard_device_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_operation_metadata.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_operation_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_operation_object.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_operation_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_operation_status.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_operation_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_organization.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_organization_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_organization_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_password_character_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_password_character_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_password_db_location.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_password_db_location.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_password_settings.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_password_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_password_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_password_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_assign_ports_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_assign_ports_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_assign_ports_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_assign_ports_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_port_assignment.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_port_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_port_assignment_entry.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_port_assignment_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_pcg_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_pcg_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_permission.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_poe_flapping_stats_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_poe_flapping_stats_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_post_expiration_action.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_post_expiration_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_psk_generation_method.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_psk_generation_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radio_mode.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radio_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radio_profile.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radio_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_client.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_client_object.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_client_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_client_object_entry.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_client_object_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_client_object_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_client_object_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_proxy.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_proxy_format_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_proxy_format_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_proxy_realm.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_proxy_realm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_radius_server_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_radius_server_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_regenerate_end_user_password_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_regenerate_end_user_password_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rf_environment_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rf_environment_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rp_channel_selection.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rp_channel_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rp_mac_oui_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rp_miscellaneous_settings.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rp_miscellaneous_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rp_neighborhood_analysis.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rp_neighborhood_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rp_radio_usage_optimization.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rp_radio_usage_optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rp_sensor_scan_settings.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rp_sensor_scan_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_rp_wmm_qos_settings.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_rp_wmm_qos_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_send_cli_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_send_cli_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_send_cli_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_send_cli_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_server_role.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_server_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_sms_log.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_sms_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_sms_log_status.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_sms_log_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_sms_template.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_sms_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_sort_field.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_sort_order.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_sort_order.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_dot1x_key_management.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_dot1x_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_key_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_key_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_ppsk_key_management.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_ppsk_key_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_psk_encryption_method.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_psk_encryption_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_psk_key_management.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_psk_key_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_sae_group.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_sae_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_wep_authentication_method.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_wep_authentication_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_wep_default_key.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_wep_default_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_wep_encryption_method.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_wep_encryption_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_ssid_wep_key_management.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_ssid_wep_key_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_subscription_data_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_subscription_data_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_subscription_message_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_subscription_message_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_subscription_status.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_subscription_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_top_applications_usage.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_top_applications_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_trend_indicator.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_trend_indicator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_building_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_building_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_classification_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_classification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_classification_rule_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_classification_rule_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_cloud_config_group_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_cloud_config_group_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_device_level_ssid_status.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_device_level_ssid_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_end_user_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_end_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_external_radius_server_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_external_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_user.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_user.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -43,15 +43,16 @@
         'display_name': 'str',
         'phone': 'str',
         'job_title': 'str',
         'locale': 'str',
         'user_role': 'XiqUserRole',
         'idle_timeout': 'int',
         'last_login_time': 'datetime',
-        'org_id': 'int'
+        'org_id': 'int',
+        'location_ids': 'list[int]'
     }
 
     attribute_map = {
         'id': 'id',
         'create_time': 'create_time',
         'update_time': 'update_time',
         'login_name': 'login_name',
@@ -60,18 +61,19 @@
         'display_name': 'display_name',
         'phone': 'phone',
         'job_title': 'job_title',
         'locale': 'locale',
         'user_role': 'user_role',
         'idle_timeout': 'idle_timeout',
         'last_login_time': 'last_login_time',
-        'org_id': 'org_id'
+        'org_id': 'org_id',
+        'location_ids': 'location_ids'
     }
 
-    def __init__(self, id=None, create_time=None, update_time=None, login_name=None, first_name=None, last_name=None, display_name=None, phone=None, job_title=None, locale=None, user_role=None, idle_timeout=None, last_login_time=None, org_id=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, create_time=None, update_time=None, login_name=None, first_name=None, last_name=None, display_name=None, phone=None, job_title=None, locale=None, user_role=None, idle_timeout=None, last_login_time=None, org_id=None, location_ids=None, local_vars_configuration=None):  # noqa: E501
         """XiqUser - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._create_time = None
@@ -83,14 +85,15 @@
         self._phone = None
         self._job_title = None
         self._locale = None
         self._user_role = None
         self._idle_timeout = None
         self._last_login_time = None
         self._org_id = None
+        self._location_ids = None
         self.discriminator = None
 
         self.id = id
         self.create_time = create_time
         self.update_time = update_time
         self.login_name = login_name
         if first_name is not None:
@@ -109,14 +112,16 @@
             self.user_role = user_role
         if idle_timeout is not None:
             self.idle_timeout = idle_timeout
         if last_login_time is not None:
             self.last_login_time = last_login_time
         if org_id is not None:
             self.org_id = org_id
+        if location_ids is not None:
+            self.location_ids = location_ids
 
     @property
     def id(self):
         """Gets the id of this XiqUser.  # noqa: E501
 
         The unique identifier  # noqa: E501
 
@@ -438,14 +443,37 @@
 
         :param org_id: The org_id of this XiqUser.  # noqa: E501
         :type: int
         """
 
         self._org_id = org_id
 
+    @property
+    def location_ids(self):
+        """Gets the location_ids of this XiqUser.  # noqa: E501
+
+        The assigned location IDs.  # noqa: E501
+
+        :return: The location_ids of this XiqUser.  # noqa: E501
+        :rtype: list[int]
+        """
+        return self._location_ids
+
+    @location_ids.setter
+    def location_ids(self, location_ids):
+        """Sets the location_ids of this XiqUser.
+
+        The assigned location IDs.  # noqa: E501
+
+        :param location_ids: The location_ids of this XiqUser.  # noqa: E501
+        :type: list[int]
+        """
+
+        self._location_ids = location_ids
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_floor_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_floor_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_internal_radius_server_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_internal_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_ldap_server_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_ldap_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_location_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_network_policy_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_network_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_radio_profile_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_radio_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_radius_client.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_radius_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_radius_client_object_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_radius_client_object_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_radius_proxy_realm.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_radius_proxy_realm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_radius_proxy_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_radius_proxy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_rp_channel_selection_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_rp_channel_selection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_user_group_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_user_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_user_profile_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_user_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_user_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_user_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -33,44 +33,49 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'login_name': 'str',
         'display_name': 'str',
         'idle_timeout': 'int',
-        'user_role': 'XiqUserRole'
+        'user_role': 'XiqUserRole',
+        'location_ids': 'list[int]'
     }
 
     attribute_map = {
         'login_name': 'login_name',
         'display_name': 'display_name',
         'idle_timeout': 'idle_timeout',
-        'user_role': 'user_role'
+        'user_role': 'user_role',
+        'location_ids': 'location_ids'
     }
 
-    def __init__(self, login_name=None, display_name=None, idle_timeout=None, user_role=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, login_name=None, display_name=None, idle_timeout=None, user_role=None, location_ids=None, local_vars_configuration=None):  # noqa: E501
         """XiqUpdateUserRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._login_name = None
         self._display_name = None
         self._idle_timeout = None
         self._user_role = None
+        self._location_ids = None
         self.discriminator = None
 
         if login_name is not None:
             self.login_name = login_name
         if display_name is not None:
             self.display_name = display_name
         if idle_timeout is not None:
             self.idle_timeout = idle_timeout
         if user_role is not None:
             self.user_role = user_role
+        if location_ids is not None:
+            self.location_ids = location_ids
 
     @property
     def login_name(self):
         """Gets the login_name of this XiqUpdateUserRequest.  # noqa: E501
 
         Login name, i.e. username or login Email  # noqa: E501
 
@@ -114,26 +119,26 @@
 
         self._display_name = display_name
 
     @property
     def idle_timeout(self):
         """Gets the idle_timeout of this XiqUpdateUserRequest.  # noqa: E501
 
-        The idle timeout in minutes, the minimum value is 5 minutes and the maximum value is 4 hours  # noqa: E501
+        The idle timeout in minutes.  # noqa: E501
 
         :return: The idle_timeout of this XiqUpdateUserRequest.  # noqa: E501
         :rtype: int
         """
         return self._idle_timeout
 
     @idle_timeout.setter
     def idle_timeout(self, idle_timeout):
         """Sets the idle_timeout of this XiqUpdateUserRequest.
 
-        The idle timeout in minutes, the minimum value is 5 minutes and the maximum value is 4 hours  # noqa: E501
+        The idle timeout in minutes.  # noqa: E501
 
         :param idle_timeout: The idle_timeout of this XiqUpdateUserRequest.  # noqa: E501
         :type: int
         """
 
         self._idle_timeout = idle_timeout
 
@@ -154,14 +159,37 @@
 
         :param user_role: The user_role of this XiqUpdateUserRequest.  # noqa: E501
         :type: XiqUserRole
         """
 
         self._user_role = user_role
 
+    @property
+    def location_ids(self):
+        """Gets the location_ids of this XiqUpdateUserRequest.  # noqa: E501
+
+        The location IDs to reassign.  # noqa: E501
+
+        :return: The location_ids of this XiqUpdateUserRequest.  # noqa: E501
+        :rtype: list[int]
+        """
+        return self._location_ids
+
+    @location_ids.setter
+    def location_ids(self, location_ids):
+        """Sets the location_ids of this XiqUpdateUserRequest.
+
+        The location IDs to reassign.  # noqa: E501
+
+        :param location_ids: The location_ids of this XiqUpdateUserRequest.  # noqa: E501
+        :type: list[int]
+        """
+
+        self._location_ids = location_ids
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_update_vlan_profile_request.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_update_vlan_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_user_group.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_user_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_user_profile.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_user_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_user_role.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_user_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_valid_daily_settings.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_valid_daily_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_valid_during_date_settings.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_valid_during_date_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_valid_for_time_period_settings.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_valid_for_time_period_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_valid_time_period_after_first_login.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_valid_time_period_after_first_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_valid_time_period_after_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_valid_time_period_after_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_viq.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_viq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_viq_license.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_viq_license.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_vlan_object_classified_entry.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_vlan_object_classified_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_vlan_profile.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_vlan_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_vlan_profile_filter.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_vlan_profile_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_voss_devices.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_voss_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_webhook_subscription.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_webhook_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wing_devices.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wing_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wired_event_entity.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wired_event_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wired_hardware_entity.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wired_hardware_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wired_hardware_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wired_hardware_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wired_quality_index_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wired_quality_index_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wired_view_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wired_view_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_apps_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_apps_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_event_retries_entity.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_event_retries_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_if_name.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_if_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_performance_entity.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_performance_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_performance_retries_entity.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_performance_retries_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_quality_index_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_quality_index_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_time_to_connect_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_time_to_connect_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_views_list_type.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_views_list_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/models/xiq_wireless_views_type_response.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/models/xiq_wireless_views_type_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/__init__.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "23.2.0.4"
+__version__ = "23.2.1.4"
 
 # import apis into sdk package
 from extremecloudiq.api.account_api import AccountApi
 from extremecloudiq.api.alert_api import AlertApi
 from extremecloudiq.api.application_api import ApplicationApi
 from extremecloudiq.api.authentication_api import AuthenticationApi
 from extremecloudiq.api.authorization_api import AuthorizationApi
@@ -94,14 +94,15 @@
 from extremecloudiq.models.xiq_active_directory_server_base_dn_fetch_mode import XiqActiveDirectoryServerBaseDnFetchMode
 from extremecloudiq.models.xiq_alert import XiqAlert
 from extremecloudiq.models.xiq_alert_category import XiqAlertCategory
 from extremecloudiq.models.xiq_alert_group_query import XiqAlertGroupQuery
 from extremecloudiq.models.xiq_alert_severity import XiqAlertSeverity
 from extremecloudiq.models.xiq_alert_source import XiqAlertSource
 from extremecloudiq.models.xiq_alert_source_type import XiqAlertSourceType
+from extremecloudiq.models.xiq_anomalies_count_vo_entity import XiqAnomaliesCountVoEntity
 from extremecloudiq.models.xiq_anomaly_device_entity import XiqAnomalyDeviceEntity
 from extremecloudiq.models.xiq_anomaly_devices_by_location_response import XiqAnomalyDevicesByLocationResponse
 from extremecloudiq.models.xiq_anomaly_location_entity import XiqAnomalyLocationEntity
 from extremecloudiq.models.xiq_anomaly_severity import XiqAnomalySeverity
 from extremecloudiq.models.xiq_anomaly_sort_field import XiqAnomalySortField
 from extremecloudiq.models.xiq_anomaly_type import XiqAnomalyType
 from extremecloudiq.models.xiq_api_token_info import XiqApiTokenInfo
@@ -110,31 +111,37 @@
 from extremecloudiq.models.xiq_application_detection_rule import XiqApplicationDetectionRule
 from extremecloudiq.models.xiq_application_detection_type import XiqApplicationDetectionType
 from extremecloudiq.models.xiq_application_sort_field import XiqApplicationSortField
 from extremecloudiq.models.xiq_application_top_clients_usage import XiqApplicationTopClientsUsage
 from extremecloudiq.models.xiq_assign_devices_country_code_request import XiqAssignDevicesCountryCodeRequest
 from extremecloudiq.models.xiq_assign_devices_location_request import XiqAssignDevicesLocationRequest
 from extremecloudiq.models.xiq_assign_devices_network_policy_request import XiqAssignDevicesNetworkPolicyRequest
+from extremecloudiq.models.xiq_assurance_scans_overview_response import XiqAssuranceScansOverviewResponse
 from extremecloudiq.models.xiq_audit_log import XiqAuditLog
 from extremecloudiq.models.xiq_audit_log_category import XiqAuditLogCategory
 from extremecloudiq.models.xiq_auth_log import XiqAuthLog
+from extremecloudiq.models.xiq_bounce_device_port_data import XiqBounceDevicePortData
+from extremecloudiq.models.xiq_bounce_device_port_operation_result import XiqBounceDevicePortOperationResult
+from extremecloudiq.models.xiq_bounce_device_port_request import XiqBounceDevicePortRequest
+from extremecloudiq.models.xiq_bounce_device_port_response import XiqBounceDevicePortResponse
 from extremecloudiq.models.xiq_building import XiqBuilding
 from extremecloudiq.models.xiq_certificate import XiqCertificate
 from extremecloudiq.models.xiq_certificate_type import XiqCertificateType
 from extremecloudiq.models.xiq_change_devices_ibeacon_request import XiqChangeDevicesIbeaconRequest
 from extremecloudiq.models.xiq_change_devices_os_mode_request import XiqChangeDevicesOsModeRequest
 from extremecloudiq.models.xiq_check_permission_request import XiqCheckPermissionRequest
 from extremecloudiq.models.xiq_check_permission_response import XiqCheckPermissionResponse
 from extremecloudiq.models.xiq_classification import XiqClassification
 from extremecloudiq.models.xiq_classification_rule import XiqClassificationRule
 from extremecloudiq.models.xiq_classification_type import XiqClassificationType
 from extremecloudiq.models.xiq_cli_output import XiqCliOutput
 from extremecloudiq.models.xiq_cli_response_code import XiqCliResponseCode
 from extremecloudiq.models.xiq_client import XiqClient
 from extremecloudiq.models.xiq_client_field import XiqClientField
+from extremecloudiq.models.xiq_client_sort_field import XiqClientSortField
 from extremecloudiq.models.xiq_client_summary import XiqClientSummary
 from extremecloudiq.models.xiq_client_usage import XiqClientUsage
 from extremecloudiq.models.xiq_client_view import XiqClientView
 from extremecloudiq.models.xiq_cloud_config_group import XiqCloudConfigGroup
 from extremecloudiq.models.xiq_connectivity_experience_data import XiqConnectivityExperienceData
 from extremecloudiq.models.xiq_connectivity_experience_view_type import XiqConnectivityExperienceViewType
 from extremecloudiq.models.xiq_copilot_events_wired_sort_field import XiqCopilotEventsWiredSortField
@@ -187,22 +194,30 @@
 from extremecloudiq.models.xiq_device_admin_state import XiqDeviceAdminState
 from extremecloudiq.models.xiq_device_alarm import XiqDeviceAlarm
 from extremecloudiq.models.xiq_device_cpu_memory_usage import XiqDeviceCpuMemoryUsage
 from extremecloudiq.models.xiq_device_field import XiqDeviceField
 from extremecloudiq.models.xiq_device_filter import XiqDeviceFilter
 from extremecloudiq.models.xiq_device_function import XiqDeviceFunction
 from extremecloudiq.models.xiq_device_ibeacon import XiqDeviceIbeacon
+from extremecloudiq.models.xiq_device_installation_report import XiqDeviceInstallationReport
 from extremecloudiq.models.xiq_device_level_ssid import XiqDeviceLevelSsid
 from extremecloudiq.models.xiq_device_level_ssid_status import XiqDeviceLevelSsidStatus
+from extremecloudiq.models.xiq_device_lldp_cdp_info import XiqDeviceLldpCdpInfo
 from extremecloudiq.models.xiq_device_location import XiqDeviceLocation
 from extremecloudiq.models.xiq_device_location_assignment import XiqDeviceLocationAssignment
 from extremecloudiq.models.xiq_device_sort_field import XiqDeviceSortField
 from extremecloudiq.models.xiq_device_stats import XiqDeviceStats
 from extremecloudiq.models.xiq_device_type import XiqDeviceType
 from extremecloudiq.models.xiq_device_view import XiqDeviceView
+from extremecloudiq.models.xiq_device_wifi_interface import XiqDeviceWifiInterface
+from extremecloudiq.models.xiq_dfs_channel_changes_entity import XiqDfsChannelChangesEntity
+from extremecloudiq.models.xiq_dfs_channel_stats_entity import XiqDfsChannelStatsEntity
+from extremecloudiq.models.xiq_dfs_recurence_channel_stats_response import XiqDfsRecurenceChannelStatsResponse
+from extremecloudiq.models.xiq_dfs_recurence_count_stats_response import XiqDfsRecurenceCountStatsResponse
+from extremecloudiq.models.xiq_duplex_data_rate_entity import XiqDuplexDataRateEntity
 from extremecloudiq.models.xiq_email_log import XiqEmailLog
 from extremecloudiq.models.xiq_email_template import XiqEmailTemplate
 from extremecloudiq.models.xiq_end_user import XiqEndUser
 from extremecloudiq.models.xiq_entitlement_type import XiqEntitlementType
 from extremecloudiq.models.xiq_error import XiqError
 from extremecloudiq.models.xiq_exos_devices import XiqExosDevices
 from extremecloudiq.models.xiq_expiration_action_type import XiqExpirationActionType
@@ -269,14 +284,16 @@
 from extremecloudiq.models.xiq_pcg_port_assignment_entry import XiqPcgPortAssignmentEntry
 from extremecloudiq.models.xiq_pcg_port_assignment_entry_detail import XiqPcgPortAssignmentEntryDetail
 from extremecloudiq.models.xiq_pcg_port_assignment_entry_device_meta import XiqPcgPortAssignmentEntryDeviceMeta
 from extremecloudiq.models.xiq_pcg_port_assignment_entry_eth_user_meta import XiqPcgPortAssignmentEntryEthUserMeta
 from extremecloudiq.models.xiq_pcg_type import XiqPcgType
 from extremecloudiq.models.xiq_permission import XiqPermission
 from extremecloudiq.models.xiq_poe_flapping_stats_response import XiqPoeFlappingStatsResponse
+from extremecloudiq.models.xiq_port_efficiency_speed_duplex_stats_response import XiqPortEfficiencySpeedDuplexStatsResponse
+from extremecloudiq.models.xiq_port_efficiency_stats_response import XiqPortEfficiencyStatsResponse
 from extremecloudiq.models.xiq_post_expiration_action import XiqPostExpirationAction
 from extremecloudiq.models.xiq_psk_generation_method import XiqPskGenerationMethod
 from extremecloudiq.models.xiq_radio_mode import XiqRadioMode
 from extremecloudiq.models.xiq_radio_profile import XiqRadioProfile
 from extremecloudiq.models.xiq_radius_client import XiqRadiusClient
 from extremecloudiq.models.xiq_radius_client_object import XiqRadiusClientObject
 from extremecloudiq.models.xiq_radius_client_object_entry import XiqRadiusClientObjectEntry
@@ -302,14 +319,15 @@
 from extremecloudiq.models.xiq_set_ssid_mode_psk_request import XiqSetSsidModePskRequest
 from extremecloudiq.models.xiq_set_ssid_mode_wep_request import XiqSetSsidModeWepRequest
 from extremecloudiq.models.xiq_sms_log import XiqSmsLog
 from extremecloudiq.models.xiq_sms_log_status import XiqSmsLogStatus
 from extremecloudiq.models.xiq_sms_template import XiqSmsTemplate
 from extremecloudiq.models.xiq_sort_field import XiqSortField
 from extremecloudiq.models.xiq_sort_order import XiqSortOrder
+from extremecloudiq.models.xiq_speed_duplex_entity import XiqSpeedDuplexEntity
 from extremecloudiq.models.xiq_ssid import XiqSsid
 from extremecloudiq.models.xiq_ssid_dot1x_encryption_method import XiqSsidDot1xEncryptionMethod
 from extremecloudiq.models.xiq_ssid_dot1x_key_management import XiqSsidDot1xKeyManagement
 from extremecloudiq.models.xiq_ssid_key_type import XiqSsidKeyType
 from extremecloudiq.models.xiq_ssid_ppsk_key_management import XiqSsidPpskKeyManagement
 from extremecloudiq.models.xiq_ssid_psk_encryption_method import XiqSsidPskEncryptionMethod
 from extremecloudiq.models.xiq_ssid_psk_key_management import XiqSsidPskKeyManagement
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/api_client.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/23.2.0.4/python'
+        self.user_agent = 'OpenAPI-Generator/23.2.1.4/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/configuration.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -333,16 +333,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 23.2.0.4\n"\
-               "SDK Package Version: 23.2.0.4".\
+               "Version of the API: 23.2.1.4\n"\
+               "SDK Package Version: 23.2.1.4".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/exceptions.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq/rest.py` & `extremecloudiq-api-23.2.1.4/extremecloudiq/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/extremecloudiq_api.egg-info/SOURCES.txt` & `extremecloudiq-api-23.2.1.4/extremecloudiq_api.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py
 extremecloudiq/models/xiq_alert.py
 extremecloudiq/models/xiq_alert_category.py
 extremecloudiq/models/xiq_alert_group_query.py
 extremecloudiq/models/xiq_alert_severity.py
 extremecloudiq/models/xiq_alert_source.py
 extremecloudiq/models/xiq_alert_source_type.py
+extremecloudiq/models/xiq_anomalies_count_vo_entity.py
 extremecloudiq/models/xiq_anomaly_device_entity.py
 extremecloudiq/models/xiq_anomaly_devices_by_location_response.py
 extremecloudiq/models/xiq_anomaly_location_entity.py
 extremecloudiq/models/xiq_anomaly_severity.py
 extremecloudiq/models/xiq_anomaly_sort_field.py
 extremecloudiq/models/xiq_anomaly_type.py
 extremecloudiq/models/xiq_api_token_info.py
@@ -90,31 +91,37 @@
 extremecloudiq/models/xiq_application_detection_rule.py
 extremecloudiq/models/xiq_application_detection_type.py
 extremecloudiq/models/xiq_application_sort_field.py
 extremecloudiq/models/xiq_application_top_clients_usage.py
 extremecloudiq/models/xiq_assign_devices_country_code_request.py
 extremecloudiq/models/xiq_assign_devices_location_request.py
 extremecloudiq/models/xiq_assign_devices_network_policy_request.py
+extremecloudiq/models/xiq_assurance_scans_overview_response.py
 extremecloudiq/models/xiq_audit_log.py
 extremecloudiq/models/xiq_audit_log_category.py
 extremecloudiq/models/xiq_auth_log.py
+extremecloudiq/models/xiq_bounce_device_port_data.py
+extremecloudiq/models/xiq_bounce_device_port_operation_result.py
+extremecloudiq/models/xiq_bounce_device_port_request.py
+extremecloudiq/models/xiq_bounce_device_port_response.py
 extremecloudiq/models/xiq_building.py
 extremecloudiq/models/xiq_certificate.py
 extremecloudiq/models/xiq_certificate_type.py
 extremecloudiq/models/xiq_change_devices_ibeacon_request.py
 extremecloudiq/models/xiq_change_devices_os_mode_request.py
 extremecloudiq/models/xiq_check_permission_request.py
 extremecloudiq/models/xiq_check_permission_response.py
 extremecloudiq/models/xiq_classification.py
 extremecloudiq/models/xiq_classification_rule.py
 extremecloudiq/models/xiq_classification_type.py
 extremecloudiq/models/xiq_cli_output.py
 extremecloudiq/models/xiq_cli_response_code.py
 extremecloudiq/models/xiq_client.py
 extremecloudiq/models/xiq_client_field.py
+extremecloudiq/models/xiq_client_sort_field.py
 extremecloudiq/models/xiq_client_summary.py
 extremecloudiq/models/xiq_client_usage.py
 extremecloudiq/models/xiq_client_view.py
 extremecloudiq/models/xiq_cloud_config_group.py
 extremecloudiq/models/xiq_connectivity_experience_data.py
 extremecloudiq/models/xiq_connectivity_experience_view_type.py
 extremecloudiq/models/xiq_copilot_events_wired_sort_field.py
@@ -167,22 +174,30 @@
 extremecloudiq/models/xiq_device_admin_state.py
 extremecloudiq/models/xiq_device_alarm.py
 extremecloudiq/models/xiq_device_cpu_memory_usage.py
 extremecloudiq/models/xiq_device_field.py
 extremecloudiq/models/xiq_device_filter.py
 extremecloudiq/models/xiq_device_function.py
 extremecloudiq/models/xiq_device_ibeacon.py
+extremecloudiq/models/xiq_device_installation_report.py
 extremecloudiq/models/xiq_device_level_ssid.py
 extremecloudiq/models/xiq_device_level_ssid_status.py
+extremecloudiq/models/xiq_device_lldp_cdp_info.py
 extremecloudiq/models/xiq_device_location.py
 extremecloudiq/models/xiq_device_location_assignment.py
 extremecloudiq/models/xiq_device_sort_field.py
 extremecloudiq/models/xiq_device_stats.py
 extremecloudiq/models/xiq_device_type.py
 extremecloudiq/models/xiq_device_view.py
+extremecloudiq/models/xiq_device_wifi_interface.py
+extremecloudiq/models/xiq_dfs_channel_changes_entity.py
+extremecloudiq/models/xiq_dfs_channel_stats_entity.py
+extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py
+extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py
+extremecloudiq/models/xiq_duplex_data_rate_entity.py
 extremecloudiq/models/xiq_email_log.py
 extremecloudiq/models/xiq_email_template.py
 extremecloudiq/models/xiq_end_user.py
 extremecloudiq/models/xiq_entitlement_type.py
 extremecloudiq/models/xiq_error.py
 extremecloudiq/models/xiq_exos_devices.py
 extremecloudiq/models/xiq_expiration_action_type.py
@@ -249,14 +264,16 @@
 extremecloudiq/models/xiq_pcg_port_assignment_entry.py
 extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py
 extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py
 extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py
 extremecloudiq/models/xiq_pcg_type.py
 extremecloudiq/models/xiq_permission.py
 extremecloudiq/models/xiq_poe_flapping_stats_response.py
+extremecloudiq/models/xiq_port_efficiency_speed_duplex_stats_response.py
+extremecloudiq/models/xiq_port_efficiency_stats_response.py
 extremecloudiq/models/xiq_post_expiration_action.py
 extremecloudiq/models/xiq_psk_generation_method.py
 extremecloudiq/models/xiq_radio_mode.py
 extremecloudiq/models/xiq_radio_profile.py
 extremecloudiq/models/xiq_radius_client.py
 extremecloudiq/models/xiq_radius_client_object.py
 extremecloudiq/models/xiq_radius_client_object_entry.py
@@ -282,14 +299,15 @@
 extremecloudiq/models/xiq_set_ssid_mode_psk_request.py
 extremecloudiq/models/xiq_set_ssid_mode_wep_request.py
 extremecloudiq/models/xiq_sms_log.py
 extremecloudiq/models/xiq_sms_log_status.py
 extremecloudiq/models/xiq_sms_template.py
 extremecloudiq/models/xiq_sort_field.py
 extremecloudiq/models/xiq_sort_order.py
+extremecloudiq/models/xiq_speed_duplex_entity.py
 extremecloudiq/models/xiq_ssid.py
 extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py
 extremecloudiq/models/xiq_ssid_dot1x_key_management.py
 extremecloudiq/models/xiq_ssid_key_type.py
 extremecloudiq/models/xiq_ssid_ppsk_key_management.py
 extremecloudiq/models/xiq_ssid_psk_encryption_method.py
 extremecloudiq/models/xiq_ssid_psk_key_management.py
@@ -439,14 +457,15 @@
 test/test_xiq_active_directory_server_base_dn_fetch_mode.py
 test/test_xiq_alert.py
 test/test_xiq_alert_category.py
 test/test_xiq_alert_group_query.py
 test/test_xiq_alert_severity.py
 test/test_xiq_alert_source.py
 test/test_xiq_alert_source_type.py
+test/test_xiq_anomalies_count_vo_entity.py
 test/test_xiq_anomaly_device_entity.py
 test/test_xiq_anomaly_devices_by_location_response.py
 test/test_xiq_anomaly_location_entity.py
 test/test_xiq_anomaly_severity.py
 test/test_xiq_anomaly_sort_field.py
 test/test_xiq_anomaly_type.py
 test/test_xiq_api_token_info.py
@@ -455,31 +474,37 @@
 test/test_xiq_application_detection_rule.py
 test/test_xiq_application_detection_type.py
 test/test_xiq_application_sort_field.py
 test/test_xiq_application_top_clients_usage.py
 test/test_xiq_assign_devices_country_code_request.py
 test/test_xiq_assign_devices_location_request.py
 test/test_xiq_assign_devices_network_policy_request.py
+test/test_xiq_assurance_scans_overview_response.py
 test/test_xiq_audit_log.py
 test/test_xiq_audit_log_category.py
 test/test_xiq_auth_log.py
+test/test_xiq_bounce_device_port_data.py
+test/test_xiq_bounce_device_port_operation_result.py
+test/test_xiq_bounce_device_port_request.py
+test/test_xiq_bounce_device_port_response.py
 test/test_xiq_building.py
 test/test_xiq_certificate.py
 test/test_xiq_certificate_type.py
 test/test_xiq_change_devices_ibeacon_request.py
 test/test_xiq_change_devices_os_mode_request.py
 test/test_xiq_check_permission_request.py
 test/test_xiq_check_permission_response.py
 test/test_xiq_classification.py
 test/test_xiq_classification_rule.py
 test/test_xiq_classification_type.py
 test/test_xiq_cli_output.py
 test/test_xiq_cli_response_code.py
 test/test_xiq_client.py
 test/test_xiq_client_field.py
+test/test_xiq_client_sort_field.py
 test/test_xiq_client_summary.py
 test/test_xiq_client_usage.py
 test/test_xiq_client_view.py
 test/test_xiq_cloud_config_group.py
 test/test_xiq_connectivity_experience_data.py
 test/test_xiq_connectivity_experience_view_type.py
 test/test_xiq_copilot_events_wired_sort_field.py
@@ -532,22 +557,30 @@
 test/test_xiq_device_admin_state.py
 test/test_xiq_device_alarm.py
 test/test_xiq_device_cpu_memory_usage.py
 test/test_xiq_device_field.py
 test/test_xiq_device_filter.py
 test/test_xiq_device_function.py
 test/test_xiq_device_ibeacon.py
+test/test_xiq_device_installation_report.py
 test/test_xiq_device_level_ssid.py
 test/test_xiq_device_level_ssid_status.py
+test/test_xiq_device_lldp_cdp_info.py
 test/test_xiq_device_location.py
 test/test_xiq_device_location_assignment.py
 test/test_xiq_device_sort_field.py
 test/test_xiq_device_stats.py
 test/test_xiq_device_type.py
 test/test_xiq_device_view.py
+test/test_xiq_device_wifi_interface.py
+test/test_xiq_dfs_channel_changes_entity.py
+test/test_xiq_dfs_channel_stats_entity.py
+test/test_xiq_dfs_recurence_channel_stats_response.py
+test/test_xiq_dfs_recurence_count_stats_response.py
+test/test_xiq_duplex_data_rate_entity.py
 test/test_xiq_email_log.py
 test/test_xiq_email_template.py
 test/test_xiq_end_user.py
 test/test_xiq_entitlement_type.py
 test/test_xiq_error.py
 test/test_xiq_exos_devices.py
 test/test_xiq_expiration_action_type.py
@@ -614,14 +647,16 @@
 test/test_xiq_pcg_port_assignment_entry.py
 test/test_xiq_pcg_port_assignment_entry_detail.py
 test/test_xiq_pcg_port_assignment_entry_device_meta.py
 test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py
 test/test_xiq_pcg_type.py
 test/test_xiq_permission.py
 test/test_xiq_poe_flapping_stats_response.py
+test/test_xiq_port_efficiency_speed_duplex_stats_response.py
+test/test_xiq_port_efficiency_stats_response.py
 test/test_xiq_post_expiration_action.py
 test/test_xiq_psk_generation_method.py
 test/test_xiq_radio_mode.py
 test/test_xiq_radio_profile.py
 test/test_xiq_radius_client.py
 test/test_xiq_radius_client_object.py
 test/test_xiq_radius_client_object_entry.py
@@ -647,14 +682,15 @@
 test/test_xiq_set_ssid_mode_psk_request.py
 test/test_xiq_set_ssid_mode_wep_request.py
 test/test_xiq_sms_log.py
 test/test_xiq_sms_log_status.py
 test/test_xiq_sms_template.py
 test/test_xiq_sort_field.py
 test/test_xiq_sort_order.py
+test/test_xiq_speed_duplex_entity.py
 test/test_xiq_ssid.py
 test/test_xiq_ssid_dot1x_encryption_method.py
 test/test_xiq_ssid_dot1x_key_management.py
 test/test_xiq_ssid_key_type.py
 test/test_xiq_ssid_ppsk_key_management.py
 test/test_xiq_ssid_psk_encryption_method.py
 test/test_xiq_ssid_psk_key_management.py
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_account_api.py` & `extremecloudiq-api-23.2.1.4/test/test_account_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_alert_api.py` & `extremecloudiq-api-23.2.1.4/test/test_alert_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_application_api.py` & `extremecloudiq-api-23.2.1.4/test/test_application_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_authentication_api.py` & `extremecloudiq-api-23.2.1.4/test/test_authentication_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_authorization_api.py` & `extremecloudiq-api-23.2.1.4/test/test_authorization_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_client_api.py` & `extremecloudiq-api-23.2.1.4/test/test_client_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -25,14 +25,28 @@
 
     def setUp(self):
         self.api = extremecloudiq.api.client_api.ClientApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
+    def test_disconnect_client(self):
+        """Test case for disconnect_client
+
+        Disconnect the client  # noqa: E501
+        """
+        pass
+
+    def test_get_active_clients_count(self):
+        """Test case for get_active_clients_count
+
+        Get active clients count  # noqa: E501
+        """
+        pass
+
     def test_get_client(self):
         """Test case for get_client
 
         Get client info  # noqa: E501
         """
         pass
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_configuration___authentication_api.py` & `extremecloudiq-api-23.2.1.4/test/test_configuration___authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_configuration___basic_api.py` & `extremecloudiq-api-23.2.1.4/test/test_configuration___basic_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_configuration___certificate_api.py` & `extremecloudiq-api-23.2.1.4/test/test_configuration___certificate_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_configuration___deployment_api.py` & `extremecloudiq-api-23.2.1.4/test/test_configuration___deployment_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_configuration___policy_api.py` & `extremecloudiq-api-23.2.1.4/test/test_configuration___policy_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_configuration___user_management_api.py` & `extremecloudiq-api-23.2.1.4/test/test_configuration___user_management_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_copilot___anomalies_api.py` & `extremecloudiq-api-23.2.1.4/test/test_notification_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import extremecloudiq
-from extremecloudiq.api.copilot___anomalies_api import CopilotAnomaliesApi  # noqa: E501
+from extremecloudiq.api.notification_api import NotificationApi  # noqa: E501
 from extremecloudiq.rest import ApiException
 
 
-class TestCopilotAnomaliesApi(unittest.TestCase):
-    """CopilotAnomaliesApi unit test stubs"""
+class TestNotificationApi(unittest.TestCase):
+    """NotificationApi unit test stubs"""
 
     def setUp(self):
-        self.api = extremecloudiq.api.copilot___anomalies_api.CopilotAnomaliesApi()  # noqa: E501
+        self.api = extremecloudiq.api.notification_api.NotificationApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_get_devices_by_location(self):
-        """Test case for get_devices_by_location
+    def test_create_subscriptions(self):
+        """Test case for create_subscriptions
 
+        Create webhook subscriptions  # noqa: E501
         """
         pass
 
-    def test_get_poe_flapping_stats(self):
-        """Test case for get_poe_flapping_stats
+    def test_delete_subscription(self):
+        """Test case for delete_subscription
 
+        Delete webhook subscription  # noqa: E501
         """
         pass
 
-    def test_list_anomaly_locations(self):
-        """Test case for list_anomaly_locations
+    def test_list(self):
+        """Test case for list
 
+        List webhook subscriptions  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_copilot___connectivity_experience_api.py` & `extremecloudiq-api-23.2.1.4/test/test_copilot___connectivity_experience_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_device_api.py` & `extremecloudiq-api-23.2.1.4/test/test_device_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -67,14 +67,21 @@
     def test_assign_devices_radius_proxy(self):
         """Test case for assign_devices_radius_proxy
 
         Assign RADIUS proxy to devices  # noqa: E501
         """
         pass
 
+    def test_bounce_device_port(self):
+        """Test case for bounce_device_port
+
+        Bounce port of a device (EXOS, VOSS and SR Switches  # noqa: E501
+        """
+        pass
+
     def test_change_device_description(self):
         """Test case for change_device_description
 
         Change description for a device  # noqa: E501
         """
         pass
 
@@ -193,14 +200,28 @@
     def test_get_device_stats(self):
         """Test case for get_device_stats
 
         Get device stats  # noqa: E501
         """
         pass
 
+    def test_get_device_wifi_interface(self):
+        """Test case for get_device_wifi_interface
+
+        Get the device WiFi interfaces stats  # noqa: E501
+        """
+        pass
+
+    def test_get_xiq_device_installation_report(self):
+        """Test case for get_xiq_device_installation_report
+
+        Get device installation report  # noqa: E501
+        """
+        pass
+
     def test_list_device_alarm(self):
         """Test case for list_device_alarm
 
         List alarms for a device  # noqa: E501
         """
         pass
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_hiq_api.py` & `extremecloudiq-api-23.2.1.4/test/test_hiq_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_inline_object.py` & `extremecloudiq-api-23.2.1.4/test/test_inline_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_location_api.py` & `extremecloudiq-api-23.2.1.4/test/test_location_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_log_api.py` & `extremecloudiq-api-23.2.1.4/test/test_log_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_network_policy_api.py` & `extremecloudiq-api-23.2.1.4/test/test_network_policy_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_notification_api.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_expiration_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
+import datetime
 
 import extremecloudiq
-from extremecloudiq.api.notification_api import NotificationApi  # noqa: E501
+from extremecloudiq.models.xiq_expiration_type import XiqExpirationType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-
-class TestNotificationApi(unittest.TestCase):
-    """NotificationApi unit test stubs"""
+class TestXiqExpirationType(unittest.TestCase):
+    """XiqExpirationType unit test stubs"""
 
     def setUp(self):
-        self.api = extremecloudiq.api.notification_api.NotificationApi()  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    def test_create_subscriptions(self):
-        """Test case for create_subscriptions
-
-        Create webhook subscriptions  # noqa: E501
-        """
         pass
 
-    def test_delete_subscription(self):
-        """Test case for delete_subscription
-
-        Delete webhook subscription  # noqa: E501
-        """
+    def tearDown(self):
         pass
 
-    def test_list(self):
-        """Test case for list
-
-        List webhook subscriptions  # noqa: E501
-        """
-        pass
+    def make_instance(self, include_optional):
+        """Test XiqExpirationType
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # model = extremecloudiq.models.xiq_expiration_type.XiqExpirationType()  # noqa: E501
+        if include_optional :
+            return XiqExpirationType(
+            )
+        else :
+            return XiqExpirationType(
+        )
+
+    def testXiqExpirationType(self):
+        """Test XiqExpirationType"""
+        inst_req_only = self.make_instance(include_optional=False)
+        inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_operation_api.py` & `extremecloudiq-api-23.2.1.4/test/test_operation_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_accounting_log.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_accounting_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_active_directory_server.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_active_directory_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_alert.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_application.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_audit_log.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_audit_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_auth_log.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_auth_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_certificate.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_classification_rule.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_classification_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_client.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_cloud_config_group.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_cloud_config_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_connectivity_experience_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_copilot_wireless_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_credential_log.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_credential_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_cwp.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_cwp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_device.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -72,15 +72,22 @@
                         location_id = 56, 
                         locations = [
                             extremecloudiq.models.xiq_location_legend.XiqLocationLegend(
                                 id = 56, 
                                 name = '0', )
                             ], 
                         country_code = 56, 
-                        description = '0', )
+                        description = '0', 
+                        lldp_cdp_infos = [
+                            extremecloudiq.models.xiq_device_lldp_cdp_info.XiqDeviceLldpCdpInfo(
+                                port_id = '0', 
+                                system_id = '0', 
+                                system_name = '0', 
+                                interface_name = '0', )
+                            ], )
                     ]
             )
         else :
             return PagedXiqDevice(
                 page = 56,
                 count = 56,
                 total_pages = 56,
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_device_alarm.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_device_alarm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_email_log.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_email_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_end_user.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_end_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_external_radius_server.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_external_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_external_user.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_external_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -44,15 +44,18 @@
                 data = [
                     extremecloudiq.models.xiq_external_user.XiqExternalUser(
                         id = 56, 
                         create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         login_name = '0', 
                         user_role = 'ADMINISTRATOR', 
-                        org_id = 56, )
+                        org_id = 56, 
+                        location_ids = [
+                            56
+                            ], )
                     ]
             )
         else :
             return PagedXiqExternalUser(
                 page = 56,
                 count = 56,
                 total_pages = 56,
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_internal_radius_device.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_internal_radius_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_internal_radius_server.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_internal_radius_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_ldap_server.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_ldap_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_network_policy.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_network_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_radio_profile.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_radio_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_radius_client_object.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_radius_client_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_radius_proxy.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_radius_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_rp_mac_oui_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_sms_log.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_sms_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_ssid.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_ssid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_user.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -52,15 +52,18 @@
                         display_name = '0', 
                         phone = '0', 
                         job_title = '0', 
                         locale = '0', 
                         user_role = 'ADMINISTRATOR', 
                         idle_timeout = 56, 
                         last_login_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        org_id = 56, )
+                        org_id = 56, 
+                        location_ids = [
+                            56
+                            ], )
                     ]
             )
         else :
             return PagedXiqUser(
                 page = 56,
                 count = 56,
                 total_pages = 56,
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_user_group.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_user_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_user_profile.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_user_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_vlan_profile.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_vlan_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_paged_xiq_wired_event_entity.py` & `extremecloudiq-api-23.2.1.4/test/test_paged_xiq_wired_event_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_user_api.py` & `extremecloudiq-api-23.2.1.4/test/test_user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_account.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_account.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_account_mode.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_account_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_account_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_account_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_accounting_log.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_accounting_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_active_directory_server.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_active_directory_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_active_directory_server_base_dn_fetch_mode.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_active_directory_server_base_dn_fetch_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_alert.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_alert.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_alert_category.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_alert_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_alert_group_query.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_alert_group_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_alert_severity.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_alert_severity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_alert_source.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_alert_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_alert_source_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_alert_source_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_anomaly_device_entity.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_anomaly_device_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -38,15 +38,15 @@
         if include_optional :
             return XiqAnomalyDeviceEntity(
                 device_id = 56, 
                 device_name = '0', 
                 pinned = True, 
                 wired = True, 
                 anomaly_id = '0', 
-                severity = 'LOW', 
+                severity = 'NONE', 
                 summary = '0', 
                 last_detected_time = 56, 
                 recommended_action = '0', 
                 anomaly_subtypes = '0', 
                 interface_name = '0'
             )
         else :
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_anomaly_devices_by_location_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_anomaly_devices_by_location_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -39,28 +39,28 @@
             return XiqAnomalyDevicesByLocationResponse(
                 location_entity = extremecloudiq.models.xiq_anomaly_location_entity.XiqAnomalyLocationEntity(
                     location_type = 'SITE', 
                     location_id = 56, 
                     location_name = '0', 
                     pinned = True, 
                     muted = True, 
-                    severity = 'LOW', 
+                    severity = 'NONE', 
                     severity_id = 56, 
                     summary = '0', 
                     affected_device_count = 56, 
                     last_detected_time = 56, 
                     anomaly_type = 'POE_FLAPPING', ), 
                 devices = [
                     extremecloudiq.models.xiq_anomaly_device_entity.XiqAnomalyDeviceEntity(
                         device_id = 56, 
                         device_name = '0', 
                         pinned = True, 
                         wired = True, 
                         anomaly_id = '0', 
-                        severity = 'LOW', 
+                        severity = 'NONE', 
                         summary = '0', 
                         last_detected_time = 56, 
                         recommended_action = '0', 
                         anomaly_subtypes = '0', 
                         interface_name = '0', )
                     ]
             )
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_anomaly_location_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -38,15 +38,15 @@
         if include_optional :
             return XiqAnomalyLocationEntity(
                 location_type = 'SITE', 
                 location_id = 56, 
                 location_name = '0', 
                 pinned = True, 
                 muted = True, 
-                severity = 'LOW', 
+                severity = 'NONE', 
                 severity_id = 56, 
                 summary = '0', 
                 affected_device_count = 56, 
                 last_detected_time = 56, 
                 anomaly_type = 'POE_FLAPPING'
             )
         else :
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_anomaly_severity.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_anomaly_severity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_anomaly_sort_field.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_anomaly_sort_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_anomaly_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_anomaly_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_api_token_info.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_api_token_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_application.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_application_detection_protocol.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_application_detection_protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_application_detection_rule.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_application_detection_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_application_detection_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_application_detection_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_application_sort_field.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_application_sort_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_application_top_clients_usage.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_application_top_clients_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_assign_devices_country_code_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_assign_devices_country_code_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_assign_devices_location_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_assign_devices_location_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_assign_devices_network_policy_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_assign_devices_network_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_auth_log.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_auth_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_audit_log.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_audit_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_audit_log_category.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_audit_log_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_building.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_building.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_certificate.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_certificate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_certificate_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_certificate_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_change_devices_ibeacon_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_change_devices_ibeacon_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_change_devices_os_mode_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_change_devices_os_mode_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_check_permission_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_check_permission_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_check_permission_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_check_permission_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_classification.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_classification_rule.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_classification_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_classification_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_classification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_cli_output.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_cli_output.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_cli_response_code.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_cli_response_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_client.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_client_field.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_client_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_client_summary.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_client_summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_client_usage.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_client_view.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_client_usage import XiqClientUsage  # noqa: E501
+from extremecloudiq.models.xiq_client_view import XiqClientView  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqClientUsage(unittest.TestCase):
-    """XiqClientUsage unit test stubs"""
+class TestXiqClientView(unittest.TestCase):
+    """XiqClientView unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqClientUsage
+        """Test XiqClientView
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_client_usage.XiqClientUsage()  # noqa: E501
+        # model = extremecloudiq.models.xiq_client_view.XiqClientView()  # noqa: E501
         if include_optional :
-            return XiqClientUsage(
-                client_id = 56, 
-                usage = 56
+            return XiqClientView(
             )
         else :
-            return XiqClientUsage(
+            return XiqClientView(
         )
 
-    def testXiqClientUsage(self):
-        """Test XiqClientUsage"""
+    def testXiqClientView(self):
+        """Test XiqClientView"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_client_view.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_voss_devices.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_client_view import XiqClientView  # noqa: E501
+from extremecloudiq.models.xiq_voss_devices import XiqVossDevices  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqClientView(unittest.TestCase):
-    """XiqClientView unit test stubs"""
+class TestXiqVossDevices(unittest.TestCase):
+    """XiqVossDevices unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqClientView
+        """Test XiqVossDevices
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_client_view.XiqClientView()  # noqa: E501
+        # model = extremecloudiq.models.xiq_voss_devices.XiqVossDevices()  # noqa: E501
         if include_optional :
-            return XiqClientView(
+            return XiqVossDevices(
+                sns = [
+                    '0'
+                    ]
             )
         else :
-            return XiqClientView(
+            return XiqVossDevices(
+                sns = [
+                    '0'
+                    ],
         )
 
-    def testXiqClientView(self):
-        """Test XiqClientView"""
+    def testXiqVossDevices(self):
+        """Test XiqVossDevices"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_cloud_config_group.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_cloud_config_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_connectivity_experience_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_connectivity_experience_view_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_connectivity_experience_view_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_copilot_events_wired_sort_field.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_copilot_events_wired_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_copilot_events_wireless_sort_field.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_copilot_events_wireless_sort_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -44,15 +44,15 @@
                 data = [
                     extremecloudiq.models.xiq_anomaly_location_entity.XiqAnomalyLocationEntity(
                         location_type = 'SITE', 
                         location_id = 56, 
                         location_name = '0', 
                         pinned = True, 
                         muted = True, 
-                        severity = 'LOW', 
+                        severity = 'NONE', 
                         severity_id = 56, 
                         summary = '0', 
                         affected_device_count = 56, 
                         last_detected_time = 56, 
                         anomaly_type = 'POE_FLAPPING', )
                     ], 
                 summary = '0'
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_copilot_wired_events_score_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_copilot_wired_events_score_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_copilot_wireless_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_copilot_wireless_events_score_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_copilot_wireless_events_score_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_country_code.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_country_code.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_building_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_building_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_classification_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_classification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_classification_rule_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_classification_rule_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_cloud_config_group_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_cloud_config_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_end_user_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_end_user_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_external_radius_server_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_external_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_floor_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_floor_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_internal_radius_server_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_internal_radius_server_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_key_based_pcg_users_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_key_based_pcg_users_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_ldap_server_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_ldap_server_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_location_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_network_policy_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_network_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_organization_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_organization_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_radio_profile_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_radio_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_radius_client.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_radius_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_radius_client_object_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_radius_client_object_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_radius_proxy_realm.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_radius_proxy_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_radius_proxy_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_radius_proxy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_rp_mac_oui_profile_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_user_group_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_user_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_user_profile_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_user_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_user_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_user_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -36,20 +36,24 @@
             optional params are included """
         # model = extremecloudiq.models.xiq_create_user_request.XiqCreateUserRequest()  # noqa: E501
         if include_optional :
             return XiqCreateUserRequest(
                 login_name = '0', 
                 display_name = '0', 
                 idle_timeout = 56, 
-                user_role = 'ADMINISTRATOR'
+                user_role = 'ADMINISTRATOR', 
+                location_ids = [
+                    56
+                    ]
             )
         else :
             return XiqCreateUserRequest(
                 login_name = '0',
                 display_name = '0',
+                idle_timeout = 56,
                 user_role = 'ADMINISTRATOR',
         )
 
     def testXiqCreateUserRequest(self):
         """Test XiqCreateUserRequest"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_vlan_object_classified_entry_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_vlan_profile_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_vlan_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_create_webhook_subscription_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_create_webhook_subscription_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_credential_log.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_credential_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_cwp.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_cwp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_data_point.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_data_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_date_time_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_date_time_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_date_time_unit_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_date_time_unit_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_default_device_password.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_default_device_password.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_delete_key_based_pcg_users_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_delete_key_based_pcg_users_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_delivery_settings.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_delivery_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_dell_devices.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_dell_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_deployment_overview.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_deployment_overview.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_deployment_policy.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_deployment_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_deployment_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_deployment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_deployment_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_deployment_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_deployment_status.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_deployment_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -66,15 +66,22 @@
                 location_id = 56, 
                 locations = [
                     extremecloudiq.models.xiq_location_legend.XiqLocationLegend(
                         id = 56, 
                         name = '0', )
                     ], 
                 country_code = 56, 
-                description = '0'
+                description = '0', 
+                lldp_cdp_infos = [
+                    extremecloudiq.models.xiq_device_lldp_cdp_info.XiqDeviceLldpCdpInfo(
+                        port_id = '0', 
+                        system_id = '0', 
+                        system_name = '0', 
+                        interface_name = '0', )
+                    ]
             )
         else :
             return XiqDevice(
                 id = 56,
                 create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
         )
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device_admin_state.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device_admin_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device_alarm.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device_alarm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device_cpu_memory_usage.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device_cpu_memory_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device_field.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device_filter.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device_function.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device_ibeacon.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device_ibeacon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device_level_ssid.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device_level_ssid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device_level_ssid_status.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device_level_ssid_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device_location.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device_location_assignment.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device_location_assignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device_stats.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device_sort_field.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_device_view.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_device_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_email_log.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_email_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_email_template.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_email_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_end_user.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_end_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_entitlement_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_entitlement_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_error.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_exos_devices.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_exos_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_expiration_action_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_expiration_action_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_expiration_settings.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_expiration_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_expiration_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_location_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_expiration_type import XiqExpirationType  # noqa: E501
+from extremecloudiq.models.xiq_location_type import XiqLocationType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqExpirationType(unittest.TestCase):
-    """XiqExpirationType unit test stubs"""
+class TestXiqLocationType(unittest.TestCase):
+    """XiqLocationType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqExpirationType
+        """Test XiqLocationType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_expiration_type.XiqExpirationType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_location_type.XiqLocationType()  # noqa: E501
         if include_optional :
-            return XiqExpirationType(
+            return XiqLocationType(
             )
         else :
-            return XiqExpirationType(
+            return XiqLocationType(
         )
 
-    def testXiqExpirationType(self):
-        """Test XiqExpirationType"""
+    def testXiqLocationType(self):
+        """Test XiqLocationType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_external_account.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_external_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_external_radius_server.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_external_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_external_user.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_external_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -38,15 +38,18 @@
         if include_optional :
             return XiqExternalUser(
                 id = 56, 
                 create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 login_name = '0', 
                 user_role = 'ADMINISTRATOR', 
-                org_id = 56
+                org_id = 56, 
+                location_ids = [
+                    56
+                    ]
             )
         else :
             return XiqExternalUser(
                 id = 56,
                 create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 login_name = '0',
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_external_user_directory.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_external_user_directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_external_user_directory_entry.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_external_user_directory_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_external_user_directory_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_external_user_directory_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_extreme_devices.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_extreme_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_firmware_activate_option.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_firmware_activate_option.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_firmware_upgrade_policy.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_firmware_upgrade_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_flap_count_entity.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_flap_count_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_floor.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_floor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_forensic_bucket.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_forensic_bucket.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_generate_api_token_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_generate_api_token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_generate_api_token_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_generate_api_token_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_get_port_assignment_details_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_get_port_assignment_details_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_grant_external_user_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_grant_external_user_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -35,15 +35,18 @@
             params are included, when True both required and
             optional params are included """
         # model = extremecloudiq.models.xiq_grant_external_user_request.XiqGrantExternalUserRequest()  # noqa: E501
         if include_optional :
             return XiqGrantExternalUserRequest(
                 login_name = '0', 
                 user_role = 'ADMINISTRATOR', 
-                org_id = 56
+                org_id = 56, 
+                location_ids = [
+                    56
+                    ]
             )
         else :
             return XiqGrantExternalUserRequest(
                 login_name = '0',
                 user_role = 'ADMINISTRATOR',
         )
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_hiq_context.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_hiq_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_hiq_status.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_hiq_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_init_key_based_pcg_network_policy_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_init_key_based_pcg_network_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_initialize_location_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_initialize_location_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_internal_radius_device.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_internal_radius_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_internal_radius_server.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_internal_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_internal_radius_server_authentication_method.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_internal_radius_server_authentication_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_internal_radius_server_authentication_method_group.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_internal_radius_server_authentication_method_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_key_based_pcg.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_key_based_pcg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_key_based_pcg_user.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_key_based_pcg_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_key_based_pcg_user_base_info.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_key_based_pcg_user_base_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_l3_address_profile.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_l3_address_profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_l3_address_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_l3_address_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_ldap_protocol_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_ldap_protocol_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_ldap_server.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_ldap_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_ldap_server_verification_mode.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_ldap_server_verification_mode.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_license_mode.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_license_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_license_status.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_license_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_location.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_location_legend.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_location_legend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_location_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_organization_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_location_type import XiqLocationType  # noqa: E501
+from extremecloudiq.models.xiq_organization_type import XiqOrganizationType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqLocationType(unittest.TestCase):
-    """XiqLocationType unit test stubs"""
+class TestXiqOrganizationType(unittest.TestCase):
+    """XiqOrganizationType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqLocationType
+        """Test XiqOrganizationType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_location_type.XiqLocationType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_organization_type.XiqOrganizationType()  # noqa: E501
         if include_optional :
-            return XiqLocationType(
+            return XiqOrganizationType(
             )
         else :
-            return XiqLocationType(
+            return XiqOrganizationType(
         )
 
-    def testXiqLocationType(self):
-        """Test XiqLocationType"""
+    def testXiqOrganizationType(self):
+        """Test XiqOrganizationType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_login_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_login_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_login_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_login_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_measurement_unit.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_measurement_unit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_network_policy.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_network_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_network_policy_field.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_network_policy_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_network_policy_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_network_policy_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_network_policy_view.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_network_policy_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_onboard_device_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_onboard_device_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_onboard_key_based_pcg_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_onboard_key_based_pcg_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_operation_metadata.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_operation_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_operation_object.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_operation_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_operation_status.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_operation_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_organization.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_organization_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wired_view_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_organization_type import XiqOrganizationType  # noqa: E501
+from extremecloudiq.models.xiq_wired_view_type import XiqWiredViewType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqOrganizationType(unittest.TestCase):
-    """XiqOrganizationType unit test stubs"""
+class TestXiqWiredViewType(unittest.TestCase):
+    """XiqWiredViewType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqOrganizationType
+        """Test XiqWiredViewType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_organization_type.XiqOrganizationType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_wired_view_type.XiqWiredViewType()  # noqa: E501
         if include_optional :
-            return XiqOrganizationType(
+            return XiqWiredViewType(
             )
         else :
-            return XiqOrganizationType(
+            return XiqWiredViewType(
         )
 
-    def testXiqOrganizationType(self):
-        """Test XiqOrganizationType"""
+    def testXiqWiredViewType(self):
+        """Test XiqWiredViewType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_password_character_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_password_character_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_password_db_location.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_password_db_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_password_settings.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_password_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_password_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_password_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_assign_ports_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_assign_ports_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_assign_ports_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_assign_ports_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_port_assignment.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_port_assignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_port_assignment_entry.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_port_assignment_entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_port_assignment_entry_detail.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_port_assignment_entry_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_port_assignment_entry_device_meta.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_port_assignment_entry_device_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_pcg_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_pcg_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_permission.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_permission.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_poe_flapping_stats_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_poe_flapping_stats_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_post_expiration_action.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_post_expiration_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_psk_generation_method.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_psk_generation_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_radio_mode.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_radio_mode.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_radio_profile.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_radio_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_radius_client.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_radius_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_radius_client_object.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_radius_client_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_radius_client_object_entry.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_radius_client_object_entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_radius_client_object_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_radius_client_object_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_radius_proxy.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_radius_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_radius_proxy_format_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_radius_proxy_format_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_radius_proxy_realm.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_radius_proxy_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_radius_server_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_radius_server_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_regenerate_end_user_password_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_regenerate_end_user_password_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_rf_environment_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_rf_environment_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_rp_channel_selection.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_rp_channel_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_rp_mac_oui_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_rp_miscellaneous_settings.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_rp_miscellaneous_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_rp_neighborhood_analysis.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_rp_neighborhood_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_rp_radio_usage_optimization.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_rp_radio_usage_optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_rp_sensor_scan_settings.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_rp_sensor_scan_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_rp_wmm_qos_settings.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_rp_wmm_qos_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_send_cli_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_send_cli_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_send_cli_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_send_cli_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_server_role.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_server_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_set_ssid_mode_dot1x_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_set_ssid_mode_dot1x_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_set_ssid_mode_ppsk_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_set_ssid_mode_ppsk_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_set_ssid_mode_psk_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_set_ssid_mode_psk_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_set_ssid_mode_wep_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_set_ssid_mode_wep_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_sms_log.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_sms_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_sms_log_status.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_sms_log_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_sms_template.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_sms_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_sort_field.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_sort_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_sort_order.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_sort_order.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_ssid.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_ssid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_dot1x_encryption_method.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_dot1x_encryption_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_dot1x_key_management.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_dot1x_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_key_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_key_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_ppsk_key_management.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_ppsk_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_psk_encryption_method.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_psk_encryption_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_psk_key_management.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_psk_key_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_sae_group.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_sae_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_wep_authentication_method.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_wep_authentication_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_wep_default_key.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_wep_default_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_wep_encryption_method.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_wep_encryption_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_ssid_wep_key_management.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_ssid_wep_key_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_subscription_data_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_subscription_data_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_subscription_message_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_subscription_message_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_subscription_status.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_subscription_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_top_applications_usage.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_top_applications_usage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_trend_indicator.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_trend_indicator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_building_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_building_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_classification_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_classification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_classification_rule_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_classification_rule_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_cloud_config_group_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_cloud_config_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_device_level_ssid_status.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_device_level_ssid_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_end_user_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_end_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_external_radius_server_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_external_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_external_user_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_external_user_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -34,15 +34,18 @@
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = extremecloudiq.models.xiq_update_external_user_request.XiqUpdateExternalUserRequest()  # noqa: E501
         if include_optional :
             return XiqUpdateExternalUserRequest(
                 user_role = 'ADMINISTRATOR', 
-                org_id = 56
+                org_id = 56, 
+                location_ids = [
+                    56
+                    ]
             )
         else :
             return XiqUpdateExternalUserRequest(
         )
 
     def testXiqUpdateExternalUserRequest(self):
         """Test XiqUpdateExternalUserRequest"""
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_floor_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_floor_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_internal_radius_server_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_internal_radius_server_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_key_based_pcg_users_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_key_based_pcg_users_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_ldap_server_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_ldap_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_location_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_network_policy_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_network_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_radio_profile_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_radio_profile_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_radius_client.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_radius_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_radius_client_object_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_radius_client_object_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_radius_proxy_realm.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_radius_proxy_realm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_radius_proxy_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_radius_proxy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_rp_channel_selection_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_rp_channel_selection_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_rp_mac_oui_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_rp_miscellaneous_settings_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_rp_miscellaneous_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_rp_neighborhood_analysis_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_rp_neighborhood_analysis_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_rp_radio_usage_optimization_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_rp_radio_usage_optimization_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_rp_sensor_scan_settings_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_rp_sensor_scan_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_rp_wmm_qos_settings_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_rp_wmm_qos_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_user_group_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_user_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_user_profile_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_user_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_user_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_user_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -36,15 +36,18 @@
             optional params are included """
         # model = extremecloudiq.models.xiq_update_user_request.XiqUpdateUserRequest()  # noqa: E501
         if include_optional :
             return XiqUpdateUserRequest(
                 login_name = '0', 
                 display_name = '0', 
                 idle_timeout = 56, 
-                user_role = 'ADMINISTRATOR'
+                user_role = 'ADMINISTRATOR', 
+                location_ids = [
+                    56
+                    ]
             )
         else :
             return XiqUpdateUserRequest(
         )
 
     def testXiqUpdateUserRequest(self):
         """Test XiqUpdateUserRequest"""
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_vlan_object_classified_entry_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_update_vlan_profile_request.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_update_vlan_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_user.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_user.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -46,15 +46,18 @@
                 display_name = '0', 
                 phone = '0', 
                 job_title = '0', 
                 locale = '0', 
                 user_role = 'ADMINISTRATOR', 
                 idle_timeout = 56, 
                 last_login_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                org_id = 56
+                org_id = 56, 
+                location_ids = [
+                    56
+                    ]
             )
         else :
             return XiqUser(
                 id = 56,
                 create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 login_name = '0',
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_user_group.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_user_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_user_profile.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_user_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_user_role.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_user_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_valid_daily_settings.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_valid_daily_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_viq.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_viq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_valid_during_date_settings.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_valid_during_date_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_valid_for_time_period_settings.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_valid_for_time_period_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_valid_time_period_after_first_login.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_valid_time_period_after_first_login.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_valid_time_period_after_id_creation.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_valid_time_period_after_id_creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_valid_time_period_after_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_valid_time_period_after_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_viq_license.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_viq_license.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_vlan_object_classified_entry.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_vlan_object_classified_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_vlan_profile.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_vlan_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_vlan_profile_filter.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_vlan_profile_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_voss_devices.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_views_list_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_voss_devices import XiqVossDevices  # noqa: E501
+from extremecloudiq.models.xiq_wireless_views_list_type import XiqWirelessViewsListType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqVossDevices(unittest.TestCase):
-    """XiqVossDevices unit test stubs"""
+class TestXiqWirelessViewsListType(unittest.TestCase):
+    """XiqWirelessViewsListType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqVossDevices
+        """Test XiqWirelessViewsListType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_voss_devices.XiqVossDevices()  # noqa: E501
+        # model = extremecloudiq.models.xiq_wireless_views_list_type.XiqWirelessViewsListType()  # noqa: E501
         if include_optional :
-            return XiqVossDevices(
-                sns = [
-                    '0'
-                    ]
+            return XiqWirelessViewsListType(
             )
         else :
-            return XiqVossDevices(
-                sns = [
-                    '0'
-                    ],
+            return XiqWirelessViewsListType(
         )
 
-    def testXiqVossDevices(self):
-        """Test XiqVossDevices"""
+    def testXiqWirelessViewsListType(self):
+        """Test XiqWirelessViewsListType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_webhook_subscription.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_webhook_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wing_devices.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wing_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wired_event_entity.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wired_event_entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wired_hardware_entity.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wired_hardware_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wired_hardware_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wired_hardware_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wired_quality_index_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wired_quality_index_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wired_view_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_bounce_device_port_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_wired_view_type import XiqWiredViewType  # noqa: E501
+from extremecloudiq.models.xiq_bounce_device_port_data import XiqBounceDevicePortData  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqWiredViewType(unittest.TestCase):
-    """XiqWiredViewType unit test stubs"""
+class TestXiqBounceDevicePortData(unittest.TestCase):
+    """XiqBounceDevicePortData unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqWiredViewType
+        """Test XiqBounceDevicePortData
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_wired_view_type.XiqWiredViewType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_bounce_device_port_data.XiqBounceDevicePortData()  # noqa: E501
         if include_optional :
-            return XiqWiredViewType(
+            return XiqBounceDevicePortData(
+                status = 56, 
+                request_id = 56, 
+                results = [
+                    extremecloudiq.models.xiq_bounce_device_port_operation_result.XiqBounceDevicePortOperationResult(
+                        status = 56, 
+                        message = '0', )
+                    ]
             )
         else :
-            return XiqWiredViewType(
+            return XiqBounceDevicePortData(
         )
 
-    def testXiqWiredViewType(self):
-        """Test XiqWiredViewType"""
+    def testXiqBounceDevicePortData(self):
+        """Test XiqBounceDevicePortData"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_apps_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_apps_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_connectivity_performance_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_connectivity_performance_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_event_retries_entity.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_event_retries_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_if_name.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_if_name.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_performance_entity.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_performance_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_performance_retries_entity.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_performance_retries_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_quality_index_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_quality_index_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_time_to_connect_entity.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_time_to_connect_entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_time_to_connect_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_time_to_connect_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_views_list_type.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_anomalies_count_vo_entity.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_wireless_views_list_type import XiqWirelessViewsListType  # noqa: E501
+from extremecloudiq.models.xiq_anomalies_count_vo_entity import XiqAnomaliesCountVoEntity  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqWirelessViewsListType(unittest.TestCase):
-    """XiqWirelessViewsListType unit test stubs"""
+class TestXiqAnomaliesCountVoEntity(unittest.TestCase):
+    """XiqAnomaliesCountVoEntity unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqWirelessViewsListType
+        """Test XiqAnomaliesCountVoEntity
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_wireless_views_list_type.XiqWirelessViewsListType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_anomalies_count_vo_entity.XiqAnomaliesCountVoEntity()  # noqa: E501
         if include_optional :
-            return XiqWirelessViewsListType(
+            return XiqAnomaliesCountVoEntity(
+                timestamp = 56, 
+                total_anomalies_count = 56, 
+                wifi_efficiency_count = 56, 
+                wifi_capacity_count = 56, 
+                poe_count = 56, 
+                pe_count = 56, 
+                dfs_count = 56, 
+                mb_cast_count = 56
             )
         else :
-            return XiqWirelessViewsListType(
+            return XiqAnomaliesCountVoEntity(
+                timestamp = 56,
         )
 
-    def testXiqWirelessViewsListType(self):
-        """Test XiqWirelessViewsListType"""
+    def testXiqAnomaliesCountVoEntity(self):
+        """Test XiqAnomaliesCountVoEntity"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.2.0.4/test/test_xiq_wireless_views_type_response.py` & `extremecloudiq-api-23.2.1.4/test/test_xiq_wireless_views_type_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.2.0.4/README.md` & `extremecloudiq-api-23.2.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # extremecloudiq-api
 ExtremeCloud IQ RESTful API for external and internal applications.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 23.2.0.4
-- Package version: 23.2.0.4
+- API version: 23.2.1.4
+- Package version: 23.2.1.4
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.extremenetworks.com/support](https://www.extremenetworks.com/support)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -104,14 +104,16 @@
 *AuthenticationApi* | [**login**](docs/AuthenticationApi.md#login) | **POST** /login | User login with username and password
 *AuthenticationApi* | [**logout**](docs/AuthenticationApi.md#logout) | **POST** /logout | User logout (Revoke the current access token)
 *AuthorizationApi* | [**check_permissions**](docs/AuthorizationApi.md#check_permissions) | **POST** /auth/permissions/:check | Check permissions
 *AuthorizationApi* | [**generate_api_token**](docs/AuthorizationApi.md#generate_api_token) | **POST** /auth/apitoken | Generate new API token
 *AuthorizationApi* | [**get_current_api_token_info**](docs/AuthorizationApi.md#get_current_api_token_info) | **GET** /auth/apitoken/info | Get current API token details
 *AuthorizationApi* | [**list_permissions**](docs/AuthorizationApi.md#list_permissions) | **GET** /auth/permissions | Get permissions for current login user
 *AuthorizationApi* | [**validate_api_token**](docs/AuthorizationApi.md#validate_api_token) | **POST** /auth/apitoken/:validate | Validate API token
+*ClientApi* | [**disconnect_client**](docs/ClientApi.md#disconnect_client) | **DELETE** /clients/byMac/{clientMac} | Disconnect the client
+*ClientApi* | [**get_active_clients_count**](docs/ClientApi.md#get_active_clients_count) | **GET** /clients/active/count | Get active clients count
 *ClientApi* | [**get_client**](docs/ClientApi.md#get_client) | **GET** /clients/{id} | Get client info
 *ClientApi* | [**get_client_summary**](docs/ClientApi.md#get_client_summary) | **GET** /clients/summary | Get client summary metrics
 *ClientApi* | [**get_client_usage**](docs/ClientApi.md#get_client_usage) | **GET** /clients/usage | Get usage per client
 *ClientApi* | [**list_active_clients**](docs/ClientApi.md#list_active_clients) | **GET** /clients/active | List active clients
 *ConfigurationAuthenticationApi* | [**create_external_radius_server**](docs/ConfigurationAuthenticationApi.md#create_external_radius_server) | **POST** /radius-servers/external | Create external RADIUS server configuration
 *ConfigurationAuthenticationApi* | [**create_internal_radius_server**](docs/ConfigurationAuthenticationApi.md#create_internal_radius_server) | **POST** /radius-servers/internal | Create internal RADIUS server configuration
 *ConfigurationAuthenticationApi* | [**create_ldap_server**](docs/ConfigurationAuthenticationApi.md#create_ldap_server) | **POST** /ldap-servers | Create LDAP server
@@ -222,16 +224,21 @@
 *ConfigurationUserManagementApi* | [**list_user_groups**](docs/ConfigurationUserManagementApi.md#list_user_groups) | **GET** /usergroups | List user groups
 *ConfigurationUserManagementApi* | [**onboard_key_based_private_client_group**](docs/ConfigurationUserManagementApi.md#onboard_key_based_private_client_group) | **POST** /pcgs/key-based/network-policy-{policyId}/:onboard | Create Key-based PCG in network policy
 *ConfigurationUserManagementApi* | [**regenerate_end_user_password**](docs/ConfigurationUserManagementApi.md#regenerate_end_user_password) | **POST** /endusers/{id}/:regenerate-password | Regenerate a new password for the end user
 *ConfigurationUserManagementApi* | [**setup_key_based_private_client_group_network_policy**](docs/ConfigurationUserManagementApi.md#setup_key_based_private_client_group_network_policy) | **POST** /pcgs/key-based | Setup a Key-based Private Client Group
 *ConfigurationUserManagementApi* | [**update_end_user**](docs/ConfigurationUserManagementApi.md#update_end_user) | **PUT** /endusers/{id} | Update an end user
 *ConfigurationUserManagementApi* | [**update_key_based_pcg_users**](docs/ConfigurationUserManagementApi.md#update_key_based_pcg_users) | **PUT** /pcgs/key-based/network-policy-{policyId}/users | Replace all users in a PCG-enabled network policy
 *ConfigurationUserManagementApi* | [**update_user_group**](docs/ConfigurationUserManagementApi.md#update_user_group) | **PUT** /usergroups/{id} | Update user group
+*CopilotAnomaliesApi* | [**get_assurance_scans_overview_data**](docs/CopilotAnomaliesApi.md#get_assurance_scans_overview_data) | **GET** /copilot/assurance-scans/overview | 
 *CopilotAnomaliesApi* | [**get_devices_by_location**](docs/CopilotAnomaliesApi.md#get_devices_by_location) | **GET** /copilot/anomalies/devices-by-location | 
+*CopilotAnomaliesApi* | [**get_dfs_recurrence_channel_stats**](docs/CopilotAnomaliesApi.md#get_dfs_recurrence_channel_stats) | **GET** /copilot/anomalies/dfs-recurrence/channel-stats | 
+*CopilotAnomaliesApi* | [**get_dfs_recurrence_count_stats**](docs/CopilotAnomaliesApi.md#get_dfs_recurrence_count_stats) | **GET** /copilot/anomalies/dfs-recurrence/count-stats | 
 *CopilotAnomaliesApi* | [**get_poe_flapping_stats**](docs/CopilotAnomaliesApi.md#get_poe_flapping_stats) | **GET** /copilot/anomalies/poeflapping/stats | 
+*CopilotAnomaliesApi* | [**get_port_efficiency_speed_duplex_stats**](docs/CopilotAnomaliesApi.md#get_port_efficiency_speed_duplex_stats) | **GET** /copilot/anomalies/port-efficiency/speed-duplex-stats | 
+*CopilotAnomaliesApi* | [**get_port_efficiency_stats**](docs/CopilotAnomaliesApi.md#get_port_efficiency_stats) | **GET** /copilot/anomalies/port-efficiency/stats | 
 *CopilotAnomaliesApi* | [**list_anomaly_locations**](docs/CopilotAnomaliesApi.md#list_anomaly_locations) | **GET** /copilot/anomalies/locations | 
 *CopilotConnectivityExperienceApi* | [**get_wired_connectivity_experience**](docs/CopilotConnectivityExperienceApi.md#get_wired_connectivity_experience) | **GET** /copilot/connectivity/wired/experience | 
 *CopilotConnectivityExperienceApi* | [**get_wired_events**](docs/CopilotConnectivityExperienceApi.md#get_wired_events) | **GET** /copilot/connectivity/wired/events | 
 *CopilotConnectivityExperienceApi* | [**get_wired_hardware**](docs/CopilotConnectivityExperienceApi.md#get_wired_hardware) | **GET** /copilot/connectivity/wired/hardware | 
 *CopilotConnectivityExperienceApi* | [**get_wired_quality_index**](docs/CopilotConnectivityExperienceApi.md#get_wired_quality_index) | **GET** /copilot/connectivity/wired/quality-index | 
 *CopilotConnectivityExperienceApi* | [**get_wireless_apps**](docs/CopilotConnectivityExperienceApi.md#get_wireless_apps) | **GET** /copilot/connectivity/wireless/apps | 
 *CopilotConnectivityExperienceApi* | [**get_wireless_connectivity_experience**](docs/CopilotConnectivityExperienceApi.md#get_wireless_connectivity_experience) | **GET** /copilot/connectivity/wireless/experience | 
@@ -242,14 +249,15 @@
 *CopilotConnectivityExperienceApi* | [**get_wireless_views**](docs/CopilotConnectivityExperienceApi.md#get_wireless_views) | **GET** /copilot/connectivity/wireless/views | 
 *DeviceApi* | [**assign_device_location**](docs/DeviceApi.md#assign_device_location) | **PUT** /devices/{id}/location | Assign location to a device
 *DeviceApi* | [**assign_device_network_policy**](docs/DeviceApi.md#assign_device_network_policy) | **PUT** /devices/{id}/network-policy | Assign network policy to a device
 *DeviceApi* | [**assign_devices_country_code**](docs/DeviceApi.md#assign_devices_country_code) | **POST** /devices/country-code/:assign | Assign a country code to devices
 *DeviceApi* | [**assign_devices_location**](docs/DeviceApi.md#assign_devices_location) | **POST** /devices/location/:assign | Assign location to multiple devices
 *DeviceApi* | [**assign_devices_network_policy**](docs/DeviceApi.md#assign_devices_network_policy) | **POST** /devices/network-policy/:assign | Assign network policy to multiple devices
 *DeviceApi* | [**assign_devices_radius_proxy**](docs/DeviceApi.md#assign_devices_radius_proxy) | **PUT** /devices/radius-proxy/:assign | Assign RADIUS proxy to devices
+*DeviceApi* | [**bounce_device_port**](docs/DeviceApi.md#bounce_device_port) | **POST** /devices/{id}/bounce-port | Bounce port of a device (EXOS, VOSS and SR Switches
 *DeviceApi* | [**change_device_description**](docs/DeviceApi.md#change_device_description) | **PUT** /devices/{id}/description | Change description for a device
 *DeviceApi* | [**change_device_level_ssid_status**](docs/DeviceApi.md#change_device_level_ssid_status) | **POST** /devices/{id}/ssid/status/:change | Enable or disable SSID for a device
 *DeviceApi* | [**change_device_status_to_manage**](docs/DeviceApi.md#change_device_status_to_manage) | **POST** /devices/{id}/:manage | Change admin state to &#39;Managed&#39; for a device
 *DeviceApi* | [**change_device_status_to_unmanage**](docs/DeviceApi.md#change_device_status_to_unmanage) | **POST** /devices/{id}/:unmanage | Change admin state to &#39;Unmanaged&#39; for a device
 *DeviceApi* | [**change_devices_ibeacon**](docs/DeviceApi.md#change_devices_ibeacon) | **PUT** /devices/ibeacon | Change iBeacon settings for devices
 *DeviceApi* | [**change_devices_os_mode**](docs/DeviceApi.md#change_devices_os_mode) | **POST** /devices/os/:change | Change device OS mode
 *DeviceApi* | [**change_hostname**](docs/DeviceApi.md#change_hostname) | **PUT** /devices/{id}/hostname | Change hostname for a device
@@ -260,14 +268,16 @@
 *DeviceApi* | [**get_device**](docs/DeviceApi.md#get_device) | **GET** /devices/{id} | Get device info for a specific device
 *DeviceApi* | [**get_device_cpu_memory_history**](docs/DeviceApi.md#get_device_cpu_memory_history) | **GET** /devices/{id}/history/cpu-mem | Get device CPU/memory usage history
 *DeviceApi* | [**get_device_ibeacon**](docs/DeviceApi.md#get_device_ibeacon) | **GET** /devices/{id}/ibeacon | Get the device iBeacon setting
 *DeviceApi* | [**get_device_level_ssid_status**](docs/DeviceApi.md#get_device_level_ssid_status) | **GET** /devices/{id}/ssid/status | Get SSID status for a device
 *DeviceApi* | [**get_device_location**](docs/DeviceApi.md#get_device_location) | **GET** /devices/{id}/location | Get location for a device
 *DeviceApi* | [**get_device_network_policy**](docs/DeviceApi.md#get_device_network_policy) | **GET** /devices/{id}/network-policy | Get network policy for a device
 *DeviceApi* | [**get_device_stats**](docs/DeviceApi.md#get_device_stats) | **GET** /devices/stats | Get device stats
+*DeviceApi* | [**get_device_wifi_interface**](docs/DeviceApi.md#get_device_wifi_interface) | **GET** /devices/{id}/interfaces/wifi | Get the device WiFi interfaces stats
+*DeviceApi* | [**get_xiq_device_installation_report**](docs/DeviceApi.md#get_xiq_device_installation_report) | **GET** /devices/{id}/installation-report | Get device installation report
 *DeviceApi* | [**list_device_alarm**](docs/DeviceApi.md#list_device_alarm) | **GET** /devices/{id}/alarms | List alarms for a device
 *DeviceApi* | [**list_devices**](docs/DeviceApi.md#list_devices) | **GET** /devices | [LRO] List devices
 *DeviceApi* | [**list_devices_by_network_policy**](docs/DeviceApi.md#list_devices_by_network_policy) | **GET** /devices/network-policy/{policyId} | List assigned devices for network policy
 *DeviceApi* | [**onboard_devices**](docs/DeviceApi.md#onboard_devices) | **POST** /devices/:onboard | Onboard Devices
 *DeviceApi* | [**override_device_level_ssid**](docs/DeviceApi.md#override_device_level_ssid) | **POST** /devices/{id}/ssid/:override | Override SSID for a device
 *DeviceApi* | [**query_devices_location**](docs/DeviceApi.md#query_devices_location) | **POST** /devices/location/:query | Query location for multiple devices
 *DeviceApi* | [**query_devices_network_policy**](docs/DeviceApi.md#query_devices_network_policy) | **POST** /devices/network-policy/:query | Query network policy for multiple devices
@@ -383,14 +393,15 @@
  - [XiqActiveDirectoryServerBaseDnFetchMode](docs/XiqActiveDirectoryServerBaseDnFetchMode.md)
  - [XiqAlert](docs/XiqAlert.md)
  - [XiqAlertCategory](docs/XiqAlertCategory.md)
  - [XiqAlertGroupQuery](docs/XiqAlertGroupQuery.md)
  - [XiqAlertSeverity](docs/XiqAlertSeverity.md)
  - [XiqAlertSource](docs/XiqAlertSource.md)
  - [XiqAlertSourceType](docs/XiqAlertSourceType.md)
+ - [XiqAnomaliesCountVoEntity](docs/XiqAnomaliesCountVoEntity.md)
  - [XiqAnomalyDeviceEntity](docs/XiqAnomalyDeviceEntity.md)
  - [XiqAnomalyDevicesByLocationResponse](docs/XiqAnomalyDevicesByLocationResponse.md)
  - [XiqAnomalyLocationEntity](docs/XiqAnomalyLocationEntity.md)
  - [XiqAnomalySeverity](docs/XiqAnomalySeverity.md)
  - [XiqAnomalySortField](docs/XiqAnomalySortField.md)
  - [XiqAnomalyType](docs/XiqAnomalyType.md)
  - [XiqApiTokenInfo](docs/XiqApiTokenInfo.md)
@@ -399,31 +410,37 @@
  - [XiqApplicationDetectionRule](docs/XiqApplicationDetectionRule.md)
  - [XiqApplicationDetectionType](docs/XiqApplicationDetectionType.md)
  - [XiqApplicationSortField](docs/XiqApplicationSortField.md)
  - [XiqApplicationTopClientsUsage](docs/XiqApplicationTopClientsUsage.md)
  - [XiqAssignDevicesCountryCodeRequest](docs/XiqAssignDevicesCountryCodeRequest.md)
  - [XiqAssignDevicesLocationRequest](docs/XiqAssignDevicesLocationRequest.md)
  - [XiqAssignDevicesNetworkPolicyRequest](docs/XiqAssignDevicesNetworkPolicyRequest.md)
+ - [XiqAssuranceScansOverviewResponse](docs/XiqAssuranceScansOverviewResponse.md)
  - [XiqAuditLog](docs/XiqAuditLog.md)
  - [XiqAuditLogCategory](docs/XiqAuditLogCategory.md)
  - [XiqAuthLog](docs/XiqAuthLog.md)
+ - [XiqBounceDevicePortData](docs/XiqBounceDevicePortData.md)
+ - [XiqBounceDevicePortOperationResult](docs/XiqBounceDevicePortOperationResult.md)
+ - [XiqBounceDevicePortRequest](docs/XiqBounceDevicePortRequest.md)
+ - [XiqBounceDevicePortResponse](docs/XiqBounceDevicePortResponse.md)
  - [XiqBuilding](docs/XiqBuilding.md)
  - [XiqCertificate](docs/XiqCertificate.md)
  - [XiqCertificateType](docs/XiqCertificateType.md)
  - [XiqChangeDevicesIbeaconRequest](docs/XiqChangeDevicesIbeaconRequest.md)
  - [XiqChangeDevicesOsModeRequest](docs/XiqChangeDevicesOsModeRequest.md)
  - [XiqCheckPermissionRequest](docs/XiqCheckPermissionRequest.md)
  - [XiqCheckPermissionResponse](docs/XiqCheckPermissionResponse.md)
  - [XiqClassification](docs/XiqClassification.md)
  - [XiqClassificationRule](docs/XiqClassificationRule.md)
  - [XiqClassificationType](docs/XiqClassificationType.md)
  - [XiqCliOutput](docs/XiqCliOutput.md)
  - [XiqCliResponseCode](docs/XiqCliResponseCode.md)
  - [XiqClient](docs/XiqClient.md)
  - [XiqClientField](docs/XiqClientField.md)
+ - [XiqClientSortField](docs/XiqClientSortField.md)
  - [XiqClientSummary](docs/XiqClientSummary.md)
  - [XiqClientUsage](docs/XiqClientUsage.md)
  - [XiqClientView](docs/XiqClientView.md)
  - [XiqCloudConfigGroup](docs/XiqCloudConfigGroup.md)
  - [XiqConnectivityExperienceData](docs/XiqConnectivityExperienceData.md)
  - [XiqConnectivityExperienceViewType](docs/XiqConnectivityExperienceViewType.md)
  - [XiqCopilotEventsWiredSortField](docs/XiqCopilotEventsWiredSortField.md)
@@ -476,22 +493,30 @@
  - [XiqDeviceAdminState](docs/XiqDeviceAdminState.md)
  - [XiqDeviceAlarm](docs/XiqDeviceAlarm.md)
  - [XiqDeviceCpuMemoryUsage](docs/XiqDeviceCpuMemoryUsage.md)
  - [XiqDeviceField](docs/XiqDeviceField.md)
  - [XiqDeviceFilter](docs/XiqDeviceFilter.md)
  - [XiqDeviceFunction](docs/XiqDeviceFunction.md)
  - [XiqDeviceIbeacon](docs/XiqDeviceIbeacon.md)
+ - [XiqDeviceInstallationReport](docs/XiqDeviceInstallationReport.md)
  - [XiqDeviceLevelSsid](docs/XiqDeviceLevelSsid.md)
  - [XiqDeviceLevelSsidStatus](docs/XiqDeviceLevelSsidStatus.md)
+ - [XiqDeviceLldpCdpInfo](docs/XiqDeviceLldpCdpInfo.md)
  - [XiqDeviceLocation](docs/XiqDeviceLocation.md)
  - [XiqDeviceLocationAssignment](docs/XiqDeviceLocationAssignment.md)
  - [XiqDeviceSortField](docs/XiqDeviceSortField.md)
  - [XiqDeviceStats](docs/XiqDeviceStats.md)
  - [XiqDeviceType](docs/XiqDeviceType.md)
  - [XiqDeviceView](docs/XiqDeviceView.md)
+ - [XiqDeviceWifiInterface](docs/XiqDeviceWifiInterface.md)
+ - [XiqDfsChannelChangesEntity](docs/XiqDfsChannelChangesEntity.md)
+ - [XiqDfsChannelStatsEntity](docs/XiqDfsChannelStatsEntity.md)
+ - [XiqDfsRecurenceChannelStatsResponse](docs/XiqDfsRecurenceChannelStatsResponse.md)
+ - [XiqDfsRecurenceCountStatsResponse](docs/XiqDfsRecurenceCountStatsResponse.md)
+ - [XiqDuplexDataRateEntity](docs/XiqDuplexDataRateEntity.md)
  - [XiqEmailLog](docs/XiqEmailLog.md)
  - [XiqEmailTemplate](docs/XiqEmailTemplate.md)
  - [XiqEndUser](docs/XiqEndUser.md)
  - [XiqEntitlementType](docs/XiqEntitlementType.md)
  - [XiqError](docs/XiqError.md)
  - [XiqExosDevices](docs/XiqExosDevices.md)
  - [XiqExpirationActionType](docs/XiqExpirationActionType.md)
@@ -558,14 +583,16 @@
  - [XiqPcgPortAssignmentEntry](docs/XiqPcgPortAssignmentEntry.md)
  - [XiqPcgPortAssignmentEntryDetail](docs/XiqPcgPortAssignmentEntryDetail.md)
  - [XiqPcgPortAssignmentEntryDeviceMeta](docs/XiqPcgPortAssignmentEntryDeviceMeta.md)
  - [XiqPcgPortAssignmentEntryEthUserMeta](docs/XiqPcgPortAssignmentEntryEthUserMeta.md)
  - [XiqPcgType](docs/XiqPcgType.md)
  - [XiqPermission](docs/XiqPermission.md)
  - [XiqPoeFlappingStatsResponse](docs/XiqPoeFlappingStatsResponse.md)
+ - [XiqPortEfficiencySpeedDuplexStatsResponse](docs/XiqPortEfficiencySpeedDuplexStatsResponse.md)
+ - [XiqPortEfficiencyStatsResponse](docs/XiqPortEfficiencyStatsResponse.md)
  - [XiqPostExpirationAction](docs/XiqPostExpirationAction.md)
  - [XiqPskGenerationMethod](docs/XiqPskGenerationMethod.md)
  - [XiqRadioMode](docs/XiqRadioMode.md)
  - [XiqRadioProfile](docs/XiqRadioProfile.md)
  - [XiqRadiusClient](docs/XiqRadiusClient.md)
  - [XiqRadiusClientObject](docs/XiqRadiusClientObject.md)
  - [XiqRadiusClientObjectEntry](docs/XiqRadiusClientObjectEntry.md)
@@ -591,14 +618,15 @@
  - [XiqSetSsidModePskRequest](docs/XiqSetSsidModePskRequest.md)
  - [XiqSetSsidModeWepRequest](docs/XiqSetSsidModeWepRequest.md)
  - [XiqSmsLog](docs/XiqSmsLog.md)
  - [XiqSmsLogStatus](docs/XiqSmsLogStatus.md)
  - [XiqSmsTemplate](docs/XiqSmsTemplate.md)
  - [XiqSortField](docs/XiqSortField.md)
  - [XiqSortOrder](docs/XiqSortOrder.md)
+ - [XiqSpeedDuplexEntity](docs/XiqSpeedDuplexEntity.md)
  - [XiqSsid](docs/XiqSsid.md)
  - [XiqSsidDot1xEncryptionMethod](docs/XiqSsidDot1xEncryptionMethod.md)
  - [XiqSsidDot1xKeyManagement](docs/XiqSsidDot1xKeyManagement.md)
  - [XiqSsidKeyType](docs/XiqSsidKeyType.md)
  - [XiqSsidPpskKeyManagement](docs/XiqSsidPpskKeyManagement.md)
  - [XiqSsidPskEncryptionMethod](docs/XiqSsidPskEncryptionMethod.md)
  - [XiqSsidPskKeyManagement](docs/XiqSsidPskKeyManagement.md)
```

### Comparing `extremecloudiq-api-23.2.0.4/setup.py` & `extremecloudiq-api-23.2.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.2.0.4
+    The version of the OpenAPI document: 23.2.1.4
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "extremecloudiq-api"
-VERSION = "23.2.0.4"
+VERSION = "23.2.1.4"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

