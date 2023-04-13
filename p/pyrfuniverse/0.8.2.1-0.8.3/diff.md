# Comparing `tmp/pyrfuniverse-0.8.2.1.tar.gz` & `tmp/pyrfuniverse-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfuniverse-0.8.2.1.tar", last modified: Mon Apr  3 12:36:51 2023, max compression
+gzip compressed data, was "pyrfuniverse-0.8.3.tar", last modified: Thu Apr 13 03:57:00 2023, max compression
```

## Comparing `pyrfuniverse-0.8.2.1.tar` & `pyrfuniverse-0.8.3.tar`

### file list

```diff
@@ -1,163 +1,167 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 12:36:51.630404 pyrfuniverse-0.8.2.1/
--rw-rw-rw-   0        0        0    11357 2022-08-10 05:19:33.000000 pyrfuniverse-0.8.2.1/LICENSE
--rw-rw-rw-   0        0        0      271 2023-04-03 12:36:51.630404 pyrfuniverse-0.8.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2444 2022-11-21 10:59:33.000000 pyrfuniverse-0.8.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 12:36:50.907084 pyrfuniverse-0.8.2.1/pyrfuniverse/
--rw-rw-rw-   0        0        0      760 2023-04-03 12:34:55.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 12:36:51.008746 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/
--rw-rw-rw-   0        0        0     1312 2023-03-21 08:36:21.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/__init__.py
--rw-rw-rw-   0        0        0     4674 2023-03-27 09:00:54.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/activelightsensor_attr.py
--rw-rw-rw-   0        0        0    13595 2023-03-27 09:02:40.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/base_attr.py
--rw-rw-rw-   0        0        0    15324 2023-03-27 09:03:45.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/camera_attr.py
--rw-rw-rw-   0        0        0      384 2023-03-27 09:05:40.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/cloth_attr.py
--rw-rw-rw-   0        0        0     1032 2023-03-27 09:05:40.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/collider_attr.py
--rw-rw-rw-   0        0        0    30402 2023-03-27 09:03:45.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/controller_attr.py
--rw-rw-rw-   0        0        0     1128 2023-03-27 05:31:46.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/custom_attr.py
--rw-rw-rw-   0        0        0     1101 2023-03-27 09:03:45.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/digit_attr.py
--rw-rw-rw-   0        0        0     3366 2023-03-31 10:51:09.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/gameobject_attr.py
--rw-rw-rw-   0        0        0     5192 2023-03-27 09:03:45.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/graspsim_attr.py
--rw-rw-rw-   0        0        0     8161 2023-03-27 09:03:45.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/humanbody_attr.py
--rw-rw-rw-   0        0        0     3157 2023-03-27 09:05:40.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/light_attr.py
--rw-rw-rw-   0        0        0     1587 2023-03-27 09:05:40.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/pointcloud_attr.py
--rw-rw-rw-   0        0        0     2988 2023-03-27 09:03:45.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/rigidbody_attr.py
--rw-rw-rw-   0        0        0      407 2023-03-27 09:05:40.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/softbody_attr.py
--rw-rw-rw-   0        0        0    23240 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/base_env.py
--rw-rw-rw-   0        0        0     1885 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator.py
-drwxrwxrwx   0        0        0        0 2023-04-03 12:36:51.194760 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/
--rw-rw-rw-   0        0        0      835 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/__init__.py
--rw-rw-rw-   0        0        0     3785 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/agent_action_pb2.py
--rw-rw-rw-   0        0        0     3885 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/agent_info_action_pair_pb2.py
--rw-rw-rw-   0        0        0     5849 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/agent_info_pb2.py
--rw-rw-rw-   0        0        0     8080 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/brain_parameters_pb2.py
--rw-rw-rw-   0        0        0     5258 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/capabilities_pb2.py
--rw-rw-rw-   0        0        0     2073 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/command_pb2.py
--rw-rw-rw-   0        0        0     2134 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/custom_reset_parameters_pb2.py
--rw-rw-rw-   0        0        0     4261 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/demonstration_meta_pb2.py
--rw-rw-rw-   0        0        0     4647 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/engine_configuration_pb2.py
--rw-rw-rw-   0        0        0     2709 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/header_pb2.py
--rw-rw-rw-   0        0        0     9625 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/observation_pb2.py
--rw-rw-rw-   0        0        0     1979 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/space_type_pb2.py
--rw-rw-rw-   0        0        0    12746 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/training_analytics_pb2.py
--rw-rw-rw-   0        0        0     3893 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_input_pb2.py
--rw-rw-rw-   0        0        0     4553 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_message_pb2.py
--rw-rw-rw-   0        0        0     3928 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_output_pb2.py
--rw-rw-rw-   0        0        0     4512 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_rl_initialization_input_pb2.py
--rw-rw-rw-   0        0        0     5963 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_rl_initialization_output_pb2.py
--rw-rw-rw-   0        0        0     8094 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_rl_input_pb2.py
--rw-rw-rw-   0        0        0     7216 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_rl_output_pb2.py
--rw-rw-rw-   0        0        0     2353 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_to_external_pb2.py
--rw-rw-rw-   0        0        0     1775 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_to_external_pb2_grpc.py
--rw-rw-rw-   0        0        0     5172 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/env_utils.py
--rw-rw-rw-   0        0        0    22174 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/environment.py
-drwxrwxrwx   0        0        0        0 2023-04-03 12:36:51.244830 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/
--rw-rw-rw-   0        0        0    14071 2023-04-03 12:36:28.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/__init__.py
--rw-rw-rw-   0        0        0     4178 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/balance_ball_env.py
--rw-rw-rw-   0        0        0    22634 2023-04-03 12:33:42.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/base_env.py
--rw-rw-rw-   0        0        0     4564 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/bouncer_env.py
--rw-rw-rw-   0        0        0     3982 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/franka_grasp_env.py
--rw-rw-rw-   0        0        0     3077 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/franka_push_env.py
-drwxrwxrwx   0        0        0        0 2023-04-03 12:36:51.279863 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/
--rw-rw-rw-   0        0        0      736 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/__init__.py
--rw-rw-rw-   0        0        0     4209 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/nail_can_env.py
--rw-rw-rw-   0        0        0     5750 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/nail_card_env.py
--rw-rw-rw-   0        0        0     3917 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py
--rw-rw-rw-   0        0        0     4149 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py
--rw-rw-rw-   0        0        0     4220 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py
--rw-rw-rw-   0        0        0     5917 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py
--rw-rw-rw-   0        0        0     5696 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py
-drwxrwxrwx   0        0        0        0 2023-04-03 12:36:51.295374 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/multi_agent/
--rw-rw-rw-   0        0        0      172 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/multi_agent/__init__.py
--rw-rw-rw-   0        0        0     9111 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/multi_agent/cleaner_env.py
--rw-rw-rw-   0        0        0    11818 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/multi_agent/navigation_env.py
--rw-rw-rw-   0        0        0     6000 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/multi_agent_navigation_env.py
--rw-rw-rw-   0        0        0      513 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/rfuniverse_robot_hub_env.py
-drwxrwxrwx   0        0        0        0 2023-04-03 12:36:51.337933 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/
--rw-rw-rw-   0        0        0      675 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/__init__.py
--rw-rw-rw-   0        0        0     7357 2022-12-15 06:20:36.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/franka_cloth_env.py
--rw-rw-rw-   0        0        0     7455 2022-12-15 06:20:57.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py
--rw-rw-rw-   0        0        0    10181 2022-12-15 08:02:41.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/franka_robotics_env.py
--rw-rw-rw-   0        0        0     8041 2022-12-15 06:20:52.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/franka_softbody_env.py
--rw-rw-rw-   0        0        0      817 2022-12-15 05:37:19.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/pick_and_place_env.py
--rw-rw-rw-   0        0        0      754 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/push_env.py
--rw-rw-rw-   0        0        0      864 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/reach_env.py
--rw-rw-rw-   0        0        0     4463 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/roller_env.py
-drwxrwxrwx   0        0        0        0 2023-04-03 12:36:51.348931 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/tobor_robotics/
--rw-rw-rw-   0        0        0      121 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/tobor_robotics/__init__.py
--rw-rw-rw-   0        0        0    10897 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py
--rw-rw-rw-   0        0        0     9736 2023-02-15 08:33:33.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py
--rw-rw-rw-   0        0        0     8205 2022-11-02 03:34:57.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/ur5_box_env.py
--rw-rw-rw-   0        0        0     8549 2022-11-02 03:34:57.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/envs/ur5_drawer_env.py
--rw-rw-rw-   0        0        0     1621 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/exception.py
--rw-rw-rw-   0        0        0     1866 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/logging_util.py
--rw-rw-rw-   0        0        0     3924 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/mock_communicator.py
-drwxrwxrwx   0        0        0        0 2023-04-03 12:36:51.373484 pyrfuniverse-0.8.2.1/pyrfuniverse/registry/
--rw-rw-rw-   0        0        0      114 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/registry/__init__.py
--rw-rw-rw-   0        0        0     1855 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/registry/base_registry_entry.py
--rw-rw-rw-   0        0        0     8085 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/registry/binary_utils.py
--rw-rw-rw-   0        0        0     3256 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/registry/remote_registry_entry.py
--rw-rw-rw-   0        0        0     5017 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/registry/unity_env_registry.py
-drwxrwxrwx   0        0        0        0 2023-04-03 12:36:51.406540 pyrfuniverse-0.8.2.1/pyrfuniverse/rfuniverse_channel/
--rw-rw-rw-   0        0        0      487 2023-03-24 04:48:34.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/rfuniverse_channel/__init__.py
--rw-rw-rw-   0        0        0    10343 2023-03-24 07:37:16.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/rfuniverse_channel/asset_channel.py
--rw-rw-rw-   0        0        0     1248 2023-03-15 04:59:29.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/rfuniverse_channel/asset_channel_ext.py
--rw-rw-rw-   0        0        0     1738 2023-03-23 09:10:05.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/rfuniverse_channel/debug_channel.py
--rw-rw-rw-   0        0        0     2188 2023-03-31 05:54:41.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/rfuniverse_channel/instance_channel.py
--rw-rw-rw-   0        0        0     2198 2022-08-25 10:50:54.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/rfuniverse_channel/rfuniverse_channel.py
--rw-rw-rw-   0        0        0     6426 2022-09-28 07:41:12.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/rpc_communicator.py
--rw-rw-rw-   0        0        0    16840 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/rpc_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-03 12:36:51.462896 pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/
--rw-rw-rw-   0        0        0      230 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/__init__.py
--rw-rw-rw-   0        0        0     4935 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/engine_configuration_channel.py
--rw-rw-rw-   0        0        0     3872 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/environment_parameters_channel.py
--rw-rw-rw-   0        0        0     2226 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/float_properties_channel.py
--rw-rw-rw-   0        0        0     3366 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/incoming_message.py
--rw-rw-rw-   0        0        0     1960 2022-09-06 06:01:55.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/outgoing_message.py
--rw-rw-rw-   0        0        0     1300 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/raw_bytes_channel.py
--rw-rw-rw-   0        0        0     1502 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/side_channel.py
--rw-rw-rw-   0        0        0     3745 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/side_channel_manager.py
--rw-rw-rw-   0        0        0     1875 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/stats_side_channel.py
--rw-rw-rw-   0        0        0    11684 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/timers.py
-drwxrwxrwx   0        0        0        0 2023-04-03 12:36:51.525743 pyrfuniverse-0.8.2.1/pyrfuniverse/utils/
--rw-rw-rw-   0        0        0      181 2022-10-31 06:20:22.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/utils/__init__.py
--rw-rw-rw-   0        0        0    13620 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/utils/active_depth_generate.py
--rw-rw-rw-   0        0        0     6006 2022-07-13 10:31:45.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/utils/controller.py
--rw-rw-rw-   0        0        0    10354 2023-02-10 17:44:40.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/utils/depth_processor.py
--rw-rw-rw-   0        0        0     3218 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/utils/interpolate_utils.py
--rw-rw-rw-   0        0        0     4304 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/utils/jaco_controller.py
--rw-rw-rw-   0        0        0     4908 2022-10-27 03:27:48.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/utils/kinova_controller.py
--rw-rw-rw-   0        0        0      755 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/utils/os_utils.py
--rw-rw-rw-   0        0        0     2656 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/utils/rfuniverse_utility.py
--rw-rw-rw-   0        0        0     5690 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/utils/stretch_controller.py
--rw-rw-rw-   0        0        0     6776 2022-08-15 11:02:54.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/utils/tobor_controller.py
--rw-rw-rw-   0        0        0     4783 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.2.1/pyrfuniverse/utils/ur5_controller.py
-drwxrwxrwx   0        0        0        0 2023-04-03 12:36:50.922592 pyrfuniverse-0.8.2.1/pyrfuniverse.egg-info/
--rw-rw-rw-   0        0        0      271 2023-04-03 12:36:50.000000 pyrfuniverse-0.8.2.1/pyrfuniverse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5995 2023-04-03 12:36:50.000000 pyrfuniverse-0.8.2.1/pyrfuniverse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 12:36:50.000000 pyrfuniverse-0.8.2.1/pyrfuniverse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2022-10-31 04:29:22.000000 pyrfuniverse-0.8.2.1/pyrfuniverse.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      108 2023-04-03 12:36:50.000000 pyrfuniverse-0.8.2.1/pyrfuniverse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-03 12:36:50.000000 pyrfuniverse-0.8.2.1/pyrfuniverse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-03 12:36:51.630404 pyrfuniverse-0.8.2.1/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-03 12:34:30.000000 pyrfuniverse-0.8.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-03 12:36:51.629405 pyrfuniverse-0.8.2.1/test/
--rw-rw-rw-   0        0        0     5541 2023-03-24 06:42:21.000000 pyrfuniverse-0.8.2.1/test/test_active_depth.py
--rw-rw-rw-   0        0        0      970 2023-03-24 08:06:33.000000 pyrfuniverse-0.8.2.1/test/test_articulation_ik.py
--rw-rw-rw-   0        0        0      744 2023-03-27 08:09:07.000000 pyrfuniverse-0.8.2.1/test/test_camera_image.py
--rw-rw-rw-   0        0        0     1151 2023-03-24 09:25:29.000000 pyrfuniverse-0.8.2.1/test/test_custom_message.py
--rw-rw-rw-   0        0        0     1038 2023-04-03 08:35:22.000000 pyrfuniverse-0.8.2.1/test/test_debug.py
--rw-rw-rw-   0        0        0      804 2023-03-24 09:25:29.000000 pyrfuniverse-0.8.2.1/test/test_grasp_pose.py
--rw-rw-rw-   0        0        0     2683 2023-03-24 09:25:29.000000 pyrfuniverse-0.8.2.1/test/test_grasp_sim.py
--rw-rw-rw-   0        0        0     1385 2023-03-24 09:25:29.000000 pyrfuniverse-0.8.2.1/test/test_humanbody_ik.py
--rw-rw-rw-   0        0        0     1996 2023-03-24 09:25:29.000000 pyrfuniverse-0.8.2.1/test/test_label.py
--rw-rw-rw-   0        0        0      702 2023-03-21 10:08:20.000000 pyrfuniverse-0.8.2.1/test/test_light.py
--rw-rw-rw-   0        0        0      573 2023-03-23 05:38:04.000000 pyrfuniverse-0.8.2.1/test/test_load_mesh.py
--rw-rw-rw-   0        0        0      984 2023-03-23 05:38:04.000000 pyrfuniverse-0.8.2.1/test/test_load_urdf.py
--rw-rw-rw-   0        0        0     1137 2023-03-20 04:13:02.000000 pyrfuniverse-0.8.2.1/test/test_object_data.py
--rw-rw-rw-   0        0        0     2149 2023-03-15 04:00:24.000000 pyrfuniverse-0.8.2.1/test/test_pick_and_place.py
--rw-rw-rw-   0        0        0     2174 2023-03-15 04:05:23.000000 pyrfuniverse-0.8.2.1/test/test_pick_and_place_flexiv.py
--rw-rw-rw-   0        0        0      570 2022-12-18 09:24:39.000000 pyrfuniverse-0.8.2.1/test/test_pick_and_place_gym.py
--rw-rw-rw-   0        0        0     1746 2023-03-15 04:45:24.000000 pyrfuniverse-0.8.2.1/test/test_point_cloud.py
--rw-rw-rw-   0        0        0      441 2023-03-24 09:50:06.000000 pyrfuniverse-0.8.2.1/test/test_point_cloud_render.py
--rw-rw-rw-   0        0        0     1891 2023-03-15 04:50:29.000000 pyrfuniverse-0.8.2.1/test/test_point_cloud_with_intrinsic_matrix.py
--rw-rw-rw-   0        0        0      380 2023-03-24 09:25:29.000000 pyrfuniverse-0.8.2.1/test/test_save_obj.py
--rw-rw-rw-   0        0        0     1024 2023-03-24 09:46:47.000000 pyrfuniverse-0.8.2.1/test/test_scene.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.412731 pyrfuniverse-0.8.3/
+-rw-rw-rw-   0        0        0    11357 2022-08-10 05:19:33.000000 pyrfuniverse-0.8.3/LICENSE
+-rw-rw-rw-   0        0        0      269 2023-04-13 03:57:00.412731 pyrfuniverse-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2639 2023-04-10 05:02:29.000000 pyrfuniverse-0.8.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 03:56:59.656519 pyrfuniverse-0.8.3/pyrfuniverse/
+-rw-rw-rw-   0        0        0      758 2023-04-13 03:24:35.000000 pyrfuniverse-0.8.3/pyrfuniverse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:56:59.756619 pyrfuniverse-0.8.3/pyrfuniverse/attributes/
+-rw-rw-rw-   0        0        0     1312 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/__init__.py
+-rw-rw-rw-   0        0        0     4757 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/activelightsensor_attr.py
+-rw-rw-rw-   0        0        0    13595 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/base_attr.py
+-rw-rw-rw-   0        0        0    17611 2023-04-10 10:01:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/camera_attr.py
+-rw-rw-rw-   0        0        0      403 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/cloth_attr.py
+-rw-rw-rw-   0        0        0     1074 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/collider_attr.py
+-rw-rw-rw-   0        0        0    31372 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/controller_attr.py
+-rw-rw-rw-   0        0        0     1162 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/custom_attr.py
+-rw-rw-rw-   0        0        0     1143 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/digit_attr.py
+-rw-rw-rw-   0        0        0     3498 2023-04-06 04:49:14.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/gameobject_attr.py
+-rw-rw-rw-   0        0        0     5346 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/graspsim_attr.py
+-rw-rw-rw-   0        0        0     8403 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/humanbody_attr.py
+-rw-rw-rw-   0        0        0     3157 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/light_attr.py
+-rw-rw-rw-   0        0        0     1647 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/pointcloud_attr.py
+-rw-rw-rw-   0        0        0     3103 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/rigidbody_attr.py
+-rw-rw-rw-   0        0        0      407 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/softbody_attr.py
+-rw-rw-rw-   0        0        0    23240 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.3/pyrfuniverse/base_env.py
+-rw-rw-rw-   0        0        0     1885 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:56:59.944455 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/
+-rw-rw-rw-   0        0        0      835 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/__init__.py
+-rw-rw-rw-   0        0        0     3785 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/agent_action_pb2.py
+-rw-rw-rw-   0        0        0     3885 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/agent_info_action_pair_pb2.py
+-rw-rw-rw-   0        0        0     5849 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/agent_info_pb2.py
+-rw-rw-rw-   0        0        0     8080 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/brain_parameters_pb2.py
+-rw-rw-rw-   0        0        0     5258 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/capabilities_pb2.py
+-rw-rw-rw-   0        0        0     2073 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/command_pb2.py
+-rw-rw-rw-   0        0        0     2134 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/custom_reset_parameters_pb2.py
+-rw-rw-rw-   0        0        0     4261 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/demonstration_meta_pb2.py
+-rw-rw-rw-   0        0        0     4647 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/engine_configuration_pb2.py
+-rw-rw-rw-   0        0        0     2709 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/header_pb2.py
+-rw-rw-rw-   0        0        0     9625 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/observation_pb2.py
+-rw-rw-rw-   0        0        0     1979 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/space_type_pb2.py
+-rw-rw-rw-   0        0        0    12746 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/training_analytics_pb2.py
+-rw-rw-rw-   0        0        0     3893 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_input_pb2.py
+-rw-rw-rw-   0        0        0     4553 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_message_pb2.py
+-rw-rw-rw-   0        0        0     3928 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_output_pb2.py
+-rw-rw-rw-   0        0        0     4512 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_initialization_input_pb2.py
+-rw-rw-rw-   0        0        0     5963 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_initialization_output_pb2.py
+-rw-rw-rw-   0        0        0     8094 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_input_pb2.py
+-rw-rw-rw-   0        0        0     7216 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_output_pb2.py
+-rw-rw-rw-   0        0        0     2353 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_to_external_pb2.py
+-rw-rw-rw-   0        0        0     1775 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_to_external_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5172 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/env_utils.py
+-rw-rw-rw-   0        0        0    22704 2023-04-07 06:51:48.000000 pyrfuniverse-0.8.3/pyrfuniverse/environment.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.026548 pyrfuniverse-0.8.3/pyrfuniverse/envs/
+-rw-rw-rw-   0        0        0    14453 2023-04-07 06:50:32.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/__init__.py
+-rw-rw-rw-   0        0        0     4178 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/balance_ball_env.py
+-rw-rw-rw-   0        0        0    24331 2023-04-12 12:00:38.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/base_env.py
+-rw-rw-rw-   0        0        0     4564 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/bouncer_env.py
+-rw-rw-rw-   0        0        0     3982 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/franka_grasp_env.py
+-rw-rw-rw-   0        0        0     3077 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/franka_push_env.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.068341 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/
+-rw-rw-rw-   0        0        0      736 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/__init__.py
+-rw-rw-rw-   0        0        0     4209 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/nail_can_env.py
+-rw-rw-rw-   0        0        0     5750 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/nail_card_env.py
+-rw-rw-rw-   0        0        0     3917 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py
+-rw-rw-rw-   0        0        0     4149 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py
+-rw-rw-rw-   0        0        0     4220 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py
+-rw-rw-rw-   0        0        0     5917 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py
+-rw-rw-rw-   0        0        0     5696 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.081873 pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent/
+-rw-rw-rw-   0        0        0      172 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent/__init__.py
+-rw-rw-rw-   0        0        0     9111 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent/cleaner_env.py
+-rw-rw-rw-   0        0        0    11818 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent/navigation_env.py
+-rw-rw-rw-   0        0        0     6000 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent_navigation_env.py
+-rw-rw-rw-   0        0        0      513 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/rfuniverse_robot_hub_env.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.123240 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/
+-rw-rw-rw-   0        0        0      675 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/__init__.py
+-rw-rw-rw-   0        0        0     7357 2022-12-15 06:20:36.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_cloth_env.py
+-rw-rw-rw-   0        0        0     7455 2022-12-15 06:20:57.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py
+-rw-rw-rw-   0        0        0    10181 2022-12-15 08:02:41.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_robotics_env.py
+-rw-rw-rw-   0        0        0     8041 2022-12-15 06:20:52.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_softbody_env.py
+-rw-rw-rw-   0        0        0      817 2022-12-15 05:37:19.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/pick_and_place_env.py
+-rw-rw-rw-   0        0        0      754 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/push_env.py
+-rw-rw-rw-   0        0        0      864 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/reach_env.py
+-rw-rw-rw-   0        0        0     4463 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/roller_env.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.132265 pyrfuniverse-0.8.3/pyrfuniverse/envs/tobor_robotics/
+-rw-rw-rw-   0        0        0      121 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/tobor_robotics/__init__.py
+-rw-rw-rw-   0        0        0    10897 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py
+-rw-rw-rw-   0        0        0     9736 2023-02-15 08:33:33.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py
+-rw-rw-rw-   0        0        0     8205 2022-11-02 03:34:57.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/ur5_box_env.py
+-rw-rw-rw-   0        0        0     8549 2022-11-02 03:34:57.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/ur5_drawer_env.py
+-rw-rw-rw-   0        0        0     1621 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/exception.py
+-rw-rw-rw-   0        0        0     1866 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/logging_util.py
+-rw-rw-rw-   0        0        0     3924 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/mock_communicator.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.161918 pyrfuniverse-0.8.3/pyrfuniverse/registry/
+-rw-rw-rw-   0        0        0      114 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/registry/__init__.py
+-rw-rw-rw-   0        0        0     1855 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/registry/base_registry_entry.py
+-rw-rw-rw-   0        0        0     8085 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/registry/binary_utils.py
+-rw-rw-rw-   0        0        0     3256 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/registry/remote_registry_entry.py
+-rw-rw-rw-   0        0        0     5017 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/registry/unity_env_registry.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.192601 pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/
+-rw-rw-rw-   0        0        0      496 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/__init__.py
+-rw-rw-rw-   0        0        0    10343 2023-04-07 06:50:42.000000 pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/asset_channel.py
+-rw-rw-rw-   0        0        0     1248 2023-03-15 04:59:29.000000 pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/asset_channel_ext.py
+-rw-rw-rw-   0        0        0     1738 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/debug_channel.py
+-rw-rw-rw-   0        0        0     2244 2023-04-06 04:49:14.000000 pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/instance_channel.py
+-rw-rw-rw-   0        0        0     2198 2022-08-25 10:50:54.000000 pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/rfuniverse_channel.py
+-rw-rw-rw-   0        0        0     6426 2022-09-28 07:41:12.000000 pyrfuniverse-0.8.3/pyrfuniverse/rpc_communicator.py
+-rw-rw-rw-   0        0        0    16840 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.3/pyrfuniverse/rpc_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.239722 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/
+-rw-rw-rw-   0        0        0      230 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/__init__.py
+-rw-rw-rw-   0        0        0     4935 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/engine_configuration_channel.py
+-rw-rw-rw-   0        0        0     3872 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/environment_parameters_channel.py
+-rw-rw-rw-   0        0        0     2226 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/float_properties_channel.py
+-rw-rw-rw-   0        0        0     3366 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/incoming_message.py
+-rw-rw-rw-   0        0        0     1960 2022-09-06 06:01:55.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/outgoing_message.py
+-rw-rw-rw-   0        0        0     1300 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/raw_bytes_channel.py
+-rw-rw-rw-   0        0        0     1502 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/side_channel.py
+-rw-rw-rw-   0        0        0     3745 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/side_channel_manager.py
+-rw-rw-rw-   0        0        0     1875 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/stats_side_channel.py
+-rw-rw-rw-   0        0        0    11684 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/timers.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.297933 pyrfuniverse-0.8.3/pyrfuniverse/utils/
+-rw-rw-rw-   0        0        0      181 2022-10-31 06:20:22.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/__init__.py
+-rw-rw-rw-   0        0        0    13620 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/active_depth_generate.py
+-rw-rw-rw-   0        0        0     6006 2022-07-13 10:31:45.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/controller.py
+-rw-rw-rw-   0        0        0    10354 2023-02-10 17:44:40.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/depth_processor.py
+-rw-rw-rw-   0        0        0     3218 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/interpolate_utils.py
+-rw-rw-rw-   0        0        0     4304 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/jaco_controller.py
+-rw-rw-rw-   0        0        0     4908 2022-10-27 03:27:48.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/kinova_controller.py
+-rw-rw-rw-   0        0        0      755 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/os_utils.py
+-rw-rw-rw-   0        0        0     2656 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/rfuniverse_utility.py
+-rw-rw-rw-   0        0        0     5690 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/stretch_controller.py
+-rw-rw-rw-   0        0        0     6776 2022-08-15 11:02:54.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/tobor_controller.py
+-rw-rw-rw-   0        0        0     4783 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/ur5_controller.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:56:59.670053 pyrfuniverse-0.8.3/pyrfuniverse.egg-info/
+-rw-rw-rw-   0        0        0      269 2023-04-13 03:56:59.000000 pyrfuniverse-0.8.3/pyrfuniverse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6086 2023-04-13 03:56:59.000000 pyrfuniverse-0.8.3/pyrfuniverse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 03:56:59.000000 pyrfuniverse-0.8.3/pyrfuniverse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2022-10-31 04:29:22.000000 pyrfuniverse-0.8.3/pyrfuniverse.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      120 2023-04-13 03:56:59.000000 pyrfuniverse-0.8.3/pyrfuniverse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 03:56:59.000000 pyrfuniverse-0.8.3/pyrfuniverse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 03:57:00.412731 pyrfuniverse-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-04-07 06:52:00.000000 pyrfuniverse-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.411729 pyrfuniverse-0.8.3/test/
+-rw-rw-rw-   0        0        0     5651 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_active_depth.py
+-rw-rw-rw-   0        0        0      995 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_articulation_ik.py
+-rw-rw-rw-   0        0        0      766 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_camera_image.py
+-rw-rw-rw-   0        0        0     1197 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_custom_message.py
+-rw-rw-rw-   0        0        0     1038 2023-04-06 04:49:14.000000 pyrfuniverse-0.8.3/test/test_debug.py
+-rw-rw-rw-   0        0        0      439 2023-04-07 05:04:11.000000 pyrfuniverse-0.8.3/test/test_digit.py
+-rw-rw-rw-   0        0        0      827 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_grasp_pose.py
+-rw-rw-rw-   0        0        0     2758 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_grasp_sim.py
+-rw-rw-rw-   0        0        0      989 2023-04-10 09:39:27.000000 pyrfuniverse-0.8.3/test/test_heat_map.py
+-rw-rw-rw-   0        0        0     1426 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_humanbody_ik.py
+-rw-rw-rw-   0        0        0     1996 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_label.py
+-rw-rw-rw-   0        0        0      702 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_light.py
+-rw-rw-rw-   0        0        0      589 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_load_mesh.py
+-rw-rw-rw-   0        0        0     1010 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_load_urdf.py
+-rw-rw-rw-   0        0        0     1137 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_object_data.py
+-rw-rw-rw-   0        0        0     2149 2023-03-15 04:00:24.000000 pyrfuniverse-0.8.3/test/test_pick_and_place.py
+-rw-rw-rw-   0        0        0     2174 2023-03-15 04:05:23.000000 pyrfuniverse-0.8.3/test/test_pick_and_place_flexiv.py
+-rw-rw-rw-   0        0        0      570 2022-12-18 09:24:39.000000 pyrfuniverse-0.8.3/test/test_pick_and_place_gym.py
+-rw-rw-rw-   0        0        0     1746 2023-03-15 04:45:24.000000 pyrfuniverse-0.8.3/test/test_point_cloud.py
+-rw-rw-rw-   0        0        0      441 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_point_cloud_render.py
+-rw-rw-rw-   0        0        0     1891 2023-03-15 04:50:29.000000 pyrfuniverse-0.8.3/test/test_point_cloud_with_intrinsic_matrix.py
+-rw-rw-rw-   0        0        0      659 2023-04-13 02:37:33.000000 pyrfuniverse-0.8.3/test/test_save_gripper.py
+-rw-rw-rw-   0        0        0      380 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_save_obj.py
+-rw-rw-rw-   0        0        0     1024 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_scene.py
+-rw-rw-rw-   0        0        0      740 2023-04-07 07:58:17.000000 pyrfuniverse-0.8.3/test/test_tobor_move.py
```

### Comparing `pyrfuniverse-0.8.2.1/LICENSE` & `pyrfuniverse-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/README.md` & `pyrfuniverse-0.8.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # pyrfuniverse
 
 [![Pypi](https://img.shields.io/pypi/v/pyrfuniverse.svg)](https://pypi.org/project/pyrfuniverse/)
 
 `pyrfuniverse` is a python package used to interact with `RFUniverse` simulation environment. It is developed upon
 [ML-Agents](https://github.com/Unity-Technologies/ml-agents) and produce new features.
 
+[Documentation](https://knotty-watch-cad.notion.site/RFUniverse-3afda956497b4c33b5a45f68b49d9816)：It is currently mostly in Chinese, we are working on finishing it and translating to English.
+
 **Note:** current branch is under development.
 
 ## Installation
 
 ### 1. Create a new conda virtual environment and activate it.
 
 ```shell
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/__init__.py` & `pyrfuniverse-0.8.3/pyrfuniverse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Version of the library that will be used to upload to pypi
-__version__ = "0.8.2.1"
+__version__ = "0.8.3"
 
 import os.path
 import json
 
 def read_config():
     if not os.path.exists(config_path):
         config = {}
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/__init__.py` & `pyrfuniverse-0.8.3/pyrfuniverse/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/activelightsensor_attr.py` & `pyrfuniverse-0.8.3/pyrfuniverse/attributes/activelightsensor_attr.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import base64
-import cv2
-import numpy as np
-import pyrfuniverse.attributes as attr
-import pyrfuniverse.utils.active_depth_generate as active_depth
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
-
-
-class ActiveLightSensorAttr(attr.CameraAttr):
-    """
-    红外深度传感器类，能够获取模拟真实深度相机噪声的深度图
-    """
-    def __init__(self, env, id: int, data=None):
-        super().__init__(env, id, data)
-        self.main_intrinsic_matrix = np.eye(4)
-        self.ir_intrinsic_matrix = np.eye(4)
-
-    def parse_message(self, msg: IncomingMessage) -> dict:
-        """
-        解析消息
-
-        Returns:
-            self.data['active_depth'] 红外深度图，shape = [w,h]
-        """
-        super().parse_message(msg)
-        if msg.read_bool() is True:
-            self.data['ir_left'] = base64.b64decode(msg.read_string())
-            self.data['ir_right'] = base64.b64decode(msg.read_string())
-
-            image_left = np.frombuffer(self.data['ir_left'], dtype=np.uint8)
-            image_left = cv2.imdecode(image_left, cv2.IMREAD_COLOR)[..., 2]
-            image_right = np.frombuffer(self.data['ir_right'], dtype=np.uint8)
-            image_right = cv2.imdecode(image_right, cv2.IMREAD_COLOR)[..., 2]
-            left_extrinsic_matrix = np.array(
-                [[0., -1., 0., -0.0175], [0., 0., -1., 0.], [1., 0., 0., 0.], [0., 0., 0., 1.]])
-            right_extrinsic_matrix = np.array(
-                [[0., -1., 0., -0.072], [0., 0., -1., 0.], [1., 0., 0., 0.], [0., 0., 0., 1.]])
-            main_extrinsic_matrix = np.array([[0., -1., 0., 0.], [0., 0., -1., 0.], [1., 0., 0., 0.], [0., 0., 0., 1.]])
-            self.data['active_depth'] = active_depth.calc_main_depth_from_left_right_ir(image_left, image_right,
-                                                                                        left_extrinsic_matrix,
-                                                                                        right_extrinsic_matrix,
-                                                                                        main_extrinsic_matrix,
-                                                                                        self.ir_intrinsic_matrix,
-                                                                                        self.ir_intrinsic_matrix,
-                                                                                        self.main_intrinsic_matrix,
-                                                                                        lr_consistency=False,
-                                                                                        main_cam_size=(
-                                                                                            self.main_intrinsic_matrix[
-                                                                                                0, 2] * 2,
-                                                                                            self.main_intrinsic_matrix[
-                                                                                                1, 2] * 2),
-                                                                                        ndisp=128,
-                                                                                        use_census=True,
-                                                                                        register_depth=True,
-                                                                                        census_wsize=7,
-                                                                                        use_noise=False)
-            self.data['active_depth'][self.data['active_depth'] > 8.] = 0
-            self.data['active_depth'][self.data['active_depth'] < 0.1] = 0
-        return self.data
-
-    def GetActiveDepth(self, main_intrinsic_matrix_local: list, ir_intrinsic_matrix_local: list):
-        """
-        获取红外深度图
-
-        Args:
-            main_intrinsic_matrix_local: List[float]主相机内参
-            ir_intrinsic_matrix_local: List[float]红外相机内参
-
-        Returns:
-            调用此接口并step后，从self.data['active_depth']获取结果
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('GetActiveDepth')
-        self.main_intrinsic_matrix = np.reshape(main_intrinsic_matrix_local, [3, 3]).T
-        self.ir_intrinsic_matrix = np.reshape(ir_intrinsic_matrix_local, [3, 3]).T
-        msg.write_float32_list(self.ir_intrinsic_matrix.T.reshape([-1]).tolist())
-
-        self.env.instance_channel.send_message(msg)
+import base64
+import cv2
+import numpy as np
+import pyrfuniverse.attributes as attr
+import pyrfuniverse.utils.active_depth_generate as active_depth
+from pyrfuniverse.side_channel.side_channel import (
+    IncomingMessage,
+    OutgoingMessage,
+)
+
+
+class ActiveLightSensorAttr(attr.CameraAttr):
+    """
+    红外深度传感器类，能够获取模拟真实深度相机噪声的深度图
+    """
+    def __init__(self, env, id: int, data=None):
+        super().__init__(env, id, data)
+        self.main_intrinsic_matrix = np.eye(4)
+        self.ir_intrinsic_matrix = np.eye(4)
+
+    def parse_message(self, msg: IncomingMessage) -> dict:
+        """
+        解析消息
+
+        Returns:
+            self.data['active_depth'] 红外深度图，shape = [w,h]
+        """
+        super().parse_message(msg)
+        if msg.read_bool() is True:
+            self.data['ir_left'] = base64.b64decode(msg.read_string())
+            self.data['ir_right'] = base64.b64decode(msg.read_string())
+
+            image_left = np.frombuffer(self.data['ir_left'], dtype=np.uint8)
+            image_left = cv2.imdecode(image_left, cv2.IMREAD_COLOR)[..., 2]
+            image_right = np.frombuffer(self.data['ir_right'], dtype=np.uint8)
+            image_right = cv2.imdecode(image_right, cv2.IMREAD_COLOR)[..., 2]
+            left_extrinsic_matrix = np.array(
+                [[0., -1., 0., -0.0175], [0., 0., -1., 0.], [1., 0., 0., 0.], [0., 0., 0., 1.]])
+            right_extrinsic_matrix = np.array(
+                [[0., -1., 0., -0.072], [0., 0., -1., 0.], [1., 0., 0., 0.], [0., 0., 0., 1.]])
+            main_extrinsic_matrix = np.array([[0., -1., 0., 0.], [0., 0., -1., 0.], [1., 0., 0., 0.], [0., 0., 0., 1.]])
+            self.data['active_depth'] = active_depth.calc_main_depth_from_left_right_ir(image_left, image_right,
+                                                                                        left_extrinsic_matrix,
+                                                                                        right_extrinsic_matrix,
+                                                                                        main_extrinsic_matrix,
+                                                                                        self.ir_intrinsic_matrix,
+                                                                                        self.ir_intrinsic_matrix,
+                                                                                        self.main_intrinsic_matrix,
+                                                                                        lr_consistency=False,
+                                                                                        main_cam_size=(
+                                                                                            self.main_intrinsic_matrix[
+                                                                                                0, 2] * 2,
+                                                                                            self.main_intrinsic_matrix[
+                                                                                                1, 2] * 2),
+                                                                                        ndisp=128,
+                                                                                        use_census=True,
+                                                                                        register_depth=True,
+                                                                                        census_wsize=7,
+                                                                                        use_noise=False)
+            self.data['active_depth'][self.data['active_depth'] > 8.] = 0
+            self.data['active_depth'][self.data['active_depth'] < 0.1] = 0
+        return self.data
+
+    def GetActiveDepth(self, main_intrinsic_matrix_local: list, ir_intrinsic_matrix_local: list):
+        """
+        获取红外深度图
+
+        Args:
+            main_intrinsic_matrix_local: List[float]主相机内参
+            ir_intrinsic_matrix_local: List[float]红外相机内参
+
+        Returns:
+            调用此接口并step后，从self.data['active_depth']获取结果
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('GetActiveDepth')
+        self.main_intrinsic_matrix = np.reshape(main_intrinsic_matrix_local, [3, 3]).T
+        self.ir_intrinsic_matrix = np.reshape(ir_intrinsic_matrix_local, [3, 3]).T
+        msg.write_float32_list(self.ir_intrinsic_matrix.T.reshape([-1]).tolist())
+
+        self.env.instance_channel.send_message(msg)
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/base_attr.py` & `pyrfuniverse-0.8.3/pyrfuniverse/attributes/base_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/collider_attr.py` & `pyrfuniverse-0.8.3/pyrfuniverse/attributes/collider_attr.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import pyrfuniverse.attributes as attr
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
-import pyrfuniverse.utils.rfuniverse_utility as utility
-
-
-def GenerateVHACDColider(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('GenerateVHACDColider')
-    return msg
-
-
-class ColliderAttr(attr.GameObjectAttr):
-    """
-    具有碰撞体的物体类
-    """
-    def parse_message(self, msg: IncomingMessage) -> dict:
-        """
-        解析消息
-
-        Returns:
-
-        """
-        super().parse_message(msg)
-        return self.data
-
-    def GenerateVHACDColider(self):
-        """
-        使用VHACD算法生成物体碰撞体
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('GenerateVHACDColider')
-
+import pyrfuniverse.attributes as attr
+from pyrfuniverse.side_channel.side_channel import (
+    IncomingMessage,
+    OutgoingMessage,
+)
+import pyrfuniverse.utils.rfuniverse_utility as utility
+
+
+def GenerateVHACDColider(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('GenerateVHACDColider')
+    return msg
+
+
+class ColliderAttr(attr.GameObjectAttr):
+    """
+    具有碰撞体的物体类
+    """
+    def parse_message(self, msg: IncomingMessage) -> dict:
+        """
+        解析消息
+
+        Returns:
+
+        """
+        super().parse_message(msg)
+        return self.data
+
+    def GenerateVHACDColider(self):
+        """
+        使用VHACD算法生成物体碰撞体
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('GenerateVHACDColider')
+
         self.env.instance_channel.send_message(msg)
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/controller_attr.py` & `pyrfuniverse-0.8.3/pyrfuniverse/attributes/controller_attr.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,971 +1,971 @@
-import numpy as np
-
-import pyrfuniverse.attributes as attr
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
-import pyrfuniverse.utils.rfuniverse_utility as utility
-
-
-
-def SetJointPosition(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'joint_positions']
-    optional_params = ['speed_scales']
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    joint_positions = kwargs['joint_positions']
-    num_joints = len(joint_positions)
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('SetJointPosition')
-    msg.write_float32_list(kwargs['joint_positions'])
-    if 'speed_scales' in kwargs.keys():
-        assert num_joints == len(kwargs['speed_scales']), \
-            'The length of joint_positions and speed_scales are not equal.'
-        msg.write_float32_list(kwargs['speed_scales'])
-    else:
-        msg.write_float32_list([1.0 for i in range(num_joints)])
-
-    return msg
-
-
-def SetJointPositionDirectly(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'joint_positions']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    joint_positions = kwargs['joint_positions']
-    num_joints = len(joint_positions)
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('SetJointPositionDirectly')
-    msg.write_float32_list(kwargs['joint_positions'])
-
-    return msg
-
-def SetIndexJointPosition(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'index','joint_position']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('SetIndexJointPosition')
-    msg.write_int32(kwargs['index'])
-    msg.write_float32(kwargs['joint_position'])
-
-    return msg
-
-def SetIndexJointPositionDirectly(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'index','joint_position']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('SetIndexJointPositionDirectly')
-    msg.write_int32(kwargs['index'])
-    msg.write_float32(kwargs['joint_position'])
-
-    return msg
-
-def SetJointPositionContinue(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'interval', 'time_joint_positions']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-
-    time_joint_positions = kwargs['time_joint_positions']
-    num_times = len(time_joint_positions)
-    # num_joints = len(time_joint_positions[0])
-    interval = kwargs['interval']
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('SetJointPositionContinue')
-    msg.write_int32(num_times)
-    # msg.write_int32(num_joints)
-    msg.write_int32(interval)
-    for i in range(num_times):
-        msg.write_float32_list(time_joint_positions[i])
-
-    return msg
-
-
-def SetJointVelocity(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'joint_velocitys']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    joint_velocitys = kwargs['joint_velocitys']
-    num_joints = len(joint_velocitys)
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('SetJointVelocity')
-    msg.write_float32_list(kwargs['joint_velocitys'])
-
-    return msg
-
-
-def SetIndexJointVelocity(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'index', 'joint_velocity']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('SetIndexJointVelocity')
-    msg.write_int32(kwargs['index'])
-    msg.write_float32(kwargs['joint_velocity'])
-
-    self.env.instance_channel.send_message(msg)
-
-def AddJointForce(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'joint_forces']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    joint_positions = kwargs['joint_positions']
-    num_joints = len(joint_positions)
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('AddJointForce')
-    msg.write_int32(num_joints)
-    for i in range(num_joints):
-        msg.write_float32(joint_positions[i][0])
-        msg.write_float32(joint_positions[i][1])
-        msg.write_float32(joint_positions[i][2])
-
-    return msg
-
-
-def AddJointForceAtPosition(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'joint_forces', 'forces_position']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    joint_positions = kwargs['joint_forces']
-    forces_position = kwargs['forces_position']
-    num_joints = len(joint_positions)
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('AddJointForceAtPosition')
-    msg.write_int32(num_joints)
-    for i in range(num_joints):
-        msg.write_float32(joint_positions[i][0])
-        msg.write_float32(joint_positions[i][1])
-        msg.write_float32(joint_positions[i][2])
-        msg.write_float32(forces_position[i][0])
-        msg.write_float32(forces_position[i][1])
-        msg.write_float32(forces_position[i][2])
-
-    return msg
-
-
-def AddJointTorque(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'joint_torque']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    joint_torque = kwargs['joint_torque']
-    num_joints = len(joint_torque)
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('AddJointTorque')
-    msg.write_int32(num_joints)
-    for i in range(num_joints):
-        msg.write_float32(joint_torque[i][0])
-        msg.write_float32(joint_torque[i][1])
-        msg.write_float32(joint_torque[i][2])
-
-    return msg
-
-
-# only work on unity 2022.1+
-def GetJointInverseDynamicsForce(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('GetJointInverseDynamicsForce')
-    return msg
-
-
-def SetImmovable(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'immovable']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('SetImmovable')
-    msg.write_bool(kwargs['immovable'])
-    return msg
-
-
-def MoveForward(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'distance', 'speed']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('MoveForward')
-    msg.write_float32(kwargs['distance'])
-    msg.write_float32(kwargs['speed'])
-    return msg
-
-
-def MoveBack(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'distance', 'speed']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('MoveBack')
-    msg.write_float32(kwargs['distance'])
-    msg.write_float32(kwargs['speed'])
-    return msg
-
-
-def TurnLeft(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'angle', 'speed']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('TurnLeft')
-    msg.write_float32(kwargs['angle'])
-    msg.write_float32(kwargs['speed'])
-    return msg
-
-
-def TurnRight(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'angle', 'speed']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('TurnRight')
-    msg.write_float32(kwargs['angle'])
-    msg.write_float32(kwargs['speed'])
-    return msg
-
-def GripperOpen(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('GripperOpen')
-    return msg
-
-def GripperClose(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('GripperClose')
-    return msg
-
-
-def EnabledNativeIK(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'enabled']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('EnabledNativeIK')
-    msg.write_bool(kwargs['enabled'])
-    return msg
-
-
-def IKTargetDoMove(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'position', 'duration']
-    optional_params = ['speed_based', 'relative']
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    if 'speed_based' not in kwargs:
-        kwargs['speed_based'] = True
-    if 'relative' not in kwargs:
-        kwargs['relative'] = False
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('IKTargetDoMove')
-    msg.write_float32(kwargs['position'][0])
-    msg.write_float32(kwargs['position'][1])
-    msg.write_float32(kwargs['position'][2])
-    msg.write_float32(kwargs['duration'])
-    msg.write_bool(kwargs['speed_based'])
-    msg.write_bool(kwargs['relative'])
-    return msg
-
-def IKTargetDoRotate(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'vector3', 'duration']
-    optional_params = ['speed_based', 'relative']
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    if 'speed_based' not in kwargs:
-        kwargs['speed_based'] = True
-    if 'relative' not in kwargs:
-        kwargs['relative'] = False
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('IKTargetDoRotate')
-    msg.write_float32(kwargs['vector3'][0])
-    msg.write_float32(kwargs['vector3'][1])
-    msg.write_float32(kwargs['vector3'][2])
-    msg.write_float32(kwargs['duration'])
-    msg.write_bool(kwargs['speed_based'])
-    msg.write_bool(kwargs['relative'])
-    return msg
-
-def IKTargetDoRotateQuaternion(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'quaternion', 'duration']
-    optional_params = ['speed_based', 'relative']
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    if 'speed_based' not in kwargs:
-        kwargs['speed_based'] = True
-    if 'relative' not in kwargs:
-        kwargs['relative'] = False
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('IKTargetDoRotateQuaternion')
-    msg.write_float32(kwargs['quaternion'][0])
-    msg.write_float32(kwargs['quaternion'][1])
-    msg.write_float32(kwargs['quaternion'][2])
-    msg.write_float32(kwargs['quaternion'][3])
-    msg.write_float32(kwargs['duration'])
-    msg.write_bool(kwargs['speed_based'])
-    msg.write_bool(kwargs['relative'])
-    return msg
-
-
-def IKTargetDoComplete(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('IKTargetDoComplete')
-    return msg
-
-
-def IKTargetDoKill(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('IKTargetDoKill')
-    return msg
-
-def SetIKTargetOffset(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id']
-    optional_params = ['position', 'rotation', 'is_quaternion']
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    if 'position' not in kwargs:
-        kwargs['position'] = [0,0,0]
-    if 'rotation' not in kwargs:
-        kwargs['rotation'] = [0,0,0,0]
-    if 'is_quaternion' not in kwargs:
-        kwargs['is_quaternion'] = False
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('SetIKTargetOffset')
-    msg.write_float32(kwargs['position'][0])
-    msg.write_float32(kwargs['position'][1])
-    msg.write_float32(kwargs['position'][2])
-    msg.write_bool(kwargs['is_quaternion'])
-    if kwargs['is_quaternion']:
-        msg.write_float32(kwargs['rotation'][0])
-        msg.write_float32(kwargs['rotation'][1])
-        msg.write_float32(kwargs['rotation'][2])
-        msg.write_float32(kwargs['rotation'][2])
-    else:
-        msg.write_float32(kwargs['rotation'][0])
-        msg.write_float32(kwargs['rotation'][1])
-        msg.write_float32(kwargs['rotation'][2])
-    return msg
-
-
-class ControllerAttr(attr.ColliderAttr):
-    """
-    机械臂控制器类
-    """
-    def parse_message(self, msg: IncomingMessage) -> dict:
-        """
-        解析消息
-
-        Returns:
-            self.data['number_of_joints'] 机械臂关节数量
-
-            self.data['positions'] 机械臂节点位置
-
-            self.data['rotations'] 机械臂节点旋转角度
-
-            self.data['quaternion'] 机械臂节点旋转四元数
-
-            self.data['local_positions'] 机械臂节点局部位置
-
-            self.data['local_rotations'] 机械臂节点局部旋转角度
-
-            self.data['local_quaternion'] 机械臂节点局部旋转四元数
-
-            self.data['velocities'] 机械臂节点速度
-
-            self.data['number_of_moveable_joints'] 机械臂活动关节数量
-
-            self.data['joint_positions'] 机械臂关节在自由度空间下位置
-
-            self.data['joint_velocities'] 机械臂关节在自由度空间下速度
-
-            self.data['all_stable'] 机械臂所有关节移动完成
-
-            self.data['move_done'] 机械臂IK移动完成状态
-
-            self.data['rotate_done'] 机械臂IK旋转完成状态
-
-            self.data['gravity_forces'] InverseDynamics抵消重力所需的力
-
-            self.data['coriolis_centrifugal_forces'] InverseDynamics抵消离心力所需的力
-
-            self.data['drive_forces'] InverseDynamics驱动力
-        """
-        super().parse_message(msg)
-        self.data['number_of_joints'] = msg.read_int32()
-        # Position
-        self.data['positions'] = np.array(msg.read_float32_list()).reshape([-1, 3]).tolist()
-        # RotationEuler
-        self.data['rotations'] = np.array(msg.read_float32_list()).reshape([-1, 3]).tolist()
-        # RotationQuaternion
-        self.data['quaternion'] = np.array(msg.read_float32_list()).reshape([-1, 4]).tolist()
-        # LocalPosition
-        self.data['local_positions'] = np.array(msg.read_float32_list()).reshape([-1, 3]).tolist()
-        # LocalRotationEuler
-        self.data['local_rotations'] = np.array(msg.read_float32_list()).reshape([-1, 3]).tolist()
-        # LocalRotationQuaternion
-        self.data['local_quaternion'] = np.array(msg.read_float32_list()).reshape([-1, 4]).tolist()
-        # Velocity
-        self.data['velocities'] = np.array(msg.read_float32_list()).reshape([-1, 3]).tolist()
-        #
-        self.data['number_of_moveable_joints'] = msg.read_int32()
-        # Each joint position
-        self.data['joint_positions'] = msg.read_float32_list()
-        # Each joint velocity
-        self.data['joint_velocities'] = msg.read_float32_list()
-        # Whether all parts are stable
-        self.data['all_stable'] = msg.read_bool()
-        self.data['move_done'] = msg.read_bool()
-        self.data['rotate_done'] = msg.read_bool()
-        if msg.read_bool() is True:
-            self.data['gravity_forces'] = msg.read_float32_list()
-            self.data['coriolis_centrifugal_forces'] = msg.read_float32_list()
-            self.data['drive_forces'] = msg.read_float32_list()
-        return self.data
-
-    def SetJointPosition(self, joint_positions: list, speed_scales = None):
-        """
-        设置机械臂所有关节目标位置
-
-        Args:
-            joint_positions: 目标位置
-            speed_scales: 速度倍数
-        """
-        num_joints = len(joint_positions)
-        if speed_scales is None:
-            speed_scales = [1.0 for i in range(num_joints)]
-        assert num_joints == len(speed_scales), \
-            'The length of joint_positions and speed_scales are not equal.'
-
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetJointPosition')
-        msg.write_float32_list(joint_positions)
-        msg.write_float32_list(speed_scales)
-
-        self.env.instance_channel.send_message(msg)
-
-    def SetJointPositionDirectly(self, joint_positions: list):
-        """
-        立即设置机械臂所有关节位置
-
-        Args:
-            joint_positions: 目标位置
-        """
-        num_joints = len(joint_positions)
-
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetJointPositionDirectly')
-        msg.write_float32_list(joint_positions)
-
-        self.env.instance_channel.send_message(msg)
-
-    def SetIndexJointPosition(self, index: int, joint_position: float):
-        """
-        设置机械臂指定关节目标位置
-
-        Args:
-            index: 关节序号
-            joint_position: 目标位置
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetIndexJointPosition')
-        msg.write_int32(index)
-        msg.write_float32(joint_position)
-
-        self.env.instance_channel.send_message(msg)
-
-    def SetIndexJointPositionDirectly(self, index: int, joint_position: float):
-        """
-        立即设置机械臂指定关节位置
-
-        Args:
-            index: 关节序号
-            joint_position: 目标位置
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetIndexJointPositionDirectly')
-        msg.write_int32(index)
-        msg.write_float32(joint_position)
-
-        self.env.instance_channel.send_message(msg)
-
-    def SetJointPositionContinue(self, interval: int, time_joint_positions: list):
-        """
-        持续设置机械臂所有关节目标位置
-
-        Args:
-            interval: 设置时间间隔(毫秒)
-            time_joint_positions: 每个time的目标位置
-
-        Returns:
-
-        """
-        num_times = len(time_joint_positions)
-
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetJointPositionContinue')
-        msg.write_int32(num_times)
-        msg.write_int32(interval)
-        for i in range(num_times):
-            msg.write_float32_list(time_joint_positions[i])
-
-        self.env.instance_channel.send_message(msg)
-
-    def SetJointVelocity(self, joint_velocitys: list):
-        """
-        设置机械臂所有关节目标速度
-
-        Args:
-            joint_velocitys: 目标速度
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetJointVelocity')
-        msg.write_float32_list(joint_velocitys)
-
-        self.env.instance_channel.send_message(msg)
-
-    def SetIndexJointVelocity(self, index: int, joint_velocity: float):
-        """
-        设置机械臂指定关节目标速度
-
-        Args:
-            index: 关节序号
-            joint_velocity: 目标速度
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetIndexJointVelocity')
-        msg.write_int32(index)
-        msg.write_float32(joint_velocity)
-
-        self.env.instance_channel.send_message(msg)
-
-    def AddJointForce(self, joint_forces: list):
-        """
-        为机械臂所有关节施加力
-
-        Args:
-            joint_forces: 力
-        """
-        num_joints = len(joint_positions)
-
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('AddJointForce')
-        msg.write_int32(num_joints)
-        for i in range(num_joints):
-            msg.write_float32(joint_forces[i][0])
-            msg.write_float32(joint_forces[i][1])
-            msg.write_float32(joint_forces[i][2])
-
-        self.env.instance_channel.send_message(msg)
-
-    def AddJointForceAtPosition(self, joint_forces: list, force_positions: list):
-        """
-        为机械臂所有关节指定位置施加力
-
-        Args:
-            joint_forces: 力
-            force_positions: 施力点
-        """
-        num_joints = len(joint_positions)
-        assert len(joint_forces) == len(force_positions), \
-            'The length of joint_forces and force_positions are not equal.'
-
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('AddJointForceAtPosition')
-        msg.write_int32(num_joints)
-        for i in range(num_joints):
-            msg.write_float32(joint_forces[i][0])
-            msg.write_float32(joint_forces[i][1])
-            msg.write_float32(joint_forces[i][2])
-            msg.write_float32(force_positions[i][0])
-            msg.write_float32(force_positions[i][1])
-            msg.write_float32(force_positions[i][2])
-
-        self.env.instance_channel.send_message(msg)
-
-    def AddJointTorque(self, joint_torques: list):
-        """
-        为机械臂所有关节施加力矩
-
-        Args:
-            joint_torques: 力矩
-        """
-        num_joints = len(joint_torque)
-
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('AddJointTorque')
-        msg.write_int32(num_joints)
-        for i in range(num_joints):
-            msg.write_float32(joint_torques[i][0])
-            msg.write_float32(joint_torques[i][1])
-            msg.write_float32(joint_torques[i][2])
-
-        self.env.instance_channel.send_message(msg)
-
-    # only work on unity 2022.1+
-    def GetJointInverseDynamicsForce(self):
-        """
-        获取机械臂所有关节逆动力学数据
-
-        Returns:
-            调用此接口并step后，从
-            self.data['gravity_forces']
-            self.data['coriolis_centrifugal_forces']
-            self.data['drive_forces']
-            获取结果
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('GetJointInverseDynamicsForce')
-
-        self.env.instance_channel.send_message(msg)
-
-    def SetImmovable(self, immovable: bool):
-        """
-        设置机械臂是否不可移动
-
-        Args:
-            immovable: 是否不可移动
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetImmovable')
-        msg.write_bool(immovable)
-
-        self.env.instance_channel.send_message(msg)
-
-    def MoveForward(self, distance: float, speed: float):
-        """
-        如果机器人在Unity端添加了继承ICustomMove接口的脚本，可通过此接口驱动前进
-        最初用于Tobor机器人
-
-        Args:
-            distance:距离
-            speed:速度
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('MoveForward')
-        msg.write_float32(distance)
-        msg.write_float32(speed)
-
-        self.env.instance_channel.send_message(msg)
-
-    def MoveBack(self, distance: float, speed: float):
-        """
-        如果机器人在Unity端添加了继承ICustomMove接口的脚本，可通过此接口驱动后退
-        最初用于Tobor机器人
-
-        Args:
-            distance:距离
-            speed:速度
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('MoveBack')
-        msg.write_float32(distance)
-        msg.write_float32(speed)
-
-        self.env.instance_channel.send_message(msg)
-
-    def TurnLeft(self, angle: float, speed: float):
-        """
-        如果机器人在Unity端添加了继承ICustomMove接口的脚本，可通过此接口驱动左转
-        最初用于Tobor机器人
-
-        Args:
-            angle:角度
-            speed:速度
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('TurnLeft')
-        msg.write_float32(angle)
-        msg.write_float32(speed)
-
-        self.env.instance_channel.send_message(msg)
-
-    def TurnRight(self, angle: float, speed: float):
-        """
-        如果机器人在Unity端添加了继承ICustomMove接口的脚本，可通过此接口驱动右转
-        最初用于Tobor机器人
-
-        Args:
-            angle:角度
-            speed:速度
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('TurnRight')
-        msg.write_float32(angle)
-        msg.write_float32(speed)
-
-        self.env.instance_channel.send_message(msg)
-
-    def GripperOpen(self):
-        """
-        如果夹爪在Unity端添加了继承ICustomGripper接口的脚本，可通过此接口驱动张开
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('GripperOpen')
-
-        self.env.instance_channel.send_message(msg)
-
-    def GripperClose(self):
-        """
-        如果夹爪在Unity端添加了继承ICustomGripper接口的脚本，可通过此接口驱动闭合
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('GripperClose')
-
-        self.env.instance_channel.send_message(msg)
-
-    def EnabledNativeIK(self, enabled: bool):
-        """
-        启用/禁用机械臂的原生IK
-
-        Args:
-            enabled: 启用/禁用
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('EnabledNativeIK')
-        msg.write_bool(enabled)
-
-        self.env.instance_channel.send_message(msg)
-
-    def IKTargetDoMove(self, position: list, duration: float, speed_based: bool = True, relative: bool = False):
-        """
-        原生IK末端点移动
-
-        Args:
-            position: 绝对位置或相对位置
-            duration: 移动持续时间或移动速度
-            speed_based: 指定duration表示移动持续时间还是移动速度
-            relative: 指定position表示绝对位置还是相对位置
-
-        Returns:
-            当移动完成时，self.data['move_done']会被置为True
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('IKTargetDoMove')
-        msg.write_float32(position[0])
-        msg.write_float32(position[1])
-        msg.write_float32(position[2])
-        msg.write_float32(duration)
-        msg.write_bool(speed_based)
-        msg.write_bool(relative)
-
-        self.env.instance_channel.send_message(msg)
-
-    def IKTargetDoRotate(self, rotation: list, duration: float, speed_based: bool = True, relative: bool = False):
-        """
-        原生IK末端点Vector3旋转
-
-        Args:
-            rotation: 绝对旋转或相对旋转
-            duration: 旋转持续时间或旋转速度
-            speed_based: 指定duration表示旋转持续时间还是旋转速度
-            relative: 指定position表示绝对旋转还是相对旋转
-
-        Returns:
-            当旋转完成时，self.data['rotate_done']会被置为True
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('IKTargetDoRotate')
-        msg.write_float32(rotation[0])
-        msg.write_float32(rotation[1])
-        msg.write_float32(rotation[2])
-        msg.write_float32(duration)
-        msg.write_bool(speed_based)
-        msg.write_bool(relative)
-
-        self.env.instance_channel.send_message(msg)
-
-    def IKTargetDoRotateQuaternion(self, quaternion: list, duration: float, speed_based: bool = True, relative: bool = False):
-        """
-        原生IK末端点四元数旋转
-
-        Args:
-            quaternion: 绝对旋转或相对旋转
-            duration: 旋转持续时间或旋转速度
-            speed_based: 指定duration表示旋转持续时间还是旋转速度
-            relative: 指定position表示绝对旋转还是相对旋转
-
-        Returns:
-            当旋转完成时，self.data['rotate_done']会被置为True
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('IKTargetDoRotateQuaternion')
-        msg.write_float32(quaternion[0])
-        msg.write_float32(quaternion[1])
-        msg.write_float32(quaternion[2])
-        msg.write_float32(quaternion[3])
-        msg.write_float32(duration)
-        msg.write_bool(speed_based)
-        msg.write_bool(relative)
-
-        self.env.instance_channel.send_message(msg)
-
-    def IKTargetDoComplete(self):
-        """
-        使原生IK末端点移动/旋转立即完成
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('IKTargetDoComplete')
-
-        self.env.instance_channel.send_message(msg)
-
-    def IKTargetDoKill(self):
-        """
-        使原生IK末端点移动/旋转停止
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('IKTargetDoKill')
-
-        self.env.instance_channel.send_message(msg)
-
-    def SetIKTargetOffset(self, position: list = [0.,0.,0.], rotation: list = [0.,0.,0.], quaternion: list = None):
-        """
-        设置原生IK末端点的偏移
-
-        Args:
-            position: 偏移位置
-            rotation: 偏移旋转Vector3
-            quaternion: 偏移旋转四元数，此值覆盖rotation
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetIKTargetOffset')
-        msg.write_float32(position[0])
-        msg.write_float32(position[1])
-        msg.write_float32(position[2])
-        msg.write_bool(quaternion is not None)
-        if quaternion is not None:
-            msg.write_float32(quaternion[0])
-            msg.write_float32(quaternion[1])
-            msg.write_float32(quaternion[2])
-            msg.write_float32(quaternion[2])
-        else:
-            msg.write_float32(rotation[0])
-            msg.write_float32(rotation[1])
-            msg.write_float32(rotation[2])
-
-        self.env.instance_channel.send_message(msg)
-
-    def WaitDo(self):
-        """
-        等待原生IK末端点移动/旋转完成
-        """
-        while not self.data['move_done'] or not self.data['rotate_done']:
+import numpy as np
+
+import pyrfuniverse.attributes as attr
+from pyrfuniverse.side_channel.side_channel import (
+    IncomingMessage,
+    OutgoingMessage,
+)
+import pyrfuniverse.utils.rfuniverse_utility as utility
+
+
+
+def SetJointPosition(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'joint_positions']
+    optional_params = ['speed_scales']
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    joint_positions = kwargs['joint_positions']
+    num_joints = len(joint_positions)
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('SetJointPosition')
+    msg.write_float32_list(kwargs['joint_positions'])
+    if 'speed_scales' in kwargs.keys():
+        assert num_joints == len(kwargs['speed_scales']), \
+            'The length of joint_positions and speed_scales are not equal.'
+        msg.write_float32_list(kwargs['speed_scales'])
+    else:
+        msg.write_float32_list([1.0 for i in range(num_joints)])
+
+    return msg
+
+
+def SetJointPositionDirectly(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'joint_positions']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    joint_positions = kwargs['joint_positions']
+    num_joints = len(joint_positions)
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('SetJointPositionDirectly')
+    msg.write_float32_list(kwargs['joint_positions'])
+
+    return msg
+
+def SetIndexJointPosition(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'index','joint_position']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('SetIndexJointPosition')
+    msg.write_int32(kwargs['index'])
+    msg.write_float32(kwargs['joint_position'])
+
+    return msg
+
+def SetIndexJointPositionDirectly(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'index','joint_position']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('SetIndexJointPositionDirectly')
+    msg.write_int32(kwargs['index'])
+    msg.write_float32(kwargs['joint_position'])
+
+    return msg
+
+def SetJointPositionContinue(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'interval', 'time_joint_positions']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+
+    time_joint_positions = kwargs['time_joint_positions']
+    num_times = len(time_joint_positions)
+    # num_joints = len(time_joint_positions[0])
+    interval = kwargs['interval']
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('SetJointPositionContinue')
+    msg.write_int32(num_times)
+    # msg.write_int32(num_joints)
+    msg.write_int32(interval)
+    for i in range(num_times):
+        msg.write_float32_list(time_joint_positions[i])
+
+    return msg
+
+
+def SetJointVelocity(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'joint_velocitys']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    joint_velocitys = kwargs['joint_velocitys']
+    num_joints = len(joint_velocitys)
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('SetJointVelocity')
+    msg.write_float32_list(kwargs['joint_velocitys'])
+
+    return msg
+
+
+def SetIndexJointVelocity(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'index', 'joint_velocity']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('SetIndexJointVelocity')
+    msg.write_int32(kwargs['index'])
+    msg.write_float32(kwargs['joint_velocity'])
+
+    self.env.instance_channel.send_message(msg)
+
+def AddJointForce(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'joint_forces']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    joint_positions = kwargs['joint_positions']
+    num_joints = len(joint_positions)
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('AddJointForce')
+    msg.write_int32(num_joints)
+    for i in range(num_joints):
+        msg.write_float32(joint_positions[i][0])
+        msg.write_float32(joint_positions[i][1])
+        msg.write_float32(joint_positions[i][2])
+
+    return msg
+
+
+def AddJointForceAtPosition(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'joint_forces', 'forces_position']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    joint_positions = kwargs['joint_forces']
+    forces_position = kwargs['forces_position']
+    num_joints = len(joint_positions)
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('AddJointForceAtPosition')
+    msg.write_int32(num_joints)
+    for i in range(num_joints):
+        msg.write_float32(joint_positions[i][0])
+        msg.write_float32(joint_positions[i][1])
+        msg.write_float32(joint_positions[i][2])
+        msg.write_float32(forces_position[i][0])
+        msg.write_float32(forces_position[i][1])
+        msg.write_float32(forces_position[i][2])
+
+    return msg
+
+
+def AddJointTorque(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'joint_torque']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    joint_torque = kwargs['joint_torque']
+    num_joints = len(joint_torque)
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('AddJointTorque')
+    msg.write_int32(num_joints)
+    for i in range(num_joints):
+        msg.write_float32(joint_torque[i][0])
+        msg.write_float32(joint_torque[i][1])
+        msg.write_float32(joint_torque[i][2])
+
+    return msg
+
+
+# only work on unity 2022.1+
+def GetJointInverseDynamicsForce(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('GetJointInverseDynamicsForce')
+    return msg
+
+
+def SetImmovable(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'immovable']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('SetImmovable')
+    msg.write_bool(kwargs['immovable'])
+    return msg
+
+
+def MoveForward(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'distance', 'speed']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('MoveForward')
+    msg.write_float32(kwargs['distance'])
+    msg.write_float32(kwargs['speed'])
+    return msg
+
+
+def MoveBack(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'distance', 'speed']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('MoveBack')
+    msg.write_float32(kwargs['distance'])
+    msg.write_float32(kwargs['speed'])
+    return msg
+
+
+def TurnLeft(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'angle', 'speed']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('TurnLeft')
+    msg.write_float32(kwargs['angle'])
+    msg.write_float32(kwargs['speed'])
+    return msg
+
+
+def TurnRight(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'angle', 'speed']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('TurnRight')
+    msg.write_float32(kwargs['angle'])
+    msg.write_float32(kwargs['speed'])
+    return msg
+
+def GripperOpen(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('GripperOpen')
+    return msg
+
+def GripperClose(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('GripperClose')
+    return msg
+
+
+def EnabledNativeIK(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'enabled']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('EnabledNativeIK')
+    msg.write_bool(kwargs['enabled'])
+    return msg
+
+
+def IKTargetDoMove(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'position', 'duration']
+    optional_params = ['speed_based', 'relative']
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    if 'speed_based' not in kwargs:
+        kwargs['speed_based'] = True
+    if 'relative' not in kwargs:
+        kwargs['relative'] = False
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('IKTargetDoMove')
+    msg.write_float32(kwargs['position'][0])
+    msg.write_float32(kwargs['position'][1])
+    msg.write_float32(kwargs['position'][2])
+    msg.write_float32(kwargs['duration'])
+    msg.write_bool(kwargs['speed_based'])
+    msg.write_bool(kwargs['relative'])
+    return msg
+
+def IKTargetDoRotate(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'vector3', 'duration']
+    optional_params = ['speed_based', 'relative']
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    if 'speed_based' not in kwargs:
+        kwargs['speed_based'] = True
+    if 'relative' not in kwargs:
+        kwargs['relative'] = False
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('IKTargetDoRotate')
+    msg.write_float32(kwargs['vector3'][0])
+    msg.write_float32(kwargs['vector3'][1])
+    msg.write_float32(kwargs['vector3'][2])
+    msg.write_float32(kwargs['duration'])
+    msg.write_bool(kwargs['speed_based'])
+    msg.write_bool(kwargs['relative'])
+    return msg
+
+def IKTargetDoRotateQuaternion(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'quaternion', 'duration']
+    optional_params = ['speed_based', 'relative']
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    if 'speed_based' not in kwargs:
+        kwargs['speed_based'] = True
+    if 'relative' not in kwargs:
+        kwargs['relative'] = False
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('IKTargetDoRotateQuaternion')
+    msg.write_float32(kwargs['quaternion'][0])
+    msg.write_float32(kwargs['quaternion'][1])
+    msg.write_float32(kwargs['quaternion'][2])
+    msg.write_float32(kwargs['quaternion'][3])
+    msg.write_float32(kwargs['duration'])
+    msg.write_bool(kwargs['speed_based'])
+    msg.write_bool(kwargs['relative'])
+    return msg
+
+
+def IKTargetDoComplete(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('IKTargetDoComplete')
+    return msg
+
+
+def IKTargetDoKill(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('IKTargetDoKill')
+    return msg
+
+def SetIKTargetOffset(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id']
+    optional_params = ['position', 'rotation', 'is_quaternion']
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    if 'position' not in kwargs:
+        kwargs['position'] = [0,0,0]
+    if 'rotation' not in kwargs:
+        kwargs['rotation'] = [0,0,0,0]
+    if 'is_quaternion' not in kwargs:
+        kwargs['is_quaternion'] = False
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('SetIKTargetOffset')
+    msg.write_float32(kwargs['position'][0])
+    msg.write_float32(kwargs['position'][1])
+    msg.write_float32(kwargs['position'][2])
+    msg.write_bool(kwargs['is_quaternion'])
+    if kwargs['is_quaternion']:
+        msg.write_float32(kwargs['rotation'][0])
+        msg.write_float32(kwargs['rotation'][1])
+        msg.write_float32(kwargs['rotation'][2])
+        msg.write_float32(kwargs['rotation'][2])
+    else:
+        msg.write_float32(kwargs['rotation'][0])
+        msg.write_float32(kwargs['rotation'][1])
+        msg.write_float32(kwargs['rotation'][2])
+    return msg
+
+
+class ControllerAttr(attr.ColliderAttr):
+    """
+    机械臂控制器类
+    """
+    def parse_message(self, msg: IncomingMessage) -> dict:
+        """
+        解析消息
+
+        Returns:
+            self.data['number_of_joints'] 机械臂关节数量
+
+            self.data['positions'] 机械臂节点位置
+
+            self.data['rotations'] 机械臂节点旋转角度
+
+            self.data['quaternion'] 机械臂节点旋转四元数
+
+            self.data['local_positions'] 机械臂节点局部位置
+
+            self.data['local_rotations'] 机械臂节点局部旋转角度
+
+            self.data['local_quaternion'] 机械臂节点局部旋转四元数
+
+            self.data['velocities'] 机械臂节点速度
+
+            self.data['number_of_moveable_joints'] 机械臂活动关节数量
+
+            self.data['joint_positions'] 机械臂关节在自由度空间下位置
+
+            self.data['joint_velocities'] 机械臂关节在自由度空间下速度
+
+            self.data['all_stable'] 机械臂所有关节移动完成
+
+            self.data['move_done'] 机械臂IK移动完成状态
+
+            self.data['rotate_done'] 机械臂IK旋转完成状态
+
+            self.data['gravity_forces'] InverseDynamics抵消重力所需的力
+
+            self.data['coriolis_centrifugal_forces'] InverseDynamics抵消离心力所需的力
+
+            self.data['drive_forces'] InverseDynamics驱动力
+        """
+        super().parse_message(msg)
+        self.data['number_of_joints'] = msg.read_int32()
+        # Position
+        self.data['positions'] = np.array(msg.read_float32_list()).reshape([-1, 3]).tolist()
+        # RotationEuler
+        self.data['rotations'] = np.array(msg.read_float32_list()).reshape([-1, 3]).tolist()
+        # RotationQuaternion
+        self.data['quaternion'] = np.array(msg.read_float32_list()).reshape([-1, 4]).tolist()
+        # LocalPosition
+        self.data['local_positions'] = np.array(msg.read_float32_list()).reshape([-1, 3]).tolist()
+        # LocalRotationEuler
+        self.data['local_rotations'] = np.array(msg.read_float32_list()).reshape([-1, 3]).tolist()
+        # LocalRotationQuaternion
+        self.data['local_quaternion'] = np.array(msg.read_float32_list()).reshape([-1, 4]).tolist()
+        # Velocity
+        self.data['velocities'] = np.array(msg.read_float32_list()).reshape([-1, 3]).tolist()
+        #
+        self.data['number_of_moveable_joints'] = msg.read_int32()
+        # Each joint position
+        self.data['joint_positions'] = msg.read_float32_list()
+        # Each joint velocity
+        self.data['joint_velocities'] = msg.read_float32_list()
+        # Whether all parts are stable
+        self.data['all_stable'] = msg.read_bool()
+        self.data['move_done'] = msg.read_bool()
+        self.data['rotate_done'] = msg.read_bool()
+        if msg.read_bool() is True:
+            self.data['gravity_forces'] = msg.read_float32_list()
+            self.data['coriolis_centrifugal_forces'] = msg.read_float32_list()
+            self.data['drive_forces'] = msg.read_float32_list()
+        return self.data
+
+    def SetJointPosition(self, joint_positions: list, speed_scales = None):
+        """
+        设置机械臂所有关节目标位置
+
+        Args:
+            joint_positions: 目标位置
+            speed_scales: 速度倍数
+        """
+        num_joints = len(joint_positions)
+        if speed_scales is None:
+            speed_scales = [1.0 for i in range(num_joints)]
+        assert num_joints == len(speed_scales), \
+            'The length of joint_positions and speed_scales are not equal.'
+
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('SetJointPosition')
+        msg.write_float32_list(joint_positions)
+        msg.write_float32_list(speed_scales)
+
+        self.env.instance_channel.send_message(msg)
+
+    def SetJointPositionDirectly(self, joint_positions: list):
+        """
+        立即设置机械臂所有关节位置
+
+        Args:
+            joint_positions: 目标位置
+        """
+        num_joints = len(joint_positions)
+
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('SetJointPositionDirectly')
+        msg.write_float32_list(joint_positions)
+
+        self.env.instance_channel.send_message(msg)
+
+    def SetIndexJointPosition(self, index: int, joint_position: float):
+        """
+        设置机械臂指定关节目标位置
+
+        Args:
+            index: 关节序号
+            joint_position: 目标位置
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('SetIndexJointPosition')
+        msg.write_int32(index)
+        msg.write_float32(joint_position)
+
+        self.env.instance_channel.send_message(msg)
+
+    def SetIndexJointPositionDirectly(self, index: int, joint_position: float):
+        """
+        立即设置机械臂指定关节位置
+
+        Args:
+            index: 关节序号
+            joint_position: 目标位置
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('SetIndexJointPositionDirectly')
+        msg.write_int32(index)
+        msg.write_float32(joint_position)
+
+        self.env.instance_channel.send_message(msg)
+
+    def SetJointPositionContinue(self, interval: int, time_joint_positions: list):
+        """
+        持续设置机械臂所有关节目标位置
+
+        Args:
+            interval: 设置时间间隔(毫秒)
+            time_joint_positions: 每个time的目标位置
+
+        Returns:
+
+        """
+        num_times = len(time_joint_positions)
+
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('SetJointPositionContinue')
+        msg.write_int32(num_times)
+        msg.write_int32(interval)
+        for i in range(num_times):
+            msg.write_float32_list(time_joint_positions[i])
+
+        self.env.instance_channel.send_message(msg)
+
+    def SetJointVelocity(self, joint_velocitys: list):
+        """
+        设置机械臂所有关节目标速度
+
+        Args:
+            joint_velocitys: 目标速度
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('SetJointVelocity')
+        msg.write_float32_list(joint_velocitys)
+
+        self.env.instance_channel.send_message(msg)
+
+    def SetIndexJointVelocity(self, index: int, joint_velocity: float):
+        """
+        设置机械臂指定关节目标速度
+
+        Args:
+            index: 关节序号
+            joint_velocity: 目标速度
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('SetIndexJointVelocity')
+        msg.write_int32(index)
+        msg.write_float32(joint_velocity)
+
+        self.env.instance_channel.send_message(msg)
+
+    def AddJointForce(self, joint_forces: list):
+        """
+        为机械臂所有关节施加力
+
+        Args:
+            joint_forces: 力
+        """
+        num_joints = len(joint_positions)
+
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('AddJointForce')
+        msg.write_int32(num_joints)
+        for i in range(num_joints):
+            msg.write_float32(joint_forces[i][0])
+            msg.write_float32(joint_forces[i][1])
+            msg.write_float32(joint_forces[i][2])
+
+        self.env.instance_channel.send_message(msg)
+
+    def AddJointForceAtPosition(self, joint_forces: list, force_positions: list):
+        """
+        为机械臂所有关节指定位置施加力
+
+        Args:
+            joint_forces: 力
+            force_positions: 施力点
+        """
+        num_joints = len(joint_positions)
+        assert len(joint_forces) == len(force_positions), \
+            'The length of joint_forces and force_positions are not equal.'
+
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('AddJointForceAtPosition')
+        msg.write_int32(num_joints)
+        for i in range(num_joints):
+            msg.write_float32(joint_forces[i][0])
+            msg.write_float32(joint_forces[i][1])
+            msg.write_float32(joint_forces[i][2])
+            msg.write_float32(force_positions[i][0])
+            msg.write_float32(force_positions[i][1])
+            msg.write_float32(force_positions[i][2])
+
+        self.env.instance_channel.send_message(msg)
+
+    def AddJointTorque(self, joint_torques: list):
+        """
+        为机械臂所有关节施加力矩
+
+        Args:
+            joint_torques: 力矩
+        """
+        num_joints = len(joint_torque)
+
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('AddJointTorque')
+        msg.write_int32(num_joints)
+        for i in range(num_joints):
+            msg.write_float32(joint_torques[i][0])
+            msg.write_float32(joint_torques[i][1])
+            msg.write_float32(joint_torques[i][2])
+
+        self.env.instance_channel.send_message(msg)
+
+    # only work on unity 2022.1+
+    def GetJointInverseDynamicsForce(self):
+        """
+        获取机械臂所有关节逆动力学数据
+
+        Returns:
+            调用此接口并step后，从
+            self.data['gravity_forces']
+            self.data['coriolis_centrifugal_forces']
+            self.data['drive_forces']
+            获取结果
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('GetJointInverseDynamicsForce')
+
+        self.env.instance_channel.send_message(msg)
+
+    def SetImmovable(self, immovable: bool):
+        """
+        设置机械臂是否不可移动
+
+        Args:
+            immovable: 是否不可移动
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('SetImmovable')
+        msg.write_bool(immovable)
+
+        self.env.instance_channel.send_message(msg)
+
+    def MoveForward(self, distance: float, speed: float):
+        """
+        如果机器人在Unity端添加了继承ICustomMove接口的脚本，可通过此接口驱动前进
+        最初用于Tobor机器人
+
+        Args:
+            distance:距离
+            speed:速度
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('MoveForward')
+        msg.write_float32(distance)
+        msg.write_float32(speed)
+
+        self.env.instance_channel.send_message(msg)
+
+    def MoveBack(self, distance: float, speed: float):
+        """
+        如果机器人在Unity端添加了继承ICustomMove接口的脚本，可通过此接口驱动后退
+        最初用于Tobor机器人
+
+        Args:
+            distance:距离
+            speed:速度
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('MoveBack')
+        msg.write_float32(distance)
+        msg.write_float32(speed)
+
+        self.env.instance_channel.send_message(msg)
+
+    def TurnLeft(self, angle: float, speed: float):
+        """
+        如果机器人在Unity端添加了继承ICustomMove接口的脚本，可通过此接口驱动左转
+        最初用于Tobor机器人
+
+        Args:
+            angle:角度
+            speed:速度
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('TurnLeft')
+        msg.write_float32(angle)
+        msg.write_float32(speed)
+
+        self.env.instance_channel.send_message(msg)
+
+    def TurnRight(self, angle: float, speed: float):
+        """
+        如果机器人在Unity端添加了继承ICustomMove接口的脚本，可通过此接口驱动右转
+        最初用于Tobor机器人
+
+        Args:
+            angle:角度
+            speed:速度
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('TurnRight')
+        msg.write_float32(angle)
+        msg.write_float32(speed)
+
+        self.env.instance_channel.send_message(msg)
+
+    def GripperOpen(self):
+        """
+        如果夹爪在Unity端添加了继承ICustomGripper接口的脚本，可通过此接口驱动张开
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('GripperOpen')
+
+        self.env.instance_channel.send_message(msg)
+
+    def GripperClose(self):
+        """
+        如果夹爪在Unity端添加了继承ICustomGripper接口的脚本，可通过此接口驱动闭合
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('GripperClose')
+
+        self.env.instance_channel.send_message(msg)
+
+    def EnabledNativeIK(self, enabled: bool):
+        """
+        启用/禁用机械臂的原生IK
+
+        Args:
+            enabled: 启用/禁用
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('EnabledNativeIK')
+        msg.write_bool(enabled)
+
+        self.env.instance_channel.send_message(msg)
+
+    def IKTargetDoMove(self, position: list, duration: float, speed_based: bool = True, relative: bool = False):
+        """
+        原生IK末端点移动
+
+        Args:
+            position: 绝对位置或相对位置
+            duration: 移动持续时间或移动速度
+            speed_based: 指定duration表示移动持续时间还是移动速度
+            relative: 指定position表示绝对位置还是相对位置
+
+        Returns:
+            当移动完成时，self.data['move_done']会被置为True
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('IKTargetDoMove')
+        msg.write_float32(position[0])
+        msg.write_float32(position[1])
+        msg.write_float32(position[2])
+        msg.write_float32(duration)
+        msg.write_bool(speed_based)
+        msg.write_bool(relative)
+
+        self.env.instance_channel.send_message(msg)
+
+    def IKTargetDoRotate(self, rotation: list, duration: float, speed_based: bool = True, relative: bool = False):
+        """
+        原生IK末端点Vector3旋转
+
+        Args:
+            rotation: 绝对旋转或相对旋转
+            duration: 旋转持续时间或旋转速度
+            speed_based: 指定duration表示旋转持续时间还是旋转速度
+            relative: 指定position表示绝对旋转还是相对旋转
+
+        Returns:
+            当旋转完成时，self.data['rotate_done']会被置为True
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('IKTargetDoRotate')
+        msg.write_float32(rotation[0])
+        msg.write_float32(rotation[1])
+        msg.write_float32(rotation[2])
+        msg.write_float32(duration)
+        msg.write_bool(speed_based)
+        msg.write_bool(relative)
+
+        self.env.instance_channel.send_message(msg)
+
+    def IKTargetDoRotateQuaternion(self, quaternion: list, duration: float, speed_based: bool = True, relative: bool = False):
+        """
+        原生IK末端点四元数旋转
+
+        Args:
+            quaternion: 绝对旋转或相对旋转
+            duration: 旋转持续时间或旋转速度
+            speed_based: 指定duration表示旋转持续时间还是旋转速度
+            relative: 指定position表示绝对旋转还是相对旋转
+
+        Returns:
+            当旋转完成时，self.data['rotate_done']会被置为True
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('IKTargetDoRotateQuaternion')
+        msg.write_float32(quaternion[0])
+        msg.write_float32(quaternion[1])
+        msg.write_float32(quaternion[2])
+        msg.write_float32(quaternion[3])
+        msg.write_float32(duration)
+        msg.write_bool(speed_based)
+        msg.write_bool(relative)
+
+        self.env.instance_channel.send_message(msg)
+
+    def IKTargetDoComplete(self):
+        """
+        使原生IK末端点移动/旋转立即完成
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('IKTargetDoComplete')
+
+        self.env.instance_channel.send_message(msg)
+
+    def IKTargetDoKill(self):
+        """
+        使原生IK末端点移动/旋转停止
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('IKTargetDoKill')
+
+        self.env.instance_channel.send_message(msg)
+
+    def SetIKTargetOffset(self, position: list = [0.,0.,0.], rotation: list = [0.,0.,0.], quaternion: list = None):
+        """
+        设置原生IK末端点的偏移
+
+        Args:
+            position: 偏移位置
+            rotation: 偏移旋转Vector3
+            quaternion: 偏移旋转四元数，此值覆盖rotation
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('SetIKTargetOffset')
+        msg.write_float32(position[0])
+        msg.write_float32(position[1])
+        msg.write_float32(position[2])
+        msg.write_bool(quaternion is not None)
+        if quaternion is not None:
+            msg.write_float32(quaternion[0])
+            msg.write_float32(quaternion[1])
+            msg.write_float32(quaternion[2])
+            msg.write_float32(quaternion[2])
+        else:
+            msg.write_float32(rotation[0])
+            msg.write_float32(rotation[1])
+            msg.write_float32(rotation[2])
+
+        self.env.instance_channel.send_message(msg)
+
+    def WaitDo(self):
+        """
+        等待原生IK末端点移动/旋转完成
+        """
+        while not self.data['move_done'] or not self.data['rotate_done']:
             self.env.step()
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/custom_attr.py` & `pyrfuniverse-0.8.3/pyrfuniverse/attributes/custom_attr.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import pyrfuniverse.attributes as attr
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
-
-
-#自定义Attr类示例
-class CustomAttr(attr.BaseAttr):
-    """
-    此类为自定义Attr类的示例，不包含实际功能
-    """
-    # 消息解析示例
-    def parse_message(self, msg: IncomingMessage) -> dict:
-        # 先完成所继承的基类的数据读取
-        super().parse_message(msg)
-        # 按顺序读取数据
-        # 此处读取顺序对应Unity的CustomAttr脚本CollectData函数中的写入顺序
-        self.data['custom_message'] = msg.read_string()
-        return self.data
-
-    # 新增接口示例
-    def CustomMessage(self, message: str):
-        msg = OutgoingMessage()
-
-        # 第一个写入的数据必须是ID
-        msg.write_int32(self.id)
-        # 第二个写入的数据必须是消息类型 此处CustomMessage对应Unity新增Attr脚本AnalysisMsg函数switch的一个分支
-        msg.write_string('CustomMessage')
-
-        # 写入数据
-        msg.write_string(message)
-
-        self.env.instance_channel.send_message(msg)
+import pyrfuniverse.attributes as attr
+from pyrfuniverse.side_channel.side_channel import (
+    IncomingMessage,
+    OutgoingMessage,
+)
+
+
+#自定义Attr类示例
+class CustomAttr(attr.BaseAttr):
+    """
+    此类为自定义Attr类的示例，不包含实际功能
+    """
+    # 消息解析示例
+    def parse_message(self, msg: IncomingMessage) -> dict:
+        # 先完成所继承的基类的数据读取
+        super().parse_message(msg)
+        # 按顺序读取数据
+        # 此处读取顺序对应Unity的CustomAttr脚本CollectData函数中的写入顺序
+        self.data['custom_message'] = msg.read_string()
+        return self.data
+
+    # 新增接口示例
+    def CustomMessage(self, message: str):
+        msg = OutgoingMessage()
+
+        # 第一个写入的数据必须是ID
+        msg.write_int32(self.id)
+        # 第二个写入的数据必须是消息类型 此处CustomMessage对应Unity新增Attr脚本AnalysisMsg函数switch的一个分支
+        msg.write_string('CustomMessage')
+
+        # 写入数据
+        msg.write_string(message)
+
+        self.env.instance_channel.send_message(msg)
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/digit_attr.py` & `pyrfuniverse-0.8.3/pyrfuniverse/attributes/digit_attr.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import pyrfuniverse.attributes as attr
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
-import base64
-
-
-class DigitAttr(attr.BaseAttr):
-    """
-    模拟Digit指尖触觉传感器类
-    """
-    def parse_message(self, msg: IncomingMessage) -> dict:
-        """
-        消息解析
-
-        Returns:
-            self.data['light'] RGB灯光图像bytes
-
-            self.data['depth'] 深度图像bytes
-        """
-        super().parse_message(msg)
-        if msg.read_bool() is True:
-            self.data['light'] = base64.b64decode(msg.read_string())
-            self.data['depth'] = base64.b64decode(msg.read_string())
-        return self.data
-
-
-    def GetData(self):
-        """
-        获取传感器数据
-
-        Returns:
-            调用此接口并step后，从
-            self.data['light']: 获取RGB灯光图像，
-            self.data['depth']: 获取深度图像
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('GetData')
-
+import pyrfuniverse.attributes as attr
+from pyrfuniverse.side_channel.side_channel import (
+    IncomingMessage,
+    OutgoingMessage,
+)
+import base64
+
+
+class DigitAttr(attr.BaseAttr):
+    """
+    模拟Digit指尖触觉传感器类
+    """
+    def parse_message(self, msg: IncomingMessage) -> dict:
+        """
+        消息解析
+
+        Returns:
+            self.data['light'] RGB灯光图像bytes
+
+            self.data['depth'] 深度图像bytes
+        """
+        super().parse_message(msg)
+        if msg.read_bool() is True:
+            self.data['light'] = base64.b64decode(msg.read_string())
+            self.data['depth'] = base64.b64decode(msg.read_string())
+        return self.data
+
+
+    def GetData(self):
+        """
+        获取传感器数据
+
+        Returns:
+            调用此接口并step后，从
+            self.data['light']: 获取RGB灯光图像，
+            self.data['depth']: 获取深度图像
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('GetData')
+
         self.env.instance_channel.send_message(msg)
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/gameobject_attr.py` & `pyrfuniverse-0.8.3/pyrfuniverse/attributes/gameobject_attr.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-import pyrfuniverse.attributes as attr
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
-import pyrfuniverse.utils.rfuniverse_utility as utility
-
-def Translate(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'translation']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-    msg = OutgoingMessage()
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('Translate')
-    for i in range(3):
-        msg.write_float32(kwargs['translation'][i])
-
-    return msg
-
-
-def Rotate(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'rotation']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-    msg = OutgoingMessage()
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('Rotate')
-    for i in range(3):
-        msg.write_float32(kwargs['rotation'][i])
-
-    return msg
-
-
-def SetColor(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'color']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-    msg = OutgoingMessage()
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('SetColor')
-    for i in range(4):
-        msg.write_float32(kwargs['color'][i])
-
-    return msg
-
-
-class GameObjectAttr(attr.BaseAttr):
-    """
-    基本视觉物体类
-    """
-    def parse_message(self, msg: IncomingMessage) -> dict:
-        """
-        解析消息
-
-        Returns:
-            self.data['3d_bounding_box'] 物体3D包围盒
-        """
-        super().parse_message(msg)
-        if msg.read_bool():
-            self.data['3d_bounding_box'] = {}
-            self.data['3d_bounding_box']['position'] = [msg.read_float32() for _ in range(3)]
-            self.data['3d_bounding_box']['rotation'] = [msg.read_float32() for _ in range(3)]
-            self.data['3d_bounding_box']['size'] = [msg.read_float32() for _ in range(3)]
-        return self.data
-
-    def SetColor(self, color: list):
-        """
-        设置物体颜色
-
-        Args:
-            color: 颜色，长度为4，分别为RGBA[0-1]
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetColor')
-        for i in range(4):
-            msg.write_float32(color[i])
-
-        self.env.instance_channel.send_message(msg)
-
-    def EnabledRender(self, enabled: bool):
-        """
-        启用或禁用渲染
-
-        Args:
-            enabled: 是否启用渲染
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('EnabledRender')
-        msg.write_bool(enabled)
-
-        self.env.instance_channel.send_message(msg)
-
-    def SetTexture(self, path: str):
-        """
-        设置物体纹理
-
-        Args:
-            path: 纹理贴图绝对路径
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetTexture')
-        msg.write_string(path)
-
-        self.env.instance_channel.send_message(msg)
-
-    def Get3DBBox(self):
-        """
-        获取该物体3D Bounding Box
-
-        Returns:
-            调用此接口并step后，从
-            self.data['3d_bounding_box']
-            获取结果
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('Get3DBBox')
-
-        self.env.instance_channel.send_message(msg)
-
-
-
+import pyrfuniverse.attributes as attr
+from pyrfuniverse.side_channel.side_channel import (
+    IncomingMessage,
+    OutgoingMessage,
+)
+import pyrfuniverse.utils.rfuniverse_utility as utility
+
+def Translate(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'translation']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+    msg = OutgoingMessage()
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('Translate')
+    for i in range(3):
+        msg.write_float32(kwargs['translation'][i])
+
+    return msg
+
+
+def Rotate(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'rotation']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+    msg = OutgoingMessage()
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('Rotate')
+    for i in range(3):
+        msg.write_float32(kwargs['rotation'][i])
+
+    return msg
+
+
+def SetColor(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'color']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+    msg = OutgoingMessage()
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('SetColor')
+    for i in range(4):
+        msg.write_float32(kwargs['color'][i])
+
+    return msg
+
+
+class GameObjectAttr(attr.BaseAttr):
+    """
+    基本视觉物体类
+    """
+    def parse_message(self, msg: IncomingMessage) -> dict:
+        """
+        解析消息
+
+        Returns:
+            self.data['3d_bounding_box'] 物体3D包围盒
+        """
+        super().parse_message(msg)
+        if msg.read_bool():
+            self.data['3d_bounding_box'] = {}
+            self.data['3d_bounding_box']['position'] = [msg.read_float32() for _ in range(3)]
+            self.data['3d_bounding_box']['rotation'] = [msg.read_float32() for _ in range(3)]
+            self.data['3d_bounding_box']['size'] = [msg.read_float32() for _ in range(3)]
+        return self.data
+
+    def SetColor(self, color: list):
+        """
+        设置物体颜色
+
+        Args:
+            color: 颜色，长度为4，分别为RGBA[0-1]
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('SetColor')
+        for i in range(4):
+            msg.write_float32(color[i])
+
+        self.env.instance_channel.send_message(msg)
+
+    def EnabledRender(self, enabled: bool):
+        """
+        启用或禁用渲染
+
+        Args:
+            enabled: 是否启用渲染
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('EnabledRender')
+        msg.write_bool(enabled)
+
+        self.env.instance_channel.send_message(msg)
+
+    def SetTexture(self, path: str):
+        """
+        设置物体纹理
+
+        Args:
+            path: 纹理贴图绝对路径
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('SetTexture')
+        msg.write_string(path)
+
+        self.env.instance_channel.send_message(msg)
+
+    def Get3DBBox(self):
+        """
+        获取该物体3D Bounding Box
+
+        Returns:
+            调用此接口并step后，从
+            self.data['3d_bounding_box']
+            获取结果
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('Get3DBBox')
+
+        self.env.instance_channel.send_message(msg)
+
+
+
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/graspsim_attr.py` & `pyrfuniverse-0.8.3/pyrfuniverse/attributes/graspsim_attr.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-import pyrfuniverse.attributes as attr
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
-
-
-class GraspSimAttr(attr.BaseAttr):
-    """
-    抓取测试农场仿真类
-    """
-    def parse_message(self, msg: IncomingMessage) -> dict:
-        """
-        消息解析
-
-        Returns:
-            self.data['done'] 模拟是否完成
-
-            self.data['points'] 抓点列表
-
-            self.data['quaternions'] 抓点对应的四元数列表
-
-            self.data['width'] 抓点对应的抓型宽度列表
-
-            self.data['success'] 抓点对应的抓取结果列表
-        """
-        super().parse_message(msg)
-        self.data['done'] = msg.read_bool()
-        if self.data['done']:
-            mode = msg.read_int32()
-            if mode == 0:
-                self.data['points'] = msg.read_float32_list()
-                self.data['quaternions'] = msg.read_float32_list()
-                self.data['width'] = msg.read_float32_list()
-            if mode == 1:
-                self.data['success'] = msg.read_float32_list()
-        return self.data
-
-    def StartGraspSim(self, mesh: str, gripper: str, points: list, normals: list, depth_range_min: float, depth_range_max: float, depth_lerp_count: int, angle_lerp_count: int, parallel_count: int = 100):
-        """
-        开始模拟抓取
-
-        Args:
-            mesh: 物体网格路径
-            gripper: 夹爪
-            points: 抓点列表
-            normals: 法线列表
-            depth_range_min: 抓型深度范围最小值
-            depth_range_max: 抓型深度范围最大值
-            depth_lerp_count: 抓型深度插值数量
-            angle_lerp_count: 抓型角度插值数量
-            parallel_count: 并行抓取数
-
-        Returns:
-            当模拟完成时，self.data['done']会被置为True
-            self.data['points']为抓点列表
-            self.data['quaternions']为抓点对应的四元数列表
-            self.data['width']为抓点对应的抓型宽度列表
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('StartGraspSim')
-        msg.write_string(mesh)
-        msg.write_string(gripper)
-        msg.write_float32_list(points)
-        msg.write_float32_list(normals)
-        msg.write_float32(depth_range_min)
-        msg.write_float32(depth_range_max)
-        msg.write_int32(depth_lerp_count)
-        msg.write_int32(angle_lerp_count)
-        msg.write_int32(parallel_count)
-
-        self.env.instance_channel.send_message(msg)
-
-    def GenerateGraspPose(self, mesh: str, gripper: str, points: list, normals: list, depth_range_min: float, depth_range_max: float, depth_lerp_count: int, angle_lerp_count: int):
-        """
-        生成抓取姿态
-
-        Args:
-            mesh: 物体网格路径
-            gripper: 夹爪
-            points: 抓点列表
-            normals: 法线列表
-            depth_range_min: 抓型深度范围最小值
-            depth_range_max: 抓型深度范围最大值
-            depth_lerp_count: 抓型深度插值数量
-            angle_lerp_count: 抓型角度插值数量
-
-        Returns:
-            生成并显示抓取姿态
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('GenerateGraspPose')
-        msg.write_string(mesh)
-        msg.write_string(gripper)
-        msg.write_float32_list(points)
-        msg.write_float32_list(normals)
-        msg.write_float32(depth_range_min)
-        msg.write_float32(depth_range_max)
-        msg.write_int32(depth_lerp_count)
-        msg.write_int32(angle_lerp_count)
-
-        self.env.instance_channel.send_message(msg)
-
-    def StartGraspTest(self, mesh: str, gripper: str, points: list, quaternions: list, parallel_count: int = 100):
-        """
-        对现有抓型进行抓取测试
-
-        Args:
-            mesh: 物体网格路径
-            gripper: 夹爪
-            points: 抓点列表
-            quaternions: 四元数列表
-            parallel_count: 并行抓取数
-
-        Returns:
-            当模拟完成时，self.data['done']会被置为True
-            self.data['success']为抓取结果列表
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('StartGraspTest')
-        msg.write_string(mesh)
-        msg.write_string(gripper)
-        msg.write_float32_list(points)
-        msg.write_float32_list(quaternions)
-        msg.write_int32(parallel_count)
-
-        self.env.instance_channel.send_message(msg)
-
-    def ShowGraspPose(self, mesh: str, gripper: str, positions: list, quaternions: list):
-        """
-        显示抓取姿态
-
-        Args:
-            mesh: 物体网格路径
-            gripper: 夹爪
-            positions: 抓点列表
-            quaternions: 四元数列表
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('ShowGraspPose')
-        msg.write_string(mesh)
-        msg.write_string(gripper)
-        msg.write_float32_list(positions)
-        msg.write_float32_list(quaternions)
-
-        self.env.instance_channel.send_message(msg)
+import pyrfuniverse.attributes as attr
+from pyrfuniverse.side_channel.side_channel import (
+    IncomingMessage,
+    OutgoingMessage,
+)
+
+
+class GraspSimAttr(attr.BaseAttr):
+    """
+    抓取测试农场仿真类
+    """
+    def parse_message(self, msg: IncomingMessage) -> dict:
+        """
+        消息解析
+
+        Returns:
+            self.data['done'] 模拟是否完成
+
+            self.data['points'] 抓点列表
+
+            self.data['quaternions'] 抓点对应的四元数列表
+
+            self.data['width'] 抓点对应的抓型宽度列表
+
+            self.data['success'] 抓点对应的抓取结果列表
+        """
+        super().parse_message(msg)
+        self.data['done'] = msg.read_bool()
+        if self.data['done']:
+            mode = msg.read_int32()
+            if mode == 0:
+                self.data['points'] = msg.read_float32_list()
+                self.data['quaternions'] = msg.read_float32_list()
+                self.data['width'] = msg.read_float32_list()
+            if mode == 1:
+                self.data['success'] = msg.read_float32_list()
+        return self.data
+
+    def StartGraspSim(self, mesh: str, gripper: str, points: list, normals: list, depth_range_min: float, depth_range_max: float, depth_lerp_count: int, angle_lerp_count: int, parallel_count: int = 100):
+        """
+        开始模拟抓取
+
+        Args:
+            mesh: 物体网格路径
+            gripper: 夹爪
+            points: 抓点列表
+            normals: 法线列表
+            depth_range_min: 抓型深度范围最小值
+            depth_range_max: 抓型深度范围最大值
+            depth_lerp_count: 抓型深度插值数量
+            angle_lerp_count: 抓型角度插值数量
+            parallel_count: 并行抓取数
+
+        Returns:
+            当模拟完成时，self.data['done']会被置为True
+            self.data['points']为抓点列表
+            self.data['quaternions']为抓点对应的四元数列表
+            self.data['width']为抓点对应的抓型宽度列表
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('StartGraspSim')
+        msg.write_string(mesh)
+        msg.write_string(gripper)
+        msg.write_float32_list(points)
+        msg.write_float32_list(normals)
+        msg.write_float32(depth_range_min)
+        msg.write_float32(depth_range_max)
+        msg.write_int32(depth_lerp_count)
+        msg.write_int32(angle_lerp_count)
+        msg.write_int32(parallel_count)
+
+        self.env.instance_channel.send_message(msg)
+
+    def GenerateGraspPose(self, mesh: str, gripper: str, points: list, normals: list, depth_range_min: float, depth_range_max: float, depth_lerp_count: int, angle_lerp_count: int):
+        """
+        生成抓取姿态
+
+        Args:
+            mesh: 物体网格路径
+            gripper: 夹爪
+            points: 抓点列表
+            normals: 法线列表
+            depth_range_min: 抓型深度范围最小值
+            depth_range_max: 抓型深度范围最大值
+            depth_lerp_count: 抓型深度插值数量
+            angle_lerp_count: 抓型角度插值数量
+
+        Returns:
+            生成并显示抓取姿态
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('GenerateGraspPose')
+        msg.write_string(mesh)
+        msg.write_string(gripper)
+        msg.write_float32_list(points)
+        msg.write_float32_list(normals)
+        msg.write_float32(depth_range_min)
+        msg.write_float32(depth_range_max)
+        msg.write_int32(depth_lerp_count)
+        msg.write_int32(angle_lerp_count)
+
+        self.env.instance_channel.send_message(msg)
+
+    def StartGraspTest(self, mesh: str, gripper: str, points: list, quaternions: list, parallel_count: int = 100):
+        """
+        对现有抓型进行抓取测试
+
+        Args:
+            mesh: 物体网格路径
+            gripper: 夹爪
+            points: 抓点列表
+            quaternions: 四元数列表
+            parallel_count: 并行抓取数
+
+        Returns:
+            当模拟完成时，self.data['done']会被置为True
+            self.data['success']为抓取结果列表
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('StartGraspTest')
+        msg.write_string(mesh)
+        msg.write_string(gripper)
+        msg.write_float32_list(points)
+        msg.write_float32_list(quaternions)
+        msg.write_int32(parallel_count)
+
+        self.env.instance_channel.send_message(msg)
+
+    def ShowGraspPose(self, mesh: str, gripper: str, positions: list, quaternions: list):
+        """
+        显示抓取姿态
+
+        Args:
+            mesh: 物体网格路径
+            gripper: 夹爪
+            positions: 抓点列表
+            quaternions: 四元数列表
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('ShowGraspPose')
+        msg.write_string(mesh)
+        msg.write_string(gripper)
+        msg.write_float32_list(positions)
+        msg.write_float32_list(quaternions)
+
+        self.env.instance_channel.send_message(msg)
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/humanbody_attr.py` & `pyrfuniverse-0.8.3/pyrfuniverse/attributes/humanbody_attr.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,242 +1,242 @@
-import pyrfuniverse.attributes as attr
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
-import pyrfuniverse.utils.rfuniverse_utility as utility
-
-
-def HumanIKTargetDoMove(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'index', 'position', 'duration']
-    optional_params = ['speed_based', 'relative']
-    utility.CheckKwargs(kwargs, compulsory_params)
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('HumanIKTargetDoMove')
-    msg.write_int32(kwargs['index'])
-    msg.write_float32(kwargs['position'][0])
-    msg.write_float32(kwargs['position'][1])
-    msg.write_float32(kwargs['position'][2])
-    msg.write_float32(kwargs['duration'])
-    if 'speed_based' in kwargs:
-        msg.write_bool(kwargs['speed_based'])
-    else:
-        msg.write_bool(True)
-    if 'relative' in kwargs:
-        msg.write_bool(kwargs['relative'])
-    else:
-        msg.write_bool(False)
-    return msg
-
-
-def HumanIKTargetDoRotate(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'index', 'vector3', 'duration']
-    optional_params = ['speed_based', 'relative']
-    utility.CheckKwargs(kwargs, compulsory_params)
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('HumanIKTargetDoRotateQuaternion')
-    msg.write_int32(kwargs['index'])
-    msg.write_float32(kwargs['vector3'][0])
-    msg.write_float32(kwargs['vector3'][1])
-    msg.write_float32(kwargs['vector3'][2])
-    msg.write_float32(kwargs['duration'])
-    if 'speed_based' in kwargs:
-        msg.write_bool(kwargs['speed_based'])
-    else:
-        msg.write_bool(True)
-    if 'relative' in kwargs:
-        msg.write_bool(kwargs['relative'])
-    else:
-        msg.write_bool(False)
-    return msg
-
-def HumanIKTargetDoRotateQuaternion(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'index', 'quaternion', 'duration']
-    optional_params = ['speed_based', 'relative']
-    utility.CheckKwargs(kwargs, compulsory_params)
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('HumanIKTargetDoRotateQuaternion')
-    msg.write_int32(kwargs['index'])
-    msg.write_float32(kwargs['quaternion'][0])
-    msg.write_float32(kwargs['quaternion'][1])
-    msg.write_float32(kwargs['quaternion'][2])
-    msg.write_float32(kwargs['quaternion'][3])
-    msg.write_float32(kwargs['duration'])
-    if 'speed_based' in kwargs:
-        msg.write_bool(kwargs['speed_based'])
-    else:
-        msg.write_bool(True)
-    if 'relative' in kwargs:
-        msg.write_bool(kwargs['relative'])
-    else:
-        msg.write_bool(False)
-    return msg
-
-
-def HumanIKTargetDoComplete(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'index']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('HumanIKTargetDoComplete')
-    msg.write_int32(kwargs['index'])
-    return msg
-
-def HumanIKTargetDoKill(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'index']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-    msg.write_int32(kwargs['id'])
-    msg.write_string('HumanIKTargetDoKill')
-    msg.write_int32(kwargs['index'])
-    return msg
-
-
-class HumanbodyAttr(attr.BaseAttr):
-    """
-    人体IK类
-    """
-    def parse_message(self, msg: IncomingMessage) -> dict:
-        """
-        解析消息
-
-        Returns:
-            self.data['move_done'] 移动完成
-
-            self.data['rotate_done'] 旋转完成
-        """
-        super().parse_message(msg)
-        self.data['move_done'] = msg.read_bool()
-        self.data['rotate_done'] = msg.read_bool()
-        return self.data
-
-    def HumanIKTargetDoMove(self, index: int, position: list, duration: float, speed_based: bool = True, relative: bool = False):
-        """
-        人体IK目标点移动
-
-        Args:
-            index: 移动的目标：0-左手，1-右手，2-左脚，3-右脚，4-头部
-            position: 绝对位置或相对位置
-            duration: 移动持续时间或移动速度
-            speed_based: 指定duration表示移动持续时间还是移动速度
-            relative: 指定position表示绝对位置还是相对位置
-
-        Returns:
-            当移动完成时，self.data['move_done']会被置为True
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('HumanIKTargetDoMove')
-        msg.write_int32(index)
-        msg.write_float32(position[0])
-        msg.write_float32(position[1])
-        msg.write_float32(position[2])
-        msg.write_float32(duration)
-        msg.write_bool(speed_based)
-        msg.write_bool(relative)
-
-        self.env.instance_channel.send_message(msg)
-
-    def HumanIKTargetDoRotate(self, index: int, rotation: list, duration: float, speed_based: bool = True, relative: bool = False):
-        """
-        人体IK目标点旋转
-
-        Args:
-            index: 移动的目标：0-左手，1-右手，2-左脚，3-右脚，4-头部
-            rotation: 绝对旋转或相对旋转
-            duration: 旋转持续时间或旋转速度
-            speed_based: 指定duration表示旋转持续时间还是旋转速度
-            relative: 指定position表示绝对旋转还是相对旋转
-
-        Returns:
-            当旋转完成时，self.data['rotate_done']会被置为True
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('HumanIKTargetDoRotate')
-        msg.write_int32(index)
-        msg.write_float32(rotation[0])
-        msg.write_float32(rotation[1])
-        msg.write_float32(rotation[2])
-        msg.write_float32(duration)
-        msg.write_bool(speed_based)
-        msg.write_bool(relative)
-
-        self.env.instance_channel.send_message(msg)
-
-    def HumanIKTargetDoRotateQuaternion(self, index: int, quaternion: list, duration: float, speed_based: bool = True, relative: bool = False):
-        """
-        人体IK目标点四元数旋转
-
-        Args:
-            index: 移动的目标：0-左手，1-右手，2-左脚，3-右脚，4-头部
-            quaternion: 绝对旋转或相对旋转
-            duration: 旋转持续时间或旋转速度
-            speed_based: 指定duration表示旋转持续时间还是旋转速度
-            relative: 指定position表示绝对旋转还是相对旋转
-
-        Returns:
-            当旋转完成时，self.data['rotate_done']会被置为True
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('HumanIKTargetDoRotateQuaternion')
-        msg.write_int32(index)
-        msg.write_float32(quaternion[0])
-        msg.write_float32(quaternion[1])
-        msg.write_float32(quaternion[2])
-        msg.write_float32(quaternion[3])
-        msg.write_float32(duration)
-        msg.write_bool(speed_based)
-        msg.write_bool(relative)
-
-        self.env.instance_channel.send_message(msg)
-
-        self.env.instance_channel.send_message(msg)
-
-    def HumanIKTargetDoComplete(self, index: int):
-        """
-        使人体IK目标点移动/旋转立即完成
-
-        Args:
-            index: 移动的目标：0-左手，1-右手，2-左脚，3-右脚，4-头部
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('HumanIKTargetDoComplete')
-        msg.write_int32(index)
-
-        self.env.instance_channel.send_message(msg)
-
-    def HumanIKTargetDoKill(self, index: int):
-        """
-        使人体IK目标点移动/旋转停止
-
-        Args:
-            index: 移动的目标：0-左手，1-右手，2-左脚，3-右脚，4-头部
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('HumanIKTargetDoKill')
-        msg.write_int32(index)
-
-        self.env.instance_channel.send_message(msg)
-
-    def WaitDo(self):
-        """
-        等待人体IK移动/旋转完成
-        """
-        while not self.data['move_done'] or not self.data['rotate_done']:
-            self.env.step()
-
+import pyrfuniverse.attributes as attr
+from pyrfuniverse.side_channel.side_channel import (
+    IncomingMessage,
+    OutgoingMessage,
+)
+import pyrfuniverse.utils.rfuniverse_utility as utility
+
+
+def HumanIKTargetDoMove(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'index', 'position', 'duration']
+    optional_params = ['speed_based', 'relative']
+    utility.CheckKwargs(kwargs, compulsory_params)
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('HumanIKTargetDoMove')
+    msg.write_int32(kwargs['index'])
+    msg.write_float32(kwargs['position'][0])
+    msg.write_float32(kwargs['position'][1])
+    msg.write_float32(kwargs['position'][2])
+    msg.write_float32(kwargs['duration'])
+    if 'speed_based' in kwargs:
+        msg.write_bool(kwargs['speed_based'])
+    else:
+        msg.write_bool(True)
+    if 'relative' in kwargs:
+        msg.write_bool(kwargs['relative'])
+    else:
+        msg.write_bool(False)
+    return msg
+
+
+def HumanIKTargetDoRotate(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'index', 'vector3', 'duration']
+    optional_params = ['speed_based', 'relative']
+    utility.CheckKwargs(kwargs, compulsory_params)
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('HumanIKTargetDoRotateQuaternion')
+    msg.write_int32(kwargs['index'])
+    msg.write_float32(kwargs['vector3'][0])
+    msg.write_float32(kwargs['vector3'][1])
+    msg.write_float32(kwargs['vector3'][2])
+    msg.write_float32(kwargs['duration'])
+    if 'speed_based' in kwargs:
+        msg.write_bool(kwargs['speed_based'])
+    else:
+        msg.write_bool(True)
+    if 'relative' in kwargs:
+        msg.write_bool(kwargs['relative'])
+    else:
+        msg.write_bool(False)
+    return msg
+
+def HumanIKTargetDoRotateQuaternion(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'index', 'quaternion', 'duration']
+    optional_params = ['speed_based', 'relative']
+    utility.CheckKwargs(kwargs, compulsory_params)
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('HumanIKTargetDoRotateQuaternion')
+    msg.write_int32(kwargs['index'])
+    msg.write_float32(kwargs['quaternion'][0])
+    msg.write_float32(kwargs['quaternion'][1])
+    msg.write_float32(kwargs['quaternion'][2])
+    msg.write_float32(kwargs['quaternion'][3])
+    msg.write_float32(kwargs['duration'])
+    if 'speed_based' in kwargs:
+        msg.write_bool(kwargs['speed_based'])
+    else:
+        msg.write_bool(True)
+    if 'relative' in kwargs:
+        msg.write_bool(kwargs['relative'])
+    else:
+        msg.write_bool(False)
+    return msg
+
+
+def HumanIKTargetDoComplete(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'index']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('HumanIKTargetDoComplete')
+    msg.write_int32(kwargs['index'])
+    return msg
+
+def HumanIKTargetDoKill(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'index']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+    msg.write_int32(kwargs['id'])
+    msg.write_string('HumanIKTargetDoKill')
+    msg.write_int32(kwargs['index'])
+    return msg
+
+
+class HumanbodyAttr(attr.BaseAttr):
+    """
+    人体IK类
+    """
+    def parse_message(self, msg: IncomingMessage) -> dict:
+        """
+        解析消息
+
+        Returns:
+            self.data['move_done'] 移动完成
+
+            self.data['rotate_done'] 旋转完成
+        """
+        super().parse_message(msg)
+        self.data['move_done'] = msg.read_bool()
+        self.data['rotate_done'] = msg.read_bool()
+        return self.data
+
+    def HumanIKTargetDoMove(self, index: int, position: list, duration: float, speed_based: bool = True, relative: bool = False):
+        """
+        人体IK目标点移动
+
+        Args:
+            index: 移动的目标：0-左手，1-右手，2-左脚，3-右脚，4-头部
+            position: 绝对位置或相对位置
+            duration: 移动持续时间或移动速度
+            speed_based: 指定duration表示移动持续时间还是移动速度
+            relative: 指定position表示绝对位置还是相对位置
+
+        Returns:
+            当移动完成时，self.data['move_done']会被置为True
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('HumanIKTargetDoMove')
+        msg.write_int32(index)
+        msg.write_float32(position[0])
+        msg.write_float32(position[1])
+        msg.write_float32(position[2])
+        msg.write_float32(duration)
+        msg.write_bool(speed_based)
+        msg.write_bool(relative)
+
+        self.env.instance_channel.send_message(msg)
+
+    def HumanIKTargetDoRotate(self, index: int, rotation: list, duration: float, speed_based: bool = True, relative: bool = False):
+        """
+        人体IK目标点旋转
+
+        Args:
+            index: 移动的目标：0-左手，1-右手，2-左脚，3-右脚，4-头部
+            rotation: 绝对旋转或相对旋转
+            duration: 旋转持续时间或旋转速度
+            speed_based: 指定duration表示旋转持续时间还是旋转速度
+            relative: 指定position表示绝对旋转还是相对旋转
+
+        Returns:
+            当旋转完成时，self.data['rotate_done']会被置为True
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('HumanIKTargetDoRotate')
+        msg.write_int32(index)
+        msg.write_float32(rotation[0])
+        msg.write_float32(rotation[1])
+        msg.write_float32(rotation[2])
+        msg.write_float32(duration)
+        msg.write_bool(speed_based)
+        msg.write_bool(relative)
+
+        self.env.instance_channel.send_message(msg)
+
+    def HumanIKTargetDoRotateQuaternion(self, index: int, quaternion: list, duration: float, speed_based: bool = True, relative: bool = False):
+        """
+        人体IK目标点四元数旋转
+
+        Args:
+            index: 移动的目标：0-左手，1-右手，2-左脚，3-右脚，4-头部
+            quaternion: 绝对旋转或相对旋转
+            duration: 旋转持续时间或旋转速度
+            speed_based: 指定duration表示旋转持续时间还是旋转速度
+            relative: 指定position表示绝对旋转还是相对旋转
+
+        Returns:
+            当旋转完成时，self.data['rotate_done']会被置为True
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('HumanIKTargetDoRotateQuaternion')
+        msg.write_int32(index)
+        msg.write_float32(quaternion[0])
+        msg.write_float32(quaternion[1])
+        msg.write_float32(quaternion[2])
+        msg.write_float32(quaternion[3])
+        msg.write_float32(duration)
+        msg.write_bool(speed_based)
+        msg.write_bool(relative)
+
+        self.env.instance_channel.send_message(msg)
+
+        self.env.instance_channel.send_message(msg)
+
+    def HumanIKTargetDoComplete(self, index: int):
+        """
+        使人体IK目标点移动/旋转立即完成
+
+        Args:
+            index: 移动的目标：0-左手，1-右手，2-左脚，3-右脚，4-头部
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('HumanIKTargetDoComplete')
+        msg.write_int32(index)
+
+        self.env.instance_channel.send_message(msg)
+
+    def HumanIKTargetDoKill(self, index: int):
+        """
+        使人体IK目标点移动/旋转停止
+
+        Args:
+            index: 移动的目标：0-左手，1-右手，2-左脚，3-右脚，4-头部
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('HumanIKTargetDoKill')
+        msg.write_int32(index)
+
+        self.env.instance_channel.send_message(msg)
+
+    def WaitDo(self):
+        """
+        等待人体IK移动/旋转完成
+        """
+        while not self.data['move_done'] or not self.data['rotate_done']:
+            self.env.step()
+
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/light_attr.py` & `pyrfuniverse-0.8.3/pyrfuniverse/attributes/light_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/pointcloud_attr.py` & `pyrfuniverse-0.8.3/pyrfuniverse/attributes/pointcloud_attr.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import numpy as np
-
-import pyrfuniverse.attributes as attr
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
-
-
-class PointCloudAttr(attr.BaseAttr):
-    """
-    点云渲染类
-    """
-    def parse_message(self, msg: IncomingMessage) -> dict:
-        """
-        解析消息
-
-        Returns:
-
-        """
-        super().parse_message(msg)
-        return self.data
-
-    def ShowPointCloud(self, positions: list = [], colors: list = [], ply_path: str = None, radius: float = 0.01):
-        """
-        显示点云
-
-        Args:
-            positions: 点位置列表
-            colors: 点颜色列表
-            ply_path: .ply文件列表，如果不为空，则positions和colors参数无效
-            radius: 点半径
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('ShowPointCloud')
-        msg.write_bool(ply_path is not None)
-        if ply_path is not None:
-            msg.write_string(ply_path)
-        else:
-            msg.write_float32_list(np.array(positions).reshape(-1).tolist())
-            msg.write_float32_list(np.array(colors).reshape(-1).tolist())
-        msg.write_float32(radius)
-
-        self.env.instance_channel.send_message(msg)
-
-    def SetRadius(self, radius: float):
-        """
-        设置点半径
-
-        Args:
-            radius: 半径
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetRadius')
-        msg.write_float32(radius)
-
+import numpy as np
+
+import pyrfuniverse.attributes as attr
+from pyrfuniverse.side_channel.side_channel import (
+    IncomingMessage,
+    OutgoingMessage,
+)
+
+
+class PointCloudAttr(attr.BaseAttr):
+    """
+    点云渲染类
+    """
+    def parse_message(self, msg: IncomingMessage) -> dict:
+        """
+        解析消息
+
+        Returns:
+
+        """
+        super().parse_message(msg)
+        return self.data
+
+    def ShowPointCloud(self, positions: list = [], colors: list = [], ply_path: str = None, radius: float = 0.01):
+        """
+        显示点云
+
+        Args:
+            positions: 点位置列表
+            colors: 点颜色列表
+            ply_path: .ply文件列表，如果不为空，则positions和colors参数无效
+            radius: 点半径
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('ShowPointCloud')
+        msg.write_bool(ply_path is not None)
+        if ply_path is not None:
+            msg.write_string(ply_path)
+        else:
+            msg.write_float32_list(np.array(positions).reshape(-1).tolist())
+            msg.write_float32_list(np.array(colors).reshape(-1).tolist())
+        msg.write_float32(radius)
+
+        self.env.instance_channel.send_message(msg)
+
+    def SetRadius(self, radius: float):
+        """
+        设置点半径
+
+        Args:
+            radius: 半径
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('SetRadius')
+        msg.write_float32(radius)
+
         self.env.instance_channel.send_message(msg)
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/attributes/rigidbody_attr.py` & `pyrfuniverse-0.8.3/pyrfuniverse/attributes/rigidbody_attr.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-import pyrfuniverse.attributes as attr
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
-import pyrfuniverse.utils.rfuniverse_utility as utility
-
-
-def SetMass(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'mass']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-    msg = OutgoingMessage()
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('SetMass')
-    msg.write_float32(kwargs['mass'])
-
-    return msg
-
-def AddForce(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['id', 'force']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-    msg = OutgoingMessage()
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('AddForce')
-    msg.write_float32(kwargs['force'][0])
-    msg.write_float32(kwargs['force'][1])
-    msg.write_float32(kwargs['force'][2])
-
-    return msg
-
-
-def SetVelocity(kwargs: dict) -> OutgoingMessage:
-    compulsory_params = ['index', 'velocity']
-    optional_params = []
-    utility.CheckKwargs(kwargs, compulsory_params)
-
-    msg = OutgoingMessage()
-
-    msg.write_int32(kwargs['id'])
-    msg.write_string('SetVelocity')
-    msg.write_float32(kwargs['velocity'][0])
-    msg.write_float32(kwargs['velocity'][1])
-    msg.write_float32(kwargs['velocity'][2])
-
-    return msg
-
-class RigidbodyAttr(attr.ColliderAttr):
-    """
-    刚体类
-    """
-    def parse_message(self, msg: IncomingMessage) -> dict:
-        """
-        解析消息
-
-        Returns:
-            self.data['velocity'] 刚体速度 Vecter3
-
-            self.data['angular_vel'] 刚体角速度 Vecter3
-        """
-        super().parse_message(msg)
-        self.data['velocity'] = [msg.read_float32() for _ in range(3)]
-        self.data['angular_vel'] = [msg.read_float32() for _ in range(3)]
-        return self.data
-
-    def SetMass(self, mass: float):
-        """
-        设置刚体质量
-
-        Args:
-            mass: 刚体质量
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetMass')
-        msg.write_float32(mass)
-
-        self.env.instance_channel.send_message(msg)
-
-    def AddForce(self, force: list):
-        """
-        为刚体施加力
-
-        Args:
-            force: 力 Vecter3
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('AddForce')
-        msg.write_float32(force[0])
-        msg.write_float32(force[1])
-        msg.write_float32(force[2])
-
-        self.env.instance_channel.send_message(msg)
-
-    def SetVelocity(self, velocity: list):
-        """
-        设置刚体速度
-
-        Args:
-            velocity: 速度 Vecter3
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetVelocity')
-        msg.write_float32(velocity[0])
-        msg.write_float32(velocity[1])
-        msg.write_float32(velocity[2])
-
+import pyrfuniverse.attributes as attr
+from pyrfuniverse.side_channel.side_channel import (
+    IncomingMessage,
+    OutgoingMessage,
+)
+import pyrfuniverse.utils.rfuniverse_utility as utility
+
+
+def SetMass(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'mass']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+    msg = OutgoingMessage()
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('SetMass')
+    msg.write_float32(kwargs['mass'])
+
+    return msg
+
+def AddForce(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['id', 'force']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+    msg = OutgoingMessage()
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('AddForce')
+    msg.write_float32(kwargs['force'][0])
+    msg.write_float32(kwargs['force'][1])
+    msg.write_float32(kwargs['force'][2])
+
+    return msg
+
+
+def SetVelocity(kwargs: dict) -> OutgoingMessage:
+    compulsory_params = ['index', 'velocity']
+    optional_params = []
+    utility.CheckKwargs(kwargs, compulsory_params)
+
+    msg = OutgoingMessage()
+
+    msg.write_int32(kwargs['id'])
+    msg.write_string('SetVelocity')
+    msg.write_float32(kwargs['velocity'][0])
+    msg.write_float32(kwargs['velocity'][1])
+    msg.write_float32(kwargs['velocity'][2])
+
+    return msg
+
+class RigidbodyAttr(attr.ColliderAttr):
+    """
+    刚体类
+    """
+    def parse_message(self, msg: IncomingMessage) -> dict:
+        """
+        解析消息
+
+        Returns:
+            self.data['velocity'] 刚体速度 Vecter3
+
+            self.data['angular_vel'] 刚体角速度 Vecter3
+        """
+        super().parse_message(msg)
+        self.data['velocity'] = [msg.read_float32() for _ in range(3)]
+        self.data['angular_vel'] = [msg.read_float32() for _ in range(3)]
+        return self.data
+
+    def SetMass(self, mass: float):
+        """
+        设置刚体质量
+
+        Args:
+            mass: 刚体质量
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('SetMass')
+        msg.write_float32(mass)
+
+        self.env.instance_channel.send_message(msg)
+
+    def AddForce(self, force: list):
+        """
+        为刚体施加力
+
+        Args:
+            force: 力 Vecter3
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('AddForce')
+        msg.write_float32(force[0])
+        msg.write_float32(force[1])
+        msg.write_float32(force[2])
+
+        self.env.instance_channel.send_message(msg)
+
+    def SetVelocity(self, velocity: list):
+        """
+        设置刚体速度
+
+        Args:
+            velocity: 速度 Vecter3
+        """
+        msg = OutgoingMessage()
+
+        msg.write_int32(self.id)
+        msg.write_string('SetVelocity')
+        msg.write_float32(velocity[0])
+        msg.write_float32(velocity[1])
+        msg.write_float32(velocity[2])
+
         self.env.instance_channel.send_message(msg)
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/base_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/base_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/__init__.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/agent_action_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/agent_action_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/agent_info_action_pair_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/agent_info_action_pair_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/agent_info_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/agent_info_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/brain_parameters_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/brain_parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/capabilities_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/capabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/command_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/command_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/custom_reset_parameters_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/custom_reset_parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/demonstration_meta_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/demonstration_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/engine_configuration_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/engine_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/header_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/header_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/observation_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/observation_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/space_type_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/space_type_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/training_analytics_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/training_analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_input_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_input_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_message_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_message_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_output_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_output_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_rl_initialization_input_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_initialization_input_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_rl_initialization_output_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_initialization_output_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_rl_input_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_input_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_rl_output_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_output_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_to_external_pb2.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_to_external_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/communicator_objects/unity_to_external_pb2_grpc.py` & `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_to_external_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/env_utils.py` & `pyrfuniverse-0.8.3/pyrfuniverse/env_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/environment.py` & `pyrfuniverse-0.8.3/pyrfuniverse/environment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,503 +1,504 @@
-import atexit
-from distutils.version import StrictVersion
-
-import numpy as np
-import os
-import subprocess
-from typing import Dict, List, Optional, Tuple, Mapping as MappingType
-
-import pyrfuniverse
-
-from pyrfuniverse.logging_util import get_logger
-from pyrfuniverse.side_channel.side_channel import SideChannel
-from pyrfuniverse.side_channel.side_channel_manager import SideChannelManager
-from pyrfuniverse import env_utils
-
-from pyrfuniverse.base_env import (
-    BaseEnv,
-    DecisionSteps,
-    TerminalSteps,
-    BehaviorSpec,
-    ActionTuple,
-    BehaviorName,
-    AgentId,
-    BehaviorMapping,
-)
-from pyrfuniverse.timers import timed, hierarchical_timer
-from pyrfuniverse.exception import (
-    UnityEnvironmentException,
-    UnityActionException,
-    UnityTimeOutException,
-    UnityCommunicatorStoppedException,
-)
-
-from pyrfuniverse.communicator_objects.command_pb2 import STEP, RESET
-from pyrfuniverse.rpc_utils import behavior_spec_from_proto, steps_from_proto
-
-from pyrfuniverse.communicator_objects.unity_rl_input_pb2 import UnityRLInputProto
-from pyrfuniverse.communicator_objects.unity_rl_output_pb2 import UnityRLOutputProto
-from pyrfuniverse.communicator_objects.agent_action_pb2 import AgentActionProto
-from pyrfuniverse.communicator_objects.unity_output_pb2 import UnityOutputProto
-from pyrfuniverse.communicator_objects.capabilities_pb2 import UnityRLCapabilitiesProto
-from pyrfuniverse.communicator_objects.unity_rl_initialization_input_pb2 import (
-    UnityRLInitializationInputProto,
-)
-
-from pyrfuniverse.communicator_objects.unity_input_pb2 import UnityInputProto
-
-from .rpc_communicator import RpcCommunicator
-import signal
-
-logger = get_logger(__name__)
-
-
-class UnityEnvironment(BaseEnv):
-    # Communication protocol version.
-    # When connecting to C#, this must be compatible with Academy.k_ApiVersion.
-    # We follow semantic versioning on the communication version, so existing
-    # functionality will work as long the major versions match.
-    # This should be changed whenever a change is made to the communication protocol.
-    # Revision history:
-    #  * 1.0.0 - initial version
-    #  * 1.1.0 - support concatenated PNGs for compressed observations.
-    #  * 1.2.0 - support compression mapping for stacked compressed observations.
-    #  * 1.3.0 - support action spaces with both continuous and discrete actions.
-    #  * 1.4.0 - support training analytics sent from python trainer to the editor.
-    #  * 1.5.0 - support variable length observation training and multi-agent groups.
-    API_VERSION = "1.5.0"
-
-    # Default port that the editor listens on. If an environment executable
-    # isn't specified, this port will be used.
-    DEFAULT_EDITOR_PORT = 5004
-
-    # Default base port for environments. Each environment will be offset from this
-    # by it's worker_id.
-    BASE_ENVIRONMENT_PORT = 5005
-
-    # Command line argument used to pass the port to the executable environment.
-    _PORT_COMMAND_LINE_ARG = "--mlagents-port"
-
-    @staticmethod
-    def _raise_version_exception(unity_com_ver: str) -> None:
-        raise UnityEnvironmentException(
-            f"The communication API version is not compatible between Unity and python. "
-            f"Python API: {UnityEnvironment.API_VERSION}, Unity API: {unity_com_ver}.\n "
-            f"Please find the versions that work best together from our release page.\n"
-            "https://github.com/Unity-Technologies/ml-agents/releases"
-        )
-
-    @staticmethod
-    def _check_communication_compatibility(
-        unity_com_ver: str, python_api_version: str, unity_package_version: str
-    ) -> bool:
-        unity_communicator_version = StrictVersion(unity_com_ver)
-        api_version = StrictVersion(python_api_version)
-        if unity_communicator_version.version[0] == 0:
-            if (
-                unity_communicator_version.version[0] != api_version.version[0]
-                or unity_communicator_version.version[1] != api_version.version[1]
-            ):
-                # Minor beta versions differ.
-                return False
-        elif unity_communicator_version.version[0] != api_version.version[0]:
-            # Major versions mismatch.
-            return False
-        else:
-            # Major versions match, so either:
-            # 1) The versions are identical, in which case there's no compatibility issues
-            # 2) The Unity version is newer, in which case we'll warn or fail on the Unity side if trying to use
-            #    unsupported features
-            # 3) The trainer version is newer, in which case new trainer features might be available but unused by C#
-            # In any of the cases, there's no reason to warn about mismatch here.
-            logger.info(
-                f"Connected to Unity environment with package version {unity_package_version} "
-                f"and communication version {unity_com_ver}"
-            )
-        return True
-
-    @staticmethod
-    def _get_capabilities_proto() -> UnityRLCapabilitiesProto:
-        capabilities = UnityRLCapabilitiesProto()
-        capabilities.baseRLCapabilities = True
-        capabilities.concatenatedPngObservations = True
-        capabilities.compressedChannelMapping = True
-        capabilities.hybridActions = True
-        capabilities.trainingAnalytics = True
-        capabilities.variableLengthObservation = True
-        capabilities.multiAgentGroups = True
-        return capabilities
-
-    @staticmethod
-    def _warn_csharp_base_capabilities(
-        caps: UnityRLCapabilitiesProto, unity_package_ver: str, python_package_ver: str
-    ) -> None:
-        if not caps.baseRLCapabilities:
-            logger.warning(
-                "WARNING: The Unity process is not running with the expected base Reinforcement Learning"
-                " capabilities. Please be sure upgrade the Unity Package to a version that is compatible with this "
-                "python package.\n"
-                f"Python package version: {python_package_ver}, C# package version: {unity_package_ver}"
-                f"Please find the versions that work best together from our release page.\n"
-                "https://github.com/Unity-Technologies/ml-agents/releases"
-            )
-
-    def __init__(
-        self,
-        file_name: Optional[str] = None,
-        worker_id: int = 0,
-        base_port: Optional[int] = None,
-        seed: int = 0,
-        no_graphics: bool = False,
-        timeout_wait: int = 60,
-        additional_args: Optional[List[str]] = None,
-        side_channels: Optional[List[SideChannel]] = None,
-        log_folder: Optional[str] = None,
-    ):
-        """
-        Starts a new unity environment and establishes a connection with the environment.
-        Notice: Currently communication between Unity and Python takes place over an open socket without authentication.
-        Ensure that the network where training takes place is secure.
-
-        :string file_name: Name of Unity environment binary.
-        :int base_port: Baseline port number to connect to Unity environment over. worker_id increments over this.
-        If no environment is specified (i.e. file_name is None), the DEFAULT_EDITOR_PORT will be used.
-        :int worker_id: Offset from base_port. Used for training multiple environments simultaneously.
-        :bool no_graphics: Whether to run the Unity simulator in no-graphics mode
-        :int timeout_wait: Time (in seconds) to wait for connection from environment.
-        :list args: Addition Unity command line arguments
-        :list side_channels: Additional side channel for no-rl communication with Unity
-        :str log_folder: Optional folder to write the Unity Player log file into.  Requires absolute path.
-        """
-        atexit.register(self._close)
-        self._additional_args = additional_args or []
-        self._no_graphics = no_graphics
-        # If base port is not specified, use BASE_ENVIRONMENT_PORT if we have
-        # an environment, otherwise DEFAULT_EDITOR_PORT
-        if base_port is None:
-            base_port = (
-                self.BASE_ENVIRONMENT_PORT if file_name else self.DEFAULT_EDITOR_PORT
-            )
-        self._port = base_port + worker_id
-        self._buffer_size = 12000
-        # If true, this means the environment was successfully loaded
-        self._loaded = False
-        # The process that is started. If None, no process was started
-        self._process: Optional[subprocess.Popen] = None
-        self._timeout_wait: int = timeout_wait
-        self._communicator = self._get_communicator(worker_id, base_port, timeout_wait)
-        self._worker_id = worker_id
-        self._side_channel_manager = SideChannelManager(side_channels)
-        self._log_folder = log_folder
-        self.academy_capabilities: UnityRLCapabilitiesProto = None  # type: ignore
-
-        # If the environment name is None, a new environment will not be launched
-        # and the communicator will directly try to connect to an existing unity environment.
-        # If the worker-id is not 0 and the environment name is None, an error is thrown
-        if file_name is None and worker_id != 0:
-            raise UnityEnvironmentException(
-                "If the environment name is None, "
-                "the worker-id must be 0 in order to connect with the Editor."
-            )
-        if file_name is not None:
-            try:
-                self._process = env_utils.launch_executable(
-                    file_name, self._executable_args()
-                )
-            except UnityEnvironmentException:
-                self._close(0)
-                raise
-        else:
-            logger.info(
-                f"Listening on port {self._port}. "
-                f"Start training by pressing the Play button in the Unity Editor."
-            )
-        self._loaded = True
-
-        rl_init_parameters_in = UnityRLInitializationInputProto(
-            seed=seed,
-            communication_version=self.API_VERSION,
-            package_version=pyrfuniverse.__version__,
-            capabilities=UnityEnvironment._get_capabilities_proto(),
-        )
-        try:
-            aca_output = self._send_academy_parameters(rl_init_parameters_in)
-            aca_params = aca_output.rl_initialization_output
-        except UnityTimeOutException:
-            self._close(0)
-            raise
-
-        if not UnityEnvironment._check_communication_compatibility(
-            aca_params.communication_version,
-            UnityEnvironment.API_VERSION,
-            aca_params.package_version,
-        ):
-            self._close(0)
-            UnityEnvironment._raise_version_exception(aca_params.communication_version)
-
-        UnityEnvironment._warn_csharp_base_capabilities(
-            aca_params.capabilities,
-            aca_params.package_version,
-            UnityEnvironment.API_VERSION,
-        )
-
-        self._env_state: Dict[str, Tuple[DecisionSteps, TerminalSteps]] = {}
-        self._env_specs: Dict[str, BehaviorSpec] = {}
-        self._env_actions: Dict[str, ActionTuple] = {}
-        self._is_first_message = True
-        self._update_behavior_specs(aca_output)
-        self.academy_capabilities = aca_params.capabilities
-
-    @staticmethod
-    def _get_communicator(worker_id, base_port, timeout_wait):
-        return RpcCommunicator(worker_id, base_port, timeout_wait)
-
-    def _executable_args(self) -> List[str]:
-        args: List[str] = []
-        if self._no_graphics:
-            args += ["-nographics", "-batchmode"]
-        args += [UnityEnvironment._PORT_COMMAND_LINE_ARG, str(self._port)]
-
-        # If the logfile arg isn't already set in the env args,
-        # try to set it to an output directory
-        logfile_set = "-logfile" in (arg.lower() for arg in self._additional_args)
-        if self._log_folder and not logfile_set:
-            log_file_path = os.path.join(
-                self._log_folder, f"Player-{self._worker_id}.log"
-            )
-            args += ["-logFile", log_file_path]
-        # Add in arguments passed explicitly by the user.
-        args += self._additional_args
-        return args
-
-    def _update_behavior_specs(self, output: UnityOutputProto) -> None:
-        init_output = output.rl_initialization_output
-        for brain_param in init_output.brain_parameters:
-            # Each BrainParameter in the rl_initialization_output should have at least one AgentInfo
-            # Get that agent, because we need some of its observations.
-            agent_infos = output.rl_output.agentInfos[brain_param.brain_name]
-            if agent_infos.value:
-                agent = agent_infos.value[0]
-                new_spec = behavior_spec_from_proto(brain_param, agent)
-                self._env_specs[brain_param.brain_name] = new_spec
-                logger.info(f"Connected new brain: {brain_param.brain_name}")
-
-    def _update_state(self, output: UnityRLOutputProto) -> None:
-        """
-        Collects experience information from all external brains in environment at current step.
-        """
-        for brain_name in self._env_specs.keys():
-            if brain_name in output.agentInfos:
-                agent_info_list = output.agentInfos[brain_name].value
-                self._env_state[brain_name] = steps_from_proto(
-                    agent_info_list, self._env_specs[brain_name]
-                )
-            else:
-                self._env_state[brain_name] = (
-                    DecisionSteps.empty(self._env_specs[brain_name]),
-                    TerminalSteps.empty(self._env_specs[brain_name]),
-                )
-        self._side_channel_manager.process_side_channel_message(output.side_channel)
-
-    def reset(self) -> None:
-        if self._loaded:
-            outputs = self._communicator.exchange(
-                self._generate_reset_input(), self._poll_process
-            )
-            if outputs is None:
-                raise UnityCommunicatorStoppedException("Communicator has exited.")
-            self._update_behavior_specs(outputs)
-            rl_output = outputs.rl_output
-            self._update_state(rl_output)
-            self._is_first_message = False
-            self._env_actions.clear()
-        else:
-            raise UnityEnvironmentException("No Unity environment is loaded.")
-
-    @timed
-    def step(self) -> None:
-        if self._is_first_message:
-            return self.reset()
-        if not self._loaded:
-            raise UnityEnvironmentException("No Unity environment is loaded.")
-        # fill the blanks for missing actions
-        for group_name in self._env_specs:
-            if group_name not in self._env_actions:
-                n_agents = 0
-                if group_name in self._env_state:
-                    n_agents = len(self._env_state[group_name][0])
-                self._env_actions[group_name] = self._env_specs[
-                    group_name
-                ].action_spec.empty_action(n_agents)
-        step_input = self._generate_step_input(self._env_actions)
-        with hierarchical_timer("communicator.exchange"):
-            outputs = self._communicator.exchange(step_input, self._poll_process)
-        if outputs is None:
-            raise UnityCommunicatorStoppedException("Communicator has exited.")
-        self._update_behavior_specs(outputs)
-        rl_output = outputs.rl_output
-        self._update_state(rl_output)
-        self._env_actions.clear()
-
-    @property
-    def behavior_specs(self) -> MappingType[str, BehaviorSpec]:
-        return BehaviorMapping(self._env_specs)
-
-    def _assert_behavior_exists(self, behavior_name: str) -> None:
-        if behavior_name not in self._env_specs:
-            raise UnityActionException(
-                f"The group {behavior_name} does not correspond to an existing "
-                f"agent group in the environment"
-            )
-
-    def set_actions(self, behavior_name: BehaviorName, action: ActionTuple) -> None:
-        self._assert_behavior_exists(behavior_name)
-        if behavior_name not in self._env_state:
-            return
-        action_spec = self._env_specs[behavior_name].action_spec
-        num_agents = len(self._env_state[behavior_name][0])
-        action = action_spec._validate_action(action, num_agents, behavior_name)
-        self._env_actions[behavior_name] = action
-
-    def set_action_for_agent(
-        self, behavior_name: BehaviorName, agent_id: AgentId, action: ActionTuple
-    ) -> None:
-        self._assert_behavior_exists(behavior_name)
-        if behavior_name not in self._env_state:
-            return
-        action_spec = self._env_specs[behavior_name].action_spec
-        action = action_spec._validate_action(action, 1, behavior_name)
-        if behavior_name not in self._env_actions:
-            num_agents = len(self._env_state[behavior_name][0])
-            self._env_actions[behavior_name] = action_spec.empty_action(num_agents)
-        try:
-            index = np.where(self._env_state[behavior_name][0].agent_id == agent_id)[0][
-                0
-            ]
-        except IndexError as ie:
-            raise IndexError(
-                "agent_id {} is did not request a decision at the previous step".format(
-                    agent_id
-                )
-            ) from ie
-        if action_spec.continuous_size > 0:
-            self._env_actions[behavior_name].continuous[index] = action.continuous[0, :]
-        if action_spec.discrete_size > 0:
-            self._env_actions[behavior_name].discrete[index] = action.discrete[0, :]
-
-    def get_steps(
-        self, behavior_name: BehaviorName
-    ) -> Tuple[DecisionSteps, TerminalSteps]:
-        self._assert_behavior_exists(behavior_name)
-        return self._env_state[behavior_name]
-
-    def _poll_process(self) -> None:
-        """
-        Check the status of the subprocess. If it has exited, raise a UnityEnvironmentException
-        :return: None
-        """
-        if not self._process:
-            return
-        poll_res = self._process.poll()
-        if poll_res is not None:
-            exc_msg = self._returncode_to_env_message(self._process.returncode)
-            raise UnityEnvironmentException(exc_msg)
-
-    def close(self):
-        """
-        Sends a shutdown signal to the unity environment, and closes the socket connection.
-        """
-        if self._loaded:
-            self._close()
-        else:
-            raise UnityEnvironmentException("No Unity environment is loaded.")
-
-    def _close(self, timeout: Optional[int] = None) -> None:
-        """
-        Close the communicator and environment subprocess (if necessary).
-
-        :int timeout: [Optional] Number of seconds to wait for the environment to shut down before
-            force-killing it.  Defaults to `self.timeout_wait`.
-        """
-        if timeout is None:
-            timeout = self._timeout_wait
-        self._loaded = False
-        self._communicator.close()
-        if self._process is not None:
-            # Wait a bit for the process to shutdown, but kill it if it takes too long
-            try:
-                self._process.wait(timeout=timeout)
-                logger.debug(self._returncode_to_env_message(self._process.returncode))
-            except subprocess.TimeoutExpired:
-                logger.warning("Environment timed out shutting down. Killing...")
-                self._process.kill()
-            # Set to None so we don't try to close multiple times.
-            self._process = None
-
-    @timed
-    def _generate_step_input(
-        self, vector_action: Dict[str, ActionTuple]
-    ) -> UnityInputProto:
-        rl_in = UnityRLInputProto()
-        for b in vector_action:
-            n_agents = len(self._env_state[b][0])
-            if n_agents == 0:
-                continue
-            for i in range(n_agents):
-                action = AgentActionProto()
-                if vector_action[b].continuous is not None:
-                    action.vector_actions_deprecated.extend(
-                        vector_action[b].continuous[i]
-                    )
-                    action.continuous_actions.extend(vector_action[b].continuous[i])
-                if vector_action[b].discrete is not None:
-                    action.vector_actions_deprecated.extend(
-                        vector_action[b].discrete[i]
-                    )
-                    action.discrete_actions.extend(vector_action[b].discrete[i])
-                rl_in.agent_actions[b].value.extend([action])
-                rl_in.command = STEP
-        rl_in.side_channel = bytes(
-            self._side_channel_manager.generate_side_channel_messages()
-        )
-        return self._wrap_unity_input(rl_in)
-
-    def _generate_reset_input(self) -> UnityInputProto:
-        rl_in = UnityRLInputProto()
-        rl_in.command = RESET
-        rl_in.side_channel = bytes(
-            self._side_channel_manager.generate_side_channel_messages()
-        )
-        return self._wrap_unity_input(rl_in)
-
-    def _send_academy_parameters(
-        self, init_parameters: UnityRLInitializationInputProto
-    ) -> UnityOutputProto:
-        inputs = UnityInputProto()
-        inputs.rl_initialization_input.CopyFrom(init_parameters)
-        return self._communicator.initialize(inputs, self._poll_process)
-
-    @staticmethod
-    def _wrap_unity_input(rl_input: UnityRLInputProto) -> UnityInputProto:
-        result = UnityInputProto()
-        result.rl_input.CopyFrom(rl_input)
-        return result
-
-    @staticmethod
-    def _returncode_to_signal_name(returncode: int) -> Optional[str]:
-        """
-        Try to convert return codes into their corresponding signal name.
-        E.g. returncode_to_signal_name(-2) -> "SIGINT"
-        """
-        try:
-            # A negative value -N indicates that the child was terminated by signal N (POSIX only).
-            s = signal.Signals(-returncode)
-            return s.name
-        except Exception:
-            # Should generally be a ValueError, but catch everything just in case.
-            return None
-
-    @staticmethod
-    def _returncode_to_env_message(returncode: int) -> str:
-        signal_name = UnityEnvironment._returncode_to_signal_name(returncode)
-        signal_name = f" ({signal_name})" if signal_name else ""
-        return f"Environment shut down with return code {returncode}{signal_name}."
+import atexit
+from distutils.version import StrictVersion
+
+import numpy as np
+import os
+import subprocess
+from typing import Dict, List, Optional, Tuple, Mapping as MappingType
+
+import pyrfuniverse
+
+from pyrfuniverse.logging_util import get_logger
+from pyrfuniverse.side_channel.side_channel import SideChannel
+from pyrfuniverse.side_channel.side_channel_manager import SideChannelManager
+from pyrfuniverse import env_utils
+
+from pyrfuniverse.base_env import (
+    BaseEnv,
+    DecisionSteps,
+    TerminalSteps,
+    BehaviorSpec,
+    ActionTuple,
+    BehaviorName,
+    AgentId,
+    BehaviorMapping,
+)
+from pyrfuniverse.timers import timed, hierarchical_timer
+from pyrfuniverse.exception import (
+    UnityEnvironmentException,
+    UnityActionException,
+    UnityTimeOutException,
+    UnityCommunicatorStoppedException,
+)
+
+from pyrfuniverse.communicator_objects.command_pb2 import STEP, RESET
+from pyrfuniverse.rpc_utils import behavior_spec_from_proto, steps_from_proto
+
+from pyrfuniverse.communicator_objects.unity_rl_input_pb2 import UnityRLInputProto
+from pyrfuniverse.communicator_objects.unity_rl_output_pb2 import UnityRLOutputProto
+from pyrfuniverse.communicator_objects.agent_action_pb2 import AgentActionProto
+from pyrfuniverse.communicator_objects.unity_output_pb2 import UnityOutputProto
+from pyrfuniverse.communicator_objects.capabilities_pb2 import UnityRLCapabilitiesProto
+from pyrfuniverse.communicator_objects.unity_rl_initialization_input_pb2 import (
+    UnityRLInitializationInputProto,
+)
+
+from pyrfuniverse.communicator_objects.unity_input_pb2 import UnityInputProto
+
+from .rpc_communicator import RpcCommunicator
+import signal
+
+logger = get_logger(__name__)
+
+
+class UnityEnvironment(BaseEnv):
+    # Communication protocol version.
+    # When connecting to C#, this must be compatible with Academy.k_ApiVersion.
+    # We follow semantic versioning on the communication version, so existing
+    # functionality will work as long the major versions match.
+    # This should be changed whenever a change is made to the communication protocol.
+    # Revision history:
+    #  * 1.0.0 - initial version
+    #  * 1.1.0 - support concatenated PNGs for compressed observations.
+    #  * 1.2.0 - support compression mapping for stacked compressed observations.
+    #  * 1.3.0 - support action spaces with both continuous and discrete actions.
+    #  * 1.4.0 - support training analytics sent from python trainer to the editor.
+    #  * 1.5.0 - support variable length observation training and multi-agent groups.
+    API_VERSION = "1.5.0"
+
+    # Default port that the editor listens on. If an environment executable
+    # isn't specified, this port will be used.
+    DEFAULT_EDITOR_PORT = 5004
+
+    # Default base port for environments. Each environment will be offset from this
+    # by it's worker_id.
+    BASE_ENVIRONMENT_PORT = 5005
+
+    # Command line argument used to pass the port to the executable environment.
+    _PORT_COMMAND_LINE_ARG = "--mlagents-port"
+
+    @staticmethod
+    def _raise_version_exception(unity_com_ver: str) -> None:
+        raise UnityEnvironmentException(
+            f"The communication API version is not compatible between Unity and python. "
+            f"Python API: {UnityEnvironment.API_VERSION}, Unity API: {unity_com_ver}.\n "
+            f"Please find the versions that work best together from our release page.\n"
+            "https://github.com/Unity-Technologies/ml-agents/releases"
+        )
+
+    @staticmethod
+    def _check_communication_compatibility(
+        unity_com_ver: str, python_api_version: str, unity_package_version: str
+    ) -> bool:
+        unity_communicator_version = StrictVersion(unity_com_ver)
+        api_version = StrictVersion(python_api_version)
+        if unity_communicator_version.version[0] == 0:
+            if (
+                unity_communicator_version.version[0] != api_version.version[0]
+                or unity_communicator_version.version[1] != api_version.version[1]
+            ):
+                # Minor beta versions differ.
+                return False
+        elif unity_communicator_version.version[0] != api_version.version[0]:
+            # Major versions mismatch.
+            return False
+        else:
+            # Major versions match, so either:
+            # 1) The versions are identical, in which case there's no compatibility issues
+            # 2) The Unity version is newer, in which case we'll warn or fail on the Unity side if trying to use
+            #    unsupported features
+            # 3) The trainer version is newer, in which case new trainer features might be available but unused by C#
+            # In any of the cases, there's no reason to warn about mismatch here.
+            logger.info(
+                f"Connected to Unity environment with package version {unity_package_version} "
+                f"and communication version {unity_com_ver}"
+            )
+        return True
+
+    @staticmethod
+    def _get_capabilities_proto() -> UnityRLCapabilitiesProto:
+        capabilities = UnityRLCapabilitiesProto()
+        capabilities.baseRLCapabilities = True
+        capabilities.concatenatedPngObservations = True
+        capabilities.compressedChannelMapping = True
+        capabilities.hybridActions = True
+        capabilities.trainingAnalytics = True
+        capabilities.variableLengthObservation = True
+        capabilities.multiAgentGroups = True
+        return capabilities
+
+    @staticmethod
+    def _warn_csharp_base_capabilities(
+        caps: UnityRLCapabilitiesProto, unity_package_ver: str, python_package_ver: str
+    ) -> None:
+        if not caps.baseRLCapabilities:
+            logger.warning(
+                "WARNING: The Unity process is not running with the expected base Reinforcement Learning"
+                " capabilities. Please be sure upgrade the Unity Package to a version that is compatible with this "
+                "python package.\n"
+                f"Python package version: {python_package_ver}, C# package version: {unity_package_ver}"
+                f"Please find the versions that work best together from our release page.\n"
+                "https://github.com/Unity-Technologies/ml-agents/releases"
+            )
+
+    def __init__(
+        self,
+        file_name: Optional[str] = None,
+        worker_id: int = 0,
+        base_port: Optional[int] = None,
+        seed: int = 0,
+        no_graphics: bool = False,
+        timeout_wait: int = 60,
+        additional_args: Optional[List[str]] = None,
+        side_channels: Optional[List[SideChannel]] = None,
+        log_folder: Optional[str] = None,
+    ):
+        """
+        Starts a new unity environment and establishes a connection with the environment.
+        Notice: Currently communication between Unity and Python takes place over an open socket without authentication.
+        Ensure that the network where training takes place is secure.
+
+        :string file_name: Name of Unity environment binary.
+        :int base_port: Baseline port number to connect to Unity environment over. worker_id increments over this.
+        If no environment is specified (i.e. file_name is None), the DEFAULT_EDITOR_PORT will be used.
+        :int worker_id: Offset from base_port. Used for training multiple environments simultaneously.
+        :bool no_graphics: Whether to run the Unity simulator in no-graphics mode
+        :int timeout_wait: Time (in seconds) to wait for connection from environment.
+        :list args: Addition Unity command line arguments
+        :list side_channels: Additional side channel for no-rl communication with Unity
+        :str log_folder: Optional folder to write the Unity Player log file into.  Requires absolute path.
+        """
+        atexit.register(self._close)
+        self._additional_args = additional_args or []
+        self._no_graphics = no_graphics
+        # If base port is not specified, use BASE_ENVIRONMENT_PORT if we have
+        # an environment, otherwise DEFAULT_EDITOR_PORT
+        if base_port is None:
+            base_port = (
+                self.BASE_ENVIRONMENT_PORT if file_name else self.DEFAULT_EDITOR_PORT
+            )
+        self._port = base_port + worker_id
+        self._buffer_size = 12000
+        # If true, this means the environment was successfully loaded
+        self._loaded = False
+        # The process that is started. If None, no process was started
+        self._process: Optional[subprocess.Popen] = None
+        self._timeout_wait: int = timeout_wait
+        self._communicator = self._get_communicator(worker_id, base_port, timeout_wait)
+        self._worker_id = worker_id
+        self._side_channel_manager = SideChannelManager(side_channels)
+        self._log_folder = log_folder
+        self.academy_capabilities: UnityRLCapabilitiesProto = None  # type: ignore
+
+        # If the environment name is None, a new environment will not be launched
+        # and the communicator will directly try to connect to an existing unity environment.
+        # If the worker-id is not 0 and the environment name is None, an error is thrown
+        if file_name is None and worker_id != 0:
+            raise UnityEnvironmentException(
+                "If the environment name is None, "
+                "the worker-id must be 0 in order to connect with the Editor."
+            )
+        if file_name is not None:
+            try:
+                self._process = env_utils.launch_executable(
+                    file_name, self._executable_args()
+                )
+            except UnityEnvironmentException:
+                self._close(0)
+                raise
+        else:
+            logger.info(
+                f"Listening on port {self._port}. "
+                f"Start training by pressing the Play button in the Unity Editor."
+            )
+        self._loaded = True
+
+        rl_init_parameters_in = UnityRLInitializationInputProto(
+            seed=seed,
+            communication_version=self.API_VERSION,
+            package_version=pyrfuniverse.__version__,
+            capabilities=UnityEnvironment._get_capabilities_proto(),
+        )
+        try:
+            aca_output = self._send_academy_parameters(rl_init_parameters_in)
+            aca_params = aca_output.rl_initialization_output
+        except UnityTimeOutException:
+            self._close(0)
+            raise
+
+        if not UnityEnvironment._check_communication_compatibility(
+            aca_params.communication_version,
+            UnityEnvironment.API_VERSION,
+            aca_params.package_version,
+        ):
+            self._close(0)
+            UnityEnvironment._raise_version_exception(aca_params.communication_version)
+
+        UnityEnvironment._warn_csharp_base_capabilities(
+            aca_params.capabilities,
+            aca_params.package_version,
+            UnityEnvironment.API_VERSION,
+        )
+
+        self._env_state: Dict[str, Tuple[DecisionSteps, TerminalSteps]] = {}
+        self._env_specs: Dict[str, BehaviorSpec] = {}
+        self._env_actions: Dict[str, ActionTuple] = {}
+        self._is_first_message = True
+        self._update_behavior_specs(aca_output)
+        self.academy_capabilities = aca_params.capabilities
+
+    @staticmethod
+    def _get_communicator(worker_id, base_port, timeout_wait):
+        return RpcCommunicator(worker_id, base_port, timeout_wait)
+
+    def _executable_args(self) -> List[str]:
+        args: List[str] = []
+        if self._no_graphics:
+            args += ["-nographics", "-batchmode"]
+        args += [UnityEnvironment._PORT_COMMAND_LINE_ARG, str(self._port)]
+
+        # If the logfile arg isn't already set in the env args,
+        # try to set it to an output directory
+        logfile_set = "-logfile" in (arg.lower() for arg in self._additional_args)
+        if self._log_folder and not logfile_set:
+            log_file_path = os.path.join(
+                self._log_folder, f"Player-{self._worker_id}.log"
+            )
+            args += ["-logFile", log_file_path]
+        # Add in arguments passed explicitly by the user.
+        args += self._additional_args
+        return args
+
+    def _update_behavior_specs(self, output: UnityOutputProto) -> None:
+        init_output = output.rl_initialization_output
+        for brain_param in init_output.brain_parameters:
+            # Each BrainParameter in the rl_initialization_output should have at least one AgentInfo
+            # Get that agent, because we need some of its observations.
+            agent_infos = output.rl_output.agentInfos[brain_param.brain_name]
+            if agent_infos.value:
+                agent = agent_infos.value[0]
+                new_spec = behavior_spec_from_proto(brain_param, agent)
+                self._env_specs[brain_param.brain_name] = new_spec
+                logger.info(f"Connected new brain: {brain_param.brain_name}")
+
+    def _update_state(self, output: UnityRLOutputProto) -> None:
+        """
+        Collects experience information from all external brains in environment at current step.
+        """
+        for brain_name in self._env_specs.keys():
+            if brain_name in output.agentInfos:
+                agent_info_list = output.agentInfos[brain_name].value
+                self._env_state[brain_name] = steps_from_proto(
+                    agent_info_list, self._env_specs[brain_name]
+                )
+            else:
+                self._env_state[brain_name] = (
+                    DecisionSteps.empty(self._env_specs[brain_name]),
+                    TerminalSteps.empty(self._env_specs[brain_name]),
+                )
+        self._side_channel_manager.process_side_channel_message(output.side_channel)
+
+    def reset(self) -> None:
+        if self._loaded:
+            outputs = self._communicator.exchange(
+                self._generate_reset_input(), self._poll_process
+            )
+            if outputs is None:
+                raise UnityCommunicatorStoppedException("Communicator has exited.")
+            self._update_behavior_specs(outputs)
+            rl_output = outputs.rl_output
+            self._update_state(rl_output)
+            self._is_first_message = False
+            self._env_actions.clear()
+        else:
+            raise UnityEnvironmentException("No Unity environment is loaded.")
+
+    @timed
+    def step(self) -> None:
+        if self._is_first_message:
+            return self.reset()
+        if not self._loaded:
+            raise UnityEnvironmentException("No Unity environment is loaded.")
+        # fill the blanks for missing actions
+        for group_name in self._env_specs:
+            if group_name not in self._env_actions:
+                n_agents = 0
+                if group_name in self._env_state:
+                    n_agents = len(self._env_state[group_name][0])
+                self._env_actions[group_name] = self._env_specs[
+                    group_name
+                ].action_spec.empty_action(n_agents)
+        step_input = self._generate_step_input(self._env_actions)
+        with hierarchical_timer("communicator.exchange"):
+            outputs = self._communicator.exchange(step_input, self._poll_process)
+        if outputs is None:
+            self._close()
+            raise UnityCommunicatorStoppedException("Communicator has exited.")
+        self._update_behavior_specs(outputs)
+        rl_output = outputs.rl_output
+        self._update_state(rl_output)
+        self._env_actions.clear()
+
+    @property
+    def behavior_specs(self) -> MappingType[str, BehaviorSpec]:
+        return BehaviorMapping(self._env_specs)
+
+    def _assert_behavior_exists(self, behavior_name: str) -> None:
+        if behavior_name not in self._env_specs:
+            raise UnityActionException(
+                f"The group {behavior_name} does not correspond to an existing "
+                f"agent group in the environment"
+            )
+
+    def set_actions(self, behavior_name: BehaviorName, action: ActionTuple) -> None:
+        self._assert_behavior_exists(behavior_name)
+        if behavior_name not in self._env_state:
+            return
+        action_spec = self._env_specs[behavior_name].action_spec
+        num_agents = len(self._env_state[behavior_name][0])
+        action = action_spec._validate_action(action, num_agents, behavior_name)
+        self._env_actions[behavior_name] = action
+
+    def set_action_for_agent(
+        self, behavior_name: BehaviorName, agent_id: AgentId, action: ActionTuple
+    ) -> None:
+        self._assert_behavior_exists(behavior_name)
+        if behavior_name not in self._env_state:
+            return
+        action_spec = self._env_specs[behavior_name].action_spec
+        action = action_spec._validate_action(action, 1, behavior_name)
+        if behavior_name not in self._env_actions:
+            num_agents = len(self._env_state[behavior_name][0])
+            self._env_actions[behavior_name] = action_spec.empty_action(num_agents)
+        try:
+            index = np.where(self._env_state[behavior_name][0].agent_id == agent_id)[0][
+                0
+            ]
+        except IndexError as ie:
+            raise IndexError(
+                "agent_id {} is did not request a decision at the previous step".format(
+                    agent_id
+                )
+            ) from ie
+        if action_spec.continuous_size > 0:
+            self._env_actions[behavior_name].continuous[index] = action.continuous[0, :]
+        if action_spec.discrete_size > 0:
+            self._env_actions[behavior_name].discrete[index] = action.discrete[0, :]
+
+    def get_steps(
+        self, behavior_name: BehaviorName
+    ) -> Tuple[DecisionSteps, TerminalSteps]:
+        self._assert_behavior_exists(behavior_name)
+        return self._env_state[behavior_name]
+
+    def _poll_process(self) -> None:
+        """
+        Check the status of the subprocess. If it has exited, raise a UnityEnvironmentException
+        :return: None
+        """
+        if not self._process:
+            return
+        poll_res = self._process.poll()
+        if poll_res is not None:
+            exc_msg = self._returncode_to_env_message(self._process.returncode)
+            raise UnityEnvironmentException(exc_msg)
+
+    def close(self):
+        """
+        Sends a shutdown signal to the unity environment, and closes the socket connection.
+        """
+        if self._loaded:
+            self._close()
+        else:
+            raise UnityEnvironmentException("No Unity environment is loaded.")
+
+    def _close(self, timeout: Optional[int] = None) -> None:
+        """
+        Close the communicator and environment subprocess (if necessary).
+
+        :int timeout: [Optional] Number of seconds to wait for the environment to shut down before
+            force-killing it.  Defaults to `self.timeout_wait`.
+        """
+        if timeout is None:
+            timeout = self._timeout_wait
+        self._loaded = False
+        self._communicator.close()
+        if self._process is not None:
+            # Wait a bit for the process to shutdown, but kill it if it takes too long
+            try:
+                self._process.wait(timeout=timeout)
+                logger.debug(self._returncode_to_env_message(self._process.returncode))
+            except subprocess.TimeoutExpired:
+                logger.warning("Environment timed out shutting down. Killing...")
+                self._process.kill()
+            # Set to None so we don't try to close multiple times.
+            self._process = None
+
+    @timed
+    def _generate_step_input(
+        self, vector_action: Dict[str, ActionTuple]
+    ) -> UnityInputProto:
+        rl_in = UnityRLInputProto()
+        for b in vector_action:
+            n_agents = len(self._env_state[b][0])
+            if n_agents == 0:
+                continue
+            for i in range(n_agents):
+                action = AgentActionProto()
+                if vector_action[b].continuous is not None:
+                    action.vector_actions_deprecated.extend(
+                        vector_action[b].continuous[i]
+                    )
+                    action.continuous_actions.extend(vector_action[b].continuous[i])
+                if vector_action[b].discrete is not None:
+                    action.vector_actions_deprecated.extend(
+                        vector_action[b].discrete[i]
+                    )
+                    action.discrete_actions.extend(vector_action[b].discrete[i])
+                rl_in.agent_actions[b].value.extend([action])
+                rl_in.command = STEP
+        rl_in.side_channel = bytes(
+            self._side_channel_manager.generate_side_channel_messages()
+        )
+        return self._wrap_unity_input(rl_in)
+
+    def _generate_reset_input(self) -> UnityInputProto:
+        rl_in = UnityRLInputProto()
+        rl_in.command = RESET
+        rl_in.side_channel = bytes(
+            self._side_channel_manager.generate_side_channel_messages()
+        )
+        return self._wrap_unity_input(rl_in)
+
+    def _send_academy_parameters(
+        self, init_parameters: UnityRLInitializationInputProto
+    ) -> UnityOutputProto:
+        inputs = UnityInputProto()
+        inputs.rl_initialization_input.CopyFrom(init_parameters)
+        return self._communicator.initialize(inputs, self._poll_process)
+
+    @staticmethod
+    def _wrap_unity_input(rl_input: UnityRLInputProto) -> UnityInputProto:
+        result = UnityInputProto()
+        result.rl_input.CopyFrom(rl_input)
+        return result
+
+    @staticmethod
+    def _returncode_to_signal_name(returncode: int) -> Optional[str]:
+        """
+        Try to convert return codes into their corresponding signal name.
+        E.g. returncode_to_signal_name(-2) -> "SIGINT"
+        """
+        try:
+            # A negative value -N indicates that the child was terminated by signal N (POSIX only).
+            s = signal.Signals(-returncode)
+            return s.name
+        except Exception:
+            # Should generally be a ValueError, but catch everything just in case.
+            return None
+
+    @staticmethod
+    def _returncode_to_env_message(returncode: int) -> str:
+        signal_name = UnityEnvironment._returncode_to_signal_name(returncode)
+        signal_name = f" ({signal_name})" if signal_name else ""
+        return f"Environment shut down with return code {returncode}{signal_name}."
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/__init__.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,401 +1,400 @@
-from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
-# from pyrfuniverse.envs.base_env import RFUniverseGymWrapper
-# from pyrfuniverse.envs.base_env import RFUniverseGymGoalWrapper
-# from pyrfuniverse.envs.franka_grasp_env import FrankaGraspEnv
-# from pyrfuniverse.envs.franka_push_env import FrankaPushEnv
-# from pyrfuniverse.envs.balance_ball_env import BalanceBallEnv
-# from pyrfuniverse.envs.balance_ball_env import BalanceBallEnvV0
-# from pyrfuniverse.envs.bouncer_env import BouncerEnv
-# from pyrfuniverse.envs.bouncer_env import BouncerEnvV0
-# from pyrfuniverse.envs.roller_env import RollerEnv
-# from pyrfuniverse.envs.roller_env import RollerEnvV0
-# from pyrfuniverse.envs.gripper_nail import NailCardEnv
-# from pyrfuniverse.envs.gripper_nail import NailCanEnv
-# from pyrfuniverse.envs.multi_agent_navigation_env import MultiAgentNavigationEnv
-# from pyrfuniverse.envs.tobor_robotiq85_manipulation_env import ToborRobotiq85ManipulationEnv
-# from pyrfuniverse.envs.ur5_box_env import Ur5BoxEnv
-# from pyrfuniverse.envs.ur5_drawer_env import Ur5DrawerEnv
-
-# Other projects based on RFUniverse
-# import pyrfuniverse.envs.robotube
-# import pyrfuniverse.envs.rcareworld
-
-__all__ = [
-    'RFUniverseBaseEnv',
-    # 'FrankaGraspEnv', 'FrankaPushEnv', 'BalanceBallEnv',
-    # 'RFUniverseGymWrapper', 'BalanceBallEnvV0', 'RFUniverseGymGoalWrapper',
-    # 'BouncerEnv', 'BouncerEnvV0', 'RollerEnv', 'RollerEnvV0', 'NailCardEnv',
-    # 'MultiAgentNavigationEnv', 'ToborRobotiq85ManipulationEnv', 'Ur5BoxEnv',
-    # 'Ur5DrawerEnv',
-]
-
-
-rfuniverse_build_base_root = '/home/haoyuan/workspace/rfuniverse/rfuniverse/rfuniverse_build/'
-
-try:
-    from gym.envs.registration import register
-
-    register(
-        id='BalanceBallEnv-v0',
-        entry_point='pyrfuniverse.envs:BalanceBallEnvV0'
-    )
-
-    register(
-        id='BouncerEnv-v0',
-        entry_point='pyrfuniverse.envs:BouncerEnvV0'
-    )
-
-    register(
-        id='RollerEnv-v0',
-        entry_point='pyrfuniverse.envs:RollerEnvV0'
-    )
-
-    register(
-        id='MultiAgentNavigation-v1',
-        entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'num_agents': 5,
-        },
-    )
-
-    register(
-        id='MultiAgentNavigation-v2',
-        entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'num_agents': 5,
-            'reset_on_collision': True
-        },
-    )
-
-    register(
-        id='MultiAgentNavigation-v3',
-        entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'num_agents': 3,
-        },
-    )
-
-    register(
-        id='MultiAgentNavigation-v4',
-        entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'num_agents': 3,
-            'reset_on_collision': True
-        },
-    )
-
-    # Franka robotics
-    for reward_type in ['sparse', 'dense']:
-        suffix = 'Dense' if reward_type == 'dense' else ''
-        kwargs = {
-            'executable_file': rfuniverse_build_base_root + 'FrankaRoboticsServer/RFUniverse.x86_64',
-            'max_episode_length': 50,
-            'reward_type': reward_type,
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody'
-        }
-
-        register(
-            id='FrankaPickAndPlace{}-v1'.format(suffix),
-            entry_point='pyrfuniverse.envs.robotics:FrankaPickAndPlaceEnv',
-            kwargs=kwargs,
-            max_episode_steps=50,
-        )
-
-        register(
-            id='FrankaReach{}-v1'.format(suffix),
-            entry_point='pyrfuniverse.envs.robotics:FrankaReachEnv',
-            kwargs=kwargs,
-            max_episode_steps=50,
-        )
-
-        register(
-            id='FrankaPush{}-v1'.format(suffix),
-            entry_point='pyrfuniverse.envs.robotics:FrankaPushEnv',
-            kwargs=kwargs,
-            max_episode_steps=50,
-        )
-
-    # Franka-Cloth env
-    franka_cloth_kwargs = {
-        'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/obi_cloth',
-        'executable_file': rfuniverse_build_base_root + 'FrankaCloth/RFUniverse.x86_64',
-        'reward_type': 'dense'
-    }
-    register(
-        id='FrankaCloth-v1',
-        entry_point='pyrfuniverse.envs.robotics:FrankaClothEnv',
-        kwargs=franka_cloth_kwargs,
-        max_episode_steps=50
-    )
-
-    # Franka-Softbody env
-    franka_softbody_kwargs = {
-        'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/softbody',
-        # 'executable_file': rfuniverse_build_base_root + 'FrankaSoftbodyServer/RFUniverse.x86_64',
-        'executable_file': None,
-        'reward_type': 'sparse'
-    }
-    register(
-        id='FrankaSoftbody-v1',
-        entry_point='pyrfuniverse.envs.robotics:FrankaSoftbodyEnv',
-        kwargs=franka_softbody_kwargs,
-        max_episode_steps=50
-    )
-
-    # Franka-ClothFold env
-    franka_cloth_fold_kwargs = {
-        'asset_bundle_file': '/home/haoyuan/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/obi_cloth',
-        # 'executable_file': rfuniverse_build_base_root + 'FrankaClothFoldServer/RFUniverse.x86_64',
-        'executable_file': None,
-        'reward_type': 'sparse'
-    }
-    register(
-        id='FrankaClothFold-v1',
-        entry_point='pyrfuniverse.envs.robotics:FrankaClothFoldEnv',
-        kwargs=franka_cloth_fold_kwargs,
-        max_episode_steps=20
-    )
-
-    # A relatively easy and naive NailCard environment
-    register(
-        id='NailCard-v1',
-        entry_point='pyrfuniverse.envs:NailCardEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'NailCardServer/RFUniverse.x86_64',
-            'rotation_factor': 0,
-            'goal_baseline': 0.02,
-        },
-        max_episode_steps=50,
-    )
-
-    # The normal version
-    register(
-        id='NailCard-v2',
-        entry_point='pyrfuniverse.envs:NailCardEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'NailCardServer/RFUniverse.x86_64',
-        },
-        max_episode_steps=50,
-    )
-
-    # Fixed the nail movement
-    register(
-        id='NailCard-v3',
-        entry_point='pyrfuniverse.envs:NailCardEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'NailCardServer/RFUniverse.x86_64',
-            'nail_movement_factor': 0
-        },
-        max_episode_steps=50,
-    )
-
-    # A relatively easy and naive NailCard environment
-    register(
-        id='Robotiq85NailCard-v1',
-        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCardEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCardServer/RFUniverse.x86_64',
-            'rotation_factor': 0,
-            'goal_baseline': 0.02,
-        },
-        max_episode_steps=50,
-    )
-
-    # The normal version
-    register(
-        id='Robotiq85NailCard-v2',
-        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCardEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCardServer/RFUniverse.x86_64',
-        },
-        max_episode_steps=50,
-    )
-
-    # Fixed the nail movement
-    register(
-        id='Robotiq85NailCard-v3',
-        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCardEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCardServer/RFUniverse.x86_64',
-            'vertical_movement_factor': 0.02,
-            'nail_movement_factor': 0
-        },
-        max_episode_steps=50,
-    )
-
-    # Robotiq85 Nail Coin
-    register(
-        id='Robotiq85NailCoin-v1',
-        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCoinEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCoinServer/RFUniverse.x86_64',
-            'vertical_movement_factor': 0.02,
-            'nail_movement_factor': 0
-        },
-        max_episode_steps=50,
-    )
-
-    # Nail-Can environment
-    register(
-        id='NailCan-v1',
-        entry_point='pyrfuniverse.envs:NailCanEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'NailCanServer/RFUniverse.x86_64',
-        }
-    )
-
-    register(
-        id='Robotiq85NailCan-v1',
-        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCanEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCanServer/RFUniverse.x86_64',
-        }
-    )
-
-    register(
-        id='Robotiq85NailBook-v1',
-        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailBookEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailBook/RFUniverse.x86_64',
-        }
-    )
-
-    # Robotiq85 insert
-    register(
-        id='Robotiq85Insert-v1',
-        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85InsertEnv',
-        kwargs={
-            'executable_file': rfuniverse_build_base_root + 'Robotiq85InsertServer/RFUniverse.x86_64',
-        }
-    )
-
-    register(
-        id='Cleaner-v1',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'executable_file': rfuniverse_build_base_root + 'CleanerServer/RFUniverse.x86_64'
-        }
-    )
-
-    register(
-        id='Cleaner-v2',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'reset_on_collision': False,
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'executable_file': rfuniverse_build_base_root + 'CleanerServer/RFUniverse.x86_64',
-        }
-    )
-
-    register(
-        id='Cleaner-v3',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64'
-        }
-    )
-
-    register(
-        id='Cleaner-v4',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'reset_on_collision': False,
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64'
-        }
-    )
-
-    register(
-        id='Cleaner-v5',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64',
-            'velocity_reward': True
-        }
-    )
-
-    register(
-        id='Cleaner-v6',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64',
-            'velocity_reward': True,
-            'collision_multiplier': 50,
-        }
-    )
-
-    register(
-        id='Cleaner-v7',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'asset_bundle_file': '/home/haoyuan/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/rigidbody',
-            # 'executable_file': rfuniverse_build_base_root + 'CleanerWithWall/RFUniverse.x86_64',
-            'executable_file': None,
-            'velocity_reward': True,
-            'collision_multiplier': 50,
-            'obs_type': 'box',
-            'max_episode_length': 200
-        }
-    )
-
-    register(
-        id='Cleaner-v8',
-        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
-        kwargs={
-            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
-            'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64',
-            'grid_reward_per_step': True
-        }
-    )
-
-    register(
-        id='UR5Box-v1',
-        entry_point='pyrfuniverse.envs:Ur5BoxEnv',
-        kwargs={
-            'max_steps': 50,
-            'reward_type': 'sparse',
-            'min_open_angle': 30,
-            'executable_file': rfuniverse_build_base_root + 'UR5Box/RFUniverse.x86_64'
-        },
-        max_episode_steps=50,
-    )
-
-    register(
-        id='ToborPull-v1',
-        entry_point='pyrfuniverse.envs.tobor_robotics:ToborPushPullEnv',
-        kwargs={
-            'max_steps': 100,
-            'asset_bundle_file': '/home/haoyuan/workspace/rfuniverse/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/articulation',
-            'pull': True,
-            'executable_file': rfuniverse_build_base_root + 'ToborPushPull/RFUniverse.x86_64'
-        },
-        max_episode_steps=100
-    )
-
-    register(
-        id='ToborPush-v1',
-        entry_point='pyrfuniverse.envs.tobor_robotics:ToborPushPullEnv',
-        kwargs={
-            'max_steps': 100,
-            'asset_bundle_file': '/home/haoyuan/workspace/rfuniverse/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/articulation',
-            'pull': False,
-            'executable_file': rfuniverse_build_base_root + 'ToborPushPull/RFUniverse.x86_64'
-        },
-        max_episode_steps=100
-    )
-
-except ImportError:
-    print('No gym installed. Please install gym!')
-    pass
+from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
+from pyrfuniverse.envs.base_env import RFUniverseGymWrapper
+from pyrfuniverse.envs.base_env import RFUniverseGymGoalWrapper
+# from pyrfuniverse.envs.franka_grasp_env import FrankaGraspEnv
+# from pyrfuniverse.envs.franka_push_env import FrankaPushEnv
+# from pyrfuniverse.envs.balance_ball_env import BalanceBallEnv
+# from pyrfuniverse.envs.balance_ball_env import BalanceBallEnvV0
+# from pyrfuniverse.envs.bouncer_env import BouncerEnv
+# from pyrfuniverse.envs.bouncer_env import BouncerEnvV0
+# from pyrfuniverse.envs.roller_env import RollerEnv
+# from pyrfuniverse.envs.roller_env import RollerEnvV0
+# from pyrfuniverse.envs.gripper_nail import NailCardEnv
+# from pyrfuniverse.envs.gripper_nail import NailCanEnv
+# from pyrfuniverse.envs.multi_agent_navigation_env import MultiAgentNavigationEnv
+# from pyrfuniverse.envs.tobor_robotiq85_manipulation_env import ToborRobotiq85ManipulationEnv
+# from pyrfuniverse.envs.ur5_box_env import Ur5BoxEnv
+# from pyrfuniverse.envs.ur5_drawer_env import Ur5DrawerEnv
+
+# Other projects based on RFUniverse
+# import pyrfuniverse.envs.robotube
+# import pyrfuniverse.envs.rcareworld
+
+__all__ = [
+    'RFUniverseBaseEnv', 'FrankaGraspEnv', 'FrankaPushEnv', 'BalanceBallEnv',
+    'RFUniverseGymWrapper', 'BalanceBallEnvV0', 'RFUniverseGymGoalWrapper',
+    'BouncerEnv', 'BouncerEnvV0', 'RollerEnv', 'RollerEnvV0', 'NailCardEnv',
+    'MultiAgentNavigationEnv', 'ToborRobotiq85ManipulationEnv', 'Ur5BoxEnv',
+    'Ur5DrawerEnv',
+]
+
+
+rfuniverse_build_base_root = '/home/haoyuan/workspace/rfuniverse/rfuniverse/rfuniverse_build/'
+
+try:
+    from gym.envs.registration import register
+
+    register(
+        id='BalanceBallEnv-v0',
+        entry_point='pyrfuniverse.envs:BalanceBallEnvV0'
+    )
+
+    register(
+        id='BouncerEnv-v0',
+        entry_point='pyrfuniverse.envs:BouncerEnvV0'
+    )
+
+    register(
+        id='RollerEnv-v0',
+        entry_point='pyrfuniverse.envs:RollerEnvV0'
+    )
+
+    register(
+        id='MultiAgentNavigation-v1',
+        entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
+        kwargs={
+            'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
+            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+            'num_agents': 5,
+        },
+    )
+
+    register(
+        id='MultiAgentNavigation-v2',
+        entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
+        kwargs={
+            'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
+            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+            'num_agents': 5,
+            'reset_on_collision': True
+        },
+    )
+
+    register(
+        id='MultiAgentNavigation-v3',
+        entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
+        kwargs={
+            'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
+            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+            'num_agents': 3,
+        },
+    )
+
+    register(
+        id='MultiAgentNavigation-v4',
+        entry_point='pyrfuniverse.envs:MultiAgentNavigationEnv',
+        kwargs={
+            'executable_file': rfuniverse_build_base_root + 'MultiAgentNavigationServer/RFUniverse.x86_64',
+            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+            'num_agents': 3,
+            'reset_on_collision': True
+        },
+    )
+
+    # Franka robotics
+    for reward_type in ['sparse', 'dense']:
+        suffix = 'Dense' if reward_type == 'dense' else ''
+        kwargs = {
+            'executable_file': rfuniverse_build_base_root + 'FrankaRoboticsServer/RFUniverse.x86_64',
+            'max_episode_length': 50,
+            'reward_type': reward_type,
+            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody'
+        }
+
+        register(
+            id='FrankaPickAndPlace{}-v1'.format(suffix),
+            entry_point='pyrfuniverse.envs.robotics:FrankaPickAndPlaceEnv',
+            kwargs=kwargs,
+            max_episode_steps=50,
+        )
+
+        register(
+            id='FrankaReach{}-v1'.format(suffix),
+            entry_point='pyrfuniverse.envs.robotics:FrankaReachEnv',
+            kwargs=kwargs,
+            max_episode_steps=50,
+        )
+
+        register(
+            id='FrankaPush{}-v1'.format(suffix),
+            entry_point='pyrfuniverse.envs.robotics:FrankaPushEnv',
+            kwargs=kwargs,
+            max_episode_steps=50,
+        )
+
+    # Franka-Cloth env
+    franka_cloth_kwargs = {
+        'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/obi_cloth',
+        'executable_file': rfuniverse_build_base_root + 'FrankaCloth/RFUniverse.x86_64',
+        'reward_type': 'dense'
+    }
+    register(
+        id='FrankaCloth-v1',
+        entry_point='pyrfuniverse.envs.robotics:FrankaClothEnv',
+        kwargs=franka_cloth_kwargs,
+        max_episode_steps=50
+    )
+
+    # Franka-Softbody env
+    franka_softbody_kwargs = {
+        'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/softbody',
+        # 'executable_file': rfuniverse_build_base_root + 'FrankaSoftbodyServer/RFUniverse.x86_64',
+        'executable_file': None,
+        'reward_type': 'sparse'
+    }
+    register(
+        id='FrankaSoftbody-v1',
+        entry_point='pyrfuniverse.envs.robotics:FrankaSoftbodyEnv',
+        kwargs=franka_softbody_kwargs,
+        max_episode_steps=50
+    )
+
+    # Franka-ClothFold env
+    franka_cloth_fold_kwargs = {
+        'asset_bundle_file': '/home/haoyuan/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/obi_cloth',
+        # 'executable_file': rfuniverse_build_base_root + 'FrankaClothFoldServer/RFUniverse.x86_64',
+        'executable_file': None,
+        'reward_type': 'sparse'
+    }
+    register(
+        id='FrankaClothFold-v1',
+        entry_point='pyrfuniverse.envs.robotics:FrankaClothFoldEnv',
+        kwargs=franka_cloth_fold_kwargs,
+        max_episode_steps=20
+    )
+
+    # A relatively easy and naive NailCard environment
+    register(
+        id='NailCard-v1',
+        entry_point='pyrfuniverse.envs:NailCardEnv',
+        kwargs={
+            'executable_file': rfuniverse_build_base_root + 'NailCardServer/RFUniverse.x86_64',
+            'rotation_factor': 0,
+            'goal_baseline': 0.02,
+        },
+        max_episode_steps=50,
+    )
+
+    # The normal version
+    register(
+        id='NailCard-v2',
+        entry_point='pyrfuniverse.envs:NailCardEnv',
+        kwargs={
+            'executable_file': rfuniverse_build_base_root + 'NailCardServer/RFUniverse.x86_64',
+        },
+        max_episode_steps=50,
+    )
+
+    # Fixed the nail movement
+    register(
+        id='NailCard-v3',
+        entry_point='pyrfuniverse.envs:NailCardEnv',
+        kwargs={
+            'executable_file': rfuniverse_build_base_root + 'NailCardServer/RFUniverse.x86_64',
+            'nail_movement_factor': 0
+        },
+        max_episode_steps=50,
+    )
+
+    # A relatively easy and naive NailCard environment
+    register(
+        id='Robotiq85NailCard-v1',
+        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCardEnv',
+        kwargs={
+            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCardServer/RFUniverse.x86_64',
+            'rotation_factor': 0,
+            'goal_baseline': 0.02,
+        },
+        max_episode_steps=50,
+    )
+
+    # The normal version
+    register(
+        id='Robotiq85NailCard-v2',
+        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCardEnv',
+        kwargs={
+            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCardServer/RFUniverse.x86_64',
+        },
+        max_episode_steps=50,
+    )
+
+    # Fixed the nail movement
+    register(
+        id='Robotiq85NailCard-v3',
+        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCardEnv',
+        kwargs={
+            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCardServer/RFUniverse.x86_64',
+            'vertical_movement_factor': 0.02,
+            'nail_movement_factor': 0
+        },
+        max_episode_steps=50,
+    )
+
+    # Robotiq85 Nail Coin
+    register(
+        id='Robotiq85NailCoin-v1',
+        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCoinEnv',
+        kwargs={
+            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCoinServer/RFUniverse.x86_64',
+            'vertical_movement_factor': 0.02,
+            'nail_movement_factor': 0
+        },
+        max_episode_steps=50,
+    )
+
+    # Nail-Can environment
+    register(
+        id='NailCan-v1',
+        entry_point='pyrfuniverse.envs:NailCanEnv',
+        kwargs={
+            'executable_file': rfuniverse_build_base_root + 'NailCanServer/RFUniverse.x86_64',
+        }
+    )
+
+    register(
+        id='Robotiq85NailCan-v1',
+        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailCanEnv',
+        kwargs={
+            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailCanServer/RFUniverse.x86_64',
+        }
+    )
+
+    register(
+        id='Robotiq85NailBook-v1',
+        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85NailBookEnv',
+        kwargs={
+            'executable_file': rfuniverse_build_base_root + 'Robotiq85NailBook/RFUniverse.x86_64',
+        }
+    )
+
+    # Robotiq85 insert
+    register(
+        id='Robotiq85Insert-v1',
+        entry_point='pyrfuniverse.envs.gripper_nail:Robotiq85InsertEnv',
+        kwargs={
+            'executable_file': rfuniverse_build_base_root + 'Robotiq85InsertServer/RFUniverse.x86_64',
+        }
+    )
+
+    register(
+        id='Cleaner-v1',
+        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+        kwargs={
+            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+            'executable_file': rfuniverse_build_base_root + 'CleanerServer/RFUniverse.x86_64'
+        }
+    )
+
+    register(
+        id='Cleaner-v2',
+        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+        kwargs={
+            'reset_on_collision': False,
+            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+            'executable_file': rfuniverse_build_base_root + 'CleanerServer/RFUniverse.x86_64',
+        }
+    )
+
+    register(
+        id='Cleaner-v3',
+        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+        kwargs={
+            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+            'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64'
+        }
+    )
+
+    register(
+        id='Cleaner-v4',
+        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+        kwargs={
+            'reset_on_collision': False,
+            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+            'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64'
+        }
+    )
+
+    register(
+        id='Cleaner-v5',
+        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+        kwargs={
+            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+            'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64',
+            'velocity_reward': True
+        }
+    )
+
+    register(
+        id='Cleaner-v6',
+        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+        kwargs={
+            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+            'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64',
+            'velocity_reward': True,
+            'collision_multiplier': 50,
+        }
+    )
+
+    register(
+        id='Cleaner-v7',
+        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+        kwargs={
+            'asset_bundle_file': '/home/haoyuan/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/rigidbody',
+            # 'executable_file': rfuniverse_build_base_root + 'CleanerWithWall/RFUniverse.x86_64',
+            'executable_file': None,
+            'velocity_reward': True,
+            'collision_multiplier': 50,
+            'obs_type': 'box',
+            'max_episode_length': 200
+        }
+    )
+
+    register(
+        id='Cleaner-v8',
+        entry_point='pyrfuniverse.envs.multi_agent:CleanerEnv',
+        kwargs={
+            'asset_bundle_file': rfuniverse_build_base_root + 'AssetBundles/rigidbody',
+            'executable_file': rfuniverse_build_base_root + 'CleanerWithWallServer/RFUniverse.x86_64',
+            'grid_reward_per_step': True
+        }
+    )
+
+    register(
+        id='UR5Box-v1',
+        entry_point='pyrfuniverse.envs:Ur5BoxEnv',
+        kwargs={
+            'max_steps': 50,
+            'reward_type': 'sparse',
+            'min_open_angle': 30,
+            'executable_file': rfuniverse_build_base_root + 'UR5Box/RFUniverse.x86_64'
+        },
+        max_episode_steps=50,
+    )
+
+    register(
+        id='ToborPull-v1',
+        entry_point='pyrfuniverse.envs.tobor_robotics:ToborPushPullEnv',
+        kwargs={
+            'max_steps': 100,
+            'asset_bundle_file': '/home/haoyuan/workspace/rfuniverse/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/articulation',
+            'pull': True,
+            'executable_file': rfuniverse_build_base_root + 'ToborPushPull/RFUniverse.x86_64'
+        },
+        max_episode_steps=100
+    )
+
+    register(
+        id='ToborPush-v1',
+        entry_point='pyrfuniverse.envs.tobor_robotics:ToborPushPullEnv',
+        kwargs={
+            'max_steps': 100,
+            'asset_bundle_file': '/home/haoyuan/workspace/rfuniverse/rfuniverse/RFUniverse/Assets/AssetBundles/Linux/articulation',
+            'pull': False,
+            'executable_file': rfuniverse_build_base_root + 'ToborPushPull/RFUniverse.x86_64'
+        },
+        max_episode_steps=100
+    )
+
+except ImportError:
+    print('No gym installed. Please install gym!')
+    pass
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/balance_ball_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/balance_ball_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/base_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/base_env.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,769 +1,795 @@
-import random
-from abc import ABC
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
-import pyrfuniverse
-from pyrfuniverse.environment import UnityEnvironment
-from pyrfuniverse.side_channel.environment_parameters_channel import EnvironmentParametersChannel
-from pyrfuniverse.rfuniverse_channel import AssetChannel
-from pyrfuniverse.rfuniverse_channel import AssetChannelExt
-from pyrfuniverse.rfuniverse_channel import InstanceChannel
-from pyrfuniverse.rfuniverse_channel import DebugChannel
-import pyrfuniverse.attributes as attr
-#import gym
-import os
-
-
-def select_available_worker_id():
-    if not os.path.exists(pyrfuniverse.user_path):
-        os.makedirs(pyrfuniverse.user_path)
-    log_file = os.path.join(pyrfuniverse.user_path, 'worker_id_log')
-
-    worker_id = 1
-    worker_id_in_use = []
-    if os.path.exists(log_file):
-        with open(log_file, 'r') as f:
-            worker_ids = f.readlines()
-            for line in worker_ids:
-                worker_id_in_use.append(int(line))
-        while worker_id in worker_id_in_use:
-            worker_id += 1
-
-    worker_id_in_use.append(worker_id)
-    with open(log_file, 'w') as f:
-        for id in worker_id_in_use:
-            f.write(str(id) + '\n')
-
-    return worker_id
-
-
-def delete_worker_id(worker_id):
-    log_file = os.path.join(pyrfuniverse.user_path, 'worker_id_log')
-
-    worker_id_in_use = []
-    if os.path.exists(log_file):
-        with open(log_file, 'r') as f:
-            worker_ids = f.readlines()
-            for line in worker_ids:
-                worker_id_in_use.append(int(line))
-
-    worker_id_in_use.remove(worker_id)
-    with open(log_file, 'w') as f:
-        for id in worker_id_in_use:
-            f.write(str(id) + '\n')
-
-
-class RFUniverseBaseEnv(ABC):
-    """
-    RFUnivers基础环境类
-    """
-    metadata = {'render.modes': ['human', 'rgb_array']}
-
-    def __init__(
-        self,
-        executable_file: str = None,
-        scene_file: str = None,
-        custom_channels: list = [],
-        assets: list = [],
-        graphics: bool = True,
-        **kwargs
-    ):
-        # time step
-        self.t = 0
-        self.worker_id = select_available_worker_id()
-        # initialize rfuniverse channels
-        self.channels = custom_channels.copy()
-        self._init_channels(kwargs)
-        self.assets = assets
-        # initialize environment
-        self.executable_file = executable_file
-        self.scene_file = scene_file
-        self.graphics = graphics
-        self.attrs = {}
-        self.data = {}
-        self.ext = AssetChannelExt(self)
-        self._init_env()
-
-    def _init_env(self):
-        if str(self.executable_file).lower() == '@editor':
-            self.env = UnityEnvironment(
-                worker_id=0,
-                side_channels=self.channels,
-                no_graphics=not self.graphics,
-            )
-        elif self.executable_file is not None:
-            self.env = UnityEnvironment(
-                worker_id=self.worker_id,
-                file_name=self.executable_file,
-                side_channels=self.channels,
-                no_graphics=not self.graphics,
-            )
-        elif os.path.exists(pyrfuniverse.executable_file):
-            self.env = UnityEnvironment(
-                worker_id=self.worker_id,
-                file_name=pyrfuniverse.executable_file,
-                side_channels=self.channels,
-                no_graphics=not self.graphics,
-            )
-        else:
-            self.env = UnityEnvironment(
-                worker_id=0,
-                side_channels=self.channels,
-                no_graphics=not self.graphics,
-            )
-        self._SendVersion()
-        if self.scene_file is not None:
-            self.LoadSceneAsync(self.scene_file, True)
-        if len(self.assets) > 0:
-            self._PreLoadAssetsAsync(self.assets, True)
-        self.env.reset()
-
-    def _init_channels(self, kwargs: dict):
-        # Compulsory channels
-        # Environment parameters channel
-        self.env_param_channel = EnvironmentParametersChannel()
-        self.channels.append(self.env_param_channel)
-        # RFUniverse channel
-        self.asset_channel = AssetChannel(self, 'd587efc8-9eb7-11ec-802a-18c04d443e7d')
-        self.instance_channel = InstanceChannel(self, '09bfcf57-9120-43dc-99f8-abeeec59df0f')
-        self.debug_channel = DebugChannel(self, '02ac5776-6a7c-54e4-011d-b4c4723831c9')
-        self.channels.append(self.asset_channel)
-        self.channels.append(self.instance_channel)
-        self.channels.append(self.debug_channel)
-
-    def _step(self):
-        self.env.step()
-
-    def step(self, count: int = 1):
-        """
-        将已经调用的接口消息发送给Unity，执行一步仿真，然后接收Unity返回的数据
-
-        Args:
-            count: 执行的步数
-        """
-        if count < 1:
-            count = 1
-        for _ in range(count):
-            self.env.step()
-
-    def close(self):
-        """
-        关闭环境
-        """
-        delete_worker_id(self.worker_id)
-        self.env.close()
-
-    def GetAttr(self, id: int):
-        """
-        根据ID获取物体
-
-        Args:
-            id: 物体ID
-        """
-        if id not in self.attrs:
-            self.attrs[id] = attr.BaseAttr(self, id)
-        return self.attrs[id]
-
-    #Env API
-    def _PreLoadAssetsAsync(self, names: list, auto_wait: bool = False) -> None:
-        msg = OutgoingMessage()
-
-        msg.write_string('PreLoadAssetsAsync')
-        count = len(names)
-        msg.write_int32(count)
-        for i in range(count):
-            msg.write_string(names[i])
-
-        self.asset_channel.send_message(msg)
-
-        if auto_wait:
-            self.WaitLoadDone()
-
-
-    def LoadSceneAsync(self, file: str, auto_wait: bool = False) -> None:
-        """
-        异步加载场景
-
-        Args:
-            file: 场景Json文件，当该值为路径时，从路径加载场景，否则从StreamingAssets加载场景
-            auto_wait: 是否等待加载完成，如果为True，则在加载完成后才返回
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('LoadSceneAsync')
-        msg.write_string(file)
-
-        self.asset_channel.send_message(msg)
-
-        if auto_wait:
-            self.WaitLoadDone()
-
-    def WaitLoadDone(self) -> None:
-        """
-        等待加载完成，使用LoadSceneAsync接口后，调用该接口可以等待加载完成
-        """
-        self.asset_channel.data['load_done'] = False
-        while not self.asset_channel.data['load_done']:
-            self.env.step()
-
-    def Pend(self) -> None:
-        """
-        挂起，直到UnityPlayer中点击EndPend按钮
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('Pend')
-
-        self.asset_channel.send_message(msg)
-
-        self.asset_channel.data['pend_done'] = False
-        while not self.asset_channel.data['pend_done']:
-            self.env.step()
-
-    def SendMessage(self, message: str, *args) -> None:
-        """
-        发送动态消息给Unity
-
-        Args:
-            message: 消息头
-            *args: 参数列表，支持的参数类型有：str, bool, int, float, list[float]
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('SendMessage')
-        msg.write_string(message)
-        for i in args:
-            if type(i) == str:
-                msg.write_string(i)
-            elif type(i) == bool:
-                msg.write_bool(i)
-            elif type(i) == int:
-                msg.write_int32(i)
-            elif type(i) == float:
-                msg.write_float32(i)
-            elif type(i) == list and type(i[0]) == float:
-                msg.write_float32_list(i)
-            else:
-                print(f'dont support this data type:{type(i)}')
-
-        self.asset_channel.send_message(msg)
-
-    def AddListener(self, message: str, fun):
-        """
-        添加动态消息监听
-
-        Args:
-            message: 消息头
-            fun: 回调函数
-        """
-        if message in self.asset_channel.messages:
-            if fun in self.asset_channel.messages[message]:
-                self.asset_channel.messages[message].append(fun)
-        else:
-            self.asset_channel.messages[message] = [fun]
-
-    def RemoveListener(self, message: str, fun):
-        """
-        移除动态消息监听
-
-        Args:
-            message: 消息头
-            fun: 回调函数
-        """
-        if message in self.asset_channel.messages:
-            if fun in self.asset_channel.messages[message]:
-                self.asset_channel.messages[message].remove(fun)
-            if len(self.asset_channel.messages[message]) == 0:
-                self.asset_channel.messages[message].pop(message)
-
-    def InstanceObject(self, name: str, id: int = None, attr_type: type = attr.BaseAttr):
-        """
-        实例化物体
-
-        Args:
-            name: 物体名
-                RfUniverseRelease中已有的资源类型及名称:
-                    GameObjcetAttr 静态物体:
-                        GameObject_Box,
-                        GameObject_Capsule,
-                        GameObject_Cylinder,
-                        GameObject_Sphere,
-                        GameObject_Quad,
-
-                        IGbison 环境:
-                            Hainesburg_mesh_texture,
-                            Halfway_mesh_texture,
-                            Hallettsville_mesh_texture,
-                            Hambleton_mesh_texture,
-                            Hammon_mesh_texture,
-                            Hatfield_mesh_texture,
-                            Haxtun_mesh_texture,
-                            Haymarket_mesh_texture,
-                            Hendrix_mesh_texture,
-                            Hercules_mesh_texture,
-                            Highspire_mesh_texture,
-                            Hitchland_mesh_texture,
-
-                    ColliderAttr 带有碰撞体的静态物体:
-                        Collider_Box,
-                        Collider_ObiBox,
-                        Collider_Capsule,
-                        Collider_Cylinder,
-                        Collider_Sphere,
-                        Collider_Quad,
-
-                    RigidbodyAttr 刚体:
-                        Rigidbody_Box,
-                        GameObject_Capsule,
-                        Rigidbody_Cylinder,
-                        Rigidbody_Sphere,
-
-                        77个YCB数据集模型: 详见The YCB Object and Model Set: https://rse-lab.cs.washington.edu/projects/posecnn/
-
-                    ControllerAttr 机械臂及关节体:
-                        gripper:
-                            allegro_hand_right,
-                            bhand,
-                            svh,
-                            robotiq_arg2f_85_model,
-                            dh_robotics_ag95_gripper,
-                        robot:
-                            kinova_gen3,
-                            kinova_gen3_robotiq85,
-                            ur5,
-                            ur5_robotiq85,
-                            franka_panda,
-                            franka_hand,
-                            tobor_robotiq85_robotiq85,
-                            flexivArm,
-                            flexivArm_ag95,
-                            yumi,
-
-                    CameraAttr 相机:
-                        Camera,
-
-                    LightAttr 灯光:
-                        Light,
-
-            id: 物体ID
-            attr_type: 物体类型
-
-        Returns:
-            物体实例
-        """
-        assert id not in self.attrs, \
-            'this ID exists'
-
-        while id is None or id in self.attrs:
-            id = random.randint(100000, 999999)
-
-        msg = OutgoingMessage()
-
-        msg.write_string('InstanceObject')
-        msg.write_string(name)
-        msg.write_int32(id)
-
-        self.asset_channel.send_message(msg)
-
-        self.attrs[id] = attr_type(self, id)
-        return self.attrs[id]
-
-    def LoadURDF(self, path: str, id: int = None, native_ik: bool = True) -> attr.ControllerAttr:
-        """
-        加载URDF模型
-
-        Args:
-            path: URDF路径
-            id: 物体ID
-            native_ik: 是否启用内置IK
-
-        Returns:
-            ControllerAttr机械臂实例
-        """
-        assert id not in self.attrs, \
-            'this ID exists'
-
-        while id is None or id in self.attrs:
-            id = random.randint(100000, 999999)
-
-        msg = OutgoingMessage()
-
-        msg.write_string('LoadURDF')
-        msg.write_int32(id)
-        msg.write_string(path)
-        msg.write_bool(native_ik)
-
-        self.asset_channel.send_message(msg)
-
-        self.attrs[id] = attr.ControllerAttr(self, id)
-        return self.attrs[id]
-
-    def LoadMesh(self, path: str, id: int = None) -> attr.RigidbodyAttr:
-        """
-        加载Mesh模型
-
-        Args:
-            path: Mesh路径
-            id: 物体ID
-
-        Returns:
-            RigidbodyAttr刚体实例
-        """
-        assert id not in self.attrs, \
-            'this ID exists'
-
-        while id is None or id in self.attrs:
-            id = random.randint(100000, 999999)
-
-        msg = OutgoingMessage()
-
-        msg.write_string('LoadMesh')
-        msg.write_int32(id)
-        msg.write_string(path)
-
-        self.asset_channel.send_message(msg)
-
-        self.attrs[id] = attr.RigidbodyAttr(self, id)
-        return self.attrs[id]
-
-    def IgnoreLayerCollision(self, layer1: int, layer2: int, ignore: bool) -> None:
-        """
-        忽略或启用指定两个层的碰撞
-
-        Args:
-            layer1: 层1
-            layer2: 层1
-            ignore: 是否忽略
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('IgnoreLayerCollision')
-        msg.write_int32(layer1)
-        msg.write_int32(layer2)
-        msg.write_bool(ignore)
-
-        self.asset_channel.send_message(msg)
-
-    def GetCurrentCollisionPairs(self) -> None:
-        """
-        获取当前碰撞对
-
-        Returns:
-            调用此接口并step后，从env.data['CurrentCollisionPairs']中获取碰撞对
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('GetCurrentCollisionPairs')
-
-        self.asset_channel.send_message(msg)
-
-    def GetRFMoveColliders(self) -> None:
-        """
-        获取RFMove碰撞体
-
-        Returns:
-            调用此接口并step后，从env.data['RFMoveColliders']中获取碰撞体
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('GetRFMoveColliders')
-
-        self.asset_channel.send_message(msg)
-
-    def SetGravity(self, x: float, y: float, z: float) -> None:
-        """
-        设置环境重力
-
-        Args:
-            x: 右方向
-            y: 上方向
-            z: 前方向
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('SetGravity')
-        msg.write_float32(x)
-        msg.write_float32(y)
-        msg.write_float32(z)
-
-        self.asset_channel.send_message(msg)
-
-    def SetGroundPhysicMaterial(self, bounciness: float, dynamic_friction: float, static_friction: float, friction_combine: int, bounce_combine: int) -> None:
-        """
-        设置环境地面物理材质
-
-        Args:
-            bounciness: 弹力
-            dynamic_friction: 动摩擦力
-            static_friction: 静摩擦力
-            friction_combine: 摩擦力组合方式
-            bounce_combine: 弹力组合方式
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('SetGroundPhysicMaterial')
-        msg.write_float32(bounciness)
-        msg.write_float32(dynamic_friction)
-        msg.write_float32(static_friction)
-        msg.write_int32(friction_combine)
-        msg.write_int32(bounce_combine)
-
-        self.asset_channel.send_message(msg)
-
-    def SetTimeStep(self, delta_time: float) -> None:
-        """
-        设置环境step时间步长
-
-        Args:
-            delta_time: 时间步长(s)
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('SetTimeStep')
-        msg.write_float32(delta_time)
-
-        self.asset_channel.send_message(msg)
-
-    def SetTimeScale(self, time_scale: float) -> None:
-        """
-        设置环境时间缩放比例
-
-        Args:
-            time_scale: 时间缩放比例
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('SetTimeScale')
-        msg.write_float32(time_scale)
-
-        self.asset_channel.send_message(msg)
-
-    def SetResolution(self, resolution_x: int, resolution_y: int) -> None:
-        """
-        设置窗口分辨率
-
-        Args:
-            resolution_x: 宽度width分辨率
-            resolution_y: 高度height分辨率
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('SetResolution')
-        msg.write_int32(resolution_x)
-        msg.write_int32(resolution_y)
-
-        self.asset_channel.send_message(msg)
-
-    def ExportOBJ(self, items_id: list, save_path: str) -> None:
-        """
-        导出指定物体列表为OBJ文件
-
-        Args:
-            items_id: 物体ID列表
-            save_path: 保存绝对路径
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('ExportOBJ')
-        msg.write_int32(len(items_id))
-        for i in items_id:
-            msg.write_int32(i)
-        msg.write_string(save_path)
-
-        self.asset_channel.send_message(msg)
-
-    def SetShadowDistance(self, distance: float) -> None:
-        """
-        设置环境阴影渲染距离
-
-        Args:
-            distance: 距离(m)
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('SetShadowDistance')
-        msg.write_float32(distance)
-
-        self.asset_channel.send_message(msg)
-
-    def SaveScene(self, file: str) -> None:
-        """
-        保存当前场景
-
-        Args:
-            file: 存储场景Json路径，当该值为路径时，保存到该路径，否则保存到StreamingAssets
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('SaveScene')
-        msg.write_string(file)
-
-        self.asset_channel.send_message(msg)
-
-    def ClearScene(self) -> None:
-        """
-        清理当前场景
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('ClearScene')
-
-        self.asset_channel.send_message(msg)
-
-    def AlignCamera(self, camera_id: int) -> None:
-        """
-        对齐视口到相机
-
-        Args:
-            camera_id: 相机ID
-        """
-        msg = OutgoingMessage()
-
-        msg.write_string('AlignCamera')
-        msg.write_int32(camera_id)
-
-        self.asset_channel.send_message(msg)
-
-
-    #Dubug API
-    def DebugGraspPoint(self, enabled: bool = True) -> None:
-        """
-        Debug显示机械臂末端点
-        """
-        msg = OutgoingMessage()
-        msg.write_string('DebugGraspPoint')
-        msg.write_bool(enabled)
-        self.debug_channel.send_message(msg)
-
-    def DebugObjectPose(self, enabled: bool = True) -> None:
-        """
-        Debug显示物体base点
-        """
-        msg = OutgoingMessage()
-        msg.write_string('DebugObjectPose')
-        msg.write_bool(enabled)
-        self.debug_channel.send_message(msg)
-
-    def DebugCollisionPair(self, enabled: bool = True) -> None:
-        """
-        Debug显示物理碰撞对
-        """
-        msg = OutgoingMessage()
-        msg.write_string('DebugCollisionPair')
-        msg.write_bool(enabled)
-        self.debug_channel.send_message(msg)
-    def DebugColliderBound(self, enabled: bool = True) -> None:
-        """
-        Debug显示碰撞包围盒
-        """
-        msg = OutgoingMessage()
-        msg.write_string('DebugColliderBound')
-        msg.write_bool(enabled)
-        self.debug_channel.send_message(msg)
-
-    def DebugObjectID(self, enabled: bool = True) -> None:
-        """
-        Debug显示碰物体ID
-        """
-        msg = OutgoingMessage()
-        msg.write_string('DebugObjectID')
-        msg.write_bool(enabled)
-        self.debug_channel.send_message(msg)
-
-    def Debug3DBBox(self, enabled: bool = True) -> None:
-        """
-        Debug显示物体3DBoundingBox
-        """
-        msg = OutgoingMessage()
-        msg.write_string('Debug3DBBox')
-        msg.write_bool(enabled)
-        self.debug_channel.send_message(msg)
-
-    def Debug2DBBox(self, enabled: bool = True) -> None:
-        """
-        Debug显示物体2DBoundingBox
-        """
-        msg = OutgoingMessage()
-        msg.write_string('Debug2DBBox')
-        msg.write_bool(enabled)
-        self.debug_channel.send_message(msg)
-
-    def DebugJointLink(self, enabled: bool = True) -> None:
-        """
-        Debug显示关节体Joint信息
-        """
-        msg = OutgoingMessage()
-        msg.write_string('DebugJointLink')
-        msg.write_bool(enabled)
-        self.debug_channel.send_message(msg)
-
-    def SendLog(self, log: str) -> None:
-        """
-        发送Log消息并显示在Unity窗口
-
-        Args:
-            log: Log内容
-        """
-        msg = OutgoingMessage()
-        msg.write_string('SendLog')
-        msg.write_string(log)
-        self.debug_channel.send_message(msg)
-
-    def _SendVersion(self) -> None:
-        msg = OutgoingMessage()
-        msg.write_string('SendVersion')
-        msg.write_string(pyrfuniverse.__version__)
-        self.debug_channel.send_message(msg)
-
-
-
-# class RFUniverseGymWrapper(RFUniverseBaseEnv, gym.Env):
-#
-#     def __init__(
-#             self,
-#             executable_file: str = None,
-#             scene_file: str = None,
-#             custom_channels: list = [],
-#             assets: list = [],
-#             **kwargs
-#     ):
-#         RFUniverseBaseEnv.__init__(
-#             self,
-#             executable_file=executable_file,
-#             scene_file=scene_file,
-#             custom_channels=custom_channels,
-#             assets=assets,
-#             **kwargs,
-#         )
-#
-#     def close(self):
-#         RFUniverseBaseEnv.close(self)
-#
-#
-# class RFUniverseGymGoalWrapper(gym.GoalEnv, RFUniverseBaseEnv):
-#
-#     def __init__(
-#             self,
-#             executable_file: str = None,
-#             scene_file: str = None,
-#             custom_channels: list = [],
-#             assets: list = [],
-#             **kwargs
-#
-#     ):
-#         RFUniverseBaseEnv.__init__(
-#             self,
-#             executable_file=executable_file,
-#             scene_file=scene_file,
-#             custom_channels=custom_channels,
-#             assets=assets,
-#             **kwargs,
-#         )
-#
-#     def reset(self):
-#         gym.GoalEnv.reset(self)
-#
-#     def close(self):
-#         RFUniverseBaseEnv.close(self)
+import random
+from abc import ABC
+from pyrfuniverse.side_channel.side_channel import (
+    IncomingMessage,
+    OutgoingMessage,
+)
+import pyrfuniverse
+from pyrfuniverse.environment import UnityEnvironment
+from pyrfuniverse.side_channel.environment_parameters_channel import EnvironmentParametersChannel
+from pyrfuniverse.rfuniverse_channel import AssetChannel
+from pyrfuniverse.rfuniverse_channel import AssetChannelExt
+from pyrfuniverse.rfuniverse_channel import InstanceChannel
+from pyrfuniverse.rfuniverse_channel import DebugChannel
+import pyrfuniverse.attributes as attr
+import gym
+import os
+
+
+def select_available_worker_id():
+    if not os.path.exists(pyrfuniverse.user_path):
+        os.makedirs(pyrfuniverse.user_path)
+    log_file = os.path.join(pyrfuniverse.user_path, 'worker_id_log')
+
+    worker_id = 1
+    worker_id_in_use = []
+    if os.path.exists(log_file):
+        with open(log_file, 'r') as f:
+            worker_ids = f.readlines()
+            for line in worker_ids:
+                worker_id_in_use.append(int(line))
+        while worker_id in worker_id_in_use:
+            worker_id += 1
+
+    worker_id_in_use.append(worker_id)
+    with open(log_file, 'w') as f:
+        for id in worker_id_in_use:
+            f.write(str(id) + '\n')
+
+    return worker_id
+
+
+def delete_worker_id(worker_id):
+    log_file = os.path.join(pyrfuniverse.user_path, 'worker_id_log')
+
+    worker_id_in_use = []
+    if os.path.exists(log_file):
+        with open(log_file, 'r') as f:
+            worker_ids = f.readlines()
+            for line in worker_ids:
+                worker_id_in_use.append(int(line))
+
+    worker_id_in_use.remove(worker_id)
+    with open(log_file, 'w') as f:
+        for id in worker_id_in_use:
+            f.write(str(id) + '\n')
+
+
+class RFUniverseBaseEnv(ABC):
+    """
+    RFUnivers基础环境类
+    """
+    metadata = {'render.modes': ['human', 'rgb_array']}
+
+    def __init__(
+        self,
+        executable_file: str = None,
+        scene_file: str = None,
+        custom_channels: list = [],
+        assets: list = [],
+        graphics: bool = True,
+        **kwargs
+    ):
+        # time step
+        self.t = 0
+        self.worker_id = select_available_worker_id()
+        # initialize rfuniverse channels
+        self.channels = custom_channels.copy()
+        self._init_channels(kwargs)
+        self.assets = assets
+        # initialize environment
+        self.executable_file = executable_file
+        self.scene_file = scene_file
+        self.graphics = graphics
+        self.attrs = {}
+        self.data = {}
+        self.ext = AssetChannelExt(self)
+        self._init_env()
+
+    def _init_env(self):
+        if str(self.executable_file).lower() == '@editor':
+            self.env = UnityEnvironment(
+                worker_id=0,
+                side_channels=self.channels,
+                no_graphics=not self.graphics,
+            )
+        elif self.executable_file is not None:
+            self.env = UnityEnvironment(
+                worker_id=self.worker_id,
+                file_name=self.executable_file,
+                side_channels=self.channels,
+                no_graphics=not self.graphics,
+            )
+        elif os.path.exists(pyrfuniverse.executable_file):
+            self.env = UnityEnvironment(
+                worker_id=self.worker_id,
+                file_name=pyrfuniverse.executable_file,
+                side_channels=self.channels,
+                no_graphics=not self.graphics,
+            )
+        else:
+            self.env = UnityEnvironment(
+                worker_id=0,
+                side_channels=self.channels,
+                no_graphics=not self.graphics,
+            )
+        self._SendVersion()
+        if self.scene_file is not None:
+            self.LoadSceneAsync(self.scene_file, True)
+        if len(self.assets) > 0:
+            self._PreLoadAssetsAsync(self.assets, True)
+        self.env.reset()
+
+    def _init_channels(self, kwargs: dict):
+        # Compulsory channels
+        # Environment parameters channel
+        self.env_param_channel = EnvironmentParametersChannel()
+        self.channels.append(self.env_param_channel)
+        # RFUniverse channel
+        self.asset_channel = AssetChannel(self, 'd587efc8-9eb7-11ec-802a-18c04d443e7d')
+        self.instance_channel = InstanceChannel(self, '09bfcf57-9120-43dc-99f8-abeeec59df0f')
+        self.debug_channel = DebugChannel(self, '02ac5776-6a7c-54e4-011d-b4c4723831c9')
+        self.channels.append(self.asset_channel)
+        self.channels.append(self.instance_channel)
+        self.channels.append(self.debug_channel)
+
+    def _step(self):
+        self.env.step()
+
+    def step(self, count: int = 1):
+        """
+        将已经调用的接口消息发送给Unity，执行一步仿真，然后接收Unity返回的数据
+
+        Args:
+            count: 执行的步数
+        """
+        if count < 1:
+            count = 1
+        for _ in range(count):
+            self.env.step()
+
+    def close(self):
+        """
+        关闭环境
+        """
+        delete_worker_id(self.worker_id)
+        self.env.close()
+
+    def GetAttr(self, id: int):
+        """
+        根据ID获取物体
+
+        Args:
+            id: 物体ID
+        """
+        if id not in self.attrs:
+            self.attrs[id] = attr.BaseAttr(self, id)
+        return self.attrs[id]
+
+    #Env API
+    def _PreLoadAssetsAsync(self, names: list, auto_wait: bool = False) -> None:
+        msg = OutgoingMessage()
+
+        msg.write_string('PreLoadAssetsAsync')
+        count = len(names)
+        msg.write_int32(count)
+        for i in range(count):
+            msg.write_string(names[i])
+
+        self.asset_channel.send_message(msg)
+
+        if auto_wait:
+            self.WaitLoadDone()
+
+
+    def LoadSceneAsync(self, file: str, auto_wait: bool = False) -> None:
+        """
+        异步加载场景
+
+        Args:
+            file: 场景Json文件，当该值为路径时，从路径加载场景，否则从StreamingAssets加载场景
+            auto_wait: 是否等待加载完成，如果为True，则在加载完成后才返回
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('LoadSceneAsync')
+        msg.write_string(file)
+
+        self.asset_channel.send_message(msg)
+
+        if auto_wait:
+            self.WaitLoadDone()
+
+    def WaitLoadDone(self) -> None:
+        """
+        等待加载完成，使用LoadSceneAsync接口后，调用该接口可以等待加载完成
+        """
+        self.asset_channel.data['load_done'] = False
+        while not self.asset_channel.data['load_done']:
+            self.env.step()
+
+    def Pend(self) -> None:
+        """
+        挂起，直到UnityPlayer中点击EndPend按钮
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('Pend')
+
+        self.asset_channel.send_message(msg)
+
+        self.asset_channel.data['pend_done'] = False
+        while not self.asset_channel.data['pend_done']:
+            self.env.step()
+
+    def SendMessage(self, message: str, *args) -> None:
+        """
+        发送动态消息给Unity
+
+        Args:
+            message: 消息头
+            *args: 参数列表，支持的参数类型有：str, bool, int, float, list[float]
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('SendMessage')
+        msg.write_string(message)
+        for i in args:
+            if type(i) == str:
+                msg.write_string(i)
+            elif type(i) == bool:
+                msg.write_bool(i)
+            elif type(i) == int:
+                msg.write_int32(i)
+            elif type(i) == float:
+                msg.write_float32(i)
+            elif type(i) == list and type(i[0]) == float:
+                msg.write_float32_list(i)
+            else:
+                print(f'dont support this data type:{type(i)}')
+
+        self.asset_channel.send_message(msg)
+
+    def AddListener(self, message: str, fun):
+        """
+        添加动态消息监听
+
+        Args:
+            message: 消息头
+            fun: 回调函数
+        """
+        if message in self.asset_channel.messages:
+            if fun in self.asset_channel.messages[message]:
+                self.asset_channel.messages[message].append(fun)
+        else:
+            self.asset_channel.messages[message] = [fun]
+
+    def RemoveListener(self, message: str, fun):
+        """
+        移除动态消息监听
+
+        Args:
+            message: 消息头
+            fun: 回调函数
+        """
+        if message in self.asset_channel.messages:
+            if fun in self.asset_channel.messages[message]:
+                self.asset_channel.messages[message].remove(fun)
+            if len(self.asset_channel.messages[message]) == 0:
+                self.asset_channel.messages[message].pop(message)
+
+    def InstanceObject(self, name: str, id: int = None, attr_type: type = attr.BaseAttr):
+        """
+        实例化物体
+
+        Args:
+            name: 物体名
+                RfUniverseRelease中已有的资源类型及名称:
+                    GameObjcetAttr 静态物体:
+                        GameObject_Box,
+                        GameObject_Capsule,
+                        GameObject_Cylinder,
+                        GameObject_Sphere,
+                        GameObject_Quad,
+
+                        IGbison 环境:
+                            Hainesburg_mesh_texture,
+                            Halfway_mesh_texture,
+                            Hallettsville_mesh_texture,
+                            Hambleton_mesh_texture,
+                            Hammon_mesh_texture,
+                            Hatfield_mesh_texture,
+                            Haxtun_mesh_texture,
+                            Haymarket_mesh_texture,
+                            Hendrix_mesh_texture,
+                            Hercules_mesh_texture,
+                            Highspire_mesh_texture,
+                            Hitchland_mesh_texture,
+
+                    ColliderAttr 带有碰撞体的静态物体:
+                        Collider_Box,
+                        Collider_ObiBox,
+                        Collider_Capsule,
+                        Collider_Cylinder,
+                        Collider_Sphere,
+                        Collider_Quad,
+
+                    RigidbodyAttr 刚体:
+                        Rigidbody_Box,
+                        GameObject_Capsule,
+                        Rigidbody_Cylinder,
+                        Rigidbody_Sphere,
+
+                        77个YCB数据集模型: 详见The YCB Object and Model Set: https://rse-lab.cs.washington.edu/projects/posecnn/
+
+                    ControllerAttr 机械臂及关节体:
+                        gripper:
+                            allegro_hand_right,
+                            bhand,
+                            svh,
+                            robotiq_arg2f_85_model,
+                            dh_robotics_ag95_gripper,
+                        robot:
+                            kinova_gen3,
+                            kinova_gen3_robotiq85,
+                            ur5,
+                            ur5_robotiq85,
+                            franka_panda,
+                            franka_hand,
+                            tobor_robotiq85_robotiq85,
+                            flexivArm,
+                            flexivArm_ag95,
+                            yumi,
+
+                    CameraAttr 相机:
+                        Camera,
+
+                    LightAttr 灯光:
+                        Light,
+
+            id: 物体ID
+            attr_type: 物体类型
+
+        Returns:
+            物体实例
+        """
+        assert id not in self.attrs, \
+            'this ID exists'
+
+        while id is None or id in self.attrs:
+            id = random.randint(100000, 999999)
+
+        msg = OutgoingMessage()
+
+        msg.write_string('InstanceObject')
+        msg.write_string(name)
+        msg.write_int32(id)
+
+        self.asset_channel.send_message(msg)
+
+        self.attrs[id] = attr_type(self, id)
+        return self.attrs[id]
+
+    def LoadURDF(self, path: str, id: int = None, native_ik: bool = True) -> attr.ControllerAttr:
+        """
+        加载URDF模型
+
+        Args:
+            path: URDF路径
+            id: 物体ID
+            native_ik: 是否启用内置IK
+
+        Returns:
+            ControllerAttr机械臂实例
+        """
+        assert id not in self.attrs, \
+            'this ID exists'
+
+        while id is None or id in self.attrs:
+            id = random.randint(100000, 999999)
+
+        msg = OutgoingMessage()
+
+        msg.write_string('LoadURDF')
+        msg.write_int32(id)
+        msg.write_string(path)
+        msg.write_bool(native_ik)
+
+        self.asset_channel.send_message(msg)
+
+        self.attrs[id] = attr.ControllerAttr(self, id)
+        return self.attrs[id]
+
+    def LoadMesh(self, path: str, id: int = None) -> attr.RigidbodyAttr:
+        """
+        加载Mesh模型
+
+        Args:
+            path: Mesh路径
+            id: 物体ID
+
+        Returns:
+            RigidbodyAttr刚体实例
+        """
+        assert id not in self.attrs, \
+            'this ID exists'
+
+        while id is None or id in self.attrs:
+            id = random.randint(100000, 999999)
+
+        msg = OutgoingMessage()
+
+        msg.write_string('LoadMesh')
+        msg.write_int32(id)
+        msg.write_string(path)
+
+        self.asset_channel.send_message(msg)
+
+        self.attrs[id] = attr.RigidbodyAttr(self, id)
+        return self.attrs[id]
+
+    def IgnoreLayerCollision(self, layer1: int, layer2: int, ignore: bool) -> None:
+        """
+        忽略或启用指定两个层的碰撞
+
+        Args:
+            layer1: 层1
+            layer2: 层1
+            ignore: 是否忽略
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('IgnoreLayerCollision')
+        msg.write_int32(layer1)
+        msg.write_int32(layer2)
+        msg.write_bool(ignore)
+
+        self.asset_channel.send_message(msg)
+
+    def GetCurrentCollisionPairs(self) -> None:
+        """
+        获取当前碰撞对
+
+        Returns:
+            调用此接口并step后，从env.data['CurrentCollisionPairs']中获取碰撞对
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('GetCurrentCollisionPairs')
+
+        self.asset_channel.send_message(msg)
+
+    def GetRFMoveColliders(self) -> None:
+        """
+        获取RFMove碰撞体
+
+        Returns:
+            调用此接口并step后，从env.data['RFMoveColliders']中获取碰撞体
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('GetRFMoveColliders')
+
+        self.asset_channel.send_message(msg)
+
+    def SetGravity(self, x: float, y: float, z: float) -> None:
+        """
+        设置环境重力
+
+        Args:
+            x: 右方向
+            y: 上方向
+            z: 前方向
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('SetGravity')
+        msg.write_float32(x)
+        msg.write_float32(y)
+        msg.write_float32(z)
+
+        self.asset_channel.send_message(msg)
+
+    def SetGroundPhysicMaterial(self, bounciness: float, dynamic_friction: float, static_friction: float, friction_combine: int, bounce_combine: int) -> None:
+        """
+        设置环境地面物理材质
+
+        Args:
+            bounciness: 弹力
+            dynamic_friction: 动摩擦力
+            static_friction: 静摩擦力
+            friction_combine: 摩擦力组合方式
+            bounce_combine: 弹力组合方式
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('SetGroundPhysicMaterial')
+        msg.write_float32(bounciness)
+        msg.write_float32(dynamic_friction)
+        msg.write_float32(static_friction)
+        msg.write_int32(friction_combine)
+        msg.write_int32(bounce_combine)
+
+        self.asset_channel.send_message(msg)
+
+    def SetTimeStep(self, delta_time: float) -> None:
+        """
+        设置环境step时间步长
+
+        Args:
+            delta_time: 时间步长(s)
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('SetTimeStep')
+        msg.write_float32(delta_time)
+
+        self.asset_channel.send_message(msg)
+
+    def SetTimeScale(self, time_scale: float) -> None:
+        """
+        设置环境时间缩放比例
+
+        Args:
+            time_scale: 时间缩放比例
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('SetTimeScale')
+        msg.write_float32(time_scale)
+
+        self.asset_channel.send_message(msg)
+
+    def SetResolution(self, resolution_x: int, resolution_y: int) -> None:
+        """
+        设置窗口分辨率
+
+        Args:
+            resolution_x: 宽度width分辨率
+            resolution_y: 高度height分辨率
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('SetResolution')
+        msg.write_int32(resolution_x)
+        msg.write_int32(resolution_y)
+
+        self.asset_channel.send_message(msg)
+
+    def ExportOBJ(self, items_id: list, save_path: str) -> None:
+        """
+        导出指定物体列表为OBJ文件，对于原生Bundle模型，需要在UnityEditor中勾选Read/Write才能正确导出
+
+        Args:
+            items_id: 物体ID列表
+            save_path: 保存绝对路径
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('ExportOBJ')
+        msg.write_int32(len(items_id))
+        for i in items_id:
+            msg.write_int32(i)
+        msg.write_string(save_path)
+
+        self.asset_channel.send_message(msg)
+
+    def SetShadowDistance(self, distance: float) -> None:
+        """
+        设置环境阴影渲染距离
+
+        Args:
+            distance: 距离(m)
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('SetShadowDistance')
+        msg.write_float32(distance)
+
+        self.asset_channel.send_message(msg)
+
+    def SaveScene(self, file: str) -> None:
+        """
+        保存当前场景
+
+        Args:
+            file: 存储场景Json路径，当该值为路径时，保存到该路径，否则保存到StreamingAssets
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('SaveScene')
+        msg.write_string(file)
+
+        self.asset_channel.send_message(msg)
+
+    def ClearScene(self) -> None:
+        """
+        清理当前场景
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('ClearScene')
+
+        self.asset_channel.send_message(msg)
+
+    def AlignCamera(self, camera_id: int) -> None:
+        """
+        对齐视口到相机
+
+        Args:
+            camera_id: 相机ID
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('AlignCamera')
+        msg.write_int32(camera_id)
+
+        self.asset_channel.send_message(msg)
+
+    def SetViewTransform(self, position: list = None, rotation: list = None) -> None:
+        """
+        设置视口位置和旋转
+
+        Args:
+            position: 位置
+            rotation: 旋转
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('SetViewTransform')
+        msg.write_bool(position is not None)
+        msg.write_bool(rotation is not None)
+        if position is not None:
+            assert type(position) == list and len(position) == 3, \
+                'Argument position must be a 3-d list.'
+            for i in range(3):
+                msg.write_float32(position[i])
+        if rotation is not None:
+            assert type(rotation) == list and len(rotation) == 3, \
+                'Argument rotation must be a 3-d list.'
+            for i in range(3):
+                msg.write_float32(rotation[i])
+
+        self.asset_channel.send_message(msg)
+
+
+    #Dubug API
+    def DebugGraspPoint(self, enabled: bool = True) -> None:
+        """
+        Debug显示机械臂末端点
+        """
+        msg = OutgoingMessage()
+        msg.write_string('DebugGraspPoint')
+        msg.write_bool(enabled)
+        self.debug_channel.send_message(msg)
+
+    def DebugObjectPose(self, enabled: bool = True) -> None:
+        """
+        Debug显示物体base点
+        """
+        msg = OutgoingMessage()
+        msg.write_string('DebugObjectPose')
+        msg.write_bool(enabled)
+        self.debug_channel.send_message(msg)
+
+    def DebugCollisionPair(self, enabled: bool = True) -> None:
+        """
+        Debug显示物理碰撞对
+        """
+        msg = OutgoingMessage()
+        msg.write_string('DebugCollisionPair')
+        msg.write_bool(enabled)
+        self.debug_channel.send_message(msg)
+    def DebugColliderBound(self, enabled: bool = True) -> None:
+        """
+        Debug显示碰撞包围盒
+        """
+        msg = OutgoingMessage()
+        msg.write_string('DebugColliderBound')
+        msg.write_bool(enabled)
+        self.debug_channel.send_message(msg)
+
+    def DebugObjectID(self, enabled: bool = True) -> None:
+        """
+        Debug显示碰物体ID
+        """
+        msg = OutgoingMessage()
+        msg.write_string('DebugObjectID')
+        msg.write_bool(enabled)
+        self.debug_channel.send_message(msg)
+
+    def Debug3DBBox(self, enabled: bool = True) -> None:
+        """
+        Debug显示物体3DBoundingBox
+        """
+        msg = OutgoingMessage()
+        msg.write_string('Debug3DBBox')
+        msg.write_bool(enabled)
+        self.debug_channel.send_message(msg)
+
+    def Debug2DBBox(self, enabled: bool = True) -> None:
+        """
+        Debug显示物体2DBoundingBox
+        """
+        msg = OutgoingMessage()
+        msg.write_string('Debug2DBBox')
+        msg.write_bool(enabled)
+        self.debug_channel.send_message(msg)
+
+    def DebugJointLink(self, enabled: bool = True) -> None:
+        """
+        Debug显示关节体Joint信息
+        """
+        msg = OutgoingMessage()
+        msg.write_string('DebugJointLink')
+        msg.write_bool(enabled)
+        self.debug_channel.send_message(msg)
+
+    def SendLog(self, log: str) -> None:
+        """
+        发送Log消息并显示在Unity窗口
+
+        Args:
+            log: Log内容
+        """
+        msg = OutgoingMessage()
+        msg.write_string('SendLog')
+        msg.write_string(log)
+        self.debug_channel.send_message(msg)
+
+    def _SendVersion(self) -> None:
+        msg = OutgoingMessage()
+        msg.write_string('SendVersion')
+        msg.write_string(pyrfuniverse.__version__)
+        self.debug_channel.send_message(msg)
+
+
+
+class RFUniverseGymWrapper(RFUniverseBaseEnv, gym.Env):
+
+    def __init__(
+            self,
+            executable_file: str = None,
+            scene_file: str = None,
+            custom_channels: list = [],
+            assets: list = [],
+            **kwargs
+    ):
+        RFUniverseBaseEnv.__init__(
+            self,
+            executable_file=executable_file,
+            scene_file=scene_file,
+            custom_channels=custom_channels,
+            assets=assets,
+            **kwargs,
+        )
+
+    def close(self):
+        RFUniverseBaseEnv.close(self)
+
+
+class RFUniverseGymGoalWrapper(gym.GoalEnv, RFUniverseBaseEnv):
+
+    def __init__(
+            self,
+            executable_file: str = None,
+            scene_file: str = None,
+            custom_channels: list = [],
+            assets: list = [],
+            **kwargs
+
+    ):
+        RFUniverseBaseEnv.__init__(
+            self,
+            executable_file=executable_file,
+            scene_file=scene_file,
+            custom_channels=custom_channels,
+            assets=assets,
+            **kwargs,
+        )
+
+    def reset(self):
+        gym.GoalEnv.reset(self)
+
+    def close(self):
+        RFUniverseBaseEnv.close(self)
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/bouncer_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/bouncer_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/franka_grasp_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/franka_grasp_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/franka_push_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/franka_push_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/__init__.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/nail_can_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/nail_can_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/nail_card_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/nail_card_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/multi_agent/cleaner_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent/cleaner_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/multi_agent/navigation_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent/navigation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/multi_agent_navigation_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent_navigation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/rfuniverse_robot_hub_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/rfuniverse_robot_hub_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/__init__.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/franka_cloth_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_cloth_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/franka_robotics_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_robotics_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/franka_softbody_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_softbody_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/pick_and_place_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/pick_and_place_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/push_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/push_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/robotics/reach_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/reach_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/roller_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/roller_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/ur5_box_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/ur5_box_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/envs/ur5_drawer_env.py` & `pyrfuniverse-0.8.3/pyrfuniverse/envs/ur5_drawer_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/exception.py` & `pyrfuniverse-0.8.3/pyrfuniverse/exception.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/logging_util.py` & `pyrfuniverse-0.8.3/pyrfuniverse/logging_util.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/mock_communicator.py` & `pyrfuniverse-0.8.3/pyrfuniverse/mock_communicator.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/registry/base_registry_entry.py` & `pyrfuniverse-0.8.3/pyrfuniverse/registry/base_registry_entry.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/registry/binary_utils.py` & `pyrfuniverse-0.8.3/pyrfuniverse/registry/binary_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/registry/remote_registry_entry.py` & `pyrfuniverse-0.8.3/pyrfuniverse/registry/remote_registry_entry.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/registry/unity_env_registry.py` & `pyrfuniverse-0.8.3/pyrfuniverse/registry/unity_env_registry.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/rfuniverse_channel/asset_channel.py` & `pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/asset_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/rfuniverse_channel/asset_channel_ext.py` & `pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/asset_channel_ext.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/rfuniverse_channel/debug_channel.py` & `pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/debug_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/rfuniverse_channel/instance_channel.py` & `pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/instance_channel.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import warnings
-
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
-from pyrfuniverse.rfuniverse_channel import RFUniverseChannel
-import pyrfuniverse.attributes as attr
-
-class InstanceChannel(RFUniverseChannel):
-
-    def __init__(self, env, channel_id: str) -> None:
-        super().__init__(channel_id)
-        self.env = env
-        self.data = {}
-
-    def _parse_message(self, msg: IncomingMessage) -> None:
-        # count = msg.read_int32()
-        # for i in range(count):
-            this_object_id = msg.read_int32()
-            this_object_type = msg.read_string()
-
-            # self.data[this_object_id] = eval('attr.' + this_object_type + '_attr.' + 'parse_message')(msg)
-
-            attr_type = eval('attr.' + this_object_type)
-
-            if this_object_id not in self.env.attrs:
-                self.env.attrs[this_object_id] = attr_type(self.env, this_object_id)
-            elif type(self.env.attrs[this_object_id]) != attr_type:
-                self.env.attrs[this_object_id] = attr_type(self.env, this_object_id, self.env.attrs[this_object_id].data)
-
-            self.data[this_object_id] = self.env.attrs[this_object_id].parse_message(msg)
-
-
-    def set_action(self, action: str, attr_name=None, **kwargs) -> None:
-        warnings.warn("set_action is deprecated, It will be removed in version 1.0", DeprecationWarning)
-        """Set action and pass corresponding parameters
-        Args:
-            action: The action name.
-            kwargs: keyword argument for action. The parameter list for each action is shown in each function.
-        """
-        try:
-            if attr_name is not None:
-                msg = eval('attr.' + attr_name + '.' + action)(kwargs)
-                self.send_message(msg)
-            else:
-                for i in attr.__all__:
-                    if eval('hasattr(attr.' + i + ',\'' + action + '\')'):
-                        msg = eval('attr.' + i + '.' + action)(kwargs)
-                        self.send_message(msg)
-        except AttributeError:
-            print('There is no action called \'%s\' or this function has bug, please fix it.' % action)
-            exit(-1)
-
-
-
+import warnings
+
+from pyrfuniverse.side_channel.side_channel import (
+    IncomingMessage,
+    OutgoingMessage,
+)
+from pyrfuniverse.rfuniverse_channel import RFUniverseChannel
+import pyrfuniverse.attributes as attr
+
+class InstanceChannel(RFUniverseChannel):
+
+    def __init__(self, env, channel_id: str) -> None:
+        super().__init__(channel_id)
+        self.env = env
+        self.data = {}
+
+    def _parse_message(self, msg: IncomingMessage) -> None:
+        # count = msg.read_int32()
+        # for i in range(count):
+            this_object_id = msg.read_int32()
+            this_object_type = msg.read_string()
+
+            # self.data[this_object_id] = eval('attr.' + this_object_type + '_attr.' + 'parse_message')(msg)
+
+            attr_type = eval('attr.' + this_object_type)
+
+            if this_object_id not in self.env.attrs:
+                self.env.attrs[this_object_id] = attr_type(self.env, this_object_id)
+            elif type(self.env.attrs[this_object_id]) != attr_type:
+                self.env.attrs[this_object_id] = attr_type(self.env, this_object_id, self.env.attrs[this_object_id].data)
+
+            self.data[this_object_id] = self.env.attrs[this_object_id].parse_message(msg)
+
+
+    def set_action(self, action: str, attr_name=None, **kwargs) -> None:
+        warnings.warn("set_action is deprecated, It will be removed in version 1.0", DeprecationWarning)
+        """Set action and pass corresponding parameters
+        Args:
+            action: The action name.
+            kwargs: keyword argument for action. The parameter list for each action is shown in each function.
+        """
+        try:
+            if attr_name is not None:
+                msg = eval('attr.' + attr_name + '.' + action)(kwargs)
+                self.send_message(msg)
+            else:
+                for i in attr.__all__:
+                    if eval('hasattr(attr.' + i + ',\'' + action + '\')'):
+                        msg = eval('attr.' + i + '.' + action)(kwargs)
+                        self.send_message(msg)
+        except AttributeError:
+            print('There is no action called \'%s\' or this function has bug, please fix it.' % action)
+            exit(-1)
+
+
+
```

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/rfuniverse_channel/rfuniverse_channel.py` & `pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/rfuniverse_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/rpc_communicator.py` & `pyrfuniverse-0.8.3/pyrfuniverse/rpc_communicator.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/rpc_utils.py` & `pyrfuniverse-0.8.3/pyrfuniverse/rpc_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/engine_configuration_channel.py` & `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/engine_configuration_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/environment_parameters_channel.py` & `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/environment_parameters_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/float_properties_channel.py` & `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/float_properties_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/incoming_message.py` & `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/incoming_message.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/outgoing_message.py` & `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/outgoing_message.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/raw_bytes_channel.py` & `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/raw_bytes_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/side_channel.py` & `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/side_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/side_channel_manager.py` & `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/side_channel_manager.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/side_channel/stats_side_channel.py` & `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/stats_side_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/timers.py` & `pyrfuniverse-0.8.3/pyrfuniverse/timers.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/utils/active_depth_generate.py` & `pyrfuniverse-0.8.3/pyrfuniverse/utils/active_depth_generate.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/utils/controller.py` & `pyrfuniverse-0.8.3/pyrfuniverse/utils/controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/utils/depth_processor.py` & `pyrfuniverse-0.8.3/pyrfuniverse/utils/depth_processor.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/utils/interpolate_utils.py` & `pyrfuniverse-0.8.3/pyrfuniverse/utils/interpolate_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/utils/jaco_controller.py` & `pyrfuniverse-0.8.3/pyrfuniverse/utils/jaco_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/utils/kinova_controller.py` & `pyrfuniverse-0.8.3/pyrfuniverse/utils/kinova_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/utils/os_utils.py` & `pyrfuniverse-0.8.3/pyrfuniverse/utils/os_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/utils/rfuniverse_utility.py` & `pyrfuniverse-0.8.3/pyrfuniverse/utils/rfuniverse_utility.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/utils/stretch_controller.py` & `pyrfuniverse-0.8.3/pyrfuniverse/utils/stretch_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/utils/tobor_controller.py` & `pyrfuniverse-0.8.3/pyrfuniverse/utils/tobor_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse/utils/ur5_controller.py` & `pyrfuniverse-0.8.3/pyrfuniverse/utils/ur5_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/pyrfuniverse.egg-info/SOURCES.txt` & `pyrfuniverse-0.8.3/pyrfuniverse.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -124,23 +124,27 @@
 pyrfuniverse/utils/tobor_controller.py
 pyrfuniverse/utils/ur5_controller.py
 test/test_active_depth.py
 test/test_articulation_ik.py
 test/test_camera_image.py
 test/test_custom_message.py
 test/test_debug.py
+test/test_digit.py
 test/test_grasp_pose.py
 test/test_grasp_sim.py
+test/test_heat_map.py
 test/test_humanbody_ik.py
 test/test_label.py
 test/test_light.py
 test/test_load_mesh.py
 test/test_load_urdf.py
 test/test_object_data.py
 test/test_pick_and_place.py
 test/test_pick_and_place_flexiv.py
 test/test_pick_and_place_gym.py
 test/test_point_cloud.py
 test/test_point_cloud_render.py
 test/test_point_cloud_with_intrinsic_matrix.py
+test/test_save_gripper.py
 test/test_save_obj.py
-test/test_scene.py
+test/test_scene.py
+test/test_tobor_move.py
```

### Comparing `pyrfuniverse-0.8.2.1/setup.py` & `pyrfuniverse-0.8.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,14 @@
     install_requires=[
         "cloudpickle",
         "grpcio>=1.11.0",
         "numpy>=1.14.1",
         "Pillow>=4.2.1",
         "protobuf==3.19.0",
         "pyyaml>=3.1.0",
-        # "gym==0.21.0",
+        "gym==0.21.0",
         "opencv-contrib-python",
     ],
     python_requires=">=3.6.1,<3.10",
 )
```

### Comparing `pyrfuniverse-0.8.2.1/test/test_active_depth.py` & `pyrfuniverse-0.8.3/test/test_active_depth.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-import os
-os.environ["OPENCV_IO_ENABLE_OPENEXR"] = "1"
-import cv2
-import numpy as np
-try:
-    import open3d as o3d
-except ImportError:
-    print('This feature requires open3d, please install with `pip install open3d`')
-    raise
-import pyrfuniverse.utils.rfuniverse_utility as utility
-import pyrfuniverse.utils.depth_processor as dp
-from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
-
-env = RFUniverseBaseEnv(scene_file='ActiveDepth.json')
-
-active_light_sensor_1 = env.GetAttr(789789)
-
-main_intrinsic_matrix = [600, 0, 0, 0, 600, 0, 240, 240, 1]
-ir_intrinsic_matrix = [480, 0, 0, 0, 480, 0, 240, 240, 1]
-
-nd_main_intrinsic_matrix = np.reshape(main_intrinsic_matrix, [3, 3]).T
-
-active_light_sensor_1.GetRGB(intrinsic_matrix=main_intrinsic_matrix)
-env.step()
-image_byte = active_light_sensor_1.data['rgb']
-image_rgb = np.frombuffer(image_byte, dtype=np.uint8)
-image_rgb = cv2.imdecode(image_rgb, cv2.IMREAD_COLOR)
-image_rgb = cv2.cvtColor(image_rgb, cv2.COLOR_BGR2RGB)
-image_rgb = np.transpose(image_rgb, [1, 0, 2])
-
-active_light_sensor_1.GetID(intrinsic_matrix=main_intrinsic_matrix)
-env.step()
-image_id = active_light_sensor_1.data['id_map']
-image_id = np.frombuffer(image_id, dtype=np.uint8)
-image_id = cv2.imdecode(image_id, cv2.IMREAD_COLOR)
-image_id = cv2.cvtColor(image_id, cv2.COLOR_BGR2RGB)
-
-active_light_sensor_1.GetDepthEXR(intrinsic_matrix=main_intrinsic_matrix)
-env.step()
-image_depth_exr = active_light_sensor_1.data['depth_exr']
-
-active_light_sensor_1.GetActiveDepth(main_intrinsic_matrix_local = main_intrinsic_matrix, ir_intrinsic_matrix_local = ir_intrinsic_matrix)
-env.step()
-image_active_depth = active_light_sensor_1.data['active_depth']
-image_active_depth = np.transpose(image_active_depth, [1, 0])
-
-local_to_world_matrix = active_light_sensor_1.data['local_to_world_matrix']
-local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
-
-# point = dp.image_array_to_point_cloud(image_rgb, image_active_depth, 45, local_to_world_matrix)
-
-color = utility.EncodeIDAsColor(568451)[0:3]
-real_point_cloud1 = dp.image_bytes_to_point_cloud_intrinsic_matrix(image_byte, image_depth_exr, nd_main_intrinsic_matrix, local_to_world_matrix)
-real_point_cloud1 = dp.mask_point_cloud_with_id_color(real_point_cloud1, image_id, color)
-active_point_cloud1 = dp.image_array_to_point_cloud_intrinsic_matrix(image_rgb, image_active_depth, nd_main_intrinsic_matrix, local_to_world_matrix)
-active_point_cloud1 = dp.mask_point_cloud_with_id_color(active_point_cloud1, image_id, color)
-filtered_point_cloud1 = dp.filter_active_depth_point_cloud_with_exact_depth_point_cloud(active_point_cloud1, real_point_cloud1)
-
-##################################################
-
-active_light_sensor_2 = env.GetAttr(123123)
-
-active_light_sensor_2.GetRGB(intrinsic_matrix=main_intrinsic_matrix)
-env.step()
-image_byte = active_light_sensor_2.data['rgb']
-image_rgb = np.frombuffer(image_byte, dtype=np.uint8)
-image_rgb = cv2.imdecode(image_rgb, cv2.IMREAD_COLOR)
-image_rgb = cv2.cvtColor(image_rgb, cv2.COLOR_BGR2RGB)
-image_rgb = np.transpose(image_rgb, [1, 0, 2])
-
-active_light_sensor_2.GetID(intrinsic_matrix=main_intrinsic_matrix)
-env.step()
-image_id = active_light_sensor_2.data['id_map']
-image_id = np.frombuffer(image_id, dtype=np.uint8)
-image_id = cv2.imdecode(image_id, cv2.IMREAD_COLOR)
-image_id = cv2.cvtColor(image_id, cv2.COLOR_BGR2RGB)
-
-active_light_sensor_2.GetDepthEXR(intrinsic_matrix=main_intrinsic_matrix)
-env.step()
-image_depth_exr = env.instance_channel.data[123123]['depth_exr']
-
-active_light_sensor_2.GetActiveDepth(main_intrinsic_matrix_local = main_intrinsic_matrix, ir_intrinsic_matrix_local = ir_intrinsic_matrix)
-env.step()
-image_active_depth = active_light_sensor_2.data['active_depth']
-image_active_depth = np.transpose(image_active_depth, [1, 0])
-
-local_to_world_matrix = active_light_sensor_2.data['local_to_world_matrix']
-local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
-
-env.close()
-
-# point = dp.image_array_to_point_cloud(image_rgb, image_active_depth, 45, local_to_world_matrix)
-real_point_cloud2 = dp.image_bytes_to_point_cloud_intrinsic_matrix(image_byte, image_depth_exr, nd_main_intrinsic_matrix, local_to_world_matrix)
-real_point_cloud2 = dp.mask_point_cloud_with_id_color(real_point_cloud2, image_id, color)
-active_point_cloud2 = dp.image_array_to_point_cloud_intrinsic_matrix(image_rgb, image_active_depth, nd_main_intrinsic_matrix, local_to_world_matrix)
-active_point_cloud2 = dp.mask_point_cloud_with_id_color(active_point_cloud2, image_id, color)
-filtered_point_cloud2 = dp.filter_active_depth_point_cloud_with_exact_depth_point_cloud(active_point_cloud2, real_point_cloud2)
-
-# unity space to open3d space and show
-real_point_cloud1.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
-real_point_cloud2.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
-active_point_cloud1.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
-active_point_cloud2.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
-filtered_point_cloud1.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
-filtered_point_cloud2.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
-coorninate = o3d.geometry.TriangleMesh.create_coordinate_frame()
-
-o3d.visualization.draw_geometries([real_point_cloud1, real_point_cloud2, coorninate])
-o3d.visualization.draw_geometries([active_point_cloud1, active_point_cloud2, coorninate])
-o3d.visualization.draw_geometries([filtered_point_cloud1, filtered_point_cloud2, coorninate])
+import os
+os.environ["OPENCV_IO_ENABLE_OPENEXR"] = "1"
+import cv2
+import numpy as np
+try:
+    import open3d as o3d
+except ImportError:
+    print('This feature requires open3d, please install with `pip install open3d`')
+    raise
+import pyrfuniverse.utils.rfuniverse_utility as utility
+import pyrfuniverse.utils.depth_processor as dp
+from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
+
+env = RFUniverseBaseEnv(scene_file='ActiveDepth.json')
+
+active_light_sensor_1 = env.GetAttr(789789)
+
+main_intrinsic_matrix = [600, 0, 0, 0, 600, 0, 240, 240, 1]
+ir_intrinsic_matrix = [480, 0, 0, 0, 480, 0, 240, 240, 1]
+
+nd_main_intrinsic_matrix = np.reshape(main_intrinsic_matrix, [3, 3]).T
+
+active_light_sensor_1.GetRGB(intrinsic_matrix=main_intrinsic_matrix)
+env.step()
+image_byte = active_light_sensor_1.data['rgb']
+image_rgb = np.frombuffer(image_byte, dtype=np.uint8)
+image_rgb = cv2.imdecode(image_rgb, cv2.IMREAD_COLOR)
+image_rgb = cv2.cvtColor(image_rgb, cv2.COLOR_BGR2RGB)
+image_rgb = np.transpose(image_rgb, [1, 0, 2])
+
+active_light_sensor_1.GetID(intrinsic_matrix=main_intrinsic_matrix)
+env.step()
+image_id = active_light_sensor_1.data['id_map']
+image_id = np.frombuffer(image_id, dtype=np.uint8)
+image_id = cv2.imdecode(image_id, cv2.IMREAD_COLOR)
+image_id = cv2.cvtColor(image_id, cv2.COLOR_BGR2RGB)
+
+active_light_sensor_1.GetDepthEXR(intrinsic_matrix=main_intrinsic_matrix)
+env.step()
+image_depth_exr = active_light_sensor_1.data['depth_exr']
+
+active_light_sensor_1.GetActiveDepth(main_intrinsic_matrix_local = main_intrinsic_matrix, ir_intrinsic_matrix_local = ir_intrinsic_matrix)
+env.step()
+image_active_depth = active_light_sensor_1.data['active_depth']
+image_active_depth = np.transpose(image_active_depth, [1, 0])
+
+local_to_world_matrix = active_light_sensor_1.data['local_to_world_matrix']
+local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
+
+# point = dp.image_array_to_point_cloud(image_rgb, image_active_depth, 45, local_to_world_matrix)
+
+color = utility.EncodeIDAsColor(568451)[0:3]
+real_point_cloud1 = dp.image_bytes_to_point_cloud_intrinsic_matrix(image_byte, image_depth_exr, nd_main_intrinsic_matrix, local_to_world_matrix)
+real_point_cloud1 = dp.mask_point_cloud_with_id_color(real_point_cloud1, image_id, color)
+active_point_cloud1 = dp.image_array_to_point_cloud_intrinsic_matrix(image_rgb, image_active_depth, nd_main_intrinsic_matrix, local_to_world_matrix)
+active_point_cloud1 = dp.mask_point_cloud_with_id_color(active_point_cloud1, image_id, color)
+filtered_point_cloud1 = dp.filter_active_depth_point_cloud_with_exact_depth_point_cloud(active_point_cloud1, real_point_cloud1)
+
+##################################################
+
+active_light_sensor_2 = env.GetAttr(123123)
+
+active_light_sensor_2.GetRGB(intrinsic_matrix=main_intrinsic_matrix)
+env.step()
+image_byte = active_light_sensor_2.data['rgb']
+image_rgb = np.frombuffer(image_byte, dtype=np.uint8)
+image_rgb = cv2.imdecode(image_rgb, cv2.IMREAD_COLOR)
+image_rgb = cv2.cvtColor(image_rgb, cv2.COLOR_BGR2RGB)
+image_rgb = np.transpose(image_rgb, [1, 0, 2])
+
+active_light_sensor_2.GetID(intrinsic_matrix=main_intrinsic_matrix)
+env.step()
+image_id = active_light_sensor_2.data['id_map']
+image_id = np.frombuffer(image_id, dtype=np.uint8)
+image_id = cv2.imdecode(image_id, cv2.IMREAD_COLOR)
+image_id = cv2.cvtColor(image_id, cv2.COLOR_BGR2RGB)
+
+active_light_sensor_2.GetDepthEXR(intrinsic_matrix=main_intrinsic_matrix)
+env.step()
+image_depth_exr = env.instance_channel.data[123123]['depth_exr']
+
+active_light_sensor_2.GetActiveDepth(main_intrinsic_matrix_local = main_intrinsic_matrix, ir_intrinsic_matrix_local = ir_intrinsic_matrix)
+env.step()
+image_active_depth = active_light_sensor_2.data['active_depth']
+image_active_depth = np.transpose(image_active_depth, [1, 0])
+
+local_to_world_matrix = active_light_sensor_2.data['local_to_world_matrix']
+local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
+
+env.close()
+
+# point = dp.image_array_to_point_cloud(image_rgb, image_active_depth, 45, local_to_world_matrix)
+real_point_cloud2 = dp.image_bytes_to_point_cloud_intrinsic_matrix(image_byte, image_depth_exr, nd_main_intrinsic_matrix, local_to_world_matrix)
+real_point_cloud2 = dp.mask_point_cloud_with_id_color(real_point_cloud2, image_id, color)
+active_point_cloud2 = dp.image_array_to_point_cloud_intrinsic_matrix(image_rgb, image_active_depth, nd_main_intrinsic_matrix, local_to_world_matrix)
+active_point_cloud2 = dp.mask_point_cloud_with_id_color(active_point_cloud2, image_id, color)
+filtered_point_cloud2 = dp.filter_active_depth_point_cloud_with_exact_depth_point_cloud(active_point_cloud2, real_point_cloud2)
+
+# unity space to open3d space and show
+real_point_cloud1.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
+real_point_cloud2.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
+active_point_cloud1.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
+active_point_cloud2.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
+filtered_point_cloud1.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
+filtered_point_cloud2.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
+coorninate = o3d.geometry.TriangleMesh.create_coordinate_frame()
+
+o3d.visualization.draw_geometries([real_point_cloud1, real_point_cloud2, coorninate])
+o3d.visualization.draw_geometries([active_point_cloud1, active_point_cloud2, coorninate])
+o3d.visualization.draw_geometries([filtered_point_cloud1, filtered_point_cloud2, coorninate])
```

### Comparing `pyrfuniverse-0.8.2.1/test/test_articulation_ik.py` & `pyrfuniverse-0.8.3/test/test_articulation_ik.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
-import pyrfuniverse.utils.rfuniverse_utility as utility
-
-env = RFUniverseBaseEnv(
-    scene_file='ArticulationIK.json'
-)
-ids = [639787, 985196, 221584, 8547820, 8547821]
-
-for id in ids:
-    current_robot = env.GetAttr(id)
-    current_robot.IKTargetDoMove(position=[0, 0, -0.5], duration=0.1, relative=True)
-    env.step()
-    while not current_robot.data['move_done']:
-        env.step()
-    current_robot.IKTargetDoMove(position=[0, -0.5, 0], duration=0.1, relative=True)
-    env.step()
-    while not current_robot.data['move_done']:
-        env.step()
-    current_robot.IKTargetDoMove(position=[0, 0.5, 0.5], duration=0.1, relative=True)
-    current_robot.IKTargetDoRotateQuaternion(quaternion=utility.UnityEularToQuaternion([90, 0, 0]), duration=30, relative=True)
-    env.step()
-    while not current_robot.data['move_done'] or not current_robot.data['rotate_done']:
-        env.step()
-
-env.Pend()
+from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
+import pyrfuniverse.utils.rfuniverse_utility as utility
+
+env = RFUniverseBaseEnv(
+    scene_file='ArticulationIK.json'
+)
+ids = [639787, 985196, 221584, 8547820, 8547821]
+
+for id in ids:
+    current_robot = env.GetAttr(id)
+    current_robot.IKTargetDoMove(position=[0, 0, -0.5], duration=0.1, relative=True)
+    env.step()
+    while not current_robot.data['move_done']:
+        env.step()
+    current_robot.IKTargetDoMove(position=[0, -0.5, 0], duration=0.1, relative=True)
+    env.step()
+    while not current_robot.data['move_done']:
+        env.step()
+    current_robot.IKTargetDoMove(position=[0, 0.5, 0.5], duration=0.1, relative=True)
+    current_robot.IKTargetDoRotateQuaternion(quaternion=utility.UnityEularToQuaternion([90, 0, 0]), duration=30, relative=True)
+    env.step()
+    while not current_robot.data['move_done'] or not current_robot.data['rotate_done']:
+        env.step()
+
+env.Pend()
 env.close()
```

### Comparing `pyrfuniverse-0.8.2.1/test/test_camera_image.py` & `pyrfuniverse-0.8.3/test/test_camera_image.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
-import pyrfuniverse.attributes as attr
-import cv2
-import numpy as np
-
-env = RFUniverseBaseEnv(assets=['Camera'])
-
-camera = env.InstanceObject(name='Camera', id=123456, attr_type=attr.CameraAttr)
-camera.SetTransform(position=[0, 0.25, 0], rotation=[30, 0, 0])
-camera.GetDepth(width=512, height=512, zero_dis=1, one_dis=5)
-camera.GetDepthEXR(width=512, height=512)
-camera.GetRGB(width=512, height=512)
-env.step()
-print(camera.data['depth'])
-print(camera.data['depth_exr'])
-print(camera.data['rgb'])
-image_np = np.frombuffer(camera.data['rgb'], dtype=np.uint8)
-image_np = cv2.imdecode(image_np, cv2.IMREAD_COLOR)
-print(image_np.shape)
-env.close()
-cv2.imshow("rgb", image_np)
-cv2.waitKey(0)
+from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
+import pyrfuniverse.attributes as attr
+import cv2
+import numpy as np
+
+env = RFUniverseBaseEnv(assets=['Camera'])
+
+camera = env.InstanceObject(name='Camera', id=123456, attr_type=attr.CameraAttr)
+camera.SetTransform(position=[0, 0.25, 0], rotation=[30, 0, 0])
+camera.GetDepth(width=512, height=512, zero_dis=1, one_dis=5)
+camera.GetDepthEXR(width=512, height=512)
+camera.GetRGB(width=512, height=512)
+env.step()
+print(camera.data['depth'])
+print(camera.data['depth_exr'])
+print(camera.data['rgb'])
+image_np = np.frombuffer(camera.data['rgb'], dtype=np.uint8)
+image_np = cv2.imdecode(image_np, cv2.IMREAD_COLOR)
+print(image_np.shape)
+env.close()
+cv2.imshow("rgb", image_np)
+cv2.waitKey(0)
```

### Comparing `pyrfuniverse-0.8.2.1/test/test_debug.py` & `pyrfuniverse-0.8.3/test/test_debug.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/test/test_grasp_pose.py` & `pyrfuniverse-0.8.3/test/test_grasp_pose.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import os
-try:
-    import pandas as pd
-except ImportError:
-    print('This feature requires pandas, please install with `pip install pandas`')
-    raise
-from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
-import pyrfuniverse.attributes as attr
-
-mesh_path = '../Mesh/drink1/drink1.obj'
-pose_path = '../Mesh/drink1/grasps_rfu.csv'
-
-data = pd.read_csv(pose_path, usecols=['x', 'y', 'z', 'qx', 'qy', 'qz', 'qw'])
-data = data.to_numpy()
-positions = data[:, 0:3].reshape(-1).tolist()
-quaternions = data[:, 3:7].reshape(-1).tolist()
-
-env = RFUniverseBaseEnv()
-grasp_sim = env.InstanceObject(id=123123, name='GraspSim', attr_type=attr.GraspSimAttr)
-grasp_sim.ShowGraspPose(mesh=os.path.abspath(mesh_path), gripper='SimpleFrankaGripper', positions=positions, quaternions=quaternions)
-
-env.Pend()
-env.close()
+import os
+try:
+    import pandas as pd
+except ImportError:
+    print('This feature requires pandas, please install with `pip install pandas`')
+    raise
+from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
+import pyrfuniverse.attributes as attr
+
+mesh_path = '../Mesh/drink1/drink1.obj'
+pose_path = '../Mesh/drink1/grasps_rfu.csv'
+
+data = pd.read_csv(pose_path, usecols=['x', 'y', 'z', 'qx', 'qy', 'qz', 'qw'])
+data = data.to_numpy()
+positions = data[:, 0:3].reshape(-1).tolist()
+quaternions = data[:, 3:7].reshape(-1).tolist()
+
+env = RFUniverseBaseEnv()
+grasp_sim = env.InstanceObject(id=123123, name='GraspSim', attr_type=attr.GraspSimAttr)
+grasp_sim.ShowGraspPose(mesh=os.path.abspath(mesh_path), gripper='SimpleFrankaGripper', positions=positions, quaternions=quaternions)
+
+env.Pend()
+env.close()
```

### Comparing `pyrfuniverse-0.8.2.1/test/test_grasp_sim.py` & `pyrfuniverse-0.8.3/test/test_grasp_sim.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import os
-import numpy as np
-
-try:
-    import pandas as pd
-except ImportError:
-    print('This feature requires pandas, please install with `pip install pandas`')
-    raise
-try:
-    import open3d as o3d
-except ImportError:
-    print('This feature requires open3d, please install with `pip install open3d`')
-    raise
-from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
-import pyrfuniverse.attributes as attr
-
-
-def get_grasp_pose(file: str, points_count, scale: float = 1):
-    mesh = o3d.io.read_triangle_mesh(file)
-    mesh.scale(scale, np.array([0, 0, 0]))
-    sample_points = mesh.sample_points_poisson_disk(points_count, use_triangle_normal=True)
-    sample_points.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
-    points = np.asarray(sample_points.points)
-    normals = np.asarray(sample_points.normals)
-    return points, normals
-
-
-mesh_path = '../Mesh/drink1/drink1.obj'
-
-points, normals = get_grasp_pose(mesh_path, 100)
-points = points.reshape(-1).tolist()
-normals = normals.reshape(-1).tolist()
-
-env = RFUniverseBaseEnv(assets=['GraspSim'])
-grasp_sim = env.InstanceObject(id=123123, name='GraspSim', attr_type=attr.GraspSimAttr)
-grasp_sim.StartGraspSim(mesh=os.path.abspath(mesh_path),
-                        gripper='franka_hand',
-                        points=points,
-                        normals=normals,
-                        depth_range_min=-0.05,
-                        depth_range_max=0,
-                        depth_lerp_count=5,
-                        angle_lerp_count=5,
-                        parallel_count=100
-                        )
-
-# only show grasp pose
-# grasp_sim.GenerateGraspPose(mesh=os.path.abspath(mesh_path),
-#                             gripper='SimpleFrankaGripper',
-#                             points=points,
-#                             normals=normals,
-#                             depth_range_min=-0.05,
-#                             depth_range_max=0,
-#                             depth_lerp_count=5,
-#                             angle_lerp_count=5,
-#                             )
-env.step()
-while not grasp_sim.data['done']:
-    env.step()
-
-points = grasp_sim.data['points']
-points = np.array(points).reshape([-1, 3])
-quaternions = grasp_sim.data['quaternions']
-quaternions = np.array(quaternions).reshape([-1, 4])
-width = grasp_sim.data['width']
-width = np.array(width).reshape([-1, 1])
-print(points.shape)
-data = np.concatenate((points, quaternions, width), axis=1)
-csv = pd.DataFrame(data, columns=['x', 'y', 'z', 'qx', 'qy', 'qz', 'qw', 'width'])
-
-csv_path = os.path.join(os.path.dirname(mesh_path), 'grasps_rfu.csv')
-csv.to_csv(csv_path, index=True, header=True)
-
-env.Pend()
-env.close()
+import os
+import numpy as np
+
+try:
+    import pandas as pd
+except ImportError:
+    print('This feature requires pandas, please install with `pip install pandas`')
+    raise
+try:
+    import open3d as o3d
+except ImportError:
+    print('This feature requires open3d, please install with `pip install open3d`')
+    raise
+from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
+import pyrfuniverse.attributes as attr
+
+
+def get_grasp_pose(file: str, points_count, scale: float = 1):
+    mesh = o3d.io.read_triangle_mesh(file)
+    mesh.scale(scale, np.array([0, 0, 0]))
+    sample_points = mesh.sample_points_poisson_disk(points_count, use_triangle_normal=True)
+    sample_points.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
+    points = np.asarray(sample_points.points)
+    normals = np.asarray(sample_points.normals)
+    return points, normals
+
+
+mesh_path = '../Mesh/drink1/drink1.obj'
+
+points, normals = get_grasp_pose(mesh_path, 100)
+points = points.reshape(-1).tolist()
+normals = normals.reshape(-1).tolist()
+
+env = RFUniverseBaseEnv(assets=['GraspSim'])
+grasp_sim = env.InstanceObject(id=123123, name='GraspSim', attr_type=attr.GraspSimAttr)
+grasp_sim.StartGraspSim(mesh=os.path.abspath(mesh_path),
+                        gripper='franka_hand',
+                        points=points,
+                        normals=normals,
+                        depth_range_min=-0.05,
+                        depth_range_max=0,
+                        depth_lerp_count=5,
+                        angle_lerp_count=5,
+                        parallel_count=100
+                        )
+
+# only show grasp pose
+# grasp_sim.GenerateGraspPose(mesh=os.path.abspath(mesh_path),
+#                             gripper='SimpleFrankaGripper',
+#                             points=points,
+#                             normals=normals,
+#                             depth_range_min=-0.05,
+#                             depth_range_max=0,
+#                             depth_lerp_count=5,
+#                             angle_lerp_count=5,
+#                             )
+env.step()
+while not grasp_sim.data['done']:
+    env.step()
+
+points = grasp_sim.data['points']
+points = np.array(points).reshape([-1, 3])
+quaternions = grasp_sim.data['quaternions']
+quaternions = np.array(quaternions).reshape([-1, 4])
+width = grasp_sim.data['width']
+width = np.array(width).reshape([-1, 1])
+print(points.shape)
+data = np.concatenate((points, quaternions, width), axis=1)
+csv = pd.DataFrame(data, columns=['x', 'y', 'z', 'qx', 'qy', 'qz', 'qw', 'width'])
+
+csv_path = os.path.join(os.path.dirname(mesh_path), 'grasps_rfu.csv')
+csv.to_csv(csv_path, index=True, header=True)
+
+env.Pend()
+env.close()
```

### Comparing `pyrfuniverse-0.8.2.1/test/test_humanbody_ik.py` & `pyrfuniverse-0.8.3/test/test_humanbody_ik.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
-
-env = RFUniverseBaseEnv(scene_file='HumanBodyIK.json')
-env.step()
-human = env.GetAttr(168242)
-for index in range(5):
-    human.HumanIKTargetDoMove(index=index,
-                              position=[0, 0, 0.5],
-                              duration=1,
-                              speed_based=False,
-                              relative=True
-                              )
-    env.step()
-    human.WaitDo()
-    human.HumanIKTargetDoMove(index=index,
-                              position=[0, 0.5, 0],
-                              duration=1,
-                              speed_based=False,
-                              relative=True
-                              )
-    env.step()
-    human.WaitDo()
-    human.HumanIKTargetDoMove(index=index,
-                              position=[0, 0, -0.5],
-                              duration=1,
-                              speed_based=False,
-                              relative=True
-                              )
-    env.step()
-    human.WaitDo()
-    human.HumanIKTargetDoMove(index=index,
-                              position=[0, -0.5, 0],
-                              duration=1,
-                              speed_based=False,
-                              relative=True
-                              )
-    env.step()
-    human.WaitDo()
-
-env.Pend()
-env.close()
+from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
+
+env = RFUniverseBaseEnv(scene_file='HumanBodyIK.json')
+env.step()
+human = env.GetAttr(168242)
+for index in range(5):
+    human.HumanIKTargetDoMove(index=index,
+                              position=[0, 0, 0.5],
+                              duration=1,
+                              speed_based=False,
+                              relative=True
+                              )
+    env.step()
+    human.WaitDo()
+    human.HumanIKTargetDoMove(index=index,
+                              position=[0, 0.5, 0],
+                              duration=1,
+                              speed_based=False,
+                              relative=True
+                              )
+    env.step()
+    human.WaitDo()
+    human.HumanIKTargetDoMove(index=index,
+                              position=[0, 0, -0.5],
+                              duration=1,
+                              speed_based=False,
+                              relative=True
+                              )
+    env.step()
+    human.WaitDo()
+    human.HumanIKTargetDoMove(index=index,
+                              position=[0, -0.5, 0],
+                              duration=1,
+                              speed_based=False,
+                              relative=True
+                              )
+    env.step()
+    human.WaitDo()
+
+env.Pend()
+env.close()
```

### Comparing `pyrfuniverse-0.8.2.1/test/test_label.py` & `pyrfuniverse-0.8.3/test/test_label.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/test/test_light.py` & `pyrfuniverse-0.8.3/test/test_light.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/test/test_load_mesh.py` & `pyrfuniverse-0.8.3/test/test_load_mesh.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import random
-import os
-from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
-
-env = RFUniverseBaseEnv()
-env.step()
-mesh = env.LoadMesh(path=os.path.abspath('../Mesh/002_master_chef_can/google_16k/textured.obj'))
-mesh.SetTransform(position=[0, 1, 0], rotation=[random.random() * 360, random.random() * 360, random.random() * 360])
-
-for i in range(100):
-    env.step(20)
-    new_mesh = mesh.Copy(new_id=mesh.id + i + 1)
-    new_mesh.SetTransform(position=[0, 1, 0], rotation=[random.random() * 360, random.random() * 360, random.random() * 360])
-
-while 1:
-    env.step()
+import random
+import os
+from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
+
+env = RFUniverseBaseEnv()
+env.step()
+mesh = env.LoadMesh(path=os.path.abspath('../Mesh/002_master_chef_can/google_16k/textured.obj'))
+mesh.SetTransform(position=[0, 1, 0], rotation=[random.random() * 360, random.random() * 360, random.random() * 360])
+
+for i in range(100):
+    env.step(20)
+    new_mesh = mesh.Copy(new_id=mesh.id + i + 1)
+    new_mesh.SetTransform(position=[0, 1, 0], rotation=[random.random() * 360, random.random() * 360, random.random() * 360])
+
+while 1:
+    env.step()
```

### Comparing `pyrfuniverse-0.8.2.1/test/test_load_urdf.py` & `pyrfuniverse-0.8.3/test/test_load_urdf.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
-import pyrfuniverse.utils.rfuniverse_utility as utility
-import os
-
-env = RFUniverseBaseEnv()
-
-ur5 = env.LoadURDF(path=os.path.abspath('../URDF/UR5/ur5_robot.urdf'), native_ik=True)
-ur5.SetTransform(position=[1, 0, 0])
-yumi = env.LoadURDF(path=os.path.abspath('../URDF/yumi_description/urdf/yumi.urdf'), native_ik=False)
-yumi.SetTransform(position=[2, 0, 0])
-kinova = env.LoadURDF(path=os.path.abspath('../URDF/kinova_gen3/GEN3_URDF_V12.urdf'), native_ik=False)
-kinova.SetTransform(position=[3, 0, 0])
-
-ur5.IKTargetDoMove(position=[0, 0.5, 0], duration=0.1, relative=True)
-env.step()
-ur5.WaitDo()
-ur5.IKTargetDoMove(position=[0, 0, -0.5], duration=0.1, relative=True)
-env.step()
-ur5.WaitDo()
-ur5.IKTargetDoMove(position=[0, -0.2, 0.3], duration=0.1, relative=True)
-ur5.IKTargetDoRotateQuaternion(quaternion=utility.UnityEularToQuaternion([0, 90, 0]), duration=30, relative=True)
-env.step()
-ur5.WaitDo()
-
-while 1:
-    env.step()
+from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
+import pyrfuniverse.utils.rfuniverse_utility as utility
+import os
+
+env = RFUniverseBaseEnv()
+
+ur5 = env.LoadURDF(path=os.path.abspath('../URDF/UR5/ur5_robot.urdf'), native_ik=True)
+ur5.SetTransform(position=[1, 0, 0])
+yumi = env.LoadURDF(path=os.path.abspath('../URDF/yumi_description/urdf/yumi.urdf'), native_ik=False)
+yumi.SetTransform(position=[2, 0, 0])
+kinova = env.LoadURDF(path=os.path.abspath('../URDF/kinova_gen3/GEN3_URDF_V12.urdf'), native_ik=False)
+kinova.SetTransform(position=[3, 0, 0])
+
+ur5.IKTargetDoMove(position=[0, 0.5, 0], duration=0.1, relative=True)
+env.step()
+ur5.WaitDo()
+ur5.IKTargetDoMove(position=[0, 0, -0.5], duration=0.1, relative=True)
+env.step()
+ur5.WaitDo()
+ur5.IKTargetDoMove(position=[0, -0.2, 0.3], duration=0.1, relative=True)
+ur5.IKTargetDoRotateQuaternion(quaternion=utility.UnityEularToQuaternion([0, 90, 0]), duration=30, relative=True)
+env.step()
+ur5.WaitDo()
+
+while 1:
+    env.step()
```

### Comparing `pyrfuniverse-0.8.2.1/test/test_object_data.py` & `pyrfuniverse-0.8.3/test/test_object_data.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/test/test_pick_and_place.py` & `pyrfuniverse-0.8.3/test/test_pick_and_place.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/test/test_pick_and_place_flexiv.py` & `pyrfuniverse-0.8.3/test/test_pick_and_place_flexiv.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/test/test_pick_and_place_gym.py` & `pyrfuniverse-0.8.3/test/test_pick_and_place_gym.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/test/test_point_cloud.py` & `pyrfuniverse-0.8.3/test/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/test/test_point_cloud_with_intrinsic_matrix.py` & `pyrfuniverse-0.8.3/test/test_point_cloud_with_intrinsic_matrix.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.2.1/test/test_scene.py` & `pyrfuniverse-0.8.3/test/test_scene.py`

 * *Files identical despite different names*

