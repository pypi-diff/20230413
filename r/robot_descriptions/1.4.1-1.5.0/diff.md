# Comparing `tmp/robot_descriptions-1.4.1.tar.gz` & `tmp/robot_descriptions-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robot_descriptions-1.4.1.tar", last modified: Tue Feb 28 10:46:01 2023, max compression
+gzip compressed data, was "robot_descriptions-1.5.0.tar", last modified: Thu Apr 13 09:26:43 2023, max compression
```

## Comparing `robot_descriptions-1.4.1.tar` & `robot_descriptions-1.5.0.tar`

### file list

```diff
@@ -1,113 +1,115 @@
--rw-r--r--   0        0        0     2290 2023-01-06 14:01:23.817479 robot_descriptions-1.4.1/.github/workflows/test.yml
--rw-r--r--   0        0        0       42 2023-01-06 14:01:23.817479 robot_descriptions-1.4.1/.gitignore
--rw-r--r--   0        0        0     4852 2023-02-28 10:27:17.404203 robot_descriptions-1.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     2045 2023-02-28 10:25:49.242791 robot_descriptions-1.4.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-01-06 14:01:23.817479 robot_descriptions-1.4.1/LICENSE
--rw-r--r--   0        0        0    14778 2023-02-28 10:24:46.999089 robot_descriptions-1.4.1/README.md
--rw-r--r--   0        0        0     2695 2023-01-19 17:56:07.944372 robot_descriptions-1.4.1/examples/display_urdf_frames.py
--rw-r--r--   0        0        0     1295 2023-01-06 14:01:23.817479 robot_descriptions-1.4.1/examples/load_in_idyntree.py
--rw-r--r--   0        0        0     1280 2023-01-06 14:01:23.817479 robot_descriptions-1.4.1/examples/load_in_mujoco.py
--rw-r--r--   0        0        0     1276 2023-01-06 14:01:23.817479 robot_descriptions-1.4.1/examples/load_in_pinocchio.py
--rw-r--r--   0        0        0     1370 2023-01-06 14:01:23.817479 robot_descriptions-1.4.1/examples/load_in_pybullet.py
--rw-r--r--   0        0        0     1280 2023-01-06 14:01:23.817479 robot_descriptions-1.4.1/examples/load_in_robomeshcat.py
--rw-r--r--   0        0        0     1280 2023-01-06 14:01:23.817479 robot_descriptions-1.4.1/examples/load_in_yourdfpy.py
--rw-r--r--   0        0        0     1642 2023-01-06 14:01:23.817479 robot_descriptions-1.4.1/examples/show_in_meshcat.py
--rw-r--r--   0        0        0     1716 2023-01-06 14:01:23.817479 robot_descriptions-1.4.1/examples/show_in_mujoco.py
--rw-r--r--   0        0        0     1505 2023-01-06 14:01:23.817479 robot_descriptions-1.4.1/examples/show_in_pybullet.py
--rw-r--r--   0        0        0     1665 2023-01-06 14:01:23.817479 robot_descriptions-1.4.1/examples/show_in_robomeshcat.py
--rw-r--r--   0        0        0     1579 2023-01-06 14:01:23.817479 robot_descriptions-1.4.1/examples/show_in_yourdfpy.py
--rw-r--r--   0        0        0     1863 2023-02-13 11:16:52.063235 robot_descriptions-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      714 2023-02-28 10:19:12.184018 robot_descriptions-1.4.1/robot_descriptions/__init__.py
--rw-r--r--   0        0        0     4385 2023-02-13 11:16:52.063235 robot_descriptions-1.4.1/robot_descriptions/_cache.py
--rw-r--r--   0        0        0     5604 2023-02-13 11:16:52.063235 robot_descriptions-1.4.1/robot_descriptions/_command_line.py
--rw-r--r--   0        0        0     4987 2023-02-28 10:23:22.295004 robot_descriptions-1.4.1/robot_descriptions/_descriptions.py
--rw-r--r--   0        0        0      674 2023-02-13 11:16:52.063235 robot_descriptions-1.4.1/robot_descriptions/_empty_description.py
--rw-r--r--   0        0        0     1114 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/_package_dirs.py
--rw-r--r--   0        0        0     9179 2023-02-28 10:25:28.919782 robot_descriptions-1.4.1/robot_descriptions/_repositories.py
--rw-r--r--   0        0        0     1024 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/a1_description.py
--rw-r--r--   0        0        0     1078 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/a1_mj_description.py
--rw-r--r--   0        0        0     1093 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/aliengo_description.py
--rw-r--r--   0        0        0     1325 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/allegro_hand_description.py
--rw-r--r--   0        0        0     1022 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/anymal_b_description.py
--rw-r--r--   0        0        0     1031 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/anymal_b_mj_description.py
--rw-r--r--   0        0        0     1022 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/anymal_c_description.py
--rw-r--r--   0        0        0     1031 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/anymal_c_mj_description.py
--rw-r--r--   0        0        0     1171 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/atlas_drc_description.py
--rw-r--r--   0        0        0     1381 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/atlas_v4_description.py
--rw-r--r--   0        0        0     1025 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/b1_description.py
--rw-r--r--   0        0        0     1016 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/barrett_hand_description.py
--rw-r--r--   0        0        0     1028 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/baxter_description.py
--rw-r--r--   0        0        0     1039 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/bolt_description.py
--rw-r--r--   0        0        0     1012 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/cassie_description.py
--rw-r--r--   0        0        0     1023 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/cassie_mj_description.py
--rw-r--r--   0        0        0     1048 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/cf2_description.py
--rw-r--r--   0        0        0     1304 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/double_pendulum_description.py
--rw-r--r--   0        0        0     1011 2023-02-22 15:58:12.265767 robot_descriptions-1.4.1/robot_descriptions/draco3_description.py
--rw-r--r--   0        0        0      997 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/edo_description.py
--rw-r--r--   0        0        0     1042 2023-02-28 10:22:37.917012 robot_descriptions-1.4.1/robot_descriptions/ergocub_description.py
--rw-r--r--   0        0        0     1034 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/eve_r3_description.py
--rw-r--r--   0        0        0     1060 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/fetch_description.py
--rw-r--r--   0        0        0     1065 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/finger_edu_description.py
--rw-r--r--   0        0        0     1043 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/gen2_description.py
--rw-r--r--   0        0        0     1020 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/gen3_mj_description.py
--rw-r--r--   0        0        0     1007 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/ginger_description.py
--rw-r--r--   0        0        0     1027 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/go1_description.py
--rw-r--r--   0        0        0     1082 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/go1_mj_description.py
--rw-r--r--   0        0        0     1047 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/hyq_description.py
--rw-r--r--   0        0        0     1035 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/icub_description.py
--rw-r--r--   0        0        0     1427 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/iiwa_description.py
--rw-r--r--   0        0        0     1013 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/jaxon_description.py
--rw-r--r--   0        0        0     1008 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/jvrc_description.py
--rw-r--r--   0        0        0     1014 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/jvrc_mj_description.py
--rw-r--r--   0        0        0     1093 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/laikago_description.py
--rw-r--r--   0        0        0      683 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/loaders/__init__.py
--rw-r--r--   0        0        0     2587 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/loaders/idyntree.py
--rw-r--r--   0        0        0     1514 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/loaders/mujoco.py
--rw-r--r--   0        0        0     2173 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/loaders/pinocchio.py
--rw-r--r--   0        0        0     1586 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/loaders/pybullet.py
--rw-r--r--   0        0        0     1612 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/loaders/robomeshcat.py
--rw-r--r--   0        0        0     1732 2023-02-22 15:58:12.265767 robot_descriptions-1.4.1/robot_descriptions/loaders/yourdfpy.py
--rw-r--r--   0        0        0     1022 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/mini_cheetah_description.py
--rw-r--r--   0        0        0     1017 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/minitaur_description.py
--rw-r--r--   0        0        0     1036 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/nextage_description.py
--rw-r--r--   0        0        0     1040 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/panda_description.py
--rw-r--r--   0        0        0     1025 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/panda_mj_description.py
--rw-r--r--   0        0        0     1011 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/pepper_description.py
--rw-r--r--   0        0        0     1032 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/poppy_ergo_jr_description.py
--rw-r--r--   0        0        0     1026 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/poppy_torso_description.py
--rw-r--r--   0        0        0     1017 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/pr2_description.py
--rw-r--r--   0        0        0     2748 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/r2_description.py
--rw-r--r--   0        0        0     1003 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/reachy_description.py
--rw-r--r--   0        0        0     1052 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/robotiq_2f85_description.py
--rw-r--r--   0        0        0     1026 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/robotiq_2f85_mj_description.py
--rw-r--r--   0        0        0     1053 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/romeo_description.py
--rw-r--r--   0        0        0     1190 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/shadow_hand_mj_description.py
--rw-r--r--   0        0        0      999 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/sigmaban_description.py
--rw-r--r--   0        0        0     1139 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/simple_humanoid_description.py
--rw-r--r--   0        0        0     1041 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/solo_description.py
--rw-r--r--   0        0        0     1035 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/spryped_description.py
--rw-r--r--   0        0        0     1286 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/talos_description.py
--rw-r--r--   0        0        0     1238 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/tiago_description.py
--rw-r--r--   0        0        0     1008 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/upkie_description.py
--rw-r--r--   0        0        0     1175 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/ur10_description.py
--rw-r--r--   0        0        0     1251 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/ur3_description.py
--rw-r--r--   0        0        0     1251 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/ur5_description.py
--rw-r--r--   0        0        0     1026 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/ur5e_mj_description.py
--rw-r--r--   0        0        0     1350 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/valkyrie_description.py
--rw-r--r--   0        0        0     1020 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/yumi_description.py
--rw-r--r--   0        0        0     1025 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/robot_descriptions/z1_description.py
--rw-r--r--   0        0        0     1002 2023-02-08 17:58:19.351928 robot_descriptions-1.4.1/tests/__init__.py
--rw-r--r--   0        0        0       59 2023-01-06 14:01:23.821479 robot_descriptions-1.4.1/tests/loaders/__init__.py
--rwxr-xr-x   0        0        0     1531 2023-01-06 14:01:23.821479 robot_descriptions-1.4.1/tests/loaders/test_idyntree.py
--rw-r--r--   0        0        0     1479 2023-01-06 14:01:23.821479 robot_descriptions-1.4.1/tests/loaders/test_mujoco.py
--rw-r--r--   0        0        0     1536 2023-01-06 14:01:23.821479 robot_descriptions-1.4.1/tests/loaders/test_pinocchio.py
--rw-r--r--   0        0        0     1976 2023-01-06 14:01:23.821479 robot_descriptions-1.4.1/tests/loaders/test_pybullet.py
--rw-r--r--   0        0        0     1547 2023-01-06 14:01:23.821479 robot_descriptions-1.4.1/tests/loaders/test_robomeshcat.py
--rw-r--r--   0        0        0     1488 2023-01-06 14:01:23.821479 robot_descriptions-1.4.1/tests/loaders/test_yourdfpy.py
--rw-r--r--   0        0        0     2802 2023-02-08 17:58:19.351928 robot_descriptions-1.4.1/tests/test_clone_to_cache.py
--rw-r--r--   0        0        0     3585 2023-02-08 17:58:19.351928 robot_descriptions-1.4.1/tests/test_clone_to_directory.py
--rw-r--r--   0        0        0     2373 2023-02-08 17:58:19.351928 robot_descriptions-1.4.1/tests/test_descriptions.py
--rw-r--r--   0        0        0     2583 2023-02-08 17:58:19.351928 robot_descriptions-1.4.1/tests/test_loaders.py
--rw-r--r--   0        0        0      987 2023-02-08 17:58:19.351928 robot_descriptions-1.4.1/tests/test_progress_bar.py
--rw-r--r--   0        0        0     2225 2023-02-13 11:16:52.067235 robot_descriptions-1.4.1/tox.ini
--rw-r--r--   0        0        0    16246 1970-01-01 00:00:00.000000 robot_descriptions-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     2290 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       42 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/.gitignore
+-rw-r--r--   0        0        0     5071 2023-04-13 09:25:54.436823 robot_descriptions-1.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2039 2023-04-13 09:16:00.609377 robot_descriptions-1.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/LICENSE
+-rw-r--r--   0        0        0    15234 2023-04-13 09:11:45.925423 robot_descriptions-1.5.0/README.md
+-rw-r--r--   0        0        0     2905 2023-03-16 09:00:10.280693 robot_descriptions-1.5.0/examples/display_urdf_frames.py
+-rw-r--r--   0        0        0     1295 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/load_in_idyntree.py
+-rw-r--r--   0        0        0     1280 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/load_in_mujoco.py
+-rw-r--r--   0        0        0     1276 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/load_in_pinocchio.py
+-rw-r--r--   0        0        0     1370 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/load_in_pybullet.py
+-rw-r--r--   0        0        0     1280 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/load_in_robomeshcat.py
+-rw-r--r--   0        0        0     1280 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/load_in_yourdfpy.py
+-rw-r--r--   0        0        0     1642 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/show_in_meshcat.py
+-rw-r--r--   0        0        0     1716 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/show_in_mujoco.py
+-rw-r--r--   0        0        0     1505 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/show_in_pybullet.py
+-rw-r--r--   0        0        0     1665 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/show_in_robomeshcat.py
+-rw-r--r--   0        0        0     1579 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/show_in_yourdfpy.py
+-rw-r--r--   0        0        0     1863 2023-02-13 11:16:52.063235 robot_descriptions-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      714 2023-04-13 09:26:03.117116 robot_descriptions-1.5.0/robot_descriptions/__init__.py
+-rw-r--r--   0        0        0     4385 2023-02-13 11:16:52.063235 robot_descriptions-1.5.0/robot_descriptions/_cache.py
+-rw-r--r--   0        0        0     5604 2023-02-13 11:16:52.063235 robot_descriptions-1.5.0/robot_descriptions/_command_line.py
+-rw-r--r--   0        0        0     5090 2023-04-13 09:12:36.338206 robot_descriptions-1.5.0/robot_descriptions/_descriptions.py
+-rw-r--r--   0        0        0      674 2023-02-13 11:16:52.063235 robot_descriptions-1.5.0/robot_descriptions/_empty_description.py
+-rw-r--r--   0        0        0     1114 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/_package_dirs.py
+-rw-r--r--   0        0        0     9642 2023-04-13 09:09:48.451600 robot_descriptions-1.5.0/robot_descriptions/_repositories.py
+-rw-r--r--   0        0        0     1024 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/a1_description.py
+-rw-r--r--   0        0        0     1078 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/a1_mj_description.py
+-rw-r--r--   0        0        0     1093 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/aliengo_description.py
+-rw-r--r--   0        0        0     1325 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/allegro_hand_description.py
+-rw-r--r--   0        0        0     1022 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/anymal_b_description.py
+-rw-r--r--   0        0        0     1031 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/anymal_b_mj_description.py
+-rw-r--r--   0        0        0     1022 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/anymal_c_description.py
+-rw-r--r--   0        0        0     1031 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/anymal_c_mj_description.py
+-rw-r--r--   0        0        0     1171 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/atlas_drc_description.py
+-rw-r--r--   0        0        0     1381 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/atlas_v4_description.py
+-rw-r--r--   0        0        0     1025 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/b1_description.py
+-rw-r--r--   0        0        0     1016 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/barrett_hand_description.py
+-rw-r--r--   0        0        0     1028 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/baxter_description.py
+-rw-r--r--   0        0        0     1039 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/bolt_description.py
+-rw-r--r--   0        0        0     1012 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/cassie_description.py
+-rw-r--r--   0        0        0     1023 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/cassie_mj_description.py
+-rw-r--r--   0        0        0     1048 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/cf2_description.py
+-rw-r--r--   0        0        0     1304 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/double_pendulum_description.py
+-rw-r--r--   0        0        0     1011 2023-02-22 15:58:12.265767 robot_descriptions-1.5.0/robot_descriptions/draco3_description.py
+-rw-r--r--   0        0        0      997 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/edo_description.py
+-rw-r--r--   0        0        0     1042 2023-02-28 10:22:37.917012 robot_descriptions-1.5.0/robot_descriptions/ergocub_description.py
+-rw-r--r--   0        0        0     1034 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/eve_r3_description.py
+-rw-r--r--   0        0        0     1060 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/fetch_description.py
+-rw-r--r--   0        0        0     1065 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/finger_edu_description.py
+-rw-r--r--   0        0        0     1043 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/gen2_description.py
+-rw-r--r--   0        0        0     1020 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/gen3_mj_description.py
+-rw-r--r--   0        0        0     1007 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/ginger_description.py
+-rw-r--r--   0        0        0     1027 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/go1_description.py
+-rw-r--r--   0        0        0     1082 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/go1_mj_description.py
+-rw-r--r--   0        0        0     1047 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/hyq_description.py
+-rw-r--r--   0        0        0     1035 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/icub_description.py
+-rw-r--r--   0        0        0     1427 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/iiwa_description.py
+-rw-r--r--   0        0        0     1013 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/jaxon_description.py
+-rw-r--r--   0        0        0     1008 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/jvrc_description.py
+-rw-r--r--   0        0        0     1014 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/jvrc_mj_description.py
+-rw-r--r--   0        0        0     1093 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/laikago_description.py
+-rw-r--r--   0        0        0      683 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/loaders/__init__.py
+-rw-r--r--   0        0        0     2587 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/loaders/idyntree.py
+-rw-r--r--   0        0        0     1514 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/loaders/mujoco.py
+-rw-r--r--   0        0        0     2173 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/loaders/pinocchio.py
+-rw-r--r--   0        0        0     2157 2023-04-03 09:25:58.942767 robot_descriptions-1.5.0/robot_descriptions/loaders/pybullet.py
+-rw-r--r--   0        0        0     1612 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/loaders/robomeshcat.py
+-rw-r--r--   0        0        0     1732 2023-02-22 15:58:12.265767 robot_descriptions-1.5.0/robot_descriptions/loaders/yourdfpy.py
+-rw-r--r--   0        0        0     1022 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/mini_cheetah_description.py
+-rw-r--r--   0        0        0     1017 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/minitaur_description.py
+-rw-r--r--   0        0        0     1036 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/nextage_description.py
+-rw-r--r--   0        0        0     1040 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/panda_description.py
+-rw-r--r--   0        0        0     1025 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/panda_mj_description.py
+-rw-r--r--   0        0        0     1011 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/pepper_description.py
+-rw-r--r--   0        0        0     1032 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/poppy_ergo_jr_description.py
+-rw-r--r--   0        0        0     1026 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/poppy_torso_description.py
+-rw-r--r--   0        0        0     1017 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/pr2_description.py
+-rw-r--r--   0        0        0     2748 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/r2_description.py
+-rw-r--r--   0        0        0     1003 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/reachy_description.py
+-rw-r--r--   0        0        0     1005 2023-03-16 16:25:43.136050 robot_descriptions-1.5.0/robot_descriptions/rhea_description.py
+-rw-r--r--   0        0        0     1052 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/robotiq_2f85_description.py
+-rw-r--r--   0        0        0     1026 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/robotiq_2f85_mj_description.py
+-rw-r--r--   0        0        0     1053 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/romeo_description.py
+-rw-r--r--   0        0        0     1190 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/shadow_hand_mj_description.py
+-rw-r--r--   0        0        0      999 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/sigmaban_description.py
+-rw-r--r--   0        0        0     1139 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/simple_humanoid_description.py
+-rw-r--r--   0        0        0     1041 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/solo_description.py
+-rw-r--r--   0        0        0     1035 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/spryped_description.py
+-rw-r--r--   0        0        0     1008 2023-04-13 09:12:21.205971 robot_descriptions-1.5.0/robot_descriptions/stretch_description.py
+-rw-r--r--   0        0        0     1286 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/talos_description.py
+-rw-r--r--   0        0        0     1238 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/tiago_description.py
+-rw-r--r--   0        0        0     1008 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/upkie_description.py
+-rw-r--r--   0        0        0     1175 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/ur10_description.py
+-rw-r--r--   0        0        0     1251 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/ur3_description.py
+-rw-r--r--   0        0        0     1251 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/ur5_description.py
+-rw-r--r--   0        0        0     1026 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/ur5e_mj_description.py
+-rw-r--r--   0        0        0     1350 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/valkyrie_description.py
+-rw-r--r--   0        0        0     1020 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/yumi_description.py
+-rw-r--r--   0        0        0     1025 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/z1_description.py
+-rw-r--r--   0        0        0     1002 2023-02-08 17:58:19.351928 robot_descriptions-1.5.0/tests/__init__.py
+-rw-r--r--   0        0        0       59 2023-01-06 14:01:23.821479 robot_descriptions-1.5.0/tests/loaders/__init__.py
+-rwxr-xr-x   0        0        0     1531 2023-01-06 14:01:23.821479 robot_descriptions-1.5.0/tests/loaders/test_idyntree.py
+-rw-r--r--   0        0        0     1479 2023-01-06 14:01:23.821479 robot_descriptions-1.5.0/tests/loaders/test_mujoco.py
+-rw-r--r--   0        0        0     1536 2023-01-06 14:01:23.821479 robot_descriptions-1.5.0/tests/loaders/test_pinocchio.py
+-rw-r--r--   0        0        0     1976 2023-01-06 14:01:23.821479 robot_descriptions-1.5.0/tests/loaders/test_pybullet.py
+-rw-r--r--   0        0        0     1547 2023-01-06 14:01:23.821479 robot_descriptions-1.5.0/tests/loaders/test_robomeshcat.py
+-rw-r--r--   0        0        0     1488 2023-01-06 14:01:23.821479 robot_descriptions-1.5.0/tests/loaders/test_yourdfpy.py
+-rw-r--r--   0        0        0     2802 2023-02-08 17:58:19.351928 robot_descriptions-1.5.0/tests/test_clone_to_cache.py
+-rw-r--r--   0        0        0     3585 2023-02-08 17:58:19.351928 robot_descriptions-1.5.0/tests/test_clone_to_directory.py
+-rw-r--r--   0        0        0     2373 2023-02-08 17:58:19.351928 robot_descriptions-1.5.0/tests/test_descriptions.py
+-rw-r--r--   0        0        0     2583 2023-02-08 17:58:19.351928 robot_descriptions-1.5.0/tests/test_loaders.py
+-rw-r--r--   0        0        0      987 2023-02-08 17:58:19.351928 robot_descriptions-1.5.0/tests/test_progress_bar.py
+-rw-r--r--   0        0        0     2225 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/tox.ini
+-rw-r--r--   0        0        0    16702 1970-01-01 00:00:00.000000 robot_descriptions-1.5.0/PKG-INFO
```

### Comparing `robot_descriptions-1.4.1/.github/workflows/test.yml` & `robot_descriptions-1.5.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/CHANGELOG.md` & `robot_descriptions-1.5.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [1.5.0] - 2023/4/13
+
+### Added
+
+- Description: Rhea
+- Description: Stretch
+- Frame selector in URDF frame display example
+- README: Conda installation instructions
+
+### Changed
+
+- Update Upkie description to v1.2.0
+
 ## [1.4.1] - 2023/2/28
 
 ### Added
 
 - Description: Draco3 (thanks to @shbang91)
 - Description: ergoCub
```

### Comparing `robot_descriptions-1.4.1/CONTRIBUTING.md` & `robot_descriptions-1.5.0/CONTRIBUTING.md`

 * *Files 20% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 2. **Repository:** If needed, add the repository containing the new description to ``_repositories.py``.
     - Use a specific git commit ID. This way the robot description will still work in the interval between a change in the file structure of the target repository and the corresponding update in `robot_descriptions`.
 3. **Submodule:** add a Python file for the robot descriptions to ``robot_descriptions/``.
     - The file name for the new submodule is ``<robot_name>_description.py`` in snake-case.
     - For example, the file name for the Kinova (maker) Gen2 (robot name) is ``gen2_description.py``.
     - Use the ``mj_description`` suffix for an MJCF description.
 4. **Listing:** Add the description metadata to the ``DESCRIPTIONS`` dictionary in ``_descriptions.py``.
-5. **Testing:** Check that all unit tests are successful by ``tox -e py``.
+5. **Testing:** Check that all unit tests are successful by ``tox``.
 6. **README:** Document the description's submodule name in the Descriptions section of the [README](README.md).
 7. **Changelog:** Write down the new model at the top of the [changelog](CHANGELOG.md).
```

### Comparing `robot_descriptions-1.4.1/LICENSE` & `robot_descriptions-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/README.md` & `robot_descriptions-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 # Robot descriptions in Python
 
 [![Build](https://img.shields.io/github/actions/workflow/status/robot-descriptions/robot_descriptions.py/test.yml?branch=master)](https://github.com/robot-descriptions/robot_descriptions.py/actions)
 [![Coverage](https://coveralls.io/repos/github/robot-descriptions/robot_descriptions.py/badge.svg?branch=master)](https://coveralls.io/github/robot-descriptions/robot_descriptions.py?branch=master)
 [![PyPI version](https://img.shields.io/pypi/v/robot_descriptions)](https://pypi.org/project/robot_descriptions/)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/robot_descriptions.svg)](https://anaconda.org/conda-forge/robot_descriptions)
 [![Contributing](https://img.shields.io/badge/PRs-welcome-green.svg)](https://github.com/robot-descriptions/robot_descriptions.py/tree/master/CONTRIBUTING.md)
 
 Import open source robot descriptions as Python modules.
 
 Importing a description for the first time automatically downloads and caches files for future imports. Most [Awesome Robot Descriptions](https://github.com/robot-descriptions/awesome-robot-descriptions) are available. All of them [load successfully](https://github.com/robot-descriptions/robot_descriptions.py#loaders) in respectively MuJoCo (MJCF) or Pinocchio, iDynTree, PyBullet and yourdfpy (URDF).
 
 ## Installation
 
+### Install from pip
 ```console
 pip install robot_descriptions
 ```
 
+### Install from conda
+```console
+conda install -c conda-forge robot_descriptions
+```
+
 ## Usage
 
 The library provides `load_robot_description` functions that return an instance of a robot description directly usable in the corresponding software. For example:
 
 ```python
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
@@ -135,14 +142,15 @@
 ### Bipeds
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `bolt_description`            | Bolt                  | ODRI                     | 6   | URDF       |
 | `cassie_description`          | Cassie                | Agility Robotics         | 16  | URDF       |
 | `cassie_mj_description`       | Cassie                | Agility Robotics         | 16  | MJCF       |
+| `rhea_description`            | Rhea                  | Gabrael Levine           | 7   | URDF       |
 | `spryped_description`         | Spryped               | Benjamin Bokser          | 8   | URDF       |
 | `upkie_description`           | Upkie                 | Tast's Robots            | 6   | URDF       |
 
 ### Dual arms
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
@@ -199,14 +207,15 @@
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `eve_r3_description`          | Eve R3                | Halodi                   | 23  | URDF       |
 | `fetch_description`           | Fetch                 | Fetch Robotics           | 14  | URDF       |
 | `ginger_description`          | Ginger                | Paaila Technology        | 49  | URDF       |
 | `pepper_description`          | Pepper                | SoftBank Robotics        | 17  | URDF       |
 | `pr2_description`             | PR2                   | Willow Garage            | 32  | URDF       |
 | `reachy_description`          | Reachy                | Pollen Robotics          | 21  | URDF       |
+| `stretch_description`         | Stretch RE1           | Hello Robot              | 14  | URDF       |
 | `tiago_description`           | TIAGo                 | PAL Robotics             | 48  | URDF       |
 
 ### Quadrupeds
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `a1_mj_description`           | A1                    | UNITREE Robotics         | 12  | MJCF       |
```

### Comparing `robot_descriptions-1.4.1/examples/display_urdf_frames.py` & `robot_descriptions-1.5.0/examples/display_urdf_frames.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,25 +22,31 @@
 
 - `MeshCat <https://github.com/rdeits/meshcat-python>`_
 - `meshcat-shapes <https://github.com/stephane-caron/meshcat-shapes>`_
 - `Pinocchio <https://github.com/stack-of-tasks/pinocchio>`_
 """
 
 import argparse
+import time
 
 import meshcat_shapes
 import numpy as np
 from meshcat import transformations
 from pinocchio.visualize import MeshcatVisualizer
+
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument("name", help="name of the robot description")
     parser.add_argument(
+        "--only",
+        help="only display the frame with this name",
+    )
+    parser.add_argument(
         "--frame-scale",
         type=float,
         default=1.0,
         help="scaling factor applied to all frames",
     )
     args = parser.parse_args()
 
@@ -52,15 +58,15 @@
     robot.setVisualizer(MeshcatVisualizer())
     robot.initViewer(open=True)
     robot.loadViewerModel(color=[1.0, 1.0, 1.0, 0.3])
     robot.display(robot.q0)
     viewer = robot.viz.viewer
 
     for frame in robot.model.frames:
-        if frame.name == "universe":
+        if frame.name == "universe" or (args.only and frame.name != args.only):
             continue
         handle = viewer["pinocchio"]["visuals"][f"{frame.name}_0"]
         meshcat_shapes.frame(
             handle["frame"],
             axis_length=0.05 * args.frame_scale,
             axis_thickness=0.001 * args.frame_scale,
             opacity=0.8,
@@ -75,7 +81,9 @@
         )
         Rx = transformations.rotation_matrix(0.5 * np.pi, [1.0, 0.0, 0.0])
         Rz = transformations.rotation_matrix(0.5 * np.pi, [0.0, 0.0, 1.0])
         trans = transformations.translation_matrix(
             [0.0, 0.0, 0.005 * args.frame_scale]
         )
         handle["text"].set_transform(trans @ Rz @ Rx)
+
+    time.sleep(1.0)  # avoid terminating too fast
```

### Comparing `robot_descriptions-1.4.1/examples/load_in_idyntree.py` & `robot_descriptions-1.5.0/examples/load_in_idyntree.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/examples/load_in_mujoco.py` & `robot_descriptions-1.5.0/examples/load_in_mujoco.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/examples/load_in_pinocchio.py` & `robot_descriptions-1.5.0/examples/load_in_pinocchio.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/examples/load_in_pybullet.py` & `robot_descriptions-1.5.0/examples/load_in_pybullet.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/examples/load_in_robomeshcat.py` & `robot_descriptions-1.5.0/examples/load_in_robomeshcat.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/examples/load_in_yourdfpy.py` & `robot_descriptions-1.5.0/examples/load_in_yourdfpy.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/examples/show_in_meshcat.py` & `robot_descriptions-1.5.0/examples/show_in_meshcat.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/examples/show_in_mujoco.py` & `robot_descriptions-1.5.0/examples/show_in_mujoco.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/examples/show_in_pybullet.py` & `robot_descriptions-1.5.0/examples/show_in_pybullet.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/examples/show_in_robomeshcat.py` & `robot_descriptions-1.5.0/examples/show_in_robomeshcat.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/examples/show_in_yourdfpy.py` & `robot_descriptions-1.5.0/examples/show_in_yourdfpy.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/pyproject.toml` & `robot_descriptions-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/__init__.py` & `robot_descriptions-1.5.0/robot_descriptions/_empty_description.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,10 +11,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Import open source robot description as Python modules."""
-
-__version__ = "1.4.1"
+"""Empty description, used in unit tests."""
```

### Comparing `robot_descriptions-1.4.1/robot_descriptions/_cache.py` & `robot_descriptions-1.5.0/robot_descriptions/_cache.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/_command_line.py` & `robot_descriptions-1.5.0/robot_descriptions/_command_line.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/_descriptions.py` & `robot_descriptions-1.5.0/robot_descriptions/_descriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,21 +102,23 @@
     "panda_mj_description": Description(Format.MJCF),
     "pepper_description": Description(Format.URDF),
     "poppy_ergo_jr_description": Description(Format.URDF),
     "poppy_torso_description": Description(Format.URDF),
     "pr2_description": Description(Format.URDF),
     "r2_description": Description(Format.URDF),
     "reachy_description": Description(Format.URDF),
+    "rhea_description": Description(Format.URDF),
     "robotiq_2f85_description": Description(Format.URDF),
     "robotiq_2f85_mj_description": Description(Format.MJCF),
     "romeo_description": Description(Format.URDF),
     "shadow_hand_mj_description": Description(Format.MJCF),
     "simple_humanoid_description": Description(Format.URDF),
     "solo_description": Description(Format.URDF),
     "spryped_description": Description(Format.URDF),
+    "stretch_description": Description(Format.URDF),
     "talos_description": Description(Format.URDF),
     "tiago_description": Description(Format.URDF),
     "upkie_description": Description(Format.URDF),
     "ur10_description": Description(Format.URDF),
     "ur3_description": Description(Format.URDF),
     "ur5_description": Description(Format.URDF),
     "ur5e_mj_description": Description(Format.MJCF),
```

### Comparing `robot_descriptions-1.4.1/robot_descriptions/_empty_description.py` & `robot_descriptions-1.5.0/robot_descriptions/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,8 +11,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Empty description, used in unit tests."""
+"""Import open source robot description as Python modules."""
+
+__version__ = "1.5.0"
```

### Comparing `robot_descriptions-1.4.1/robot_descriptions/_package_dirs.py` & `robot_descriptions-1.5.0/robot_descriptions/_package_dirs.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/_repositories.py` & `robot_descriptions-1.5.0/robot_descriptions/_repositories.py`

 * *Files 5% similar despite different names*

```diff
@@ -173,14 +173,19 @@
         cache_path="poppy_torso_description",
     ),
     "reachy_description": Repository(
         url="https://github.com/aubrune/reachy_description.git",
         commit="release-1.0.0",
         cache_path="reachy_description",
     ),
+    "rhea_description": Repository(
+        url="https://github.com/G-Levine/rhea_description.git",
+        commit="1dc0f1abcf51b5d8a8f7ff8a548399ff0df1414f",
+        cache_path="rhea_description",
+    ),
     "robot-assets": Repository(
         url="https://github.com/ankurhanda/robot-assets.git",
         commit="12f1a3c89c9975194551afaed0dfae1e09fdb27c",
         cache_path="robot-assets",
     ),
     "roboschool": Repository(
         url="https://github.com/openai/roboschool.git",
@@ -213,14 +218,19 @@
         cache_path="simple_humanoid_description",
     ),
     "spryped": Repository(
         url="https://github.com/bbokser/spryped.git",
         commit="f360a6b78667a4d97c86cad465ef8f4c9512462b",
         cache_path="spryped",
     ),
+    "stretch_description": Repository(
+        url="https://github.com/robot-descriptions/stretch_description.git",
+        commit="d9a614f8572d5a73f78a7f358107233c40a78b13",
+        cache_path="stretch_description",
+    ),
     "talos-data": Repository(
         url="https://github.com/stack-of-tasks/talos-data.git",
         commit="v2.0.0",
         cache_path="talos_data",  # match package name
     ),
     "unitree_mujoco": Repository(
         url="https://github.com/unitreerobotics/unitree_mujoco.git",
@@ -230,11 +240,11 @@
     "unitree_ros": Repository(
         url="https://github.com/unitreerobotics/unitree_ros.git",
         commit="059bd619c14c5d06346bcdec57b4191dccee2b86",
         cache_path="unitree_ros",
     ),
     "upkie_description": Repository(
         url="https://github.com/tasts-robots/upkie_description.git",
-        commit="v1.1.0",
+        commit="3bc5251b7255641d275de8c6b949e13bf1a608ea",
         cache_path="upkie_description",
     ),
 }
```

### Comparing `robot_descriptions-1.4.1/robot_descriptions/a1_description.py` & `robot_descriptions-1.5.0/robot_descriptions/a1_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/a1_mj_description.py` & `robot_descriptions-1.5.0/robot_descriptions/a1_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/aliengo_description.py` & `robot_descriptions-1.5.0/robot_descriptions/aliengo_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/allegro_hand_description.py` & `robot_descriptions-1.5.0/robot_descriptions/allegro_hand_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/anymal_b_description.py` & `robot_descriptions-1.5.0/robot_descriptions/anymal_b_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/anymal_b_mj_description.py` & `robot_descriptions-1.5.0/robot_descriptions/anymal_b_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/anymal_c_description.py` & `robot_descriptions-1.5.0/robot_descriptions/anymal_c_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/anymal_c_mj_description.py` & `robot_descriptions-1.5.0/robot_descriptions/anymal_c_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/atlas_drc_description.py` & `robot_descriptions-1.5.0/robot_descriptions/atlas_drc_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/atlas_v4_description.py` & `robot_descriptions-1.5.0/robot_descriptions/atlas_v4_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/b1_description.py` & `robot_descriptions-1.5.0/robot_descriptions/b1_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/barrett_hand_description.py` & `robot_descriptions-1.5.0/robot_descriptions/barrett_hand_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/baxter_description.py` & `robot_descriptions-1.5.0/robot_descriptions/baxter_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/bolt_description.py` & `robot_descriptions-1.5.0/robot_descriptions/bolt_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/cassie_description.py` & `robot_descriptions-1.5.0/robot_descriptions/cassie_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/cassie_mj_description.py` & `robot_descriptions-1.5.0/robot_descriptions/cassie_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/cf2_description.py` & `robot_descriptions-1.5.0/robot_descriptions/cf2_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/double_pendulum_description.py` & `robot_descriptions-1.5.0/robot_descriptions/double_pendulum_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/draco3_description.py` & `robot_descriptions-1.5.0/robot_descriptions/draco3_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/edo_description.py` & `robot_descriptions-1.5.0/robot_descriptions/edo_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/ergocub_description.py` & `robot_descriptions-1.5.0/robot_descriptions/ergocub_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/eve_r3_description.py` & `robot_descriptions-1.5.0/robot_descriptions/eve_r3_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/fetch_description.py` & `robot_descriptions-1.5.0/robot_descriptions/fetch_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/finger_edu_description.py` & `robot_descriptions-1.5.0/robot_descriptions/finger_edu_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/gen2_description.py` & `robot_descriptions-1.5.0/robot_descriptions/gen2_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/gen3_mj_description.py` & `robot_descriptions-1.5.0/robot_descriptions/gen3_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/ginger_description.py` & `robot_descriptions-1.5.0/robot_descriptions/ginger_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/go1_description.py` & `robot_descriptions-1.5.0/robot_descriptions/go1_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/go1_mj_description.py` & `robot_descriptions-1.5.0/robot_descriptions/go1_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/hyq_description.py` & `robot_descriptions-1.5.0/robot_descriptions/hyq_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/icub_description.py` & `robot_descriptions-1.5.0/robot_descriptions/icub_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/iiwa_description.py` & `robot_descriptions-1.5.0/robot_descriptions/iiwa_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/jaxon_description.py` & `robot_descriptions-1.5.0/robot_descriptions/jaxon_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/jvrc_description.py` & `robot_descriptions-1.5.0/robot_descriptions/jvrc_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/jvrc_mj_description.py` & `robot_descriptions-1.5.0/robot_descriptions/jvrc_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/laikago_description.py` & `robot_descriptions-1.5.0/robot_descriptions/laikago_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/loaders/__init__.py` & `robot_descriptions-1.5.0/robot_descriptions/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/loaders/idyntree.py` & `robot_descriptions-1.5.0/robot_descriptions/loaders/idyntree.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/loaders/mujoco.py` & `robot_descriptions-1.5.0/robot_descriptions/loaders/mujoco.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/loaders/pinocchio.py` & `robot_descriptions-1.5.0/robot_descriptions/loaders/pinocchio.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/loaders/pybullet.py` & `robot_descriptions-1.5.0/robot_descriptions/loaders/pybullet.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,27 +24,37 @@
 
 import pybullet
 
 
 def load_robot_description(
     description_name: str,
     commit: Optional[str] = None,
+    **kwargs,
 ) -> int:
     """Load a robot description in PyBullet.
 
     Args:
         description_name: Name of the robot description.
         commit: If specified, check out that commit from the cloned robot
             description repository.
+        kwargs: arguments passed to pybullet.loadURDF function, including:
+            basePosition: 3D position of the base of the robot in world
+                coordinates.
+            baseOrientation: orientation in quaternion (xyzw) of the base of
+                the robot in world coordinates.
+            flags: int flags for the URDF loading in pybullet.
+            useFixedBase: boolean indicating use a fix joint between world and
+                robot base.
+            physicsClientId: int indicating the pybullet client id.
 
     Returns:
-        Identifier of the robot in PyBullet.
+        Integer identifier of the robot in PyBullet.
     """
     if commit is not None:
         os.environ["ROBOT_DESCRIPTION_COMMIT"] = commit
     module = import_module(f"robot_descriptions.{description_name}")
     if not hasattr(module, "URDF_PATH"):
         raise ValueError(f"{description_name} is not a URDF description")
 
     pybullet.setAdditionalSearchPath(module.PACKAGE_PATH)
-    robot = pybullet.loadURDF(module.URDF_PATH)
+    robot = pybullet.loadURDF(module.URDF_PATH, **kwargs)
     return robot
```

### Comparing `robot_descriptions-1.4.1/robot_descriptions/loaders/robomeshcat.py` & `robot_descriptions-1.5.0/robot_descriptions/loaders/robomeshcat.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/loaders/yourdfpy.py` & `robot_descriptions-1.5.0/robot_descriptions/loaders/yourdfpy.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/mini_cheetah_description.py` & `robot_descriptions-1.5.0/robot_descriptions/mini_cheetah_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/minitaur_description.py` & `robot_descriptions-1.5.0/robot_descriptions/minitaur_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/nextage_description.py` & `robot_descriptions-1.5.0/robot_descriptions/nextage_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/panda_description.py` & `robot_descriptions-1.5.0/robot_descriptions/panda_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/panda_mj_description.py` & `robot_descriptions-1.5.0/robot_descriptions/panda_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/pepper_description.py` & `robot_descriptions-1.5.0/robot_descriptions/pepper_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/poppy_ergo_jr_description.py` & `robot_descriptions-1.5.0/robot_descriptions/poppy_ergo_jr_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/poppy_torso_description.py` & `robot_descriptions-1.5.0/robot_descriptions/poppy_torso_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/pr2_description.py` & `robot_descriptions-1.5.0/robot_descriptions/pr2_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/r2_description.py` & `robot_descriptions-1.5.0/robot_descriptions/r2_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/reachy_description.py` & `robot_descriptions-1.5.0/robot_descriptions/reachy_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/robotiq_2f85_description.py` & `robot_descriptions-1.5.0/robot_descriptions/robotiq_2f85_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/robotiq_2f85_mj_description.py` & `robot_descriptions-1.5.0/robot_descriptions/robotiq_2f85_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/romeo_description.py` & `robot_descriptions-1.5.0/robot_descriptions/romeo_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/shadow_hand_mj_description.py` & `robot_descriptions-1.5.0/robot_descriptions/shadow_hand_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/sigmaban_description.py` & `robot_descriptions-1.5.0/robot_descriptions/sigmaban_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/simple_humanoid_description.py` & `robot_descriptions-1.5.0/robot_descriptions/simple_humanoid_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/solo_description.py` & `robot_descriptions-1.5.0/robot_descriptions/solo_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/spryped_description.py` & `robot_descriptions-1.5.0/robot_descriptions/spryped_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/talos_description.py` & `robot_descriptions-1.5.0/robot_descriptions/talos_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/tiago_description.py` & `robot_descriptions-1.5.0/robot_descriptions/tiago_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/upkie_description.py` & `robot_descriptions-1.5.0/robot_descriptions/upkie_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/ur10_description.py` & `robot_descriptions-1.5.0/robot_descriptions/ur10_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/ur3_description.py` & `robot_descriptions-1.5.0/robot_descriptions/ur3_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/ur5_description.py` & `robot_descriptions-1.5.0/robot_descriptions/ur5_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/ur5e_mj_description.py` & `robot_descriptions-1.5.0/robot_descriptions/ur5e_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/valkyrie_description.py` & `robot_descriptions-1.5.0/robot_descriptions/valkyrie_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/yumi_description.py` & `robot_descriptions-1.5.0/robot_descriptions/yumi_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/robot_descriptions/z1_description.py` & `robot_descriptions-1.5.0/robot_descriptions/z1_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/tests/__init__.py` & `robot_descriptions-1.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/tests/loaders/test_idyntree.py` & `robot_descriptions-1.5.0/tests/loaders/test_idyntree.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/tests/loaders/test_mujoco.py` & `robot_descriptions-1.5.0/tests/loaders/test_mujoco.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/tests/loaders/test_pinocchio.py` & `robot_descriptions-1.5.0/tests/loaders/test_pinocchio.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/tests/loaders/test_pybullet.py` & `robot_descriptions-1.5.0/tests/loaders/test_pybullet.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/tests/loaders/test_robomeshcat.py` & `robot_descriptions-1.5.0/tests/loaders/test_robomeshcat.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/tests/loaders/test_yourdfpy.py` & `robot_descriptions-1.5.0/tests/loaders/test_yourdfpy.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/tests/test_clone_to_cache.py` & `robot_descriptions-1.5.0/tests/test_clone_to_cache.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/tests/test_clone_to_directory.py` & `robot_descriptions-1.5.0/tests/test_clone_to_directory.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/tests/test_descriptions.py` & `robot_descriptions-1.5.0/tests/test_descriptions.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/tests/test_loaders.py` & `robot_descriptions-1.5.0/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/tests/test_progress_bar.py` & `robot_descriptions-1.5.0/tests/test_progress_bar.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/tox.ini` & `robot_descriptions-1.5.0/tox.ini`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.4.1/PKG-INFO` & `robot_descriptions-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot_descriptions
-Version: 1.4.1
+Version: 1.5.0
 Summary: Import open source robot description as Python modules.
 Keywords: robot,description,urdf,mjcf
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,26 +30,33 @@
 Provides-Extra: opts
 
 # Robot descriptions in Python
 
 [![Build](https://img.shields.io/github/actions/workflow/status/robot-descriptions/robot_descriptions.py/test.yml?branch=master)](https://github.com/robot-descriptions/robot_descriptions.py/actions)
 [![Coverage](https://coveralls.io/repos/github/robot-descriptions/robot_descriptions.py/badge.svg?branch=master)](https://coveralls.io/github/robot-descriptions/robot_descriptions.py?branch=master)
 [![PyPI version](https://img.shields.io/pypi/v/robot_descriptions)](https://pypi.org/project/robot_descriptions/)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/robot_descriptions.svg)](https://anaconda.org/conda-forge/robot_descriptions)
 [![Contributing](https://img.shields.io/badge/PRs-welcome-green.svg)](https://github.com/robot-descriptions/robot_descriptions.py/tree/master/CONTRIBUTING.md)
 
 Import open source robot descriptions as Python modules.
 
 Importing a description for the first time automatically downloads and caches files for future imports. Most [Awesome Robot Descriptions](https://github.com/robot-descriptions/awesome-robot-descriptions) are available. All of them [load successfully](https://github.com/robot-descriptions/robot_descriptions.py#loaders) in respectively MuJoCo (MJCF) or Pinocchio, iDynTree, PyBullet and yourdfpy (URDF).
 
 ## Installation
 
+### Install from pip
 ```console
 pip install robot_descriptions
 ```
 
+### Install from conda
+```console
+conda install -c conda-forge robot_descriptions
+```
+
 ## Usage
 
 The library provides `load_robot_description` functions that return an instance of a robot description directly usable in the corresponding software. For example:
 
 ```python
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
@@ -166,14 +173,15 @@
 ### Bipeds
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `bolt_description`            | Bolt                  | ODRI                     | 6   | URDF       |
 | `cassie_description`          | Cassie                | Agility Robotics         | 16  | URDF       |
 | `cassie_mj_description`       | Cassie                | Agility Robotics         | 16  | MJCF       |
+| `rhea_description`            | Rhea                  | Gabrael Levine           | 7   | URDF       |
 | `spryped_description`         | Spryped               | Benjamin Bokser          | 8   | URDF       |
 | `upkie_description`           | Upkie                 | Tast's Robots            | 6   | URDF       |
 
 ### Dual arms
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
@@ -230,14 +238,15 @@
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `eve_r3_description`          | Eve R3                | Halodi                   | 23  | URDF       |
 | `fetch_description`           | Fetch                 | Fetch Robotics           | 14  | URDF       |
 | `ginger_description`          | Ginger                | Paaila Technology        | 49  | URDF       |
 | `pepper_description`          | Pepper                | SoftBank Robotics        | 17  | URDF       |
 | `pr2_description`             | PR2                   | Willow Garage            | 32  | URDF       |
 | `reachy_description`          | Reachy                | Pollen Robotics          | 21  | URDF       |
+| `stretch_description`         | Stretch RE1           | Hello Robot              | 14  | URDF       |
 | `tiago_description`           | TIAGo                 | PAL Robotics             | 48  | URDF       |
 
 ### Quadrupeds
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `a1_mj_description`           | A1                    | UNITREE Robotics         | 12  | MJCF       |
```

