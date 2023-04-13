# Comparing `tmp/alphamed-federated-0.4.4.tar.gz` & `tmp/alphamed-federated-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphamed-federated-0.4.4.tar", last modified: Mon Mar 27 03:23:56 2023, max compression
+gzip compressed data, was "alphamed-federated-0.4.5.tar", last modified: Thu Apr 13 06:23:26 2023, max compression
```

## Comparing `alphamed-federated-0.4.4.tar` & `alphamed-federated-0.4.5.tar`

### file list

```diff
@@ -1,174 +1,215 @@
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.127128 alphamed-federated-0.4.4/
--rw-r--r--   0 huangyichun   (501) staff       (20)    11357 2022-12-23 06:45:03.000000 alphamed-federated-0.4.4/LICENSE
--rw-r--r--   0 huangyichun   (501) staff       (20)    16954 2023-03-27 03:23:56.126721 alphamed-federated-0.4.4/PKG-INFO
--rw-r--r--   0 huangyichun   (501) staff       (20)     3447 2023-02-10 08:29:13.000000 alphamed-federated-0.4.4/README.md
--rw-r--r--   0 huangyichun   (501) staff       (20)      945 2023-03-27 03:23:36.000000 alphamed-federated-0.4.4/pyproject.toml
--rw-r--r--   0 huangyichun   (501) staff       (20)       38 2023-03-27 03:23:56.127601 alphamed-federated-0.4.4/setup.cfg
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.010488 alphamed-federated-0.4.4/src/
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.021142 alphamed-federated-0.4.4/src/alphafed/
--rw-r--r--   0 huangyichun   (501) staff       (20)      121 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/__init__.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.025569 alphamed-federated-0.4.4/src/alphafed/auto_ml/
--rw-r--r--   0 huangyichun   (501) staff       (20)      180 2022-11-17 10:32:12.000000 alphamed-federated-0.4.4/src/alphafed/auto_ml/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    14678 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/auto_ml/auto_model.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.027221 alphamed-federated-0.4.4/src/alphafed/auto_ml/cvat/
--rw-r--r--   0 huangyichun   (501) staff       (20)        0 2022-11-17 10:32:12.000000 alphamed-federated-0.4.4/src/alphafed/auto_ml/cvat/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     3578 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/auto_ml/cvat/annotation.py
--rw-r--r--   0 huangyichun   (501) staff       (20)      116 2022-11-17 10:32:12.000000 alphamed-federated-0.4.4/src/alphafed/auto_ml/exceptions.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     5758 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/auto_ml/pretrained.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.030523 alphamed-federated-0.4.4/src/alphafed/contractor/
--rw-r--r--   0 huangyichun   (501) staff       (20)      116 2022-09-28 02:13:07.000000 alphamed-federated-0.4.4/src/alphafed/contractor/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     4717 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/contractor/common.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     9772 2023-02-14 06:54:49.000000 alphamed-federated-0.4.4/src/alphafed/contractor/task_contractor.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    23796 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/contractor/task_message_contractor.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.036143 alphamed-federated-0.4.4/src/alphafed/data_channel/
--rw-r--r--   0 huangyichun   (501) staff       (20)      125 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/data_channel/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     6048 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/data_channel/data_channel.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     2105 2022-07-29 05:54:38.000000 alphamed-federated-0.4.4/src/alphafed/data_channel/data_channel_pb2.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     2534 2022-07-29 05:56:31.000000 alphamed-federated-0.4.4/src/alphafed/data_channel/data_channel_pb2_grpc.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    17562 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/data_channel/grpc_data_channel.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    11060 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/data_channel/shared_file_data_channel.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.004934 alphamed-federated-0.4.4/src/alphafed/docs/
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.003928 alphamed-federated-0.4.4/src/alphafed/docs/auto_ml/
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.038168 alphamed-federated-0.4.4/src/alphafed/docs/auto_ml/res/
--rw-r--r--   0 huangyichun   (501) staff       (20)    27911 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/docs/auto_ml/res/auto.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    11996 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/docs/auto_ml/res/res_net.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.040838 alphamed-federated-0.4.4/src/alphafed/docs/customized_scheduler/
--rw-r--r--   0 huangyichun   (501) staff       (20)     6225 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/docs/customized_scheduler/contractor.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    18479 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/docs/customized_scheduler/scheduler.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     5049 2023-02-10 08:25:15.000000 alphamed-federated-0.4.4/src/alphafed/docs/customized_scheduler/simple_task.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.042816 alphamed-federated-0.4.4/src/alphafed/docs/mock/
--rw-r--r--   0 huangyichun   (501) staff       (20)      782 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/docs/mock/net.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     5008 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/docs/mock/scheduler.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.005110 alphamed-federated-0.4.4/src/alphafed/docs/tutorial/
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.043658 alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.045987 alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/auto_model_fed_avg/
--rw-r--r--   0 huangyichun   (501) staff       (20)    23001 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/auto_model_fed_avg/auto_fed_avg.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    11996 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/auto_model_fed_avg/res_net.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.048161 alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/auto_model_local/
--rw-r--r--   0 huangyichun   (501) staff       (20)    21045 2023-02-07 05:16:51.000000 alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/auto_model_local/auto.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    11996 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/auto_model_local/res_net.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1481 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/cnn_net.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.049667 alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/simple_fed_avg/
--rw-r--r--   0 huangyichun   (501) staff       (20)     3039 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/simple_fed_avg/contractor.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    12438 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/simple_fed_avg/scheduler.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.050321 alphamed-federated-0.4.4/src/alphafed/examples/
--rw-r--r--   0 huangyichun   (501) staff       (20)        0 2022-10-09 06:53:49.000000 alphamed-federated-0.4.4/src/alphafed/examples/__init__.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.050744 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/
--rw-r--r--   0 huangyichun   (501) staff       (20)        0 2022-11-17 10:32:12.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/__init__.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.055677 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/
--rw-r--r--   0 huangyichun   (501) staff       (20)      732 2022-11-17 10:32:12.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)      541 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/clean_history_msg.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.057183 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/
--rw-r--r--   0 huangyichun   (501) staff       (20)    28837 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/auto.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    15644 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/inception3.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.059246 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/res_local/
--rw-r--r--   0 huangyichun   (501) staff       (20)    27956 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/res_local/auto.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    15644 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/res_local/inception3.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1348 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/run_aggregator.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1308 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_2.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1308 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_4.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1041 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/run_local.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.062957 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/
--rw-r--r--   0 huangyichun   (501) staff       (20)      732 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)      533 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/clean_history_msg.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.063498 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/
--rw-r--r--   0 huangyichun   (501) staff       (20)    30857 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/auto.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.066256 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/
--rw-r--r--   0 huangyichun   (501) staff       (20)       41 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    14317 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/convolutions.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.067087 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/
--rw-r--r--   0 huangyichun   (501) staff       (20)        0 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    22522 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/senet.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    12274 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/layer_factories.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.067844 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/
--rw-r--r--   0 huangyichun   (501) staff       (20)    29972 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/auto.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.070248 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/
--rw-r--r--   0 huangyichun   (501) staff       (20)       41 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    14317 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/convolutions.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.071620 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/
--rw-r--r--   0 huangyichun   (501) staff       (20)        0 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    22522 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/senet.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    12274 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/layer_factories.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1354 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_aggregator.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1314 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_2.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1314 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_4.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1043 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_local.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.077492 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/
--rw-r--r--   0 huangyichun   (501) staff       (20)      732 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)      533 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/clean_history_msg.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.079175 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/
--rw-r--r--   0 huangyichun   (501) staff       (20)    27957 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/auto.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    11996 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/res_net.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.081291 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/
--rw-r--r--   0 huangyichun   (501) staff       (20)    27051 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/auto.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    11996 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/res_net.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1388 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_aggregator.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1292 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_2.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1292 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_4.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1096 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_local.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.084888 alphamed-federated-0.4.4/src/alphafed/examples/data_channel/
--rw-r--r--   0 huangyichun   (501) staff       (20)      578 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/data_channel/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)      497 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/examples/data_channel/clean_history_msg.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     4544 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/examples/data_channel/run_receiver_2.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     3866 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/examples/data_channel/run_receiver_4.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     6242 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/examples/data_channel/run_sender.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.093582 alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/
--rw-r--r--   0 huangyichun   (501) staff       (20)      732 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)      492 2022-10-19 07:07:15.000000 alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/clean_history_msg.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    23586 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/demo_FedIRM.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    20482 2023-02-13 06:54:32.000000 alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/demos.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1265 2023-02-13 06:54:35.000000 alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/run_aggregator.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1030 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/run_data_owner_2.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1030 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/run_data_owner_3.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1030 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/run_data_owner_4.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1030 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/run_data_owner_5.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.097898 alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/
--rw-r--r--   0 huangyichun   (501) staff       (20)      385 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)      494 2022-10-19 07:07:15.000000 alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/clean_history_msg.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    23092 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/demos.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.102168 alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/psi/
--rw-r--r--   0 huangyichun   (501) staff       (20)      592 2022-10-09 06:53:49.000000 alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/psi/demos.py
--rw-r--r--   0 huangyichun   (501) staff       (20)      819 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/psi/run_collaborator_2.py
--rw-r--r--   0 huangyichun   (501) staff       (20)      819 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/psi/run_collaborator_3.py
--rw-r--r--   0 huangyichun   (501) staff       (20)      819 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/psi/run_collaborator_4.py
--rw-r--r--   0 huangyichun   (501) staff       (20)      819 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/psi/run_collaborator_5.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1046 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/psi/run_initiator.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1218 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/run_collaborater.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1117 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/run_host.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.109794 alphamed-federated-0.4.4/src/alphafed/fed_avg/
--rw-r--r--   0 huangyichun   (501) staff       (20)      103 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/fed_avg/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     9619 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/fed_avg/contractor.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     2026 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/fed_avg/dp_contractor.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     8964 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/fed_avg/dp_fed_avg.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    32945 2023-03-02 10:47:51.000000 alphamed-federated-0.4.4/src/alphafed/fed_avg/fed_avg.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    10441 2023-02-06 08:09:56.000000 alphamed-federated-0.4.4/src/alphafed/fed_avg/secure_contractor.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    34059 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/fed_avg/secure_fed_avg.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1827 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/fs.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.114315 alphamed-federated-0.4.4/src/alphafed/hetero_nn/
--rw-r--r--   0 huangyichun   (501) staff       (20)      116 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/hetero_nn/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    12136 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/hetero_nn/contractor.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    49865 2023-03-01 10:18:34.000000 alphamed-federated-0.4.4/src/alphafed/hetero_nn/hetero_nn.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.117738 alphamed-federated-0.4.4/src/alphafed/hetero_nn/psi/
--rw-r--r--   0 huangyichun   (501) staff       (20)      105 2022-09-28 02:13:07.000000 alphamed-federated-0.4.4/src/alphafed/hetero_nn/psi/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     3489 2022-09-28 02:13:07.000000 alphamed-federated-0.4.4/src/alphafed/hetero_nn/psi/psi.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    14497 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/hetero_nn/psi/rsa_intersecter.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     3753 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/hetero_nn/psi/rsa_psi_contractor.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    14008 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/hetero_nn/secure_contractor.py
--rw-r--r--   0 huangyichun   (501) staff       (20)    74293 2023-03-01 09:07:57.000000 alphamed-federated-0.4.4/src/alphafed/hetero_nn/secure_hetero_nn.py
--rw-r--r--   0 huangyichun   (501) staff       (20)      741 2023-02-28 09:59:36.000000 alphamed-federated-0.4.4/src/alphafed/loggers.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     6428 2023-03-23 10:03:36.000000 alphamed-federated-0.4.4/src/alphafed/mock.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     5037 2023-02-10 02:27:48.000000 alphamed-federated-0.4.4/src/alphafed/perf_bench.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     6441 2023-02-28 09:58:22.000000 alphamed-federated-0.4.4/src/alphafed/scheduler.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.122570 alphamed-federated-0.4.4/src/alphafed/secure/
--rw-r--r--   0 huangyichun   (501) staff       (20)       59 2022-08-18 07:27:08.000000 alphamed-federated-0.4.4/src/alphafed/secure/__init__.py
--rw-r--r--   0 huangyichun   (501) staff       (20)      685 2022-08-17 06:37:43.000000 alphamed-federated-0.4.4/src/alphafed/secure/aes.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1242 2022-08-25 03:23:41.000000 alphamed-federated-0.4.4/src/alphafed/secure/ecdhe.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     2602 2022-08-25 03:24:12.000000 alphamed-federated-0.4.4/src/alphafed/secure/shamir.py
--rw-r--r--   0 huangyichun   (501) staff       (20)      621 2022-08-25 03:23:05.000000 alphamed-federated-0.4.4/src/alphafed/secure/tools.py
--rw-r--r--   0 huangyichun   (501) staff       (20)     1864 2022-12-06 10:16:32.000000 alphamed-federated-0.4.4/src/alphafed/utils.py
-drwxr-xr-x   0 huangyichun   (501) staff       (20)        0 2023-03-27 03:23:56.126235 alphamed-federated-0.4.4/src/alphamed_federated.egg-info/
--rw-r--r--   0 huangyichun   (501) staff       (20)    16954 2023-03-27 03:23:55.000000 alphamed-federated-0.4.4/src/alphamed_federated.egg-info/PKG-INFO
--rw-r--r--   0 huangyichun   (501) staff       (20)     6969 2023-03-27 03:23:56.000000 alphamed-federated-0.4.4/src/alphamed_federated.egg-info/SOURCES.txt
--rw-r--r--   0 huangyichun   (501) staff       (20)        1 2023-03-27 03:23:55.000000 alphamed-federated-0.4.4/src/alphamed_federated.egg-info/dependency_links.txt
--rw-r--r--   0 huangyichun   (501) staff       (20)      208 2023-03-27 03:23:55.000000 alphamed-federated-0.4.4/src/alphamed_federated.egg-info/requires.txt
--rw-r--r--   0 huangyichun   (501) staff       (20)        9 2023-03-27 03:23:55.000000 alphamed-federated-0.4.4/src/alphamed_federated.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.429064 alphamed-federated-0.4.5/
+-rw-rw-rw-   0        0        0    11357 2023-03-29 15:01:00.000000 alphamed-federated-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0    17211 2023-04-13 06:23:26.428065 alphamed-federated-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3447 2023-03-29 15:01:00.000000 alphamed-federated-0.4.5/README.md
+-rw-rw-rw-   0        0        0      945 2023-04-13 06:22:31.000000 alphamed-federated-0.4.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:23:26.429064 alphamed-federated-0.4.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.074804 alphamed-federated-0.4.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.096609 alphamed-federated-0.4.5/src/alphafed/
+-rw-rw-rw-   0        0        0      121 2023-03-29 15:01:28.000000 alphamed-federated-0.4.5/src/alphafed/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.104612 alphamed-federated-0.4.5/src/alphafed/auto_ml/
+-rw-rw-rw-   0        0        0      180 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/auto_ml/__init__.py
+-rw-rw-rw-   0        0        0    14678 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/auto_ml/auto_model.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.110178 alphamed-federated-0.4.5/src/alphafed/auto_ml/cvat/
+-rw-rw-rw-   0        0        0        0 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/auto_ml/cvat/__init__.py
+-rw-rw-rw-   0        0        0     3578 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/auto_ml/cvat/annotation.py
+-rw-rw-rw-   0        0        0      116 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/auto_ml/exceptions.py
+-rw-rw-rw-   0        0        0     5758 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/auto_ml/pretrained.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.117275 alphamed-federated-0.4.5/src/alphafed/contractor/
+-rw-rw-rw-   0        0        0      116 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/contractor/__init__.py
+-rw-rw-rw-   0        0        0     4717 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/contractor/common.py
+-rw-rw-rw-   0        0        0     9772 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/contractor/task_contractor.py
+-rw-rw-rw-   0        0        0    25099 2023-04-13 03:25:38.000000 alphamed-federated-0.4.5/src/alphafed/contractor/task_message_contractor.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.133459 alphamed-federated-0.4.5/src/alphafed/data_channel/
+-rw-rw-rw-   0        0        0      125 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/data_channel/__init__.py
+-rw-rw-rw-   0        0        0     6048 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/data_channel/data_channel.py
+-rw-rw-rw-   0        0        0     2105 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/data_channel/data_channel_pb2.py
+-rw-rw-rw-   0        0        0     2534 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/data_channel/data_channel_pb2_grpc.py
+-rw-rw-rw-   0        0        0    17562 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/data_channel/grpc_data_channel.py
+-rw-rw-rw-   0        0        0    11060 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/data_channel/shared_file_data_channel.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.037626 alphamed-federated-0.4.5/src/alphafed/docs/
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.032626 alphamed-federated-0.4.5/src/alphafed/docs/auto_ml/
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.137458 alphamed-federated-0.4.5/src/alphafed/docs/auto_ml/res/
+-rw-rw-rw-   0        0        0    27911 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/docs/auto_ml/res/auto.py
+-rw-rw-rw-   0        0        0    11996 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/docs/auto_ml/res/res_net.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.143461 alphamed-federated-0.4.5/src/alphafed/docs/customized_scheduler/
+-rw-rw-rw-   0        0        0     6225 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/docs/customized_scheduler/contractor.py
+-rw-rw-rw-   0        0        0    18538 2023-04-12 12:57:03.000000 alphamed-federated-0.4.5/src/alphafed/docs/customized_scheduler/scheduler.py
+-rw-rw-rw-   0        0        0     5049 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/docs/customized_scheduler/simple_task.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.145462 alphamed-federated-0.4.5/src/alphafed/docs/fed_avg/
+-rw-rw-rw-   0        0        0      782 2023-03-29 15:01:29.000000 alphamed-federated-0.4.5/src/alphafed/docs/fed_avg/net.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.148458 alphamed-federated-0.4.5/src/alphafed/docs/mock/
+-rw-rw-rw-   0        0        0      782 2023-03-29 15:01:30.000000 alphamed-federated-0.4.5/src/alphafed/docs/mock/net.py
+-rw-rw-rw-   0        0        0     5008 2023-03-29 15:01:30.000000 alphamed-federated-0.4.5/src/alphafed/docs/mock/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.037626 alphamed-federated-0.4.5/src/alphafed/docs/tutorial/
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.150459 alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.153457 alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/auto_model_fed_avg/
+-rw-rw-rw-   0        0        0    23001 2023-03-29 15:01:30.000000 alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/auto_model_fed_avg/auto_fed_avg.py
+-rw-rw-rw-   0        0        0    11996 2023-03-29 15:01:30.000000 alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/auto_model_fed_avg/res_net.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.158574 alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/auto_model_local/
+-rw-rw-rw-   0        0        0    21045 2023-03-29 15:01:31.000000 alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/auto_model_local/auto.py
+-rw-rw-rw-   0        0        0    11996 2023-03-29 15:01:31.000000 alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/auto_model_local/res_net.py
+-rw-rw-rw-   0        0        0     1481 2023-03-29 15:01:30.000000 alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/cnn_net.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.162562 alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/simple_fed_avg/
+-rw-rw-rw-   0        0        0     3039 2023-03-29 15:03:24.000000 alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/simple_fed_avg/contractor.py
+-rw-rw-rw-   0        0        0    12837 2023-04-12 12:49:52.000000 alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/simple_fed_avg/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.164563 alphamed-federated-0.4.5/src/alphafed/examples/
+-rw-rw-rw-   0        0        0        0 2023-03-29 15:03:24.000000 alphamed-federated-0.4.5/src/alphafed/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.165582 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/
+-rw-rw-rw-   0        0        0        0 2023-03-29 15:03:24.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.178564 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/
+-rw-rw-rw-   0        0        0      732 2023-03-29 15:03:24.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/__init__.py
+-rw-rw-rw-   0        0        0      541 2023-03-29 15:03:24.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/clean_history_msg.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.181565 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/
+-rw-rw-rw-   0        0        0    28837 2023-03-29 15:03:24.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/auto.py
+-rw-rw-rw-   0        0        0    15644 2023-03-29 15:03:27.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/inception3.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.186325 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/res_local/
+-rw-rw-rw-   0        0        0    27956 2023-04-07 07:21:53.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/res_local/auto.py
+-rw-rw-rw-   0        0        0    15644 2023-03-29 15:03:29.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/res_local/inception3.py
+-rw-rw-rw-   0        0        0     1348 2023-03-29 15:03:24.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/run_aggregator.py
+-rw-rw-rw-   0        0        0     1308 2023-03-29 15:03:24.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_2.py
+-rw-rw-rw-   0        0        0     1308 2023-03-29 15:03:24.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_4.py
+-rw-rw-rw-   0        0        0     1041 2023-03-29 15:03:24.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/run_local.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.198644 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/
+-rw-rw-rw-   0        0        0      732 2023-03-29 15:03:29.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/__init__.py
+-rw-rw-rw-   0        0        0      533 2023-03-29 15:03:29.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/clean_history_msg.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.201642 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/
+-rw-rw-rw-   0        0        0    30857 2023-03-29 15:03:29.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/auto.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.208166 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/
+-rw-rw-rw-   0        0        0       41 2023-03-29 15:03:31.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/__init__.py
+-rw-rw-rw-   0        0        0    14317 2023-03-29 15:03:31.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/convolutions.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.213166 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/
+-rw-rw-rw-   0        0        0        0 2023-03-29 15:03:31.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/__init__.py
+-rw-rw-rw-   0        0        0    22522 2023-03-29 15:03:31.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/senet.py
+-rw-rw-rw-   0        0        0    12274 2023-03-29 15:03:31.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/layer_factories.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.214166 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/
+-rw-rw-rw-   0        0        0    29972 2023-03-29 15:03:31.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/auto.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.221485 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/
+-rw-rw-rw-   0        0        0       41 2023-03-29 15:03:33.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/__init__.py
+-rw-rw-rw-   0        0        0    14317 2023-03-29 15:03:33.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/convolutions.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.225483 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/
+-rw-rw-rw-   0        0        0        0 2023-03-29 15:03:33.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/__init__.py
+-rw-rw-rw-   0        0        0    22522 2023-03-29 15:03:33.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/senet.py
+-rw-rw-rw-   0        0        0    12274 2023-03-29 15:03:33.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/layer_factories.py
+-rw-rw-rw-   0        0        0     1354 2023-03-29 15:03:29.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_aggregator.py
+-rw-rw-rw-   0        0        0     1314 2023-03-29 15:03:29.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_2.py
+-rw-rw-rw-   0        0        0     1314 2023-03-29 15:03:29.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_4.py
+-rw-rw-rw-   0        0        0     1043 2023-03-29 15:03:29.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_local.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.238481 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/
+-rw-rw-rw-   0        0        0      732 2023-03-29 15:03:33.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/__init__.py
+-rw-rw-rw-   0        0        0      533 2023-03-29 15:03:33.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/clean_history_msg.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.242480 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/
+-rw-rw-rw-   0        0        0    27957 2023-03-29 15:03:33.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/auto.py
+-rw-rw-rw-   0        0        0    11996 2023-03-29 15:03:33.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/res_net.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.246481 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/
+-rw-rw-rw-   0        0        0    27051 2023-03-29 15:03:34.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/auto.py
+-rw-rw-rw-   0        0        0    11996 2023-03-29 15:03:34.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/res_net.py
+-rw-rw-rw-   0        0        0     1388 2023-03-29 15:03:33.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_aggregator.py
+-rw-rw-rw-   0        0        0     1292 2023-03-29 15:03:33.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_2.py
+-rw-rw-rw-   0        0        0     1292 2023-03-29 15:03:33.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_4.py
+-rw-rw-rw-   0        0        0     1096 2023-03-29 15:03:33.000000 alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_local.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.257791 alphamed-federated-0.4.5/src/alphafed/examples/data_channel/
+-rw-rw-rw-   0        0        0      578 2023-03-29 15:03:35.000000 alphamed-federated-0.4.5/src/alphafed/examples/data_channel/__init__.py
+-rw-rw-rw-   0        0        0      497 2023-03-29 15:03:35.000000 alphamed-federated-0.4.5/src/alphafed/examples/data_channel/clean_history_msg.py
+-rw-rw-rw-   0        0        0     4544 2023-03-29 15:03:35.000000 alphamed-federated-0.4.5/src/alphafed/examples/data_channel/run_receiver_2.py
+-rw-rw-rw-   0        0        0     3866 2023-03-29 15:03:35.000000 alphamed-federated-0.4.5/src/alphafed/examples/data_channel/run_receiver_4.py
+-rw-rw-rw-   0        0        0     6242 2023-03-29 15:03:35.000000 alphamed-federated-0.4.5/src/alphafed/examples/data_channel/run_sender.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.274357 alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/
+-rw-rw-rw-   0        0        0      736 2023-04-13 02:23:18.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/__init__.py
+-rw-rw-rw-   0        0        0      492 2023-03-29 15:03:35.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/clean_history_msg.py
+-rw-rw-rw-   0        0        0    23586 2023-03-29 15:03:35.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/demo_FedIRM.py
+-rw-rw-rw-   0        0        0    20482 2023-03-29 15:03:35.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/demos.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.278355 alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/model/
+-rw-rw-rw-   0        0        0     5021 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/model/my_scheduler.py
+-rw-rw-rw-   0        0        0      782 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/model/net.py
+-rw-rw-rw-   0        0        0     1265 2023-03-29 15:03:35.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/run_aggregator.py
+-rw-rw-rw-   0        0        0     1030 2023-03-29 15:03:35.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/run_data_owner_2.py
+-rw-rw-rw-   0        0        0     1030 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/run_data_owner_3.py
+-rw-rw-rw-   0        0        0     1030 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/run_data_owner_4.py
+-rw-rw-rw-   0        0        0     1030 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/run_data_owner_5.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.290971 alphamed-federated-0.4.5/src/alphafed/examples/fed_md/
+-rw-rw-rw-   0        0        0      736 2023-04-13 02:23:18.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_md/__init__.py
+-rw-rw-rw-   0        0        0      492 2023-03-29 15:03:35.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_md/clean_history_msg.py
+-rw-rw-rw-   0        0        0     7556 2023-04-13 06:17:28.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_md/demos.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.299304 alphamed-federated-0.4.5/src/alphafed/examples/fed_md/model/
+-rw-rw-rw-   0        0        0    10630 2023-04-12 09:11:34.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_md/model/contractor.py
+-rw-rw-rw-   0        0        0      384 2023-04-12 09:11:32.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_md/model/loss.py
+-rw-rw-rw-   0        0        0     6818 2023-04-12 09:48:27.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_md/model/my_homo_fed_md_impl.py
+-rw-rw-rw-   0        0        0      782 2023-04-12 09:11:31.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_md/model/net.py
+-rw-rw-rw-   0        0        0    31535 2023-04-13 06:16:45.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_md/model/scheduler.py
+-rw-rw-rw-   0        0        0      514 2023-04-13 06:17:45.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_md/run_aggregator.py
+-rw-rw-rw-   0        0        0      499 2023-04-13 06:17:54.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_md/run_data_owner_2.py
+-rw-rw-rw-   0        0        0      499 2023-04-13 06:18:22.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_md/run_data_owner_4.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.311889 alphamed-federated-0.4.5/src/alphafed/examples/fed_per/
+-rw-rw-rw-   0        0        0      736 2023-04-13 02:23:18.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_per/__init__.py
+-rw-rw-rw-   0        0        0      492 2023-03-29 15:03:35.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_per/clean_history_msg.py
+-rw-rw-rw-   0        0        0     5747 2023-04-13 06:05:41.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_per/demos.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.317896 alphamed-federated-0.4.5/src/alphafed/examples/fed_per/model/
+-rw-rw-rw-   0        0        0     1420 2023-04-11 09:28:02.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_per/model/contractor.py
+-rw-rw-rw-   0        0        0     5033 2023-04-12 04:47:33.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_per/model/my_homo_fed_per_impl.py
+-rw-rw-rw-   0        0        0      939 2023-04-11 09:28:02.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_per/model/net.py
+-rw-rw-rw-   0        0        0    11157 2023-04-13 06:00:22.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_per/model/scheduler.py
+-rw-rw-rw-   0        0        0      516 2023-04-13 05:55:12.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_per/run_aggregator.py
+-rw-rw-rw-   0        0        0      501 2023-04-13 06:06:23.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_per/run_data_owner_2.py
+-rw-rw-rw-   0        0        0      501 2023-04-13 06:06:34.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_per/run_data_owner_4.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.330528 alphamed-federated-0.4.5/src/alphafed/examples/fed_prox/
+-rw-rw-rw-   0        0        0      736 2023-04-13 02:23:18.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_prox/__init__.py
+-rw-rw-rw-   0        0        0      492 2023-03-29 15:03:35.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_prox/clean_history_msg.py
+-rw-rw-rw-   0        0        0     5870 2023-04-13 05:44:09.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_prox/demos.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.335252 alphamed-federated-0.4.5/src/alphafed/examples/fed_prox/model/
+-rw-rw-rw-   0        0        0     5124 2023-04-11 08:25:09.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_prox/model/my_fed_prox_impl.py
+-rw-rw-rw-   0        0        0      782 2023-04-10 09:03:18.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_prox/model/net.py
+-rw-rw-rw-   0        0        0     2425 2023-04-10 09:03:17.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_prox/model/scheduler.py
+-rw-rw-rw-   0        0        0      518 2023-04-13 05:55:53.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_prox/run_aggregator.py
+-rw-rw-rw-   0        0        0      503 2023-04-13 05:55:51.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_prox/run_data_owner_2.py
+-rw-rw-rw-   0        0        0      503 2023-04-13 05:55:48.000000 alphamed-federated-0.4.5/src/alphafed/examples/fed_prox/run_data_owner_4.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.345351 alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/
+-rw-rw-rw-   0        0        0      389 2023-04-13 04:20:24.000000 alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/clean_history_msg.py
+-rw-rw-rw-   0        0        0    23092 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/demos.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.357359 alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/psi/
+-rw-rw-rw-   0        0        0      592 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/psi/demos.py
+-rw-rw-rw-   0        0        0      819 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/psi/run_collaborator_2.py
+-rw-rw-rw-   0        0        0      819 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/psi/run_collaborator_3.py
+-rw-rw-rw-   0        0        0      819 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/psi/run_collaborator_4.py
+-rw-rw-rw-   0        0        0      819 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/psi/run_collaborator_5.py
+-rw-rw-rw-   0        0        0     1046 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/psi/run_initiator.py
+-rw-rw-rw-   0        0        0     1218 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/run_collaborater.py
+-rw-rw-rw-   0        0        0     1117 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/run_host.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.368826 alphamed-federated-0.4.5/src/alphafed/fed_avg/
+-rw-rw-rw-   0        0        0      103 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/fed_avg/__init__.py
+-rw-rw-rw-   0        0        0     9619 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/fed_avg/contractor.py
+-rw-rw-rw-   0        0        0     2026 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/fed_avg/dp_contractor.py
+-rw-rw-rw-   0        0        0     8964 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/fed_avg/dp_fed_avg.py
+-rw-rw-rw-   0        0        0    33004 2023-04-12 12:58:20.000000 alphamed-federated-0.4.5/src/alphafed/fed_avg/fed_avg.py
+-rw-rw-rw-   0        0        0    10441 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/fed_avg/secure_contractor.py
+-rw-rw-rw-   0        0        0    34059 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/fed_avg/secure_fed_avg.py
+-rw-rw-rw-   0        0        0     1827 2023-03-29 15:01:28.000000 alphamed-federated-0.4.5/src/alphafed/fs.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.378070 alphamed-federated-0.4.5/src/alphafed/hetero_nn/
+-rw-rw-rw-   0        0        0      116 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/hetero_nn/__init__.py
+-rw-rw-rw-   0        0        0    12136 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/hetero_nn/contractor.py
+-rw-rw-rw-   0        0        0    49965 2023-04-12 13:02:10.000000 alphamed-federated-0.4.5/src/alphafed/hetero_nn/hetero_nn.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.384065 alphamed-federated-0.4.5/src/alphafed/hetero_nn/psi/
+-rw-rw-rw-   0        0        0      105 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/hetero_nn/psi/__init__.py
+-rw-rw-rw-   0        0        0     3489 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/hetero_nn/psi/psi.py
+-rw-rw-rw-   0        0        0    14497 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/hetero_nn/psi/rsa_intersecter.py
+-rw-rw-rw-   0        0        0     3753 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/hetero_nn/psi/rsa_psi_contractor.py
+-rw-rw-rw-   0        0        0    14008 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/hetero_nn/secure_contractor.py
+-rw-rw-rw-   0        0        0    74393 2023-04-12 13:02:27.000000 alphamed-federated-0.4.5/src/alphafed/hetero_nn/secure_hetero_nn.py
+-rw-rw-rw-   0        0        0      741 2023-03-29 15:01:28.000000 alphamed-federated-0.4.5/src/alphafed/loggers.py
+-rw-rw-rw-   0        0        0     6428 2023-03-29 15:01:28.000000 alphamed-federated-0.4.5/src/alphafed/mock.py
+-rw-rw-rw-   0        0        0     5037 2023-03-29 15:01:28.000000 alphamed-federated-0.4.5/src/alphafed/perf_bench.py
+-rw-rw-rw-   0        0        0     6441 2023-03-29 15:01:28.000000 alphamed-federated-0.4.5/src/alphafed/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.395068 alphamed-federated-0.4.5/src/alphafed/secure/
+-rw-rw-rw-   0        0        0       59 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/secure/__init__.py
+-rw-rw-rw-   0        0        0      685 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/secure/aes.py
+-rw-rw-rw-   0        0        0     1242 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/secure/ecdhe.py
+-rw-rw-rw-   0        0        0     2602 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/secure/shamir.py
+-rw-rw-rw-   0        0        0      621 2023-03-29 15:03:36.000000 alphamed-federated-0.4.5/src/alphafed/secure/tools.py
+-rw-rw-rw-   0        0        0     1864 2023-03-29 15:01:28.000000 alphamed-federated-0.4.5/src/alphafed/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:23:26.426066 alphamed-federated-0.4.5/src/alphamed_federated.egg-info/
+-rw-rw-rw-   0        0        0    17211 2023-04-13 06:23:25.000000 alphamed-federated-0.4.5/src/alphamed_federated.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8530 2023-04-13 06:23:26.000000 alphamed-federated-0.4.5/src/alphamed_federated.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:23:25.000000 alphamed-federated-0.4.5/src/alphamed_federated.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      208 2023-04-13 06:23:25.000000 alphamed-federated-0.4.5/src/alphamed_federated.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 06:23:25.000000 alphamed-federated-0.4.5/src/alphamed_federated.egg-info/top_level.txt
```

### Comparing `alphamed-federated-0.4.4/LICENSE` & `alphamed-federated-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/PKG-INFO` & `alphamed-federated-0.4.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,257 +1,257 @@
-Metadata-Version: 2.1
-Name: alphamed-federated
-Version: 0.4.4
-Summary: AlphaMed Federated Learning Module
-Author-email: Huang Yi Chun <huangyichun@jinghang.ai>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright [yyyy] [name of copyright owner]
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Project-URL: Homepage, https://github.com/ssplabs/alphafed
-Project-URL: Bug Tracker, https://github.com/ssplabs/alphafed/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# AlphaMed
-
-AlphaMed 是一个基于区块链技术的去中心化联邦学习解决方案，旨在使医疗机构能够在保证其医疗数据隐私和安全的同时，实现多机构联合建模。医疗机构可以在本地节点实现模型的训练，并支持以匿名的身份将加密的参数共享至聚合节点，从而实现更安全、可信的联邦学习。
-
-相比于传统的联邦学习，AlphaMed 平台不仅能够确保只有合法的且经过许可的参与者才能加入网络，同时支持节点的匿名化的参与联合建模。同时，区块链的共识算法能够确保网络中的节点得到一直的决策，恶意的参与者或者数据投毒等攻击将被拒绝，从而保证了联邦学习更好的安全性。
-
-在联邦学习的过程中，各个参与方都受到智能合约的约束，并且所有的事件、操作都将被记录在区块链的分布式账本上，可追溯、可审计，使得联合机器学习的安全性和隐私保护能力极大的提升。
-
-[开始构建第一个联邦学习任务](src/alphafed/docs/fed_avg/README.md)
-
-[在不同结构的数据源之间构建异构联邦学习任务](src/alphafed/docs/hetero_nn/README.md)
-
-如果 AlphaMed 平台预置的现有算法依然无法满足业务需要，还可以自行设计联邦学习算法，并使其运行在 AlphaMed 平台之上。[这里](src/alphafed/docs/customized_scheduler/README.md)展示了如果自定义联邦学习算法，并通过 AlphaMed 平台实际执行联邦学习任务。为了帮助开发者调试自己的代码，AlphaMed 平台还提供了一套[模拟运行环境](src/alphafed/docs/mock/README.md)，以在本地节点模拟实际运行环境，包括联邦学习运行环境。
-
-AlphaMed 平台除面向算法工程师提供了开发联邦学习模型的支持外，还面向模型使用者提供了预训练模型的支持。与传统预训练模型相比，AlphaMed 平台上的预训练模型支持功能更为强大、使用更为方便。在 AlphaMed 平台上，不仅可以寻找并下载心仪的预训练模型，更可以利用私有数据微调、部署预训练模型，使其更加适配于私有的业务数据。
-
-AlphaMed 平台预置了一定数量的预训练模型，同时也支持第三方开发者开发上传自己的预训练模型。[这里展示了如何设计自己的预训练模型。](src/alphafed/docs/auto_ml/README.md)
-
-## 项目目录说明
-
-src/alphafed  
-├── auto_ml  *AutoML 模块*  
-│   └── cvat  *CVAT 工具*  
-├── contractor  *合约消息工具*  
-├── data_channel  *数据传输工具*  
-├── docs  *说明文档*  
-│   ├── auto_ml  *AutoML 说明文档*  
-│   ├── customized_scheduler  *自定义调度器说明文档*  
-│   ├── fed_avg  *FedAvg 横向联邦说明文档*  
-│   ├── hetero_nn  *HeteroNN 异构联邦说明文档*  
-│   ├── mock  *模拟调试说明文档*  
-│   └── tutorial  *tutorial 示例说明文档，包含所有主要功能*  
-├── examples  *脚本测试代码 / 示例代码*  
-├── fed_avg  *FedAvg 横向联邦模块*  
-├── hetero_nn  *HeteroNN 异构联邦模块*  
-│   └── psi  *隐私求交模块*  
-├── secure  *安全工具*  
-├── fs.py  *文件系统工具*  
-├── loggers.py  *日志工具*  
-├── mock.py  *模拟调试工具*  
-└── utils.py  *其它工具*
+Metadata-Version: 2.1
+Name: alphamed-federated
+Version: 0.4.5
+Summary: AlphaMed Federated Learning Module
+Author-email: Huang Yi Chun <huangyichun@jinghang.ai>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Project-URL: Homepage, https://github.com/ssplabs/alphafed
+Project-URL: Bug Tracker, https://github.com/ssplabs/alphafed/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AlphaMed
+
+AlphaMed 是一个基于区块链技术的去中心化联邦学习解决方案，旨在使医疗机构能够在保证其医疗数据隐私和安全的同时，实现多机构联合建模。医疗机构可以在本地节点实现模型的训练，并支持以匿名的身份将加密的参数共享至聚合节点，从而实现更安全、可信的联邦学习。
+
+相比于传统的联邦学习，AlphaMed 平台不仅能够确保只有合法的且经过许可的参与者才能加入网络，同时支持节点的匿名化的参与联合建模。同时，区块链的共识算法能够确保网络中的节点得到一直的决策，恶意的参与者或者数据投毒等攻击将被拒绝，从而保证了联邦学习更好的安全性。
+
+在联邦学习的过程中，各个参与方都受到智能合约的约束，并且所有的事件、操作都将被记录在区块链的分布式账本上，可追溯、可审计，使得联合机器学习的安全性和隐私保护能力极大的提升。
+
+[开始构建第一个联邦学习任务](src/alphafed/docs/fed_avg/README.md)
+
+[在不同结构的数据源之间构建异构联邦学习任务](src/alphafed/docs/hetero_nn/README.md)
+
+如果 AlphaMed 平台预置的现有算法依然无法满足业务需要，还可以自行设计联邦学习算法，并使其运行在 AlphaMed 平台之上。[这里](src/alphafed/docs/customized_scheduler/README.md)展示了如果自定义联邦学习算法，并通过 AlphaMed 平台实际执行联邦学习任务。为了帮助开发者调试自己的代码，AlphaMed 平台还提供了一套[模拟运行环境](src/alphafed/docs/mock/README.md)，以在本地节点模拟实际运行环境，包括联邦学习运行环境。
+
+AlphaMed 平台除面向算法工程师提供了开发联邦学习模型的支持外，还面向模型使用者提供了预训练模型的支持。与传统预训练模型相比，AlphaMed 平台上的预训练模型支持功能更为强大、使用更为方便。在 AlphaMed 平台上，不仅可以寻找并下载心仪的预训练模型，更可以利用私有数据微调、部署预训练模型，使其更加适配于私有的业务数据。
+
+AlphaMed 平台预置了一定数量的预训练模型，同时也支持第三方开发者开发上传自己的预训练模型。[这里展示了如何设计自己的预训练模型。](src/alphafed/docs/auto_ml/README.md)
+
+## 项目目录说明
+
+src/alphafed  
+├── auto_ml  *AutoML 模块*  
+│   └── cvat  *CVAT 工具*  
+├── contractor  *合约消息工具*  
+├── data_channel  *数据传输工具*  
+├── docs  *说明文档*  
+│   ├── auto_ml  *AutoML 说明文档*  
+│   ├── customized_scheduler  *自定义调度器说明文档*  
+│   ├── fed_avg  *FedAvg 横向联邦说明文档*  
+│   ├── hetero_nn  *HeteroNN 异构联邦说明文档*  
+│   ├── mock  *模拟调试说明文档*  
+│   └── tutorial  *tutorial 示例说明文档，包含所有主要功能*  
+├── examples  *脚本测试代码 / 示例代码*  
+├── fed_avg  *FedAvg 横向联邦模块*  
+├── hetero_nn  *HeteroNN 异构联邦模块*  
+│   └── psi  *隐私求交模块*  
+├── secure  *安全工具*  
+├── fs.py  *文件系统工具*  
+├── loggers.py  *日志工具*  
+├── mock.py  *模拟调试工具*  
+└── utils.py  *其它工具*
```

### Comparing `alphamed-federated-0.4.4/README.md` & `alphamed-federated-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/pyproject.toml` & `alphamed-federated-0.4.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphamed-federated"
-version = "0.4.4"
+version = "0.4.5"
 dependencies = [
     "cloudpickle==2.0.0",
     "grpcio==1.47.0",
     "protobuf==3.20.0",
     "pycryptodomex==3.15.0",
     "requests==2.28.1",
     "torch==1.11.0",
```

### Comparing `alphamed-federated-0.4.4/src/alphafed/auto_ml/auto_model.py` & `alphamed-federated-0.4.5/src/alphafed/auto_ml/auto_model.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/auto_ml/cvat/annotation.py` & `alphamed-federated-0.4.5/src/alphafed/auto_ml/cvat/annotation.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/auto_ml/pretrained.py` & `alphamed-federated-0.4.5/src/alphafed/auto_ml/pretrained.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/contractor/common.py` & `alphamed-federated-0.4.5/src/alphafed/contractor/common.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/contractor/task_contractor.py` & `alphamed-federated-0.4.5/src/alphafed/contractor/task_contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/contractor/task_message_contractor.py` & `alphamed-federated-0.4.5/src/alphafed/contractor/task_message_contractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,28 +174,31 @@
         return AcceptSharedFileSendingDataEvent(session_id=session_id, receiver=receiver)
 
 
 @dataclass
 class UploadTaskAchievementEvent(ContractEvent):
     """A event of uploading task achievement materials."""
 
-    TYPE = 'upload_task_achieve'
+    TYPE = 'task_file_upload'
 
-    model: str
-    report: str = None
+    FILE_TYPE_REPORT = 'report'
+    FILE_TYPE_MODEL = 'model'
+
+    file_type: str
+    file_url: str
 
     @classmethod
     def contract_to_event(cls, contract: dict) -> 'UploadTaskAchievementEvent':
         event_type = contract.get('type')
-        model = contract.get('model')
-        report = contract.get('report')
+        file_type = contract.get('file_type')
+        file_url = contract.get('file_url')
         assert event_type == cls.TYPE, f'合约类型错误: {event_type}'
-        assert model and isinstance(model, str), f'invalid model: {model}'
-        assert not report or isinstance(report, str), f'invalid report: {report}'
-        return UploadTaskAchievementEvent(model=model, report=report)
+        assert file_type in (cls.FILE_TYPE_REPORT, cls.FILE_TYPE_MODEL), f'invalid file_type: {file_type}'
+        assert file_url and isinstance(file_url, str), f'invalid file_url: {file_url}'
+        return UploadTaskAchievementEvent(file_type=file_type, file_url=file_url)
 
 
 @dataclass
 class NoticeTaskCompletionEvent(ContractEvent):
     """A event of noticing task manager that current task is complete."""
 
     TYPE = 'notice_task_completion'
@@ -238,21 +241,23 @@
 
 class TaskMessageContractor(Contractor):
     """公共合约."""
 
     _URL = 'http://federated-service:9080/fed-service/api/v2/message'
 
     _TASK_INSIDE = 'task_inside'
-    _UPLOAD_TASK_ACHIEVE = 'task_result_upload'
+    _UPLOAD_TASK_ACHIEVE = 'task_file_upload'
     _TASK_FINISH = 'task_finish'
 
     _TITLE_ALL = (_TASK_INSIDE, _UPLOAD_TASK_ACHIEVE, _TASK_FINISH)
 
     _CHANNEL = 'federated'
 
+    EMPTY_ACHIVEMENT = 'https://minio.ssplabs.com/playground-saas/tmp.zip'
+
     def __init__(self, task_id: str) -> None:
         super().__init__()
         self.task_id = task_id
         self._event_factory = TaskMessageEventFactory
         self._task_contractor = TaskContractor(task_id=task_id)
 
     def _validate_response(self, resp: Response) -> dict:
@@ -491,56 +496,78 @@
             else:
                 time.sleep(1)
 
     @retry()
     def query_address(self, target: str) -> Optional[str]:
         """Query address of the target."""
         return self._task_contractor.query_address(target=target)
+    
+    def upload_metric_report(self, receivers: List[str], report_file: str = None):
+        """Upload metrics report materials after a task is complete.
 
-    def upload_task_achivement(self,
-                               aggregator: str,
-                               model_file: str,
-                               report_file: str = ''):
-        """Upload achivement materials after a task is complete.
-
-        :args
-            :aggregator
-                The ID of the aggregator.
-            :model_file
-                Local path of the model file.
-            :report_file
+        Args:
+            receivers:
+                Specify who can receive and download this report.
+            report_file:
                 Local path of the report file.
+
+        If nothing need be uploaded, specify report_file to None or an empty value.
         """
-        assert aggregator and isinstance(aggregator, str), f'unknown aggregator: {aggregator}'
-        assert (
-            model_file and isinstance(model_file, str)
-            and os.path.exists(model_file)
-            and os.path.isfile(model_file)
-        ), f'the model_file does not exist or can not be accessed: {model_file}'
-        if report_file:
+        if not receivers or not report_file:
+            report_file_url = self.EMPTY_ACHIVEMENT
+        else:
             assert (
-                isinstance(report_file, str)
-                and os.path.exists(report_file)
-                and os.path.isfile(report_file)
+                isinstance(receivers, list) and all(isinstance(_receiver, str) for _receiver in receivers)
+            ), f'invalid receivers: {receivers}'
+            assert (
+                isinstance(report_file, str) and os.path.isfile(report_file)
             ), f'the report_file does not exist or can not be accessed: {report_file}'
 
-        with open(model_file, 'rb') as model_fp:
-            model_file_url = self.upload_file(fp=model_fp,
-                                              persistent=True,
-                                              upload_name=os.path.basename(model_file))
-        report_file_url = ''
-        if report_file:
             with open(report_file, 'rb') as report_fp:
                 report_file_url = self.upload_file(fp=report_fp,
                                                    persistent=True,
                                                    upload_name=os.path.basename(report_file))
 
-        event = UploadTaskAchievementEvent(report=report_file_url,
-                                           model=model_file_url)
-        TxId = self._new_contract(targets=[aggregator],
+        event = UploadTaskAchievementEvent(file_type=UploadTaskAchievementEvent.FILE_TYPE_REPORT,
+                                           file_url=report_file_url)
+        TxId = self._new_contract(targets=receivers,
+                                  event=event,
+                                  message_title=self._UPLOAD_TASK_ACHIEVE)
+        if not TxId:
+            raise ContractException('failed to notify task completion')
+    
+    def upload_model(self, receivers: List[str], model_file: str = None):
+        """Upload final model after a task is complete.
+
+        Args:
+            receivers:
+                Specify who can receive and download this report.
+            model_file:
+                Local path of the model file.
+
+        If nothing need be uploaded, specify model_file to None or an empty value.
+        """
+        if not receivers or not model_file:
+            model_file_url = self.EMPTY_ACHIVEMENT
+        else:
+            assert (
+                isinstance(receivers, list) and all(isinstance(_receiver, str) for _receiver in receivers)
+            ), f'invalid receivers: {receivers}'
+            assert (
+                isinstance(model_file, str) and os.path.isfile(model_file)
+            ), f'the model_file does not exist or can not be accessed: {model_file}'
+
+            with open(model_file, 'rb') as model_fp:
+                model_file_url = self.upload_file(fp=model_fp,
+                                                  persistent=True,
+                                                  upload_name=os.path.basename(model_file))
+
+        event = UploadTaskAchievementEvent(file_type=UploadTaskAchievementEvent.FILE_TYPE_MODEL,
+                                           file_url=model_file_url)
+        TxId = self._new_contract(targets=receivers,
                                   event=event,
                                   message_title=self._UPLOAD_TASK_ACHIEVE)
         if not TxId:
             raise ContractException('failed to notify task completion')
 
     def notify_task_completion(self, result: bool):
         """Notify task manager a task is complete.
```

### Comparing `alphamed-federated-0.4.4/src/alphafed/data_channel/data_channel.py` & `alphamed-federated-0.4.5/src/alphafed/data_channel/data_channel.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/data_channel/data_channel_pb2.py` & `alphamed-federated-0.4.5/src/alphafed/data_channel/data_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/data_channel/data_channel_pb2_grpc.py` & `alphamed-federated-0.4.5/src/alphafed/data_channel/data_channel_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/data_channel/grpc_data_channel.py` & `alphamed-federated-0.4.5/src/alphafed/data_channel/grpc_data_channel.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/data_channel/shared_file_data_channel.py` & `alphamed-federated-0.4.5/src/alphafed/data_channel/shared_file_data_channel.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/docs/auto_ml/res/auto.py` & `alphamed-federated-0.4.5/src/alphafed/docs/auto_ml/res/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/docs/auto_ml/res/res_net.py` & `alphamed-federated-0.4.5/src/alphafed/docs/auto_ml/res/res_net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/docs/customized_scheduler/contractor.py` & `alphamed-federated-0.4.5/src/alphafed/docs/customized_scheduler/contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/docs/customized_scheduler/scheduler.py` & `alphamed-federated-0.4.5/src/alphafed/docs/customized_scheduler/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -420,17 +420,18 @@
         uploads the final parameters and tells L1 task manager the task is complete.
         As a participant, do nothing.
         """
         self.push_log(f'Closing task {self.task_id} ...')
         if self.is_initiator:
             self._switch_status(self._FINISHING)
             report_file_path, model_file_path = self._prepare_task_output()
-            self.contractor.upload_task_achivement(aggregator=self.contractor.EVERYONE[0],
-                                                   report_file=report_file_path,
-                                                   model_file=model_file_path)
+            self.contractor.upload_metric_report(receivers=self.contractor.EVERYONE,
+                                                 report_file=report_file_path)
+            self.contractor.upload_model(receivers=self.contractor.EVERYONE,
+                                         model_file=model_file_path)
             self.contractor.notify_task_completion(result=True)
         self.push_log(f'Task {self.task_id} closed. Byebye!')
 
     def _prepare_task_output(self) -> Tuple[str, str]:
         """Generate final output files of the task.
 
         Return:
```

### Comparing `alphamed-federated-0.4.4/src/alphafed/docs/customized_scheduler/simple_task.py` & `alphamed-federated-0.4.5/src/alphafed/docs/customized_scheduler/simple_task.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/docs/mock/net.py` & `alphamed-federated-0.4.5/src/alphafed/docs/mock/net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/docs/mock/scheduler.py` & `alphamed-federated-0.4.5/src/alphafed/docs/mock/scheduler.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/auto_model_fed_avg/auto_fed_avg.py` & `alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/auto_model_fed_avg/auto_fed_avg.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/auto_model_fed_avg/res_net.py` & `alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/auto_model_fed_avg/res_net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/auto_model_local/auto.py` & `alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/auto_model_local/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/auto_model_local/res_net.py` & `alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/auto_model_local/res_net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/cnn_net.py` & `alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/cnn_net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/simple_fed_avg/contractor.py` & `alphamed-federated-0.4.5/src/alphafed/docs/tutorial/res/simple_fed_avg/contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/docs/tutorial/res/simple_fed_avg/scheduler.py` & `alphamed-federated-0.4.5/src/alphafed/examples/fed_per/model/scheduler.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,259 +1,275 @@
+"""HomoFedPer Scheduler."""
 import io
+import json
 import os
-from abc import ABCMeta, abstractmethod
-from tempfile import TemporaryFile
+import sys
+import traceback
+from abc import abstractmethod
+from typing import Dict, Tuple, final
 from zipfile import ZipFile
 
 import torch
-from torch.nn import Module
-from torch.utils.tensorboard import SummaryWriter
+from torch.nn import Module, Sequential
 
-from alphafed.data_channel import SharedFileDataChannel
-from alphafed.fs import get_result_dir
-from alphafed.scheduler import Scheduler
+from alphafed import logger
+from alphafed.fed_avg import FedAvgScheduler
+from alphafed.fed_avg.fed_avg import ResetRound, SkipRound
+from alphafed.scheduler import TaskComplete, TaskFailed
+
+from .contractor import CollaboratorCompleteEvent, HomoFedPerContractor
+
+
+class HomoFedPerScheduler(FedAvgScheduler):
+
+    _FINISHED = 'finished'
+
+    def __init__(self,
+                 max_rounds: int = 0,
+                 merge_epochs: int = 1,
+                 calculation_timeout: int = 300,
+                 schedule_timeout: int = 30,
+                 log_rounds: int = 0):
+        super().__init__(max_rounds=max_rounds,
+                         merge_epochs=merge_epochs,
+                         calculation_timeout=calculation_timeout,
+                         schedule_timeout=schedule_timeout,
+                         log_rounds=log_rounds,
+                         involve_aggregator=False)
 
-from .contractor import (CheckInEvent, CheckInResponseEvent, CloseEvent,
-                         SimpleFedAvgContractor, StartEvent)
+    def _init_contractor(self) -> HomoFedPerContractor:
+        return HomoFedPerContractor(task_id=self.task_id)
 
+    @abstractmethod
+    def build_global_model(self) -> Module:
+        """Return a global model object which will be used for training."""
 
-class SimpleFedAvgScheduler(Scheduler, metaclass=ABCMeta):
-
-    def __init__(self, rounds: int) -> None:
-        super().__init__()
-        # 自定义一些初始化参数，此处只定义了 rounds 一个参数，用于设置训练的轮数
-        self.rounds = rounds
-
-    def _run(self, id: str, task_id: str, is_initiator: bool = False, recover: bool = False):
-        """运行调度器的入口。
+    @final
+    @property
+    def global_model(self) -> Module:
+        """Get the model object which is used for training."""
+        if not hasattr(self, '_global_model'):
+            self._global_model = self.build_global_model()
+        return self._global_model
 
-        实际运行时由任务管理器负责传入接口参数，模拟环境下需要调试者自行传入模拟值。
+    @abstractmethod
+    def build_personalized_layer(self) -> Module:
+        """Return a personalized layer object which will be used for training."""
 
-        参数说明:
-            id: 当前节点 ID
-            task_id: 当前任务 ID
-            is_initiator: 当前节点是否是任务发起方
-            recover: 是否使用恢复模式启动
-        """
-        # 先记录传入的参数，由于不支持恢复模式，可以忽略 recover
-        self.id = id
-        self.task_id = task_id
-        self.is_initiator = is_initiator
-
-        # 发起方作为聚合方，其它节点作为参与方
-        if self.is_initiator:
-            self._run_as_aggregator()
+    @final
+    @property
+    def personalized_layer(self) -> Module:
+        """Get the model object which is used for training."""
+        if not hasattr(self, '_personalized_layer'):
+            self._personalized_layer = self.build_personalized_layer()
+        return self._personalized_layer
+
+    @final
+    def build_model(self) -> Module:
+        if self.is_aggregator:
+            return self.global_model
         else:
-            self._run_as_collaborator()
+            return Sequential(
+                self.global_model,
+                self.personalized_layer
+            )
 
-    @abstractmethod
-    def before_check_in(self, is_aggregator: bool):
-        """完成集合前初始化本地资源。"""
+    def state_dict(self) -> Dict[str, torch.Tensor]:
+        return self.global_model.state_dict()
 
-    @abstractmethod
-    def before_training(self, is_aggregator: bool):
-        """训练开始前的初始化工作。"""
+    def load_state_dict(self, state_dict: Dict[str, torch.Tensor]):
+        return self.global_model.load_state_dict(state_dict)
 
-    @property
-    @abstractmethod
-    def model(self) -> Module:
-        """获取训练使用的模型对象。"""
+    def _run(self, id: str, task_id: str, is_initiator: bool = False, recover: bool = False):
+        self._setup_context(id=id, task_id=task_id, is_initiator=is_initiator)
+        self.push_log(message='Local context is ready.')
+        try:
+            if recover:
+                self._recover_progress()
+            else:
+                self._clean_progress()
+            self._launch_process()
+        except Exception:
+            err_stack = '\n'.join(traceback.format_exception(*sys.exc_info()))
+            self.push_log(err_stack)
+
+    def _recover_progress(self):
+        """Try to recover and continue from last running."""
+        if not os.path.isfile(self._context_file):
+            raise TaskFailed('Failed to recover progress: missing cached context.')
+
+        with open(self._context_file, 'r') as f:
+            context_info: dict = json.load(f)
+        round = context_info.get('round')
+        ckpt_file = context_info.get('ckpt_file')
+        assert round and isinstance(round, int) and round > 0, f'Invalid round: {round} .'
+        assert ckpt_file and isinstance(ckpt_file, str), f'Invalid ckpt_file: {ckpt_file} .'
+        if not os.path.isfile(ckpt_file):
+            raise TaskFailed('Failed to recover progress: missing checkpoint parameters.')
+
+        self.current_round = round
+        with open(ckpt_file, 'rb') as f:
+            state_dict = torch.load(f)
+            if self.is_aggregator:
+                self.global_model.load_state_dict(state_dict)
+            else:
+                self.model.load_state_dict(state_dict)
 
-    @abstractmethod
-    def train_an_epoch(self):
-        """完成一个 epoch 训练的逻辑。"""
+    def _save_model(self):
+        """Save latest model state."""
+        with open(self._ckpt_file, 'wb') as f:
+            if self.is_aggregator:
+                torch.save(self.global_model.state_dict(), f)
+            else:
+                torch.save(self.model.state_dict(), f)
+        self.push_log('Saved latest parameters locally.')
 
-    @abstractmethod
-    def run_test(self, writer: SummaryWriter):
-        """测试的逻辑。"""
+    def _launch_process(self):
+        try:
+            assert self.status == self._INIT, 'must begin from initial status'
+            self.push_log(f'Node {self.id} is up.')
+
+            self._switch_status(self._GETHORING)
+            self._check_in()
+
+            self._switch_status(self._READY)
+            while self.status == self._READY:
+                try:
+                    self._switch_status(self._SYNCHRONIZING)
+                    self._sync_state()
+
+                    self._switch_status(self._IN_A_ROUND)
+                    self._run_a_round()
+                    self._persistent_running_context()
+                    self._switch_status(self._READY)
+                except ResetRound:
+                    self.push_log('WARNING: Reset runtime context, there might be an error raised.')
+                    self._switch_status(self._READY)
+                    continue
+
+                if self.is_aggregator:
+                    is_finished = self.is_task_finished()
+                    self._switch_status(self._READY)
+                    self.current_round += 1
+                    if is_finished:
+                        self.push_log(f'Obtained the final results of task {self.task_id}')
+                        self._switch_status(self._FINISHING)
+                        self._close_task()  # 聚合方退出
+
+        except TaskComplete:
+            self._close_task()  # 数据持有方退出
+            logger.info('training task complete')
+
+    def _check_and_run_test(self):
+        """Run test if match configured conditions."""
+        if self.is_aggregator:
+            return
+        if (
+            self.current_round == 1
+            or (self.log_rounds > 0 and self.current_round % self.log_rounds == 0)
+            or self.current_round == self.max_rounds
+        ):
+            self.push_log('Begin to make a model test.')
+            self.run_test()
+            self.push_log('Finished a round of test.')
+
+    def _close_task(self):
+        """Close the FedAvg calculation.
+
+        As an aggregator, broadcasts the finish task event to all participants,
+        uploads the final parameters and tells L1 task manager the task is complete.
+        As a participant, do nothing.
+        """
+        self.push_log(f'Closing task {self.task_id} ...')
+        self.contractor: HomoFedPerContractor
+        if self.is_aggregator:
+            # 任务成功结束，聚合方处理
+            self.contractor.finish_task()
+            _, model_file_path = self._prepare_task_output()
+            # 报告上传和模型上传
+            self.contractor.upload_metric_report(receivers=[self.id])
+            self.contractor.upload_model(receivers=[self.id],
+                                         model_file=model_file_path)
+            self._wait_for_all_complete()
+            self.contractor.notify_task_completion(result=True)
+
+        else:  # 数据持有方
+            report_file_path, model_file_path = self._prepare_task_output()
+            # 报告上传和模型上传
+            self.contractor.upload_metric_report(receivers=[self.id],
+                                                 report_file=report_file_path)
+            self.contractor.upload_model(receivers=[self.id],
+                                         model_file=model_file_path)
+            self.contractor.notify_collaborator_complete(peer_id=self.id, host=self._aggregator)
+        self._switch_status(self._FINISHED)
+        self.push_log(f'Task {self.task_id} closed. Byebye!')
 
-    def _run_as_aggregator(self):
-        """作为聚合方运行."""
-        # 初始化本地资源
-        self.contractor = SimpleFedAvgContractor(task_id=self.task_id)
-        self.data_channel = SharedFileDataChannel(contractor=self.contractor)
-
-        self.collaborators = self.contractor.query_nodes()
-        self.collaborators.remove(self.id)  # 把自己移出去
-        self.checked_in = set()  # 记录集合的参与方
-        self.result_dir = get_result_dir(self.task_id)
-        self.log_dir = os.path.join(self.result_dir, 'tb_logs')  # 记录测试评估指标的目录
-        self.tb_writer = SummaryWriter(log_dir=self.log_dir)  # 记录测试评估指标的 writter
-
-        self.round = 0
-
-        # 调用 before_check_in 执行用户自定义的额外初始化逻辑。
-        # 聚合方与参与方的初始化逻辑可能会不一样，所以加一个 is_aggregator 参数已做区分。接口定义也据此更新。
-        self.before_check_in(is_aggregator=True)
-        self.push_log(f'节点 {self.id} 初始化完毕。')
+    def _prepare_task_output(self) -> Tuple[str, str]:
+        """Generate final output files of the task.
 
-        # 监听集合请求
-        self.push_log('开始等待参与成员集合 ...')
-        for _event in self.contractor.contract_events():
-            if isinstance(_event, CheckInEvent):
-                # 收到集合请求后，记录参与者，并向请求方回复集合响应
-                self.checked_in.add(_event.peer_id)
-                self.contractor.response_check_in(aggr_id=self.id, peer_id=_event.peer_id)
-                self.push_log(f'成员 {_event.peer_id} 加入。')
-                # 统计参与者数量，如果集合完成退出循环
-                if len(self.collaborators) == len(self.checked_in):
-                    break  # 退出监听循环
-        self.push_log(f'参与成员集合完毕，共有 {len(self.checked_in)} 位参与者。')
-
-        # 完成训练初始化工作
-        self.model  # 初始化模型
-        # 调用 before_training 执行用户自定义的额外初始化逻辑。
-        # 聚合方与参与方的初始化逻辑可能会不一样，所以加一个 is_aggregator 参数已做区分。接口定义也据此更新。
-        self.before_training(is_aggregator=True)
-        self.push_log(f'节点 {self.id} 准备就绪，可以开始执行计算任务。')
-
-        for _round in range(self.rounds):
-            # 发送开始训练的通知
-            self.round = _round
-            self.contractor.start()
-            self.push_log(f'第 {_round + 1} 轮训练开始。')
-            # 计数训练轮次，发送全局模型
-            with TemporaryFile() as f:
-                torch.save(self.model.state_dict(), f)
-                f.seek(0)
-                self.push_log('开始发送全局模型 ...')
-                self.data_channel.batch_send_stream(source=self.id,
-                                                    target=self.collaborators,
-                                                    data_stream=f.read(),
-                                                    ensure_all_succ=True)
-            self.push_log('发送全局模型完成。')
-            # 监听本地模型传输请求，收集本地模型
-            self.updates = []  # 记录本地模型参数更新
-            self.push_log('开始等待收集本地模型 ...')
-            training_results = self.data_channel.batch_receive_stream(
-                receiver=self.id,
-                source_list=self.collaborators,
-                ensure_all_succ=True
-            )
-            for _source, _result in training_results.items():
-                buffer = io.BytesIO(_result)
-                state_dict = torch.load(buffer)
-                self.updates.append(state_dict)
-                self.push_log(f'收到来自 {_source} 的本地模型。')
-            # 聚合得到新的全局模型
-            self.push_log('开始执行参数聚合 ...')
-            self._make_aggregation()
-            self.push_log('参数聚合完成。')
-            # 如果达到训练轮次，循环结束
-
-            # 使用测试数据做一次测试，得到全局模型的评估指标数据
-            # 测试时指定 TensorBoard 的 writter，否则用户使用自定义的 writter，无法控制日志文件目录。
-            # 接口定义也据此更新。
-            self.push_log('训练完成，测试训练效果 ...')
-            self.run_test(writer=self.tb_writer)
-            self.push_log('测试完成。')
-
-        # 上传模型文件和评估指标数据
-        # 打包记录测试时写入的所有 TensorBoard 日志文件
-        self.push_log('整理计算结果，准备上传 ...')
-        report_file = os.path.join(self.result_dir, "report.zip")
-        with ZipFile(report_file, 'w') as report_zip:
-            for path, _, filenames in os.walk(self.log_dir):
-                rel_dir = os.path.relpath(path=path, start=self.result_dir)
-                rel_dir = rel_dir.lstrip('.')  # ./file => file
-                for _file in filenames:
-                    rel_path = os.path.join(rel_dir, _file)
-                    report_zip.write(os.path.join(path, _file), rel_path)
-        report_file_path = os.path.abspath(report_file)
-        # 记录训练后的模型参数
-        model_file = os.path.join(self.result_dir, "model.pt")
+        Return:
+            Local paths of the report file and model file.
+        """
+        self.push_log('Uploading task achievement and closing task ...')
+
+        report_file_path = None
+        if not self.is_aggregator:
+            report_file = os.path.join(self._result_dir, "report.zip")
+            with ZipFile(report_file, 'w') as report_zip:
+                for path, _, filenames in os.walk(self._log_dir):
+                    rel_dir = os.path.relpath(path=path, start=self._result_dir)
+                    rel_dir = rel_dir.lstrip('.')  # ./file => file
+                    for _file in filenames:
+                        rel_path = os.path.join(rel_dir, _file)
+                        report_zip.write(os.path.join(path, _file), rel_path)
+            report_file_path = os.path.abspath(report_file)
+
+        model_file = os.path.join(
+            self._result_dir,
+            "global_model.pt" if self.is_aggregator else "personalized_model.pt"
+        )
         with open(model_file, 'wb') as f:
-            torch.save(self.model.state_dict(), f)
+            torch.save(self.global_model.state_dict() if self.is_aggregator else self.model.state_dict(), f)
         model_file_path = os.path.abspath(model_file)
-        # 调用接口执行上传
-        self.contractor.upload_task_achivement(aggregator=self.contractor.EVERYONE[0],
-                                               report_file=report_file_path,
-                                               model_file=model_file_path)
-        self.push_log('计算结果上传完成。')
-
-        # 通知任务管理器训练结束，完成训练退出
-        self.contractor.notify_task_completion(result=True)
-        self.contractor.close()
-        self.push_log('计算任务完成。')
-
-    def _make_aggregation(self):
-        """执行参数聚合。"""
-        # 模型参数清零
-        global_params = self.model.state_dict()
-        for _param in global_params.values():
-            if isinstance(_param, torch.Tensor):
-                _param.zero_()
-        # 累加收到的本地模型参数
-        for _update in self.updates:
-            for _key in global_params.keys():
-                global_params[_key].add_(_update[_key])
-        # 求平均值获得新的全局参数
-        count = len(self.collaborators)
-        for _key in global_params.keys():
-            if global_params[_key].dtype in (
-                torch.uint8, torch.int8, torch.int16, torch.int32, torch.int64
-            ):
-                global_params[_key].div_(count, rounding_mode='trunc')
-            else:
-                global_params[_key].div_(count)
-        self.model.load_state_dict(global_params)
 
-    def _run_as_collaborator(self):
-        """作为参与方运行。"""
-        # 初始化本地资源
-        self.contractor = SimpleFedAvgContractor(task_id=self.task_id)
-        self.data_channel = SharedFileDataChannel(contractor=self.contractor)
-
-        # 调用 before_check_in 执行用户自定义的额外初始化逻辑。
-        # 聚合方与参与方的初始化逻辑可能会不一样，所以加一个 is_aggregator 参数已做区分。接口定义也据此更新。
-        self.before_check_in(is_aggregator=False)
-        self.push_log(f'节点 {self.id} 初始化完毕。')
-
-        # 广播发送集合请求
-        self.push_log('发送集合请求，等待聚合方响应。')
-        self.contractor.check_in(peer_id=self.id)
-        # 监听集合响应，收到集合响应后，记录聚合方
+        self.push_log('Task achievement files are ready.')
+        return report_file_path, model_file_path
+
+    def _wait_for_all_complete(self):
+        """Wait for all collaborators complete their tasks."""
+        self.push_log('Waiting for all collaborators complete their tasks ...')
+        results = {_peer_id: False for _peer_id in self.participants if _peer_id != self.id}
         for _event in self.contractor.contract_events():
-            if isinstance(_event, CheckInResponseEvent):
-                self.aggregator = _event.aggr_id
-                self.push_log('收到响应，集合成功。')
-                break  # 退出监听循环
-
-        # 完成训练初始化工作
-        self.model  # 初始化模型
-        # 调用 before_training 执行用户自定义的额外初始化逻辑。
-        # 聚合方与参与方的初始化逻辑可能会不一样，所以加一个 is_aggregator 参数已做区分。接口定义也据此更新。
-        self.before_training(is_aggregator=False)
-        self.push_log(f'节点 {self.id} 准备就绪，可以开始执行计算任务。')
-
-        while True:
-            self.push_log('等待训练开始信号 ...')
-            # 监听开始训练消息或训练结束消息；如果收到开始训练消息，跳到第 6 步；如果收到训练结束消息，完成训练退出
-            for _event in self.contractor.contract_events():
-                if isinstance(_event, StartEvent):
-                    self.push_log('开始训练 ...')
-                    break  # 退出监听循环
-                elif isinstance(_event, CloseEvent):
-                    self.push_log('训练完成。')
-                    return  # 退出训练
-            # 监听传输全局模型消息
-            self.push_log('等待接收全局模型 ...')
-            _, data_stream = self.data_channel.receive_stream(receiver=self.id,
-                                                              source=self.aggregator)
-            buffer = io.BytesIO(data_stream)
-            new_state = torch.load(buffer)
-            self.model.load_state_dict(new_state)
-            self.push_log('接收全局模型成功。')
-            # 在本地做一个 epoch 的训练，更新本地模型
-            self.push_log('开始训练本地模型 ...')
-            self.train_an_epoch()
-            self.push_log('训练本地模型完成。')
-            # 将本地模型发送给聚合方
-            with TemporaryFile() as f:
-                torch.save(self.model.state_dict(), f)
-                f.seek(0)
-                self.push_log('准备发送本地模型 ...')
-                self.data_channel.send_stream(source=self.id,
-                                              target=self.aggregator,
-                                              data_stream=f.read())
-                self.push_log('发送本地模型完成。')
-            # 继续循环
+            if isinstance(_event, CollaboratorCompleteEvent):
+                results[_event.peer_id] = True
+                if all(results.values()):
+                    break
+        self.push_log('All collaborators have completed their tasks.')
+
+    def _run_as_data_owner(self):
+        try:
+            self._wait_for_starting_round()
+            self._switch_status(self._UPDATING)
+            self._wait_for_updating_model()
+            self._save_model()
+            self._switch_status(self._CALCULATING)
+            self.push_log('Begin to run calculation ...')
+            self._execute_training()
+            self.push_log('Local calculation complete.')
+
+            self._wait_for_uploading_model()
+            buffer = io.BytesIO()
+            torch.save(self.state_dict(), buffer)
+            self.push_log('Pushing local update to the aggregator ...')
+            self.data_channel.send_stream(source=self.id,
+                                          target=self._aggregator,
+                                          data_stream=buffer.getvalue())
+            self.push_log('Successfully pushed local update to the aggregator.')
+
+            self._check_and_run_test()
+
+            self._switch_status(self._CLOSING_ROUND)
+            self._wait_for_closing_round()
+        except SkipRound:
+            pass
+
+        self.push_log(f'ID: {self.id} finished training task of round {self.current_round}.')
```

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/__init__.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/clean_history_msg.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/clean_history_msg.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/auto.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/inception3.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/inception3.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/res_local/auto.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/res_local/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/res_local/inception3.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/res_local/inception3.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/run_aggregator.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/run_aggregator.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_2.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_2.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_4.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_4.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/breast_density_classification/run_local.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/breast_density_classification/run_local.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/__init__.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/clean_history_msg.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/clean_history_msg.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/auto.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/convolutions.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/convolutions.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/senet.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/senet.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/layer_factories.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/layer_factories.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/auto.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/convolutions.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/convolutions.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/senet.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/senet.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/layer_factories.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/layer_factories.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_aggregator.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_aggregator.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_2.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_2.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_4.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_4.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_local.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_local.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/__init__.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/__init__.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/clean_history_msg.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/clean_history_msg.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/auto.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/res_net.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/res_net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/auto.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/res_net.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/res_net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_aggregator.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_aggregator.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_2.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_2.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_4.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_4.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_local.py` & `alphamed-federated-0.4.5/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_local.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/data_channel/__init__.py` & `alphamed-federated-0.4.5/src/alphafed/examples/data_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/data_channel/run_receiver_2.py` & `alphamed-federated-0.4.5/src/alphafed/examples/data_channel/run_receiver_2.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/data_channel/run_receiver_4.py` & `alphamed-federated-0.4.5/src/alphafed/examples/data_channel/run_receiver_4.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/data_channel/run_sender.py` & `alphamed-federated-0.4.5/src/alphafed/examples/data_channel/run_sender.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/__init__.py` & `alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # CPU mode
-DEV_TASK_ID = 'c9e3231c7c924700b05180650416f2a3'
+DEV_TASK_ID = 'd041d19f-59d0-467f-bc6c-7f5cf42436c2'
 
 AGGREGATOR_ID = 'QmXLxxW7W1cxdU7eeeq5yRXte53zekxiTRApSWxxssdzQP'
 DATA_OWNER_2_ID = 'QmUXV1ds7mNfZ5udaLauubMC5ve4mGpuwS6sTy6Keh2VJN'
 DATA_OWNER_3_ID = 'QmXG7aTnKk1AcLhKmauCkYpYafoxj1dG5xLBnCQNniuaeF'
 DATA_OWNER_4_ID = 'QmfFQ1CDXU8kYGMSkqPGqMw7NfnjGsfr3jPU9GbSBY4P3J'
 DATA_OWNER_5_ID = 'QmYX5KatFyFve3xVjadX2h7fEt1SzpdA8wnQsQ4v9muCyR'
```

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/demo_FedIRM.py` & `alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/demo_FedIRM.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/demos.py` & `alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/demos.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/run_aggregator.py` & `alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/run_aggregator.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/run_data_owner_2.py` & `alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/run_data_owner_2.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/run_data_owner_3.py` & `alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/run_data_owner_3.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/run_data_owner_4.py` & `alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/run_data_owner_4.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/fed_avg/run_data_owner_5.py` & `alphamed-federated-0.4.5/src/alphafed/examples/fed_avg/run_data_owner_5.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/demos.py` & `alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/demos.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/psi/demos.py` & `alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/psi/demos.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/psi/run_collaborator_2.py` & `alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/psi/run_collaborator_2.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/psi/run_collaborator_3.py` & `alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/psi/run_collaborator_3.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/psi/run_collaborator_4.py` & `alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/psi/run_collaborator_4.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/psi/run_collaborator_5.py` & `alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/psi/run_collaborator_5.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/psi/run_initiator.py` & `alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/psi/run_initiator.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/run_collaborater.py` & `alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/run_collaborater.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/examples/hetero_nn/run_host.py` & `alphamed-federated-0.4.5/src/alphafed/examples/hetero_nn/run_host.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/fed_avg/contractor.py` & `alphamed-federated-0.4.5/src/alphafed/fed_avg/contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/fed_avg/dp_contractor.py` & `alphamed-federated-0.4.5/src/alphafed/fed_avg/dp_contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/fed_avg/dp_fed_avg.py` & `alphamed-federated-0.4.5/src/alphafed/fed_avg/dp_fed_avg.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/fed_avg/fed_avg.py` & `alphamed-federated-0.4.5/src/alphafed/fed_avg/fed_avg.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,17 +414,18 @@
         As a participant, do nothing.
         """
         self.push_log(f'Closing task {self.task_id} ...')
         if is_succ and self.is_aggregator:
             self._switch_status(self._FINISHING)
             self.contractor.finish_task()
             report_file_path, model_file_path = self._prepare_task_output()
-            self.contractor.upload_task_achivement(aggregator=self.contractor.EVERYONE[0],
-                                                   report_file=report_file_path,
-                                                   model_file=model_file_path)
+            self.contractor.upload_metric_report(receivers=self.contractor.EVERYONE,
+                                                 report_file=report_file_path)
+            self.contractor.upload_model(receivers=self.contractor.EVERYONE,
+                                         model_file=model_file_path)
             self.contractor.notify_task_completion(result=True)
         elif self.is_aggregator:
             self.contractor.finish_task()
             self.contractor.notify_task_completion(result=False)
         self.push_log(f'Task {self.task_id} closed. Byebye!')
 
     def _wait_for_gathering(self):
```

### Comparing `alphamed-federated-0.4.4/src/alphafed/fed_avg/secure_contractor.py` & `alphamed-federated-0.4.5/src/alphafed/fed_avg/secure_contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/fed_avg/secure_fed_avg.py` & `alphamed-federated-0.4.5/src/alphafed/fed_avg/secure_fed_avg.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/fs.py` & `alphamed-federated-0.4.5/src/alphafed/fs.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/hetero_nn/contractor.py` & `alphamed-federated-0.4.5/src/alphafed/hetero_nn/contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/hetero_nn/hetero_nn.py` & `alphamed-federated-0.4.5/src/alphafed/hetero_nn/hetero_nn.py`

 * *Files 1% similar despite different names*

```diff
@@ -742,17 +742,18 @@
         uploads the final parameters and tells L1 task manager the task is complete.
         """
         self.push_log(f'Closing task {self.task_id} ...')
 
         self._switch_status(self._FINISHING)
         if is_succ:
             report_file_path, model_file_path = self._prepare_task_output()
-            self.contractor.upload_task_achivement(aggregator=self.id,
-                                                   report_file=report_file_path,
-                                                   model_file=model_file_path)
+            self.contractor.upload_metric_report(receivers=[self.id],
+                                                 report_file=report_file_path)
+            self.contractor.upload_model(receivers=[self.id],
+                                         model_file=model_file_path)
             self.contractor.finish_task(is_succ=True)
             self._wait_for_all_complete()
             self.contractor.notify_task_completion(result=True)
             self.push_log(f'Task {self.task_id} complete. Byebye!')
         else:
             self.contractor.finish_task(is_succ=False)
             self.push_log(f'Task {self.task_id} failed. Byebye!')
@@ -1164,16 +1165,17 @@
     def _close_task(self, is_succ: bool = True):
         """Close the task and upload the final parameters."""
         self.push_log(f'Closing task {self.task_id} ...')
 
         self._switch_status(self._FINISHING)
         if is_succ:
             model_file_path = self._prepare_task_output()
-            self.contractor.upload_task_achivement(aggregator=self.id,
-                                                   model_file=model_file_path)
+            self.contractor.upload_metric_report(receivers=[self.id])
+            self.contractor.upload_model(receivers=[self.id],
+                                         model_file=model_file_path)
             self.contractor.notify_collaborator_complete(peer_id=self.id, host=self.host)
             self.push_log(f'Task {self.task_id} complete. Byebye!')
         else:
             self.push_log(f'Task {self.task_id} failed. Byebye!')
 
     def _prepare_task_output(self) -> Tuple[str, str]:
         """Generate final output files of the task.
```

### Comparing `alphamed-federated-0.4.4/src/alphafed/hetero_nn/psi/psi.py` & `alphamed-federated-0.4.5/src/alphafed/hetero_nn/psi/psi.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/hetero_nn/psi/rsa_intersecter.py` & `alphamed-federated-0.4.5/src/alphafed/hetero_nn/psi/rsa_intersecter.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/hetero_nn/psi/rsa_psi_contractor.py` & `alphamed-federated-0.4.5/src/alphafed/hetero_nn/psi/rsa_psi_contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/hetero_nn/secure_contractor.py` & `alphamed-federated-0.4.5/src/alphafed/hetero_nn/secure_contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/hetero_nn/secure_hetero_nn.py` & `alphamed-federated-0.4.5/src/alphafed/hetero_nn/secure_hetero_nn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1101,17 +1101,18 @@
         self.push_log(f'Closing task {self.task_id} ...')
 
         logger.info(f'"ValueError: result ciphertext is transparent" present for {self.transparent_err_count} times.')
 
         self._switch_status(self._FINISHING)
         if is_succ:
             report_file_path, model_file_path = self._prepare_task_output()
-            self.contractor.upload_task_achivement(aggregator=self.id,
-                                                   report_file=report_file_path,
-                                                   model_file=model_file_path)
+            self.contractor.upload_metric_report(receivers=[self.id],
+                                                 report_file=report_file_path)
+            self.contractor.upload_model(receivers=[self.id],
+                                         model_file=model_file_path)
             self.contractor.finish_task(is_succ=True)
             self._wait_for_all_complete()
             self.contractor.notify_task_completion(result=True)
             self.push_log(f'Task {self.task_id} complete. Byebye!')
         else:
             self.contractor.finish_task(is_succ=False)
             self.push_log(f'Task {self.task_id} failed. Byebye!')
@@ -1639,16 +1640,17 @@
     def _close_task(self, is_succ: bool = True):
         """Close the task and upload the final parameters."""
         self.push_log(f'Closing task {self.task_id} ...')
 
         self._switch_status(self._FINISHING)
         if is_succ:
             model_file_path = self._prepare_task_output()
-            self.contractor.upload_task_achivement(aggregator=self.id,
-                                                   model_file=model_file_path)
+            self.contractor.upload_metric_report(receivers=[self.id])
+            self.contractor.upload_model(receivers=[self.id],
+                                         model_file=model_file_path)
             self.contractor.notify_collaborator_complete(peer_id=self.id, host=self.host)
             self.push_log(f'Task {self.task_id} complete. Byebye!')
         else:
             self.push_log(f'Task {self.task_id} failed. Byebye!')
 
     def _prepare_task_output(self) -> Tuple[str, str]:
         """Generate final output files of the task.
```

### Comparing `alphamed-federated-0.4.4/src/alphafed/loggers.py` & `alphamed-federated-0.4.5/src/alphafed/loggers.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/mock.py` & `alphamed-federated-0.4.5/src/alphafed/mock.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/perf_bench.py` & `alphamed-federated-0.4.5/src/alphafed/perf_bench.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/scheduler.py` & `alphamed-federated-0.4.5/src/alphafed/scheduler.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/secure/aes.py` & `alphamed-federated-0.4.5/src/alphafed/secure/aes.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/secure/ecdhe.py` & `alphamed-federated-0.4.5/src/alphafed/secure/ecdhe.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/secure/shamir.py` & `alphamed-federated-0.4.5/src/alphafed/secure/shamir.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/secure/tools.py` & `alphamed-federated-0.4.5/src/alphafed/secure/tools.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphafed/utils.py` & `alphamed-federated-0.4.5/src/alphafed/utils.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.4/src/alphamed_federated.egg-info/PKG-INFO` & `alphamed-federated-0.4.5/src/alphamed_federated.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,257 +1,257 @@
-Metadata-Version: 2.1
-Name: alphamed-federated
-Version: 0.4.4
-Summary: AlphaMed Federated Learning Module
-Author-email: Huang Yi Chun <huangyichun@jinghang.ai>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright [yyyy] [name of copyright owner]
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Project-URL: Homepage, https://github.com/ssplabs/alphafed
-Project-URL: Bug Tracker, https://github.com/ssplabs/alphafed/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# AlphaMed
-
-AlphaMed 是一个基于区块链技术的去中心化联邦学习解决方案，旨在使医疗机构能够在保证其医疗数据隐私和安全的同时，实现多机构联合建模。医疗机构可以在本地节点实现模型的训练，并支持以匿名的身份将加密的参数共享至聚合节点，从而实现更安全、可信的联邦学习。
-
-相比于传统的联邦学习，AlphaMed 平台不仅能够确保只有合法的且经过许可的参与者才能加入网络，同时支持节点的匿名化的参与联合建模。同时，区块链的共识算法能够确保网络中的节点得到一直的决策，恶意的参与者或者数据投毒等攻击将被拒绝，从而保证了联邦学习更好的安全性。
-
-在联邦学习的过程中，各个参与方都受到智能合约的约束，并且所有的事件、操作都将被记录在区块链的分布式账本上，可追溯、可审计，使得联合机器学习的安全性和隐私保护能力极大的提升。
-
-[开始构建第一个联邦学习任务](src/alphafed/docs/fed_avg/README.md)
-
-[在不同结构的数据源之间构建异构联邦学习任务](src/alphafed/docs/hetero_nn/README.md)
-
-如果 AlphaMed 平台预置的现有算法依然无法满足业务需要，还可以自行设计联邦学习算法，并使其运行在 AlphaMed 平台之上。[这里](src/alphafed/docs/customized_scheduler/README.md)展示了如果自定义联邦学习算法，并通过 AlphaMed 平台实际执行联邦学习任务。为了帮助开发者调试自己的代码，AlphaMed 平台还提供了一套[模拟运行环境](src/alphafed/docs/mock/README.md)，以在本地节点模拟实际运行环境，包括联邦学习运行环境。
-
-AlphaMed 平台除面向算法工程师提供了开发联邦学习模型的支持外，还面向模型使用者提供了预训练模型的支持。与传统预训练模型相比，AlphaMed 平台上的预训练模型支持功能更为强大、使用更为方便。在 AlphaMed 平台上，不仅可以寻找并下载心仪的预训练模型，更可以利用私有数据微调、部署预训练模型，使其更加适配于私有的业务数据。
-
-AlphaMed 平台预置了一定数量的预训练模型，同时也支持第三方开发者开发上传自己的预训练模型。[这里展示了如何设计自己的预训练模型。](src/alphafed/docs/auto_ml/README.md)
-
-## 项目目录说明
-
-src/alphafed  
-├── auto_ml  *AutoML 模块*  
-│   └── cvat  *CVAT 工具*  
-├── contractor  *合约消息工具*  
-├── data_channel  *数据传输工具*  
-├── docs  *说明文档*  
-│   ├── auto_ml  *AutoML 说明文档*  
-│   ├── customized_scheduler  *自定义调度器说明文档*  
-│   ├── fed_avg  *FedAvg 横向联邦说明文档*  
-│   ├── hetero_nn  *HeteroNN 异构联邦说明文档*  
-│   ├── mock  *模拟调试说明文档*  
-│   └── tutorial  *tutorial 示例说明文档，包含所有主要功能*  
-├── examples  *脚本测试代码 / 示例代码*  
-├── fed_avg  *FedAvg 横向联邦模块*  
-├── hetero_nn  *HeteroNN 异构联邦模块*  
-│   └── psi  *隐私求交模块*  
-├── secure  *安全工具*  
-├── fs.py  *文件系统工具*  
-├── loggers.py  *日志工具*  
-├── mock.py  *模拟调试工具*  
-└── utils.py  *其它工具*
+Metadata-Version: 2.1
+Name: alphamed-federated
+Version: 0.4.5
+Summary: AlphaMed Federated Learning Module
+Author-email: Huang Yi Chun <huangyichun@jinghang.ai>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Project-URL: Homepage, https://github.com/ssplabs/alphafed
+Project-URL: Bug Tracker, https://github.com/ssplabs/alphafed/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AlphaMed
+
+AlphaMed 是一个基于区块链技术的去中心化联邦学习解决方案，旨在使医疗机构能够在保证其医疗数据隐私和安全的同时，实现多机构联合建模。医疗机构可以在本地节点实现模型的训练，并支持以匿名的身份将加密的参数共享至聚合节点，从而实现更安全、可信的联邦学习。
+
+相比于传统的联邦学习，AlphaMed 平台不仅能够确保只有合法的且经过许可的参与者才能加入网络，同时支持节点的匿名化的参与联合建模。同时，区块链的共识算法能够确保网络中的节点得到一直的决策，恶意的参与者或者数据投毒等攻击将被拒绝，从而保证了联邦学习更好的安全性。
+
+在联邦学习的过程中，各个参与方都受到智能合约的约束，并且所有的事件、操作都将被记录在区块链的分布式账本上，可追溯、可审计，使得联合机器学习的安全性和隐私保护能力极大的提升。
+
+[开始构建第一个联邦学习任务](src/alphafed/docs/fed_avg/README.md)
+
+[在不同结构的数据源之间构建异构联邦学习任务](src/alphafed/docs/hetero_nn/README.md)
+
+如果 AlphaMed 平台预置的现有算法依然无法满足业务需要，还可以自行设计联邦学习算法，并使其运行在 AlphaMed 平台之上。[这里](src/alphafed/docs/customized_scheduler/README.md)展示了如果自定义联邦学习算法，并通过 AlphaMed 平台实际执行联邦学习任务。为了帮助开发者调试自己的代码，AlphaMed 平台还提供了一套[模拟运行环境](src/alphafed/docs/mock/README.md)，以在本地节点模拟实际运行环境，包括联邦学习运行环境。
+
+AlphaMed 平台除面向算法工程师提供了开发联邦学习模型的支持外，还面向模型使用者提供了预训练模型的支持。与传统预训练模型相比，AlphaMed 平台上的预训练模型支持功能更为强大、使用更为方便。在 AlphaMed 平台上，不仅可以寻找并下载心仪的预训练模型，更可以利用私有数据微调、部署预训练模型，使其更加适配于私有的业务数据。
+
+AlphaMed 平台预置了一定数量的预训练模型，同时也支持第三方开发者开发上传自己的预训练模型。[这里展示了如何设计自己的预训练模型。](src/alphafed/docs/auto_ml/README.md)
+
+## 项目目录说明
+
+src/alphafed  
+├── auto_ml  *AutoML 模块*  
+│   └── cvat  *CVAT 工具*  
+├── contractor  *合约消息工具*  
+├── data_channel  *数据传输工具*  
+├── docs  *说明文档*  
+│   ├── auto_ml  *AutoML 说明文档*  
+│   ├── customized_scheduler  *自定义调度器说明文档*  
+│   ├── fed_avg  *FedAvg 横向联邦说明文档*  
+│   ├── hetero_nn  *HeteroNN 异构联邦说明文档*  
+│   ├── mock  *模拟调试说明文档*  
+│   └── tutorial  *tutorial 示例说明文档，包含所有主要功能*  
+├── examples  *脚本测试代码 / 示例代码*  
+├── fed_avg  *FedAvg 横向联邦模块*  
+├── hetero_nn  *HeteroNN 异构联邦模块*  
+│   └── psi  *隐私求交模块*  
+├── secure  *安全工具*  
+├── fs.py  *文件系统工具*  
+├── loggers.py  *日志工具*  
+├── mock.py  *模拟调试工具*  
+└── utils.py  *其它工具*
```

### Comparing `alphamed-federated-0.4.4/src/alphamed_federated.egg-info/SOURCES.txt` & `alphamed-federated-0.4.5/src/alphamed_federated.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 src/alphafed/data_channel/grpc_data_channel.py
 src/alphafed/data_channel/shared_file_data_channel.py
 src/alphafed/docs/auto_ml/res/auto.py
 src/alphafed/docs/auto_ml/res/res_net.py
 src/alphafed/docs/customized_scheduler/contractor.py
 src/alphafed/docs/customized_scheduler/scheduler.py
 src/alphafed/docs/customized_scheduler/simple_task.py
+src/alphafed/docs/fed_avg/net.py
 src/alphafed/docs/mock/net.py
 src/alphafed/docs/mock/scheduler.py
 src/alphafed/docs/tutorial/res/cnn_net.py
 src/alphafed/docs/tutorial/res/auto_model_fed_avg/auto_fed_avg.py
 src/alphafed/docs/tutorial/res/auto_model_fed_avg/res_net.py
 src/alphafed/docs/tutorial/res/auto_model_local/auto.py
 src/alphafed/docs/tutorial/res/auto_model_local/res_net.py
@@ -88,14 +89,46 @@
 src/alphafed/examples/fed_avg/demo_FedIRM.py
 src/alphafed/examples/fed_avg/demos.py
 src/alphafed/examples/fed_avg/run_aggregator.py
 src/alphafed/examples/fed_avg/run_data_owner_2.py
 src/alphafed/examples/fed_avg/run_data_owner_3.py
 src/alphafed/examples/fed_avg/run_data_owner_4.py
 src/alphafed/examples/fed_avg/run_data_owner_5.py
+src/alphafed/examples/fed_avg/model/my_scheduler.py
+src/alphafed/examples/fed_avg/model/net.py
+src/alphafed/examples/fed_md/__init__.py
+src/alphafed/examples/fed_md/clean_history_msg.py
+src/alphafed/examples/fed_md/demos.py
+src/alphafed/examples/fed_md/run_aggregator.py
+src/alphafed/examples/fed_md/run_data_owner_2.py
+src/alphafed/examples/fed_md/run_data_owner_4.py
+src/alphafed/examples/fed_md/model/contractor.py
+src/alphafed/examples/fed_md/model/loss.py
+src/alphafed/examples/fed_md/model/my_homo_fed_md_impl.py
+src/alphafed/examples/fed_md/model/net.py
+src/alphafed/examples/fed_md/model/scheduler.py
+src/alphafed/examples/fed_per/__init__.py
+src/alphafed/examples/fed_per/clean_history_msg.py
+src/alphafed/examples/fed_per/demos.py
+src/alphafed/examples/fed_per/run_aggregator.py
+src/alphafed/examples/fed_per/run_data_owner_2.py
+src/alphafed/examples/fed_per/run_data_owner_4.py
+src/alphafed/examples/fed_per/model/contractor.py
+src/alphafed/examples/fed_per/model/my_homo_fed_per_impl.py
+src/alphafed/examples/fed_per/model/net.py
+src/alphafed/examples/fed_per/model/scheduler.py
+src/alphafed/examples/fed_prox/__init__.py
+src/alphafed/examples/fed_prox/clean_history_msg.py
+src/alphafed/examples/fed_prox/demos.py
+src/alphafed/examples/fed_prox/run_aggregator.py
+src/alphafed/examples/fed_prox/run_data_owner_2.py
+src/alphafed/examples/fed_prox/run_data_owner_4.py
+src/alphafed/examples/fed_prox/model/my_fed_prox_impl.py
+src/alphafed/examples/fed_prox/model/net.py
+src/alphafed/examples/fed_prox/model/scheduler.py
 src/alphafed/examples/hetero_nn/__init__.py
 src/alphafed/examples/hetero_nn/clean_history_msg.py
 src/alphafed/examples/hetero_nn/demos.py
 src/alphafed/examples/hetero_nn/run_collaborater.py
 src/alphafed/examples/hetero_nn/run_host.py
 src/alphafed/examples/hetero_nn/psi/demos.py
 src/alphafed/examples/hetero_nn/psi/run_collaborator_2.py
```

