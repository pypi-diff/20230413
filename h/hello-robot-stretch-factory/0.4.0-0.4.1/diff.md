# Comparing `tmp/hello_robot_stretch_factory-0.4.0.tar.gz` & `tmp/hello_robot_stretch_factory-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_robot_stretch_factory-0.4.0.tar", last modified: Tue Apr 11 22:29:49 2023, max compression
+gzip compressed data, was "hello_robot_stretch_factory-0.4.1.tar", last modified: Wed Apr 12 23:17:11 2023, max compression
```

## Comparing `hello_robot_stretch_factory-0.4.0.tar` & `hello_robot_stretch_factory-0.4.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-11 22:29:49.283499 hello_robot_stretch_factory-0.4.0/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      929 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/LICENSE.md
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      816 2023-04-11 22:29:49.283499 hello_robot_stretch_factory-0.4.0/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      355 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/README.md
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-11 22:29:49.279500 hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      816 2023-04-11 22:29:49.000000 hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1796 2023-04-11 22:29:49.000000 hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/SOURCES.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2023-04-11 22:29:49.000000 hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/dependency_links.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       74 2023-04-11 22:29:49.000000 hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/requires.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       16 2023-04-11 22:29:49.000000 hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/top_level.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2023-04-11 22:29:49.283499 hello_robot_stretch_factory-0.4.0/setup.cfg
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      995 2023-04-11 22:29:27.000000 hello_robot_stretch_factory-0.4.0/setup.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-11 22:29:49.283499 hello_robot_stretch_factory-0.4.0/stretch_factory/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6326 2022-09-26 22:58:30.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/device_mgmt.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4425 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_available.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5248 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_installed.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3861 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_recommended.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    37370 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_updater.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5254 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2726 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_version.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    20922 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/hello_device_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12828 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/param_mgmt.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-11 22:29:49.283499 hello_robot_stretch_factory-0.4.0/test/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      685 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/test/test_firmware_updater.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      668 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/test/test_usb_reset.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-11 22:29:49.279500 hello_robot_stretch_factory-0.4.0/tools/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2456 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/RE1_migrate_contacts.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6621 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/RE1_migrate_params.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    22012 2023-03-09 23:32:07.000000 hello_robot_stretch_factory-0.4.0/tools/REx_D435i_check.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5418 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_base_calibrate_imu_collect.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    32027 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_base_calibrate_imu_process.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5950 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_base_calibrate_wheel_separation.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4771 2023-03-09 23:32:07.000000 hello_robot_stretch_factory-0.4.0/tools/REx_calibrate_gravity_comp.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7203 2023-03-09 23:32:07.000000 hello_robot_stretch_factory-0.4.0/tools/REx_calibrate_guarded_contact.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3578 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_calibrate_range.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1728 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_cliff_sensor_calibrate.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18552 2023-03-09 23:32:07.000000 hello_robot_stretch_factory-0.4.0/tools/REx_discover_hello_devices.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1442 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_id_change.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1354 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_id_scan.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5045 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1374 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_reboot.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1188 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_set_baud.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4410 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/tools/REx_firmware_flash.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5804 2023-04-11 22:29:18.000000 hello_robot_stretch_factory-0.4.0/tools/REx_firmware_updater.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1583 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_gamepad_configure.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2338 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_gripper_calibrate.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1947 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_hello_dynamixel_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      870 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_stepper_calibration_YAML_to_flash.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      685 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_stepper_calibration_flash_to_YAML.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1168 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_stepper_calibration_run.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18644 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_stepper_ctrl_tuning.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1163 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_stepper_gains.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4064 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_stepper_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      852 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_stepper_mechaduino_menu.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    10577 2023-04-11 22:29:02.000000 hello_robot_stretch_factory-0.4.0/tools/REx_trace_firmware.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7819 2023-04-11 22:29:02.000000 hello_robot_stretch_factory-0.4.0/tools/REx_trace_robot.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2347 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_usb_reset.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1379 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_wacc_calibrate.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-12 23:17:11.756573 hello_robot_stretch_factory-0.4.1/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      929 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/LICENSE.md
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      816 2023-04-12 23:17:11.756573 hello_robot_stretch_factory-0.4.1/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      355 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/README.md
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-12 23:17:11.752573 hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      816 2023-04-12 23:17:11.000000 hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1796 2023-04-12 23:17:11.000000 hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2023-04-12 23:17:11.000000 hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       74 2023-04-12 23:17:11.000000 hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/requires.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       16 2023-04-12 23:17:11.000000 hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/top_level.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2023-04-12 23:17:11.756573 hello_robot_stretch_factory-0.4.1/setup.cfg
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      995 2023-04-12 23:14:54.000000 hello_robot_stretch_factory-0.4.1/setup.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-12 23:17:11.756573 hello_robot_stretch_factory-0.4.1/stretch_factory/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/__init__.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6326 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/device_mgmt.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4425 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_available.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5248 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_installed.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3861 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_recommended.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    37370 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_updater.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5254 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2726 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_version.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    20922 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/hello_device_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12828 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/param_mgmt.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-12 23:17:11.756573 hello_robot_stretch_factory-0.4.1/test/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      685 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/test/test_firmware_updater.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      668 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/test/test_usb_reset.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-12 23:17:11.752573 hello_robot_stretch_factory-0.4.1/tools/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2456 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/RE1_migrate_contacts.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6621 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/RE1_migrate_params.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    22012 2023-02-03 03:51:49.000000 hello_robot_stretch_factory-0.4.1/tools/REx_D435i_check.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5418 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_base_calibrate_imu_collect.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    32027 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_base_calibrate_imu_process.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5950 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_base_calibrate_wheel_separation.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4771 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_calibrate_gravity_comp.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7456 2023-04-12 23:11:21.000000 hello_robot_stretch_factory-0.4.1/tools/REx_calibrate_guarded_contact.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3578 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_calibrate_range.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1728 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_cliff_sensor_calibrate.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18552 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_discover_hello_devices.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1442 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_id_change.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1354 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_id_scan.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5045 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1374 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_reboot.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1188 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_set_baud.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4410 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/tools/REx_firmware_flash.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5804 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/tools/REx_firmware_updater.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1583 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_gamepad_configure.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2338 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_gripper_calibrate.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1947 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_hello_dynamixel_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      870 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_stepper_calibration_YAML_to_flash.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      685 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_stepper_calibration_flash_to_YAML.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1168 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_stepper_calibration_run.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18644 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_stepper_ctrl_tuning.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1163 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_stepper_gains.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4064 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_stepper_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      852 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_stepper_mechaduino_menu.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    10577 2023-04-03 20:35:08.000000 hello_robot_stretch_factory-0.4.1/tools/REx_trace_firmware.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7819 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/tools/REx_trace_robot.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2347 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_usb_reset.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1379 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_wacc_calibrate.py
```

### Comparing `hello_robot_stretch_factory-0.4.0/LICENSE.md` & `hello_robot_stretch_factory-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/PKG-INFO` & `hello_robot_stretch_factory-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello_robot_stretch_factory
-Version: 0.4.0
+Version: 0.4.1
 Summary: Stretch Factory Tools
 Home-page: https://github.com/hello-robot/stretch_factory
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/PKG-INFO` & `hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello-robot-stretch-factory
-Version: 0.4.0
+Version: 0.4.1
 Summary: Stretch Factory Tools
 Home-page: https://github.com/hello-robot/stretch_factory
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/SOURCES.txt` & `hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/setup.py` & `hello_robot_stretch_factory-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 script_path='./tools'
 ex_scripts = glob.glob(script_path+'/*.py') + glob.glob(script_path+'/*.sh')
 stretch_scripts=[f for f in ex_scripts if isfile(f)]
 
 setuptools.setup(
     name="hello_robot_stretch_factory",
-    version="0.4.0",
+    version="0.4.1",
     author="Hello Robot Inc.",
     author_email="support@hello-robot.com",
     description="Stretch Factory Tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hello-robot/stretch_factory",
     scripts = stretch_scripts,
```

### Comparing `hello_robot_stretch_factory-0.4.0/stretch_factory/device_mgmt.py` & `hello_robot_stretch_factory-0.4.1/stretch_factory/device_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_available.py` & `hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_available.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_installed.py` & `hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_installed.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_recommended.py` & `hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_recommended.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_updater.py` & `hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_utils.py` & `hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_version.py` & `hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_version.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/stretch_factory/hello_device_utils.py` & `hello_robot_stretch_factory-0.4.1/stretch_factory/hello_device_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/stretch_factory/param_mgmt.py` & `hello_robot_stretch_factory-0.4.1/stretch_factory/param_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/test/test_firmware_updater.py` & `hello_robot_stretch_factory-0.4.1/test/test_firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/test/test_usb_reset.py` & `hello_robot_stretch_factory-0.4.1/test/test_usb_reset.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/RE1_migrate_contacts.py` & `hello_robot_stretch_factory-0.4.1/tools/RE1_migrate_contacts.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/RE1_migrate_params.py` & `hello_robot_stretch_factory-0.4.1/tools/RE1_migrate_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_D435i_check.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_D435i_check.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_base_calibrate_imu_collect.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_base_calibrate_imu_collect.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_base_calibrate_imu_process.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_base_calibrate_imu_process.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_base_calibrate_wheel_separation.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_base_calibrate_wheel_separation.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_calibrate_gravity_comp.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_calibrate_gravity_comp.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_calibrate_guarded_contact.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_calibrate_guarded_contact.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 #!/usr/bin/env python
+import os
+
 from stretch_body.hello_utils import *
 import stretch_body.scope
 import argparse
 import click
 
 print_stretch_re_use()
 
@@ -28,14 +30,19 @@
     exit(1)
 
 j.pull_status()
 if not j.motor.status['pos_calibrated']:
     print('Joint not calibrated. Exiting.')
     exit(1)
 
+if args.lift:
+    click.secho("The Arm and Wrist yaw will need to be first homed. Ensure workspace is collision free.",fg="yellow")
+    click.confirm("Proceed?")
+    os.system('stretch_arm_home.py')
+    os.system('stretch_wrist_yaw_home.py')
 
 if (j.name in j.user_params and 'contact_models' in j.user_params[j.name]) and ('effort_pct' in j.user_params[j.name]['contact_models']) \
         and ('contact_thresh_default' in j.user_params[j.name]['contact_models']['effort_pct']):
     click.secho('------------------------',fg="yellow")
     click.secho('NOTE: This tool updates contact_thresh_default for %s in stretch_configuration_params.yaml'%j.name.upper(),fg="yellow")
     click.secho('NOTE: Your stretch_user_params.yaml overrides contact_thresh_default for %s'%j.name.upper(),fg="yellow")
     click.secho('NOTE: As such, the updated calibration will not change the contact behavior unless you remove the user params.',fg="yellow")
```

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_calibrate_range.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_calibrate_range.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_cliff_sensor_calibrate.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_cliff_sensor_calibrate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_discover_hello_devices.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_discover_hello_devices.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_id_change.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_id_change.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_id_scan.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_id_scan.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_jog.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_reboot.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_reboot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_set_baud.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_set_baud.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_firmware_flash.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_firmware_flash.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_firmware_updater.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_gamepad_configure.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_gamepad_configure.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_gripper_calibrate.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_gripper_calibrate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_hello_dynamixel_jog.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_hello_dynamixel_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_stepper_calibration_YAML_to_flash.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_stepper_calibration_YAML_to_flash.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_stepper_calibration_flash_to_YAML.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_stepper_calibration_flash_to_YAML.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_stepper_calibration_run.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_stepper_calibration_run.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_stepper_ctrl_tuning.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_stepper_ctrl_tuning.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_stepper_gains.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_stepper_gains.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_stepper_jog.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_stepper_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_stepper_mechaduino_menu.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_stepper_mechaduino_menu.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_trace_firmware.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_trace_firmware.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_trace_robot.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_trace_robot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_usb_reset.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_usb_reset.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.0/tools/REx_wacc_calibrate.py` & `hello_robot_stretch_factory-0.4.1/tools/REx_wacc_calibrate.py`

 * *Files identical despite different names*

