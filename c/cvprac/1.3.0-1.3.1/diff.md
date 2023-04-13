# Comparing `tmp/cvprac-1.3.0.tar.gz` & `tmp/cvprac-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprac-1.3.0.tar", last modified: Tue Mar  7 17:16:22 2023, max compression
+gzip compressed data, was "cvprac-1.3.1.tar", last modified: Thu Apr 13 15:55:33 2023, max compression
```

## Comparing `cvprac-1.3.0.tar` & `cvprac-1.3.1.tar`

### file list

```diff
@@ -1,126 +1,128 @@
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.904875 cvprac-1.3.0/
--rw-r--r--   0 mhartzel   (501) staff       (20)    16636 2020-02-04 01:08:03.000000 cvprac-1.3.0/.pylintrc
--rw-r--r--   0 mhartzel   (501) staff       (20)     1522 2019-09-25 14:39:35.000000 cvprac-1.3.0/LICENSE
--rw-r--r--   0 mhartzel   (501) staff       (20)      505 2022-10-07 20:29:41.000000 cvprac-1.3.0/MANIFEST.in
--rw-r--r--   0 mhartzel   (501) staff       (20)     2377 2022-05-20 17:35:24.000000 cvprac-1.3.0/Makefile
--rw-r--r--   0 mhartzel   (501) staff       (20)    18387 2023-03-07 17:16:22.903990 cvprac-1.3.0/PKG-INFO
--rw-r--r--   0 mhartzel   (501) staff       (20)    17444 2022-10-07 20:29:41.000000 cvprac-1.3.0/README.md
--rw-r--r--   0 mhartzel   (501) staff       (20)        6 2023-03-07 16:28:44.000000 cvprac-1.3.0/VERSION
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.478322 cvprac-1.3.0/cvprac/
--rw-r--r--   0 mhartzel   (501) staff       (20)     1649 2023-03-07 16:28:44.000000 cvprac-1.3.0/cvprac/__init__.py
--rw-r--r--   0 mhartzel   (501) staff       (20)   185122 2023-03-07 16:02:05.000000 cvprac-1.3.0/cvprac/cvp_api.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    49662 2023-03-07 16:02:05.000000 cvprac-1.3.0/cvprac/cvp_client.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     2477 2019-09-25 14:39:35.000000 cvprac-1.3.0/cvprac/cvp_client_errors.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.500813 cvprac-1.3.0/cvprac.egg-info/
--rw-r--r--   0 mhartzel   (501) staff       (20)    18387 2023-03-07 17:16:22.000000 cvprac-1.3.0/cvprac.egg-info/PKG-INFO
--rw-r--r--   0 mhartzel   (501) staff       (20)     4373 2023-03-07 17:16:22.000000 cvprac-1.3.0/cvprac.egg-info/SOURCES.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)        1 2023-03-07 17:16:22.000000 cvprac-1.3.0/cvprac.egg-info/dependency_links.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)       83 2023-03-07 17:16:22.000000 cvprac-1.3.0/cvprac.egg-info/requires.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)       26 2023-03-07 17:16:22.000000 cvprac-1.3.0/cvprac.egg-info/top_level.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)      855 2019-09-25 14:39:35.000000 cvprac-1.3.0/cvprac.spec
--rw-r--r--   0 mhartzel   (501) staff       (20)       68 2022-10-07 20:29:41.000000 cvprac-1.3.0/dev-requirements.txt
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.678015 cvprac-1.3.0/docs/
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.693643 cvprac-1.3.0/docs/labs/
--rw-r--r--   0 mhartzel   (501) staff       (20)     2373 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/README.md
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.701586 cvprac-1.3.0/docs/labs/lab01-cvp-info/
--rw-r--r--   0 mhartzel   (501) staff       (20)      519 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab01-cvp-info/get_cvp_info.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.732587 cvprac-1.3.0/docs/labs/lab02-inventory-operations/
--rw-r--r--   0 mhartzel   (501) staff       (20)     2514 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab02-inventory-operations/compliance_check.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1010 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab02-inventory-operations/get_running_configs.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1139 2022-10-07 20:29:41.000000 cvprac-1.3.0/docs/labs/lab02-inventory-operations/get_running_configs_by_time.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1208 2022-10-07 20:29:41.000000 cvprac-1.3.0/docs/labs/lab02-inventory-operations/remove_all_devices_legacy.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1287 2022-10-07 20:29:41.000000 cvprac-1.3.0/docs/labs/lab02-inventory-operations/remove_and_decommission_device.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1289 2022-10-07 20:29:41.000000 cvprac-1.3.0/docs/labs/lab02-inventory-operations/remove_devices_from_container_legacy.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1315 2022-10-07 20:29:41.000000 cvprac-1.3.0/docs/labs/lab02-inventory-operations/remove_devices_legacy.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.792679 cvprac-1.3.0/docs/labs/lab03-configlet-management/
--rw-r--r--   0 mhartzel   (501) staff       (20)      707 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab03-configlet-management/assign_configlet_to_device.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      669 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab03-configlet-management/backup_configlets.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1514 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab03-configlet-management/backup_configletsV2.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      124 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab03-configlet-management/common.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     2100 2022-10-07 20:29:41.000000 cvprac-1.3.0/docs/labs/lab03-configlet-management/config_search.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      121 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab03-configlet-management/configlet_list.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)      648 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab03-configlet-management/create_configlet.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      615 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab03-configlet-management/create_configlet_from_file.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1351 2023-03-07 16:02:05.000000 cvprac-1.3.0/docs/labs/lab03-configlet-management/get_applied_netelements.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1616 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab03-configlet-management/get_configlets.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      861 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab03-configlet-management/reorder_configlet_on_device.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      766 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab03-configlet-management/update_configlet.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.817778 cvprac-1.3.0/docs/labs/lab04-container-management/
--rw-r--r--   0 mhartzel   (501) staff       (20)      673 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab04-container-management/add_image_to_container.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      721 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab04-container-management/assign_configlet_to_container.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      655 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab04-container-management/create_container.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      676 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab04-container-management/remove_image_from_container.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1026 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab04-container-management/rename_container.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.837751 cvprac-1.3.0/docs/labs/lab05-device-management/
--rw-r--r--   0 mhartzel   (501) staff       (20)      659 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab05-device-management/add_image_to_devices.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     4334 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab05-device-management/add_image_wo_tempaction.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      662 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab05-device-management/remove_image_from_device.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1244 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab05-device-management/set_mgmt_ip.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.853471 cvprac-1.3.0/docs/labs/lab06-provisioning/
--rw-r--r--   0 mhartzel   (501) staff       (20)     5781 2023-03-07 16:02:05.000000 cvprac-1.3.0/docs/labs/lab06-provisioning/atd_e2e_provisioning_workflow.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     2864 2022-10-07 20:29:41.000000 cvprac-1.3.0/docs/labs/lab06-provisioning/auto_reconcile_on_rc_change.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     3562 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab06-provisioning/change_control_custom_rapi.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      890 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab06-provisioning/change_control_workflow.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1506 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab06-provisioning/change_control_workflow_rapi.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.859080 cvprac-1.3.0/docs/labs/lab06-provisioning/configlets/
--rw-r--r--   0 mhartzel   (501) staff       (20)     6573 2023-03-07 16:02:05.000000 cvprac-1.3.0/docs/labs/lab06-provisioning/configlets/AVD_leaf1.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     6573 2023-03-07 16:02:05.000000 cvprac-1.3.0/docs/labs/lab06-provisioning/configlets/AVD_leaf2.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     6577 2023-03-07 16:02:05.000000 cvprac-1.3.0/docs/labs/lab06-provisioning/configlets/AVD_leaf3.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     6581 2023-03-07 16:02:05.000000 cvprac-1.3.0/docs/labs/lab06-provisioning/configlets/AVD_leaf4.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     3654 2023-03-07 16:02:05.000000 cvprac-1.3.0/docs/labs/lab06-provisioning/configlets/AVD_spine1.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     3658 2023-03-07 16:02:05.000000 cvprac-1.3.0/docs/labs/lab06-provisioning/configlets/AVD_spine2.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     2184 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab06-provisioning/gen_builder.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     8347 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab06-provisioning/mlag_issu.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      781 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab06-provisioning/move_device.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     4909 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab06-provisioning/vc_task_retrigger.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.870446 cvprac-1.3.0/docs/labs/lab07-aaa/
--rw-r--r--   0 mhartzel   (501) staff       (20)      263 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab07-aaa/aaa_users.csv
--rw-r--r--   0 mhartzel   (501) staff       (20)      964 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab07-aaa/add_new_user_cvaas.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      823 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab07-aaa/add_new_user_onprem.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1078 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab07-aaa/add_users_from_csv_cvaas.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      786 2022-10-07 20:29:41.000000 cvprac-1.3.0/docs/labs/lab07-aaa/create_svc_account.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      854 2022-10-07 20:29:41.000000 cvprac-1.3.0/docs/labs/lab07-aaa/create_svc_account_token.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1106 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab07-aaa/create_terminattr_tokens.py
--rw-r--r--   0 mhartzel   (501) staff       (20)       33 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab07-aaa/cvaas.tok
--rw-r--r--   0 mhartzel   (501) staff       (20)      576 2022-10-07 20:29:41.000000 cvprac-1.3.0/docs/labs/lab07-aaa/delete_all_expired_svc_account_tokens.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      590 2022-10-07 20:29:41.000000 cvprac-1.3.0/docs/labs/lab07-aaa/delete_svc_account.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      808 2023-03-07 16:02:05.000000 cvprac-1.3.0/docs/labs/lab07-aaa/delete_svc_account_created_by_user.py
--rw-r--r--   0 mhartzel   (501) staff       (20)      673 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab07-aaa/get_user_info.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1013 2022-10-07 20:29:41.000000 cvprac-1.3.0/docs/labs/lab07-aaa/svc_account_misc.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.872025 cvprac-1.3.0/docs/labs/lab08-resource-apis/
--rw-r--r--   0 mhartzel   (501) staff       (20)     6229 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/lab08-resource-apis/resource_cvprac.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     4449 2023-03-07 16:02:05.000000 cvprac-1.3.0/docs/labs/lab08-resource-apis/topology_tag_assignment.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.877377 cvprac-1.3.0/docs/labs/static/
--rw-r--r--   0 mhartzel   (501) staff       (20)   117691 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/static/serviceaccount1.png
--rw-r--r--   0 mhartzel   (501) staff       (20)   123315 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/static/serviceaccount2.png
--rw-r--r--   0 mhartzel   (501) staff       (20)   106538 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/labs/static/serviceaccount3.png
--rw-r--r--   0 mhartzel   (501) staff       (20)     1999 2019-09-25 14:39:35.000000 cvprac-1.3.0/docs/release-notes-0.7.0.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     2157 2019-09-25 14:39:35.000000 cvprac-1.3.0/docs/release-notes-0.8.0.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     2384 2019-09-25 14:39:35.000000 cvprac-1.3.0/docs/release-notes-0.9.0.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     3171 2019-09-25 14:39:35.000000 cvprac-1.3.0/docs/release-notes-1.0.0.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1759 2019-09-25 14:39:35.000000 cvprac-1.3.0/docs/release-notes-1.0.1.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     3148 2020-02-04 01:24:48.000000 cvprac-1.3.0/docs/release-notes-1.0.2.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)      303 2020-06-04 16:29:41.000000 cvprac-1.3.0/docs/release-notes-1.0.3.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     3328 2020-08-18 17:37:36.000000 cvprac-1.3.0/docs/release-notes-1.0.4.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1588 2021-05-17 20:03:41.000000 cvprac-1.3.0/docs/release-notes-1.0.5.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     2154 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/release-notes-1.0.6.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1407 2022-05-20 17:35:24.000000 cvprac-1.3.0/docs/release-notes-1.0.7.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     3350 2022-05-20 21:38:36.000000 cvprac-1.3.0/docs/release-notes-1.2.0.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1523 2022-10-10 14:46:28.000000 cvprac-1.3.0/docs/release-notes-1.2.2.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1716 2023-03-07 16:28:44.000000 cvprac-1.3.0/docs/release-notes-1.3.0.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)       24 2023-03-07 16:02:05.000000 cvprac-1.3.0/requirements.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)       38 2023-03-07 17:16:22.905077 cvprac-1.3.0/setup.cfg
--rw-r--r--   0 mhartzel   (501) staff       (20)     4721 2023-03-07 16:02:05.000000 cvprac-1.3.0/setup.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.343214 cvprac-1.3.0/test/
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.880656 cvprac-1.3.0/test/fixtures/
--rw-r--r--   0 mhartzel   (501) staff       (20)      398 2023-03-06 22:32:53.000000 cvprac-1.3.0/test/fixtures/cvp_nodes.yaml
--rw-r--r--   0 mhartzel   (501) staff       (20)  3941571 2019-09-25 14:39:35.000000 cvprac-1.3.0/test/fixtures/image-file.swix
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.894307 cvprac-1.3.0/test/lib/
--rw-r--r--   0 mhartzel   (501) staff       (20)     2634 2023-03-07 16:02:05.000000 cvprac-1.3.0/test/lib/systestlib.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.901333 cvprac-1.3.0/test/system/
--rw-r--r--   0 mhartzel   (501) staff       (20)     6699 2023-03-07 16:02:05.000000 cvprac-1.3.0/test/system/test_cvp_base.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    34161 2023-03-07 15:44:06.000000 cvprac-1.3.0/test/system/test_cvp_change_control_api.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    18114 2022-05-20 17:35:24.000000 cvprac-1.3.0/test/system/test_cvp_client.py
--rw-r--r--   0 mhartzel   (501) staff       (20)   116901 2023-03-07 16:02:05.000000 cvprac-1.3.0/test/system/test_cvp_client_api.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-03-07 17:16:22.902834 cvprac-1.3.0/test/unit/
--rw-r--r--   0 mhartzel   (501) staff       (20)    26712 2023-03-07 16:02:05.000000 cvprac-1.3.0/test/unit/test_client.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.613809 cvprac-1.3.1/
+-rw-r--r--   0 mhartzel   (501) staff       (20)    16636 2020-02-04 01:08:03.000000 cvprac-1.3.1/.pylintrc
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1522 2019-09-25 14:39:35.000000 cvprac-1.3.1/LICENSE
+-rw-r--r--   0 mhartzel   (501) staff       (20)      505 2022-10-07 20:29:41.000000 cvprac-1.3.1/MANIFEST.in
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2377 2022-05-20 17:35:24.000000 cvprac-1.3.1/Makefile
+-rw-r--r--   0 mhartzel   (501) staff       (20)    18387 2023-04-13 15:55:33.613223 cvprac-1.3.1/PKG-INFO
+-rw-r--r--   0 mhartzel   (501) staff       (20)    17444 2022-10-07 20:29:41.000000 cvprac-1.3.1/README.md
+-rw-r--r--   0 mhartzel   (501) staff       (20)        6 2023-04-13 15:53:28.000000 cvprac-1.3.1/VERSION
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:32.786621 cvprac-1.3.1/cvprac/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1649 2023-04-13 15:53:28.000000 cvprac-1.3.1/cvprac/__init__.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)   187191 2023-04-13 15:49:42.000000 cvprac-1.3.1/cvprac/cvp_api.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)    49662 2023-03-07 16:02:05.000000 cvprac-1.3.1/cvprac/cvp_client.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2477 2019-09-25 14:39:35.000000 cvprac-1.3.1/cvprac/cvp_client_errors.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:32.824365 cvprac-1.3.1/cvprac.egg-info/
+-rw-r--r--   0 mhartzel   (501) staff       (20)    18387 2023-04-13 15:55:32.000000 cvprac-1.3.1/cvprac.egg-info/PKG-INFO
+-rw-r--r--   0 mhartzel   (501) staff       (20)     4424 2023-04-13 15:55:32.000000 cvprac-1.3.1/cvprac.egg-info/SOURCES.txt
+-rw-r--r--   0 mhartzel   (501) staff       (20)        1 2023-04-13 15:55:32.000000 cvprac-1.3.1/cvprac.egg-info/dependency_links.txt
+-rw-r--r--   0 mhartzel   (501) staff       (20)       83 2023-04-13 15:55:32.000000 cvprac-1.3.1/cvprac.egg-info/requires.txt
+-rw-r--r--   0 mhartzel   (501) staff       (20)       26 2023-04-13 15:55:32.000000 cvprac-1.3.1/cvprac.egg-info/top_level.txt
+-rw-r--r--   0 mhartzel   (501) staff       (20)      855 2019-09-25 14:39:35.000000 cvprac-1.3.1/cvprac.spec
+-rw-r--r--   0 mhartzel   (501) staff       (20)       68 2022-10-07 20:29:41.000000 cvprac-1.3.1/dev-requirements.txt
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.069627 cvprac-1.3.1/docs/
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.088745 cvprac-1.3.1/docs/labs/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2373 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/README.md
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.115081 cvprac-1.3.1/docs/labs/lab01-cvp-info/
+-rw-r--r--   0 mhartzel   (501) staff       (20)      519 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab01-cvp-info/get_cvp_info.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.150073 cvprac-1.3.1/docs/labs/lab02-inventory-operations/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2514 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab02-inventory-operations/compliance_check.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1010 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab02-inventory-operations/get_running_configs.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1139 2022-10-07 20:29:41.000000 cvprac-1.3.1/docs/labs/lab02-inventory-operations/get_running_configs_by_time.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1208 2022-10-07 20:29:41.000000 cvprac-1.3.1/docs/labs/lab02-inventory-operations/remove_all_devices_legacy.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1287 2022-10-07 20:29:41.000000 cvprac-1.3.1/docs/labs/lab02-inventory-operations/remove_and_decommission_device.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1289 2022-10-07 20:29:41.000000 cvprac-1.3.1/docs/labs/lab02-inventory-operations/remove_devices_from_container_legacy.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1315 2022-10-07 20:29:41.000000 cvprac-1.3.1/docs/labs/lab02-inventory-operations/remove_devices_legacy.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.229478 cvprac-1.3.1/docs/labs/lab03-configlet-management/
+-rw-r--r--   0 mhartzel   (501) staff       (20)      707 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab03-configlet-management/assign_configlet_to_device.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      669 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab03-configlet-management/backup_configlets.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1514 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab03-configlet-management/backup_configletsV2.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      124 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab03-configlet-management/common.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2100 2022-10-07 20:29:41.000000 cvprac-1.3.1/docs/labs/lab03-configlet-management/config_search.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      121 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab03-configlet-management/configlet_list.txt
+-rw-r--r--   0 mhartzel   (501) staff       (20)      648 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab03-configlet-management/create_configlet.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      615 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab03-configlet-management/create_configlet_from_file.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1351 2023-03-07 16:02:05.000000 cvprac-1.3.1/docs/labs/lab03-configlet-management/get_applied_netelements.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1616 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab03-configlet-management/get_configlets.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      861 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab03-configlet-management/reorder_configlet_on_device.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      766 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab03-configlet-management/update_configlet.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.251340 cvprac-1.3.1/docs/labs/lab04-container-management/
+-rw-r--r--   0 mhartzel   (501) staff       (20)      673 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab04-container-management/add_image_to_container.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      721 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab04-container-management/assign_configlet_to_container.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      655 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab04-container-management/create_container.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      676 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab04-container-management/remove_image_from_container.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1026 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab04-container-management/rename_container.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.266695 cvprac-1.3.1/docs/labs/lab05-device-management/
+-rw-r--r--   0 mhartzel   (501) staff       (20)      659 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab05-device-management/add_image_to_devices.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     4334 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab05-device-management/add_image_wo_tempaction.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      662 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab05-device-management/remove_image_from_device.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1244 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab05-device-management/set_mgmt_ip.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.308736 cvprac-1.3.1/docs/labs/lab06-provisioning/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     5781 2023-03-07 16:02:05.000000 cvprac-1.3.1/docs/labs/lab06-provisioning/atd_e2e_provisioning_workflow.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2864 2022-10-07 20:29:41.000000 cvprac-1.3.1/docs/labs/lab06-provisioning/auto_reconcile_on_rc_change.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     3562 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab06-provisioning/change_control_custom_rapi.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      890 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab06-provisioning/change_control_workflow.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1506 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab06-provisioning/change_control_workflow_rapi.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.386538 cvprac-1.3.1/docs/labs/lab06-provisioning/configlets/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     6573 2023-03-07 16:02:05.000000 cvprac-1.3.1/docs/labs/lab06-provisioning/configlets/AVD_leaf1.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     6573 2023-03-07 16:02:05.000000 cvprac-1.3.1/docs/labs/lab06-provisioning/configlets/AVD_leaf2.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     6577 2023-03-07 16:02:05.000000 cvprac-1.3.1/docs/labs/lab06-provisioning/configlets/AVD_leaf3.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     6581 2023-03-07 16:02:05.000000 cvprac-1.3.1/docs/labs/lab06-provisioning/configlets/AVD_leaf4.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     3654 2023-03-07 16:02:05.000000 cvprac-1.3.1/docs/labs/lab06-provisioning/configlets/AVD_spine1.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     3658 2023-03-07 16:02:05.000000 cvprac-1.3.1/docs/labs/lab06-provisioning/configlets/AVD_spine2.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2184 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab06-provisioning/gen_builder.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     8347 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab06-provisioning/mlag_issu.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      781 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab06-provisioning/move_device.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     4909 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab06-provisioning/vc_task_retrigger.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.519087 cvprac-1.3.1/docs/labs/lab07-aaa/
+-rw-r--r--   0 mhartzel   (501) staff       (20)      263 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab07-aaa/aaa_users.csv
+-rw-r--r--   0 mhartzel   (501) staff       (20)      964 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab07-aaa/add_new_user_cvaas.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      823 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab07-aaa/add_new_user_onprem.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1078 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab07-aaa/add_users_from_csv_cvaas.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      786 2022-10-07 20:29:41.000000 cvprac-1.3.1/docs/labs/lab07-aaa/create_svc_account.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      854 2022-10-07 20:29:41.000000 cvprac-1.3.1/docs/labs/lab07-aaa/create_svc_account_token.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1106 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab07-aaa/create_terminattr_tokens.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)       33 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab07-aaa/cvaas.tok
+-rw-r--r--   0 mhartzel   (501) staff       (20)      576 2022-10-07 20:29:41.000000 cvprac-1.3.1/docs/labs/lab07-aaa/delete_all_expired_svc_account_tokens.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      590 2022-10-07 20:29:41.000000 cvprac-1.3.1/docs/labs/lab07-aaa/delete_svc_account.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      808 2023-03-07 16:02:05.000000 cvprac-1.3.1/docs/labs/lab07-aaa/delete_svc_account_created_by_user.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)      673 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab07-aaa/get_user_info.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1013 2022-10-07 20:29:41.000000 cvprac-1.3.1/docs/labs/lab07-aaa/svc_account_misc.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.521700 cvprac-1.3.1/docs/labs/lab08-resource-apis/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     6229 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/lab08-resource-apis/resource_cvprac.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)     4449 2023-03-07 16:02:05.000000 cvprac-1.3.1/docs/labs/lab08-resource-apis/topology_tag_assignment.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.538862 cvprac-1.3.1/docs/labs/static/
+-rw-r--r--   0 mhartzel   (501) staff       (20)   117691 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/static/serviceaccount1.png
+-rw-r--r--   0 mhartzel   (501) staff       (20)   123315 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/static/serviceaccount2.png
+-rw-r--r--   0 mhartzel   (501) staff       (20)   106538 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/labs/static/serviceaccount3.png
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1999 2019-09-25 14:39:35.000000 cvprac-1.3.1/docs/release-notes-0.7.0.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2157 2019-09-25 14:39:35.000000 cvprac-1.3.1/docs/release-notes-0.8.0.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2384 2019-09-25 14:39:35.000000 cvprac-1.3.1/docs/release-notes-0.9.0.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     3171 2019-09-25 14:39:35.000000 cvprac-1.3.1/docs/release-notes-1.0.0.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1759 2019-09-25 14:39:35.000000 cvprac-1.3.1/docs/release-notes-1.0.1.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     3148 2020-02-04 01:24:48.000000 cvprac-1.3.1/docs/release-notes-1.0.2.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)      303 2020-06-04 16:29:41.000000 cvprac-1.3.1/docs/release-notes-1.0.3.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     3328 2020-08-18 17:37:36.000000 cvprac-1.3.1/docs/release-notes-1.0.4.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1588 2021-05-17 20:03:41.000000 cvprac-1.3.1/docs/release-notes-1.0.5.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2154 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/release-notes-1.0.6.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1407 2022-05-20 17:35:24.000000 cvprac-1.3.1/docs/release-notes-1.0.7.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     3350 2022-05-20 21:38:36.000000 cvprac-1.3.1/docs/release-notes-1.2.0.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1523 2022-10-10 14:46:28.000000 cvprac-1.3.1/docs/release-notes-1.2.2.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)     1716 2023-03-07 20:14:16.000000 cvprac-1.3.1/docs/release-notes-1.3.0.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)      206 2023-04-13 15:53:28.000000 cvprac-1.3.1/docs/release-notes-1.3.1.rst
+-rw-r--r--   0 mhartzel   (501) staff       (20)       24 2023-03-07 16:02:05.000000 cvprac-1.3.1/requirements.txt
+-rw-r--r--   0 mhartzel   (501) staff       (20)       38 2023-04-13 15:55:33.613919 cvprac-1.3.1/setup.cfg
+-rw-r--r--   0 mhartzel   (501) staff       (20)     4721 2023-03-07 16:02:05.000000 cvprac-1.3.1/setup.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:32.563440 cvprac-1.3.1/test/
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.551935 cvprac-1.3.1/test/fixtures/
+-rw-r--r--   0 mhartzel   (501) staff       (20)      399 2023-04-11 23:33:16.000000 cvprac-1.3.1/test/fixtures/cvp_nodes.yaml
+-rw-r--r--   0 mhartzel   (501) staff       (20)  3941571 2019-09-25 14:39:35.000000 cvprac-1.3.1/test/fixtures/image-file.swix
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.574991 cvprac-1.3.1/test/lib/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     2634 2023-03-07 16:02:05.000000 cvprac-1.3.1/test/lib/systestlib.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.601032 cvprac-1.3.1/test/system/
+-rw-r--r--   0 mhartzel   (501) staff       (20)     6699 2023-03-07 16:02:05.000000 cvprac-1.3.1/test/system/test_cvp_base.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)    34161 2023-03-07 15:44:06.000000 cvprac-1.3.1/test/system/test_cvp_change_control_api.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)    18114 2022-05-20 17:35:24.000000 cvprac-1.3.1/test/system/test_cvp_client.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)   119358 2023-04-13 15:49:42.000000 cvprac-1.3.1/test/system/test_cvp_client_api.py
+drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2023-04-13 15:55:33.609347 cvprac-1.3.1/test/unit/
+-rw-r--r--   0 mhartzel   (501) staff       (20)    10898 2023-04-13 15:49:42.000000 cvprac-1.3.1/test/unit/test_api.py
+-rw-r--r--   0 mhartzel   (501) staff       (20)    26712 2023-03-07 16:02:05.000000 cvprac-1.3.1/test/unit/test_client.py
```

### Comparing `cvprac-1.3.0/.pylintrc` & `cvprac-1.3.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/LICENSE` & `cvprac-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/Makefile` & `cvprac-1.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/PKG-INFO` & `cvprac-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cvprac
-Version: 1.3.0
+Version: 1.3.1
 Summary: Arista Cloudvision(R) Portal Rest API Client written in python
 Home-page: https://github.com/aristanetworks/cvprac
 Author: Arista Networks, Inc.
 Author-email: eosplus-dev@arista.com
 License: BSD-3
-Download-URL: https://github.com/aristanetworks/cvprac/tarball/1.3.0
+Download-URL: https://github.com/aristanetworks/cvprac/tarball/1.3.1
 Keywords: networking CloudVision development rest api
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `cvprac-1.3.0/README.md` & `cvprac-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/cvprac/__init__.py` & `cvprac-1.3.1/cvprac/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,9 +28,9 @@
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 ''' RESTful API Client class for Cloudvision(R) Portal
 '''
 
-__version__ = '1.3.0'
+__version__ = '1.3.1'
 __author__ = 'Arista Networks, Inc.'
```

### Comparing `cvprac-1.3.0/cvprac/cvp_api.py` & `cvprac-1.3.1/cvprac/cvp_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 import operator
 import os
 import time
 # This import is for proper file IO handling support for both Python 2 and 3
 # pylint: disable=redefined-builtin
 from io import open
 from datetime import datetime
+from re import split
 
 from cvprac.cvp_client_errors import CvpApiError
 
 try:
     from urllib import quote_plus as qplus
 except (AttributeError, ImportError):
     from urllib.parse import quote_plus as qplus
@@ -1173,14 +1174,15 @@
                        timeout=self.request_timeout)
 
         # Get the key for the configlet
         data = self.clnt.get('/configlet/getConfigletByName.do?name=%s'
                              % qplus(name), timeout=self.request_timeout)
         return data['key']
 
+
     def delete_configlet(self, name, key):
         ''' Delete the configlet.
 
             Args:
                 name (str): Configlet name
                 key (str): Configlet key
         '''
@@ -1304,30 +1306,80 @@
         data = {
             'key': key,
             'note': note,
         }
         return self.clnt.post('/configlet/addNoteToConfiglet.do',
                               data=data, timeout=self.request_timeout)
 
+    def sanitize_warnings(self, data):
+        ''' Sanitize the warnings returned after validation.
+            
+            In some cases where the configlets has both errors
+            and warnings, CVP may split any warnings that have 
+            `,` across multiple strings.
+            This method concats the strings back into one string
+            per warning, and correct the warningCount. 
+
+            Args:
+                data (dict): A dict that contians the result
+                    of the validation operation
+            Returns:
+                response (dict): A dict that contains the result of the
+                    validation operation
+        '''
+        if "warnings" not in data:
+            # nothing to do here, we can return as is
+            return data
+        # Since there may be warnings incorrectly split on
+        # ', ' within the warning text by CVP, we join all the 
+        # warnings together using ', ' into one large string
+        temp_warnings = ", ".join(data['warnings']).strip()
+
+        # To split the large string again we match on the 
+        # 'at line XXX' that should indicate the end of the warning.
+        # We capture as well the remaining \\n or whitespace and include
+        # the extra ', ' added in the previous step in the matching criteria.
+        # The extra ', ' is not included in the strings of the new list
+        temp_warnings = split(
+            r'(.*?at line \d+.*?),\s+',
+            temp_warnings
+        )
+
+        # The behaviour of re.split will add empty strings
+        # if the regex matches on the begging or ending of the line.
+        # Refer to https://docs.python.org/3/library/re.html#re.split
+
+        # Use filter to remove any empty strings
+        # that re.split inserted
+        data['warnings'] = list(filter(None, temp_warnings))
+        # Update the count of warnings to the correct value
+        data['warningCount'] = len(data['warnings'])
+        return data
+
     def validate_config_for_device(self, device_mac, config):
         ''' Validate a config against a device
 
             Args:
                 device_mac (str): Device MAC address
                 config (str): Switch config statements
 
             Returns:
                 response (dict): A dict that contains the result of the
                     validation operation
         '''
         self.log.debug('validate_config_for_device: device_mac: %s config: %s'
                        % (device_mac, config))
         body = {'netElementId': device_mac, 'config': config}
-        return self.clnt.post('/configlet/validateConfig.do', data=body,
-                              timeout=self.request_timeout)
+        return self.sanitize_warnings(
+            self.clnt.post(
+                '/configlet/validateConfig.do',
+                data=body,
+                timeout=self.request_timeout
+            )
+        )
 
     def validate_config(self, device_mac, config):
         ''' Validate a config against a device and parse response to
             produce log messages are return a flag for the config validity.
 
             Args:
                 device_mac (str): Device MAC address
```

### Comparing `cvprac-1.3.0/cvprac/cvp_client.py` & `cvprac-1.3.1/cvprac/cvp_client.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/cvprac/cvp_client_errors.py` & `cvprac-1.3.1/cvprac/cvp_client_errors.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/cvprac.egg-info/PKG-INFO` & `cvprac-1.3.1/cvprac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cvprac
-Version: 1.3.0
+Version: 1.3.1
 Summary: Arista Cloudvision(R) Portal Rest API Client written in python
 Home-page: https://github.com/aristanetworks/cvprac
 Author: Arista Networks, Inc.
 Author-email: eosplus-dev@arista.com
 License: BSD-3
-Download-URL: https://github.com/aristanetworks/cvprac/tarball/1.3.0
+Download-URL: https://github.com/aristanetworks/cvprac/tarball/1.3.1
 Keywords: networking CloudVision development rest api
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `cvprac-1.3.0/cvprac.egg-info/SOURCES.txt` & `cvprac-1.3.1/cvprac.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 docs/release-notes-1.0.4.rst
 docs/release-notes-1.0.5.rst
 docs/release-notes-1.0.6.rst
 docs/release-notes-1.0.7.rst
 docs/release-notes-1.2.0.rst
 docs/release-notes-1.2.2.rst
 docs/release-notes-1.3.0.rst
+docs/release-notes-1.3.1.rst
 docs/labs/README.md
 docs/labs/lab01-cvp-info/get_cvp_info.py
 docs/labs/lab02-inventory-operations/compliance_check.py
 docs/labs/lab02-inventory-operations/get_running_configs.py
 docs/labs/lab02-inventory-operations/get_running_configs_by_time.py
 docs/labs/lab02-inventory-operations/remove_all_devices_legacy.py
 docs/labs/lab02-inventory-operations/remove_and_decommission_device.py
@@ -97,8 +98,9 @@
 test/fixtures/cvp_nodes.yaml
 test/fixtures/image-file.swix
 test/lib/systestlib.py
 test/system/test_cvp_base.py
 test/system/test_cvp_change_control_api.py
 test/system/test_cvp_client.py
 test/system/test_cvp_client_api.py
+test/unit/test_api.py
 test/unit/test_client.py
```

### Comparing `cvprac-1.3.0/cvprac.spec` & `cvprac-1.3.1/cvprac.spec`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/README.md` & `cvprac-1.3.1/docs/labs/README.md`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab01-cvp-info/get_cvp_info.py` & `cvprac-1.3.1/docs/labs/lab01-cvp-info/get_cvp_info.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab02-inventory-operations/compliance_check.py` & `cvprac-1.3.1/docs/labs/lab02-inventory-operations/compliance_check.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab02-inventory-operations/get_running_configs.py` & `cvprac-1.3.1/docs/labs/lab02-inventory-operations/get_running_configs.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab02-inventory-operations/get_running_configs_by_time.py` & `cvprac-1.3.1/docs/labs/lab02-inventory-operations/get_running_configs_by_time.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab02-inventory-operations/remove_all_devices_legacy.py` & `cvprac-1.3.1/docs/labs/lab02-inventory-operations/remove_all_devices_legacy.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab02-inventory-operations/remove_and_decommission_device.py` & `cvprac-1.3.1/docs/labs/lab02-inventory-operations/remove_and_decommission_device.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab02-inventory-operations/remove_devices_from_container_legacy.py` & `cvprac-1.3.1/docs/labs/lab02-inventory-operations/remove_devices_from_container_legacy.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab02-inventory-operations/remove_devices_legacy.py` & `cvprac-1.3.1/docs/labs/lab02-inventory-operations/remove_devices_legacy.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab03-configlet-management/assign_configlet_to_device.py` & `cvprac-1.3.1/docs/labs/lab03-configlet-management/assign_configlet_to_device.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab03-configlet-management/backup_configlets.py` & `cvprac-1.3.1/docs/labs/lab03-configlet-management/backup_configlets.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab03-configlet-management/backup_configletsV2.py` & `cvprac-1.3.1/docs/labs/lab03-configlet-management/backup_configletsV2.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab03-configlet-management/config_search.py` & `cvprac-1.3.1/docs/labs/lab03-configlet-management/config_search.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab03-configlet-management/create_configlet.py` & `cvprac-1.3.1/docs/labs/lab03-configlet-management/create_configlet.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab03-configlet-management/create_configlet_from_file.py` & `cvprac-1.3.1/docs/labs/lab03-configlet-management/create_configlet_from_file.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab03-configlet-management/get_applied_netelements.py` & `cvprac-1.3.1/docs/labs/lab03-configlet-management/get_applied_netelements.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab03-configlet-management/get_configlets.py` & `cvprac-1.3.1/docs/labs/lab03-configlet-management/get_configlets.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab03-configlet-management/reorder_configlet_on_device.py` & `cvprac-1.3.1/docs/labs/lab03-configlet-management/reorder_configlet_on_device.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab03-configlet-management/update_configlet.py` & `cvprac-1.3.1/docs/labs/lab03-configlet-management/update_configlet.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab04-container-management/add_image_to_container.py` & `cvprac-1.3.1/docs/labs/lab04-container-management/add_image_to_container.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab04-container-management/assign_configlet_to_container.py` & `cvprac-1.3.1/docs/labs/lab04-container-management/assign_configlet_to_container.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab04-container-management/create_container.py` & `cvprac-1.3.1/docs/labs/lab04-container-management/create_container.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab04-container-management/remove_image_from_container.py` & `cvprac-1.3.1/docs/labs/lab04-container-management/remove_image_from_container.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab04-container-management/rename_container.py` & `cvprac-1.3.1/docs/labs/lab04-container-management/rename_container.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab05-device-management/add_image_to_devices.py` & `cvprac-1.3.1/docs/labs/lab05-device-management/add_image_to_devices.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab05-device-management/add_image_wo_tempaction.py` & `cvprac-1.3.1/docs/labs/lab05-device-management/add_image_wo_tempaction.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab05-device-management/remove_image_from_device.py` & `cvprac-1.3.1/docs/labs/lab05-device-management/remove_image_from_device.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab05-device-management/set_mgmt_ip.py` & `cvprac-1.3.1/docs/labs/lab05-device-management/set_mgmt_ip.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab06-provisioning/atd_e2e_provisioning_workflow.py` & `cvprac-1.3.1/docs/labs/lab06-provisioning/atd_e2e_provisioning_workflow.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab06-provisioning/auto_reconcile_on_rc_change.py` & `cvprac-1.3.1/docs/labs/lab06-provisioning/auto_reconcile_on_rc_change.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab06-provisioning/change_control_custom_rapi.py` & `cvprac-1.3.1/docs/labs/lab06-provisioning/change_control_custom_rapi.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab06-provisioning/change_control_workflow.py` & `cvprac-1.3.1/docs/labs/lab06-provisioning/change_control_workflow.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab06-provisioning/change_control_workflow_rapi.py` & `cvprac-1.3.1/docs/labs/lab06-provisioning/change_control_workflow_rapi.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab06-provisioning/configlets/AVD_leaf1.cfg` & `cvprac-1.3.1/docs/labs/lab06-provisioning/configlets/AVD_leaf1.cfg`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab06-provisioning/configlets/AVD_leaf2.cfg` & `cvprac-1.3.1/docs/labs/lab06-provisioning/configlets/AVD_leaf2.cfg`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab06-provisioning/configlets/AVD_leaf3.cfg` & `cvprac-1.3.1/docs/labs/lab06-provisioning/configlets/AVD_leaf3.cfg`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab06-provisioning/configlets/AVD_leaf4.cfg` & `cvprac-1.3.1/docs/labs/lab06-provisioning/configlets/AVD_leaf4.cfg`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab06-provisioning/configlets/AVD_spine1.cfg` & `cvprac-1.3.1/docs/labs/lab06-provisioning/configlets/AVD_spine1.cfg`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab06-provisioning/configlets/AVD_spine2.cfg` & `cvprac-1.3.1/docs/labs/lab06-provisioning/configlets/AVD_spine2.cfg`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab06-provisioning/gen_builder.py` & `cvprac-1.3.1/docs/labs/lab06-provisioning/gen_builder.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab06-provisioning/mlag_issu.py` & `cvprac-1.3.1/docs/labs/lab06-provisioning/mlag_issu.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab06-provisioning/move_device.py` & `cvprac-1.3.1/docs/labs/lab06-provisioning/move_device.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab06-provisioning/vc_task_retrigger.py` & `cvprac-1.3.1/docs/labs/lab06-provisioning/vc_task_retrigger.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab07-aaa/add_new_user_cvaas.py` & `cvprac-1.3.1/docs/labs/lab07-aaa/add_new_user_cvaas.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab07-aaa/add_new_user_onprem.py` & `cvprac-1.3.1/docs/labs/lab07-aaa/add_new_user_onprem.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab07-aaa/add_users_from_csv_cvaas.py` & `cvprac-1.3.1/docs/labs/lab07-aaa/add_users_from_csv_cvaas.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab07-aaa/create_svc_account.py` & `cvprac-1.3.1/docs/labs/lab07-aaa/create_svc_account.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab07-aaa/create_svc_account_token.py` & `cvprac-1.3.1/docs/labs/lab07-aaa/create_svc_account_token.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab07-aaa/create_terminattr_tokens.py` & `cvprac-1.3.1/docs/labs/lab07-aaa/create_terminattr_tokens.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab07-aaa/delete_all_expired_svc_account_tokens.py` & `cvprac-1.3.1/docs/labs/lab07-aaa/delete_all_expired_svc_account_tokens.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab07-aaa/delete_svc_account.py` & `cvprac-1.3.1/docs/labs/lab07-aaa/delete_svc_account.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab07-aaa/delete_svc_account_created_by_user.py` & `cvprac-1.3.1/docs/labs/lab07-aaa/delete_svc_account_created_by_user.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab07-aaa/get_user_info.py` & `cvprac-1.3.1/docs/labs/lab07-aaa/get_user_info.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab07-aaa/svc_account_misc.py` & `cvprac-1.3.1/docs/labs/lab07-aaa/svc_account_misc.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab08-resource-apis/resource_cvprac.py` & `cvprac-1.3.1/docs/labs/lab08-resource-apis/resource_cvprac.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/lab08-resource-apis/topology_tag_assignment.py` & `cvprac-1.3.1/docs/labs/lab08-resource-apis/topology_tag_assignment.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/static/serviceaccount1.png` & `cvprac-1.3.1/docs/labs/static/serviceaccount1.png`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/static/serviceaccount2.png` & `cvprac-1.3.1/docs/labs/static/serviceaccount2.png`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/labs/static/serviceaccount3.png` & `cvprac-1.3.1/docs/labs/static/serviceaccount3.png`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/release-notes-0.7.0.rst` & `cvprac-1.3.1/docs/release-notes-0.7.0.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/release-notes-0.8.0.rst` & `cvprac-1.3.1/docs/release-notes-0.8.0.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/release-notes-0.9.0.rst` & `cvprac-1.3.1/docs/release-notes-0.9.0.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/release-notes-1.0.0.rst` & `cvprac-1.3.1/docs/release-notes-1.0.0.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/release-notes-1.0.1.rst` & `cvprac-1.3.1/docs/release-notes-1.0.1.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/release-notes-1.0.2.rst` & `cvprac-1.3.1/docs/release-notes-1.0.2.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/release-notes-1.0.4.rst` & `cvprac-1.3.1/docs/release-notes-1.0.4.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/release-notes-1.0.5.rst` & `cvprac-1.3.1/docs/release-notes-1.0.5.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/release-notes-1.0.6.rst` & `cvprac-1.3.1/docs/release-notes-1.0.6.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/release-notes-1.0.7.rst` & `cvprac-1.3.1/docs/release-notes-1.0.7.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/release-notes-1.2.0.rst` & `cvprac-1.3.1/docs/release-notes-1.2.0.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/release-notes-1.2.2.rst` & `cvprac-1.3.1/docs/release-notes-1.2.2.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/docs/release-notes-1.3.0.rst` & `cvprac-1.3.1/docs/release-notes-1.3.0.rst`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/setup.py` & `cvprac-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/test/fixtures/image-file.swix` & `cvprac-1.3.1/test/fixtures/image-file.swix`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/test/lib/systestlib.py` & `cvprac-1.3.1/test/lib/systestlib.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/test/system/test_cvp_base.py` & `cvprac-1.3.1/test/system/test_cvp_base.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/test/system/test_cvp_change_control_api.py` & `cvprac-1.3.1/test/system/test_cvp_change_control_api.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/test/system/test_cvp_client.py` & `cvprac-1.3.1/test/system/test_cvp_client.py`

 * *Files identical despite different names*

### Comparing `cvprac-1.3.0/test/system/test_cvp_client_api.py` & `cvprac-1.3.1/test/system/test_cvp_client_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 '''
 import os
 import shutil
 import sys
 import time
 import unittest
 import uuid
+from pkg_resources import parse_version
 from pprint import pprint
 import urllib3
 from test_cvp_base import TestCvpClientBase
 from requests.exceptions import Timeout
 from cvprac.cvp_client_errors import CvpApiError, CvpRequestError
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
@@ -686,21 +687,56 @@
     def test_api_validate_config(self):
         ''' Verify valid config returns True
         '''
         config = 'interface ethernet1\n description test'
         result = self.api.validate_config(self.device['key'], config)
         self.assertEqual(result, True)
 
+    def test_api_validate_config_warn(self):
+        ''' Verify config with only warnings returns True
+        '''
+        config = 'interface ethernet1\n description test\nspanning-tree portfast'
+        result = self.api.validate_config(self.device['key'], config)
+        self.assertEqual(result, True)
+
     def test_api_validate_config_error(self):
         ''' Verify an invalid config returns False
         '''
         config = 'interface ethernet1\n typocommand test'
         result = self.api.validate_config(self.device['key'], config)
         self.assertEqual(result, False)
 
+    def test_api_validate_config_device(self):
+        ''' Verify config with only warnings returns True
+        '''
+        # The current APIVersions do not allow the cut off at CVP 2021.1.X
+        # that this error message changes. So this is version comparision and
+        # parsing is repetitive.
+        if not self.clnt.apiversion:
+            self.api.get_cvp_info()
+        version_components = self.clnt.version.split(".")
+        if len(version_components) < 3:
+            version_components.append("0")
+            self.log.info('Version found with less than 3 components.'
+                          ' Appending 0. Updated Version String - %s',
+                          ".".join(version_components))
+        full_version = ".".join(version_components)
+
+        config = 'interface ethernet1\n description test\nspanning-tree portfast\n!\nruter bgp something'
+        result = self.api.validate_config_for_device(self.device['key'], config)
+        expected_warning = "! portfast should only be enabled on ports connected to a single host. Connecting hubs, concentrators, switches, bridges, etc. to this interface when portfast is enabled can cause temporary bridging loops. Use with CAUTION. at line 3"
+        self.assertTrue(expected_warning in result["warnings"][0])
+        expected_error = "> ruter bgp something% Invalid input "
+        # Error message format changes as of 2021.1.0 or 2021.1.1
+        if parse_version(full_version) >= parse_version("2021.1.0"):
+            expected_error += "(at token 0: 'ruter') "
+        expected_error += "at line 5"
+        self.assertEqual(result['errors'][0]["error"], expected_error)
+        self.assertEqual(result['warningCount'], 1)
+
     def test_api_get_task_by_id_bad(self):
         ''' Verify get_task_by_id with bad task id
         '''
         result = self.api.get_task_by_id(10000000)
         self.assertIsNone(result)
 
     def test_api_get_task_by_id_fmt_bad(self):
@@ -785,17 +821,23 @@
                     if 'Entity does not exist' in e.msg:
                         # Configlet Builder for 2021.x - 2022.1.1
                         try:
                             cfglt = self.api.get_configlet_by_name(
                                 'SYS_TelemetryBuilderV4')
                         except CvpApiError as e:
                             if 'Entity does not exist' in e.msg:
-                                # Configlet Builder for 2022.2.0 +
-                                cfglt = self.api.get_configlet_by_name(
-                                    'SYS_TelemetryBuilderV5')
+                                # Configlet Builder for 2022.2.0 - 2022.3.X
+                                try:
+                                    cfglt = self.api.get_configlet_by_name(
+                                        'SYS_TelemetryBuilderV5')
+                                except CvpApiError as e:
+                                    if 'Entity does not exist' in e.msg:
+                                        # Configlet Builder for 2022.3.X+
+                                        cfglt = self.api.get_configlet_by_name(
+                                            'SYS_TelemetryBuilderV6')
                     else:
                         raise
             else:
                 raise
         result = self.api.get_configlet_builder(cfglt['key'])
 
         # Verify the following keys and types are
```

### Comparing `cvprac-1.3.0/test/unit/test_client.py` & `cvprac-1.3.1/test/unit/test_client.py`

 * *Files identical despite different names*

