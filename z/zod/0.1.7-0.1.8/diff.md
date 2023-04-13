# Comparing `tmp/zod-0.1.7.tar.gz` & `tmp/zod-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zod-0.1.7.tar", max compression
+gzip compressed data, was "zod-0.1.8.tar", max compression
```

## Comparing `zod-0.1.7.tar` & `zod-0.1.8.tar`

### file list

```diff
@@ -1,61 +1,65 @@
--rw-r--r--   0        0        0     1073 2023-03-27 08:17:47.222173 zod-0.1.7/LICENSE
--rw-r--r--   0        0        0     4474 2023-03-27 08:17:47.222173 zod-0.1.7/README.md
--rw-r--r--   0        0        0     1683 2023-03-27 08:17:47.226173 zod-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      864 2023-03-27 08:17:47.226173 zod-0.1.7/zod/__init__.py
--rw-r--r--   0        0        0     4945 2023-03-27 08:17:47.226173 zod-0.1.7/zod/anno/lane.py
--rw-r--r--   0        0        0     4354 2023-03-27 08:17:47.226173 zod-0.1.7/zod/anno/object.py
--rw-r--r--   0        0        0     2446 2023-03-27 08:17:47.226173 zod-0.1.7/zod/anno/parser.py
--rw-r--r--   0        0        0      349 2023-03-27 08:17:47.226173 zod-0.1.7/zod/anno/road_condition.py
--rw-r--r--   0        0        0    20435 2023-03-27 08:17:47.226173 zod-0.1.7/zod/anno/tsr/class_map.py
--rw-r--r--   0        0        0     1191 2023-03-27 08:17:47.226173 zod-0.1.7/zod/anno/tsr/traffic_sign.py
--rw-r--r--   0        0        0    12632 2023-03-27 08:17:47.226173 zod-0.1.7/zod/cli/download_zod.py
--rw-r--r--   0        0        0     6647 2023-03-27 08:17:47.226173 zod-0.1.7/zod/cli/extract_tsr_patches.py
--rw-r--r--   0        0        0     6049 2023-03-27 08:17:47.226173 zod-0.1.7/zod/cli/generate_coco_json.py
--rw-r--r--   0        0        0     1733 2023-03-27 08:17:47.226173 zod-0.1.7/zod/cli/main.py
--rw-r--r--   0        0        0     3682 2023-03-27 08:17:47.226173 zod-0.1.7/zod/cli/visualize_lidar.py
--rw-r--r--   0        0        0     1768 2023-03-27 08:17:47.226173 zod-0.1.7/zod/constants.py
--rw-r--r--   0        0        0      184 2023-03-27 08:17:47.226173 zod-0.1.7/zod/data_classes/__init__.py
--rw-r--r--   0        0        0      400 2023-03-27 08:17:47.226173 zod-0.1.7/zod/data_classes/_serializable.py
--rw-r--r--   0        0        0    10364 2023-03-27 08:17:47.226173 zod-0.1.7/zod/data_classes/box.py
--rw-r--r--   0        0        0     3021 2023-03-27 08:17:47.226173 zod-0.1.7/zod/data_classes/calibration.py
--rw-r--r--   0        0        0     5057 2023-03-27 08:17:47.226173 zod-0.1.7/zod/data_classes/frame.py
--rw-r--r--   0        0        0     1271 2023-03-27 08:17:47.226173 zod-0.1.7/zod/data_classes/geometry.py
--rw-r--r--   0        0        0     5516 2023-03-27 08:17:47.226173 zod-0.1.7/zod/data_classes/info.py
--rw-r--r--   0        0        0      894 2023-03-27 08:17:47.226173 zod-0.1.7/zod/data_classes/metadata.py
--rw-r--r--   0        0        0     7226 2023-03-27 08:17:47.226173 zod-0.1.7/zod/data_classes/oxts.py
--rw-r--r--   0        0        0     5562 2023-03-27 08:17:47.226173 zod-0.1.7/zod/data_classes/sensor.py
--rw-r--r--   0        0        0     2892 2023-03-27 08:17:47.226173 zod-0.1.7/zod/data_classes/sequence.py
--rw-r--r--   0        0        0       65 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/README.md
--rw-r--r--   0        0        0      299 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/detection/__init__.py
--rw-r--r--   0        0        0     4427 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/detection/_experimental/eval.py
--rw-r--r--   0        0        0    12061 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/detection/_experimental/matching.py
--rw-r--r--   0        0        0     4614 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/detection/_experimental/utils.py
--rw-r--r--   0        0        0      548 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/detection/_nuscenes_eval/LICENCE.txt
--rw-r--r--   0        0        0      661 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/detection/_nuscenes_eval/changes.txt
--rw-r--r--   0        0        0     4576 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/detection/_nuscenes_eval/common/data_classes.py
--rw-r--r--   0        0        0     4046 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/detection/_nuscenes_eval/common/utils.py
--rw-r--r--   0        0        0    21852 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/detection/_nuscenes_eval/detection/README.md
--rw-r--r--   0        0        0     7651 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/detection/_nuscenes_eval/detection/algo.py
--rw-r--r--   0        0        0     1016 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/detection/_nuscenes_eval/detection/constants.py
--rw-r--r--   0        0        0    15069 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
--rw-r--r--   0        0        0      123 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/detection/constants.py
--rw-r--r--   0        0        0     8031 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/detection/eval_nuscenes_style.py
--rw-r--r--   0        0        0       67 2023-03-27 08:17:47.226173 zod-0.1.7/zod/eval/tsr.py
--rw-r--r--   0        0        0     1990 2023-03-27 08:17:47.226173 zod-0.1.7/zod/utils/compensation.py
--rw-r--r--   0        0        0     4443 2023-03-27 08:17:47.226173 zod-0.1.7/zod/utils/geometry.py
--rw-r--r--   0        0        0      978 2023-03-27 08:17:47.226173 zod-0.1.7/zod/utils/polygon_transformations.py
--rw-r--r--   0        0        0      914 2023-03-27 08:17:47.226173 zod-0.1.7/zod/utils/utils.py
--rw-r--r--   0        0        0     2703 2023-03-27 08:17:47.226173 zod-0.1.7/zod/utils/visualization.py
--rw-r--r--   0        0        0     5481 2023-03-27 08:17:47.230173 zod-0.1.7/zod/visualization/bev_utils.py
--rw-r--r--   0        0        0     2941 2023-03-27 08:17:47.230173 zod-0.1.7/zod/visualization/colorlabeler.py
--rw-r--r--   0        0        0      259 2023-03-27 08:17:47.230173 zod-0.1.7/zod/visualization/ego_road_visualization.py
--rw-r--r--   0        0        0      264 2023-03-27 08:17:47.230173 zod-0.1.7/zod/visualization/lane_markings_visualization.py
--rw-r--r--   0        0        0     6028 2023-03-27 08:17:47.230173 zod-0.1.7/zod/visualization/lidar_bev.py
--rw-r--r--   0        0        0     4410 2023-03-27 08:17:47.230173 zod-0.1.7/zod/visualization/lidar_on_image.py
--rw-r--r--   0        0        0     4599 2023-03-27 08:17:47.230173 zod-0.1.7/zod/visualization/object_visualization.py
--rw-r--r--   0        0        0     1763 2023-03-27 08:17:47.230173 zod-0.1.7/zod/visualization/oxts_on_image.py
--rw-r--r--   0        0        0     3253 2023-03-27 08:17:47.230173 zod-0.1.7/zod/visualization/oxts_visualization.py
--rw-r--r--   0        0        0      762 2023-03-27 08:17:47.230173 zod-0.1.7/zod/visualization/polygon_utils.py
--rw-r--r--   0        0        0     3429 2023-03-27 08:17:47.230173 zod-0.1.7/zod/zod_frames.py
--rw-r--r--   0        0        0     3402 2023-03-27 08:17:47.230173 zod-0.1.7/zod/zod_sequences.py
--rw-r--r--   0        0        0     5962 1970-01-01 00:00:00.000000 zod-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-13 12:11:08.669985 zod-0.1.8/LICENSE
+-rw-r--r--   0        0        0     4501 2023-04-13 12:11:08.669985 zod-0.1.8/README.md
+-rw-r--r--   0        0        0     1683 2023-04-13 12:11:08.669985 zod-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      982 2023-04-13 12:11:08.673985 zod-0.1.8/zod/__init__.py
+-rw-r--r--   0        0        0     3380 2023-04-13 12:11:08.673985 zod-0.1.8/zod/_zod_dataset.py
+-rw-r--r--   0        0        0     4945 2023-04-13 12:11:08.673985 zod-0.1.8/zod/anno/lane.py
+-rw-r--r--   0        0        0     4354 2023-04-13 12:11:08.673985 zod-0.1.8/zod/anno/object.py
+-rw-r--r--   0        0        0     2446 2023-04-13 12:11:08.673985 zod-0.1.8/zod/anno/parser.py
+-rw-r--r--   0        0        0      349 2023-04-13 12:11:08.673985 zod-0.1.8/zod/anno/road_condition.py
+-rw-r--r--   0        0        0    20456 2023-04-13 12:11:08.673985 zod-0.1.8/zod/anno/tsr/class_map.py
+-rw-r--r--   0        0        0     1686 2023-04-13 12:11:08.673985 zod-0.1.8/zod/anno/tsr/traffic_sign.py
+-rw-r--r--   0        0        0    14001 2023-04-13 12:11:08.673985 zod-0.1.8/zod/cli/download_zod.py
+-rw-r--r--   0        0        0     6619 2023-04-13 12:11:08.673985 zod-0.1.8/zod/cli/extract_tsr_patches.py
+-rw-r--r--   0        0        0     6049 2023-04-13 12:11:08.673985 zod-0.1.8/zod/cli/generate_coco_json.py
+-rw-r--r--   0        0        0     1733 2023-04-13 12:11:08.673985 zod-0.1.8/zod/cli/main.py
+-rw-r--r--   0        0        0      655 2023-04-13 12:11:08.673985 zod-0.1.8/zod/cli/utils.py
+-rw-r--r--   0        0        0     3682 2023-04-13 12:11:08.673985 zod-0.1.8/zod/cli/visualize_lidar.py
+-rw-r--r--   0        0        0     2146 2023-04-13 12:11:08.673985 zod-0.1.8/zod/constants.py
+-rw-r--r--   0        0        0      184 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/__init__.py
+-rw-r--r--   0        0        0      400 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/_serializable.py
+-rw-r--r--   0        0        0    10575 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/box.py
+-rw-r--r--   0        0        0     3021 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/calibration.py
+-rw-r--r--   0        0        0     7226 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/ego_motion.py
+-rw-r--r--   0        0        0     5063 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/frame.py
+-rw-r--r--   0        0        0     1271 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/geometry.py
+-rw-r--r--   0        0        0     5516 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/info.py
+-rw-r--r--   0        0        0      894 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/metadata.py
+-rw-r--r--   0        0        0      317 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/oxts.py
+-rw-r--r--   0        0        0     5562 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/sensor.py
+-rw-r--r--   0        0        0     3610 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/sequence.py
+-rw-r--r--   0        0        0       65 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/README.md
+-rw-r--r--   0        0        0      299 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/__init__.py
+-rw-r--r--   0        0        0     4427 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_experimental/eval.py
+-rw-r--r--   0        0        0    12061 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_experimental/matching.py
+-rw-r--r--   0        0        0     4614 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_experimental/utils.py
+-rw-r--r--   0        0        0      548 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/LICENCE.txt
+-rw-r--r--   0        0        0      661 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/changes.txt
+-rw-r--r--   0        0        0     4576 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/common/data_classes.py
+-rw-r--r--   0        0        0     4046 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/common/utils.py
+-rw-r--r--   0        0        0    21852 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/README.md
+-rw-r--r--   0        0        0     7651 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/algo.py
+-rw-r--r--   0        0        0     1016 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/constants.py
+-rw-r--r--   0        0        0    15069 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
+-rw-r--r--   0        0        0      123 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/constants.py
+-rw-r--r--   0        0        0     8031 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/eval_nuscenes_style.py
+-rw-r--r--   0        0        0       67 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/tsr.py
+-rw-r--r--   0        0        0     1996 2023-04-13 12:11:08.677985 zod-0.1.8/zod/utils/compensation.py
+-rw-r--r--   0        0        0     4443 2023-04-13 12:11:08.677985 zod-0.1.8/zod/utils/geometry.py
+-rw-r--r--   0        0        0      978 2023-04-13 12:11:08.677985 zod-0.1.8/zod/utils/polygon_transformations.py
+-rw-r--r--   0        0        0      914 2023-04-13 12:11:08.677985 zod-0.1.8/zod/utils/utils.py
+-rw-r--r--   0        0        0     2703 2023-04-13 12:11:08.677985 zod-0.1.8/zod/utils/visualization.py
+-rw-r--r--   0        0        0     5481 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/bev_utils.py
+-rw-r--r--   0        0        0     2941 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/colorlabeler.py
+-rw-r--r--   0        0        0      259 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/ego_road_visualization.py
+-rw-r--r--   0        0        0      264 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/lane_markings_visualization.py
+-rw-r--r--   0        0        0     6028 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/lidar_bev.py
+-rw-r--r--   0        0        0     4410 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/lidar_on_image.py
+-rw-r--r--   0        0        0     4639 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/object_visualization.py
+-rw-r--r--   0        0        0     1769 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/oxts_on_image.py
+-rw-r--r--   0        0        0     3259 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/oxts_visualization.py
+-rw-r--r--   0        0        0      762 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/polygon_utils.py
+-rw-r--r--   0        0        0      685 2023-04-13 12:11:08.677985 zod-0.1.8/zod/zod_drives.py
+-rw-r--r--   0        0        0      577 2023-04-13 12:11:08.677985 zod-0.1.8/zod/zod_frames.py
+-rw-r--r--   0        0        0      576 2023-04-13 12:11:08.677985 zod-0.1.8/zod/zod_sequences.py
+-rw-r--r--   0        0        0     5989 1970-01-01 00:00:00.000000 zod-0.1.8/PKG-INFO
```

### Comparing `zod-0.1.7/LICENSE` & `zod-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/README.md` & `zod-0.1.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -24,35 +24,35 @@
 To install the full devkit, with the CLI and all dependencies, run:
 ```bash
 pip install "zod[all]"
 ```
 
 ## Download using the CLI
 
-This is an example of how to download the ZOD Frames mini-dataset using the CLI. Prerequisites are that you have applied for access and received a download link. To download the mini-dataset, run:
+This is an example of how to download the ZOD Frames mini-dataset using the CLI. Prerequisites are that you have applied for access and received a download link.
+The simplest way to download the dataset is to use the CLI interactively:
 ```bash
-zod download --url "<download-link>" --output-dir <path/to/outputdir> frames --mini
+zod download
 ```
-similarly, to download the full dataset (including all lidar scans before and after the keyframe), run:
+This will prompt you for the required information, present you with a summary of the download, and then ask for confirmation. You can of course also specify all the required information directly on the command line, and avoid the confirmation using `--no-confirm` or `-y`. For example:
 ```bash
-zod download --url "<download-link>" --output-dir <path/to/outputdir> frames --lidar --num-scans-before -1 --num-scans-after -1 --oxts --images --blur --dnat --calibrations --annotations
+zod download -y --url="<download-link>" --output-dir=<path/to/outputdir> --subset=frames --version=mini
 ```
-this will download all the previous and future lidar scans (as `num-scans-before=-1` and `num-scans-after=-1`), the OxTS data, the images (with both the blur and DNAT anonymization), the calibration files, the annotations, and all other necessary files. If you dont want any previous or future lidar scans, run:
+By default, all data streams are downloaded for ZodSequences and ZodDrives. For ZodFrames, DNAT versions of the images, and surrounding (non-keyframe) lidar scans are excluded. To download them as well, run:
 ```bash
-zod download --url "<download-link>" --output-dir <path/to/outputdir> frames --lidar --num-scans-before 0 --num-scans-after 0 --oxts --images --blur --dnat --calibrations --annotations
+zod download -y --url="<download-link>" --output-dir=<path/to/outputdir> --subset=frames --version=full --num-scans-before=-1 --num-scans-after=-1 --dnat
 ```
-
-For a full list of options for ZOD download, run:
+If you want to exclude some of the data streams, you can do so by specifying the `--no-<stream>` flag. For example, to download only the DNAT images, infos, and annotations, run:
+```bash
+zod download --dnat --no-blur --no-lidar --no-oxts --no-vehicle-data
+```
+Finally, for a full list of options you can of course run:
 ```bash
 zod download --help
-zod download --url="<url>" --output-dir=<dir> frames --help
-zod download --url="<url>" --output-dir=<dir> sequences --help
 ```
-depending on which dataset you want to download.
-
 
 ## Anonymization
 To preserve privacy, the dataset is anonymized. The anonymization is performed by [brighterAI](https://brighter.ai/), and we provide two separate modes of anonymization: deep fakes (DNAT) and blur. In our paper, we show that the performance of an object detector is not affected by the anonymization method. For more details regarding this experiment, please refer to our [coming soon]().
 
 ## Citation
 If you publish work that uses Zenseact Open Dataset, please cite: [coming soon]()
```

### Comparing `zod-0.1.7/pyproject.toml` & `zod-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zod"
-version = "0.1.7"
+version = "0.1.8"
 description = "Zenseact Open Dataset"
 authors = ["Zenseact <opendataset@zenseact.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zod.zenseact.com"
 repository = "https://github.com/zenseact/zod"
```

### Comparing `zod-0.1.7/zod/__init__.py` & `zod-0.1.8/zod/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Top-level package for Zenseact Open Dataset (ZOD)."""
 
+from ._zod_dataset import ZodDataset as ZodDataset  # For type hinting
 from .constants import AnnotationProject as AnnotationProject
 from .constants import Anonymization as Anonymization
 from .constants import Camera as Camera
 from .constants import Lidar as Lidar
 from .data_classes.frame import ZodFrame as ZodFrame
 from .data_classes.sequence import ZodSequence as ZodSequence
+from .zod_drives import ZodDrives as ZodDrives
 from .zod_frames import ZodFrames as ZodFrames
 from .zod_sequences import ZodSequences as ZodSequences
 
 try:
     # importlib.metadata is present in Python 3.8 and later
     import importlib.metadata as importlib_metadata
 except ImportError:
```

### Comparing `zod-0.1.7/zod/anno/lane.py` & `zod-0.1.8/zod/anno/lane.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/anno/object.py` & `zod-0.1.8/zod/anno/object.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/anno/parser.py` & `zod-0.1.8/zod/anno/parser.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/anno/tsr/class_map.py` & `zod-0.1.8/zod/anno/tsr/class_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Class map for the traffic sign classification dataset."""
 
 CLASS_NAME_TO_CLASS_IDX = {
+    "Unclear": None,
     "NotListed": 0,
     "Indication_CameraSurveillance": 1,
     "Mandatory_PassOnEitherSide": 2,
     "Mandatory_PassOnThisSideLeft": 3,
     "Mandatory_PassOnThisSideRight": 4,
     "Mandatory_ProceedStraight": 5,
     "Mandatory_ProceedStraightOrTurnRight": 6,
```

### Comparing `zod-0.1.7/zod/cli/download_zod.py` & `zod-0.1.8/zod/cli/download_zod.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 import os
 import os.path as osp
 import subprocess
 import tarfile
 import threading
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
+from enum import Enum
 
 from tqdm import tqdm
 
+from zod.cli.utils import SubDataset
+
 try:
     import click.exceptions
     import dropbox
     import dropbox.exceptions
     import dropbox.files
     import dropbox.sharing
     import typer
@@ -26,14 +29,19 @@
 REFRESH_TOKEN = "z2h_5rjphJEAAAAAAAAAAUWtQlltCYlMbZ2WqMgtymELhiSuKIksxAYeArubKnZV"
 CHUNK_SIZE = 1024 * 1024  # 1 MB
 TIMEOUT = 60 * 60  # 1 hour
 
 app = typer.Typer(help="Zenseact Open Dataset Donwloader", no_args_is_help=True)
 
 
+class Version(str, Enum):
+    FULL = "full"
+    MINI = "mini"
+
+
 @dataclass
 class DownloadExtractInfo:
     """Information about a file to extract."""
 
     url: str
     file_path: str
     extract_dir: str
@@ -44,37 +52,44 @@
     extract: bool
 
 
 @dataclass
 class FilterSettings:
     """Filter settings."""
 
-    mini: bool
+    version: Version
     annotations: bool
     images: bool
     blur: bool
     dnat: bool
     lidar: bool
     oxts: bool
-    calibrations: bool
+    infos: bool
+    vehicle_data: bool
     num_scans_before: int
     num_scans_after: int
 
+    def __str__(self):
+        return "\n".join([f"    {key}: {value}" for key, value in self.__dict__.items()])
+
 
 @dataclass
 class DownloadSettings:
     """Download settings."""
 
     url: str
     output_dir: str
     rm: bool
     dry_run: bool
     extract: bool
     parallel: bool
 
+    def __str__(self):
+        return "\n".join([f"    {key}: {value}" for key, value in self.__dict__.items()])
+
 
 class ResumableDropbox(dropbox.Dropbox):
     """A patched dropbox client that allows to resume downloads."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._headers = {} if self._headers is None else self._headers
@@ -192,33 +207,31 @@
 
     if info.rm and not info.dry_run:
         os.remove(download_path)
 
 
 def _filter_entry(entry: dropbox.files.Metadata, settings: FilterSettings) -> bool:
     """Filter the entry based on the flags."""
-    if settings.mini and "mini" not in entry.name:
-        # If mini is set, we only want to download the mini dataset
-        return False
-    # If we are downloading the full dataset, we don't want the mini dataset
-    if not settings.mini and "mini" in entry.name:
+    if settings.version == "mini":
+        return "mini" in entry.name
+    elif "mini" in entry.name:
         return False
 
     if not settings.annotations and "annotations" in entry.name:
         return False
     if "images" in entry.name:
         if not settings.images:
             return False
         if not settings.blur and "blur" in entry.name:
             return False
         if not settings.dnat and "dnat" in entry.name:
             return False
     if not settings.oxts and "oxts" in entry.name:
         return False
-    if not settings.calibrations and "calibrations" in entry.name:
+    if not settings.infos and "infos" in entry.name:
         return False
     if "lidar" in entry.name:
         if not settings.lidar:
             return False
         distance = entry.name.split("_")[2][:2]
         if "after" in entry.name and (int(distance) > settings.num_scans_after):
             return False
@@ -272,97 +285,126 @@
     entries = res.entries
     while res.has_more:
         res = dbx.files_list_folder_continue(res.cursor)
         entries.extend(res.entries)
     return url, entries
 
 
-@app.callback(no_args_is_help=True)
-def common(
-    ctx: typer.Context,
-    url: str = typer.Option(..., help="The dropbox shared folder url"),
-    output_dir: str = typer.Option(..., help="The output directory"),
-    rm: bool = typer.Option(False, help="Whether to remove the downloaded archives"),
-    dry_run: bool = typer.Option(
-        False, help="Whether to only print the files that would be downloaded"
-    ),
-    extract: bool = typer.Option(True, help="Whether to unpack the archives"),
-    parallel: bool = typer.Option(True, help="Whether to download files in parallel"),
-):
-    ctx.obj = DownloadSettings(
-        url=url,
-        output_dir=output_dir,
-        rm=rm,
-        dry_run=dry_run,
-        extract=extract,
-        parallel=parallel,
-    )
+def _print_summary(download_settings, filter_settings, subset):
+    print("\nDownload settings:")
+    print(download_settings)
+    print("\nFilter settings:")
+    if filter_settings.version == Version.MINI:
+        print("    version: mini\n    (other settings are ignored for mini)")
+    else:
+        print(filter_settings)
+    if subset == SubDataset.FRAMES and (
+        filter_settings.num_scans_before == filter_settings.num_scans_after == 0
+    ):
+        typer.secho(
+            "Note! The current settings will only download the core lidar frames. "
+            "If you need surrounding scans, set --num-scans-before and/or --num-scans-after.",
+            fg=typer.colors.YELLOW,
+        )
+    print("\n")
+
+
+REQ = "Required Arguments"
+GEN = "General Download Settings"
+FIL = "General Filter Settings"
+FRA = "Frames Filter Settings"
+SEQ = "Sequences/Drives Filter Settings"
 
 
 @app.command()
-def frames(
-    ctx: typer.Context,
-    mini: bool = typer.Option(False, help="Whether to download the mini dataset"),
-    annotations: bool = typer.Option(True, help="Whether to download the annotations"),
-    images: bool = typer.Option(True, help="Whether to download the images"),
-    blur: bool = typer.Option(True, help="Whether to download the blur images"),
-    dnat: bool = typer.Option(False, help="Whether to download the dnat images"),
-    lidar: bool = typer.Option(True, help="Whether to download the lidar data"),
+def download(
+    url: str = typer.Option(
+        ...,
+        help="The dropbox shared folder url",
+        prompt="What is the dropbox url to the dataset (you can get it from zod.zenseact.com)?",
+        prompt_required=False,
+        rich_help_panel=REQ,
+    ),
+    output_dir: str = typer.Option(
+        ...,
+        help="Output directory where dataset will be extracted",
+        prompt="Where do you want to extract the dataset (e.g. ~/data/zod)?",
+        prompt_required=False,
+        rich_help_panel=REQ,
+    ),
+    subset: SubDataset = typer.Option(
+        ...,
+        help="The sub-dataset to download",
+        prompt="Which sub-dataset do you want to download?",
+        prompt_required=False,
+        rich_help_panel=REQ,
+    ),
+    version: Version = typer.Option(
+        ...,
+        help="The version of the dataset to download",
+        prompt="Which version do you want to download?",
+        prompt_required=False,
+        rich_help_panel=REQ,
+    ),
+    # General download settings
+    rm: bool = typer.Option(False, help="Remove the downloaded archives", rich_help_panel=GEN),
+    dry_run: bool = typer.Option(False, help="Print what would be downloaded", rich_help_panel=GEN),
+    extract: bool = typer.Option(True, help="Unpack the archives", rich_help_panel=GEN),
+    parallel: bool = typer.Option(True, help="Download files in parallel", rich_help_panel=GEN),
+    no_confirm: bool = typer.Option(
+        False,
+        "-y",
+        "--no-confirm/--confirm",
+        help="Don't ask for confirmation",
+        is_flag=True,
+        flag_value=False,
+        rich_help_panel=GEN,
+    ),
+    # Filter settings
+    annotations: bool = typer.Option(True, help="Download annotations", rich_help_panel=FIL),
+    images: bool = typer.Option(True, help="Whether to download the images", rich_help_panel=FIL),
+    blur: bool = typer.Option(True, help="Download blur images", rich_help_panel=FIL),
+    lidar: bool = typer.Option(True, help="Download lidar data", rich_help_panel=FIL),
+    oxts: bool = typer.Option(True, help="Download oxts data", rich_help_panel=FIL),
+    infos: bool = typer.Option(True, help="Download infos", rich_help_panel=FIL),
+    vehicle_data: bool = typer.Option(True, help="Download the vehicle data", rich_help_panel=SEQ),
+    dnat: bool = typer.Option(False, help="Download DNAT images", rich_help_panel=FRA),
     num_scans_before: int = typer.Option(
-        0, help="Number of earlier lidar scans to download (-1 == all)"
+        0, help="Number of earlier lidar scans to download (-1 == all)", rich_help_panel=FRA
     ),
     num_scans_after: int = typer.Option(
-        0, help="Number of later lidar scans to download (-1 == all)"
+        0, help="Number of later lidar scans to download (-1 == all)", rich_help_panel=FRA
     ),
-    oxts: bool = typer.Option(True, help="Whether to download the oxts data"),
-    calibrations: bool = typer.Option(True, help="Whether to download the calibration data"),
 ):
     """Download the Zenseact Open Dataset."""
-
-    if images:
-        assert blur or dnat, "Must download at least one type of image"
-
-    dl_settings: DownloadSettings = ctx.obj
+    download_settings = DownloadSettings(
+        url=url,
+        output_dir=output_dir,
+        rm=rm,
+        dry_run=dry_run,
+        extract=extract,
+        parallel=parallel,
+    )
     filter_settings = FilterSettings(
-        mini=mini,
+        version=version,
         annotations=annotations,
         images=images,
         blur=blur,
         dnat=dnat,
         lidar=lidar,
         oxts=oxts,
-        calibrations=calibrations,
-        num_scans_before=num_scans_before,
-        num_scans_after=num_scans_after,
-    )
-    _download_dataset(dl_settings, filter_settings, "single_frames")
-
-
-@app.command()
-def sequences(
-    ctx: typer.Context,
-    mini: bool = typer.Option(False, help="Whether to download the mini dataset"),
-    annotations: bool = typer.Option(True, help="Whether to download the annotations"),
-    images: bool = typer.Option(True, help="Whether to download the images"),
-    lidar: bool = typer.Option(True, help="Whether to download the lidar data"),
-    oxts: bool = typer.Option(True, help="Whether to download the oxts data"),
-    calibrations: bool = typer.Option(True, help="Whether to download the calibration data"),
-):
-    """Download the Zenseact Open Dataset."""
-    dl_settings: DownloadSettings = ctx.obj
-    filter_settings = FilterSettings(
-        mini=mini,
-        annotations=annotations,
-        images=images,
-        blur=True,
-        dnat=False,
-        lidar=lidar,
-        oxts=oxts,
-        calibrations=calibrations,
-        num_scans_before=-1,
-        num_scans_after=-1,
+        infos=infos,
+        vehicle_data=vehicle_data,
+        num_scans_before=num_scans_before if subset == SubDataset.FRAMES else -1,
+        num_scans_after=num_scans_after if subset == SubDataset.FRAMES else -1,
     )
-    _download_dataset(dl_settings, filter_settings, "sequences")
+    if not no_confirm:
+        _print_summary(download_settings, filter_settings, subset)
+        typer.confirm(
+            f"Download with the above settings?",
+            abort=True,
+        )
+    _download_dataset(download_settings, filter_settings, subset.folder)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `zod-0.1.7/zod/cli/extract_tsr_patches.py` & `zod-0.1.8/zod/cli/extract_tsr_patches.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,22 +99,22 @@
 
     new_cropped_frames = []
     # load the image
     image_path = frame.info.get_key_camera_frame(constants.Anonymization.BLUR).filepath
     image = cv2.cvtColor(cv2.imread(image_path), cv2.COLOR_BGR2RGB)
     for traffic_sign in traffic_signs:
         cls_name = traffic_sign.traffic_sign_class
-        train_or_val = constants.TRAIN if frame.frame_id in train_ids else constants.VAL
+        train_or_val = constants.TRAIN if frame.info.id in train_ids else constants.VAL
         cls_folder = os.path.join(args.output_folder, train_or_val, cls_name)
 
         if not os.path.exists(cls_folder):
             os.makedirs(cls_folder)
             os.chmod(cls_folder, 0o775)
 
-        new_frame_id = f"{frame.frame_id}_{traffic_sign.uuid}"
+        new_frame_id = f"{frame.info.id}_{traffic_sign.uuid}"
         output_file = os.path.join(
             cls_folder,
             f"{new_frame_id}.png",
         )
         if not args.overwrite and os.path.exists(output_file):
             continue
 
@@ -166,15 +166,15 @@
         os.makedirs(args.output_folder)
         os.chmod(args.output_folder, 0o775)
     zod_frames = ZodFrames(args.dataset_root, version="full")
     print(f"Will process {len(zod_frames)} full frames.")
 
     traffic_sign_frames = process_map(
         _process_frame,
-        zod_frames.get_all_frames().values(),
+        zod_frames,
         repeat(args),
         desc="Processing frames in ZOD",
         max_workers=args.num_workers,
         chunksize=1 if args.num_workers == 1 else 100,
     )
 
     # flatten the returned list
```

### Comparing `zod-0.1.7/zod/cli/generate_coco_json.py` & `zod-0.1.8/zod/cli/generate_coco_json.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/cli/main.py` & `zod-0.1.8/zod/cli/main.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/cli/visualize_lidar.py` & `zod-0.1.8/zod/cli/visualize_lidar.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/constants.py` & `zod-0.1.8/zod/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,51 +16,63 @@
 DB_DATE_STRING_FORMAT_W_MICROSECONDS = "%Y-%m-%dT%H:%M:%S.%f%z"
 
 # Train-val splits
 TRAIN = "train"
 VAL = "val"
 FULL = "full"
 MINI = "mini"
+VERSIONS = (FULL, MINI)
 TRAINVAL_FILES = {
     FRAMES: {
         FULL: f"trainval_frames_full.json",
         MINI: f"trainval_frames_mini.json",
     },
     SEQUENCES: {
         FULL: f"trainval_sequences_full.json",
         MINI: f"trainval_sequences_mini.json",
     },
+    DRIVES: {
+        FULL: f"trainval_drives_full.json",
+        MINI: f"trainval_drives_mini.json",
+    },
 }
 SPLIT_FILES = {
+    FRAMES: {
+        FULL: {
+            TRAIN: "splits/frames_full_train.txt",
+            VAL: "splits/frames_full_val.txt",
+        },
+        MINI: {
+            TRAIN: "splits/frames_mini_train.txt",
+            VAL: "splits/frames_mini_val.txt",
+        },
+    },
     SEQUENCES: {
         FULL: {
             TRAIN: "splits/sequences_full_train.txt",
             VAL: "splits/sequences_full_val.txt",
         },
         MINI: {
             TRAIN: "splits/sequences_mini_train.txt",
             VAL: "splits/sequences_mini_val.txt",
         },
     },
-    FRAMES: {
+    DRIVES: {
         FULL: {
-            TRAIN: "splits/frames_full_train.txt",
-            VAL: "splits/frames_full_val.txt",
+            TRAIN: "splits/drives_full_train.txt",
+            VAL: "splits/drives_full_val.txt",
         },
         MINI: {
-            TRAIN: "splits/frames_mini_train.txt",
-            VAL: "splits/frames_mini_val.txt",
+            TRAIN: "splits/drives_mini_train.txt",
+            VAL: "splits/drives_mini_val.txt",
         },
     },
 }
 
 
-VERSIONS = (FULL, MINI)
-
-
 class Anonymization(Enum):
     BLUR = "blur"
     DNAT = "dnat"
     ORIGINAL = "original"
 
 
 class AnnotationProject(Enum):
```

### Comparing `zod-0.1.7/zod/data_classes/box.py` & `zod-0.1.8/zod/data_classes/box.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,22 @@
 
     def convert_to(self, frame: CoordinateFrame, calib: Calibration):
         if frame == self.frame:
             return
         self._transform(calib.get_extrinsics(self.frame), new_frame=EGO)
         self._transform_inv(calib.get_extrinsics(frame), new_frame=frame)
 
+    def copy(self):
+        return Box3D(
+            center=self.center.copy(),
+            size=self.size.copy(),
+            orientation=Quaternion(self.orientation),
+            frame=self.frame,
+        )
+
     @property
     def corners(self) -> np.ndarray:
         """Get the corners of the bounding box in the current frame.
 
         Order of points are:
          - rear left bottom
          - rear right bottom
```

### Comparing `zod-0.1.7/zod/data_classes/calibration.py` & `zod-0.1.8/zod/data_classes/calibration.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/data_classes/frame.py` & `zod-0.1.8/zod/data_classes/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import numpy as np
 
 from zod.constants import AnnotationProject, Anonymization, Camera, Lidar
 from zod.utils.compensation import motion_compensate_scanwise
 
 from .calibration import Calibration
+from .ego_motion import EgoMotion
 from .info import Information
 from .metadata import FrameMetaData
-from .oxts import EgoMotion
 from .sensor import CameraFrame, LidarData, LidarFrame
 
 
 class ZodFrame:
     def __init__(self, info: Information):
         self.info: Information = info  # Holds all the paths to the files
         self._ego_motion: EgoMotion = None  # This is the lightweight version of oxts
```

### Comparing `zod-0.1.7/zod/data_classes/geometry.py` & `zod-0.1.8/zod/data_classes/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/data_classes/info.py` & `zod-0.1.8/zod/data_classes/info.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/data_classes/metadata.py` & `zod-0.1.8/zod/data_classes/metadata.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/data_classes/oxts.py` & `zod-0.1.8/zod/data_classes/ego_motion.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/data_classes/sensor.py` & `zod-0.1.8/zod/data_classes/sensor.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/data_classes/sequence.py` & `zod-0.1.8/zod/data_classes/sequence.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, List, Optional
 
 from zod.constants import AnnotationProject, Lidar
 from zod.utils.compensation import motion_compensate_scanwise
 
 from .calibration import Calibration
+from .ego_motion import EgoMotion
 from .info import Information
 from .metadata import SequenceMetadata
-from .oxts import EgoMotion
 from .sensor import LidarData
 
 
 class ZodSequence:
     def __init__(self, info: Information):
         self.info: Information = info  # holds all the paths to the files
         self._ego_motion: EgoMotion = None  # this is the light-weight version of oxts
@@ -71,7 +71,30 @@
             compensated_scan = motion_compensate_scanwise(
                 scan, self.ego_motion, self.calibration.lidars[Lidar.VELODYNE], timestamp
             )
             lidar_scans[i] = compensated_scan
         aggregated = lidar_scans[0]
         aggregated.extend(*lidar_scans[1:])
         return aggregated
+
+    def get_keyframe_lidar(self, motion_compensated=True) -> LidarData:
+        """Get the keyframe point cloud.
+
+        Args:
+            motion_compensated (bool, optional): Whether to motion compensate the point cloud
+             to camera (and annotation) timestamp. Defaults to True.
+
+        Returns:
+            LidarData: The point cloud.
+        """
+
+        lidar_scan = self.info.get_key_lidar_frame(Lidar.VELODYNE).read()
+
+        if not motion_compensated:
+            return lidar_scan
+
+        return motion_compensate_scanwise(
+            lidar_scan,
+            self.ego_motion,
+            self.calibration.lidars[Lidar.VELODYNE],
+            self.info.keyframe_time.timestamp(),
+        )
```

### Comparing `zod-0.1.7/zod/eval/detection/_experimental/eval.py` & `zod-0.1.8/zod/eval/detection/_experimental/eval.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/eval/detection/_experimental/matching.py` & `zod-0.1.8/zod/eval/detection/_experimental/matching.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/eval/detection/_experimental/utils.py` & `zod-0.1.8/zod/eval/detection/_experimental/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/eval/detection/_nuscenes_eval/LICENCE.txt` & `zod-0.1.8/zod/eval/detection/_nuscenes_eval/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/eval/detection/_nuscenes_eval/changes.txt` & `zod-0.1.8/zod/eval/detection/_nuscenes_eval/changes.txt`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/eval/detection/_nuscenes_eval/common/data_classes.py` & `zod-0.1.8/zod/eval/detection/_nuscenes_eval/common/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/eval/detection/_nuscenes_eval/common/utils.py` & `zod-0.1.8/zod/eval/detection/_nuscenes_eval/common/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/eval/detection/_nuscenes_eval/detection/README.md` & `zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/eval/detection/_nuscenes_eval/detection/algo.py` & `zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/algo.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/eval/detection/_nuscenes_eval/detection/constants.py` & `zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/constants.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/eval/detection/_nuscenes_eval/detection/data_classes.py` & `zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/eval/detection/eval_nuscenes_style.py` & `zod-0.1.8/zod/eval/detection/eval_nuscenes_style.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/utils/compensation.py` & `zod-0.1.8/zod/utils/compensation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 import numpy as np
 
 from zod.data_classes.calibration import LidarCalibration
-from zod.data_classes.oxts import EgoMotion
+from zod.data_classes.ego_motion import EgoMotion
 from zod.data_classes.sensor import LidarData
 
 
 def motion_compensate_scanwise(
     lidar_data: LidarData,
     ego_motion: EgoMotion,
     calibration: LidarCalibration,
```

### Comparing `zod-0.1.7/zod/utils/geometry.py` & `zod-0.1.8/zod/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/utils/polygon_transformations.py` & `zod-0.1.8/zod/utils/polygon_transformations.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/utils/utils.py` & `zod-0.1.8/zod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/utils/visualization.py` & `zod-0.1.8/zod/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/visualization/bev_utils.py` & `zod-0.1.8/zod/visualization/bev_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/visualization/colorlabeler.py` & `zod-0.1.8/zod/visualization/colorlabeler.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/visualization/lidar_bev.py` & `zod-0.1.8/zod/visualization/lidar_bev.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/visualization/lidar_on_image.py` & `zod-0.1.8/zod/visualization/lidar_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/visualization/object_visualization.py` & `zod-0.1.8/zod/visualization/object_visualization.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,16 +74,17 @@
     calib,
     color=(0, 0, 100),
     scale_factor=None,
     line_thickness=2,
     camera: Camera = Camera.FRONT,
 ):
     """Visualize 2D box of annotated object on the image."""
-    box3d.convert_to(camera, calib)
-    render_3d_box(image, box3d, calib, color, line_thickness)
+    box3d_copy = box3d.copy()
+    box3d_copy.convert_to(camera, calib)
+    render_3d_box(image, box3d_copy, calib, color, line_thickness)
     return image
 
 
 def overlay_object_properties_on_image(
     image: np.ndarray,
     annotation: ObjectAnnotation,
     color: Tuple[int, int, int] = (255, 0, 0),
```

### Comparing `zod-0.1.7/zod/visualization/oxts_on_image.py` & `zod-0.1.8/zod/visualization/oxts_on_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module to perform OxTS extraction and visualize GPS track projection on image plane."""
 import cv2
 import numpy as np
 
 from zod.constants import Camera
 from zod.data_classes.calibration import Calibration
-from zod.data_classes.oxts import EgoMotion
+from zod.data_classes.ego_motion import EgoMotion
 from zod.utils.geometry import get_points_in_camera_fov, project_3d_to_2d_kannala, transform_points
 
 
 def visualize_oxts_on_image(
     oxts: EgoMotion, key_timestamp, calibs: Calibration, image, camera=Camera.FRONT
 ):
     """Visualize oxts track on image plane."""
```

### Comparing `zod-0.1.7/zod/visualization/oxts_visualization.py` & `zod-0.1.8/zod/visualization/oxts_visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import json
 from typing import List, Optional, Sequence
 
 import numpy as np
 import plotly.express as px
 
-from zod.data_classes.oxts import EgoMotion
+from zod.data_classes.ego_motion import EgoMotion
 
 MAPS_STYLE = "open-street-map"
 SIZE_MAX = 7
 OPACITY_LEVEL = 1
 DEFAULT_COLOR = "red"
 DEFAULT_SIZE = 1
```

### Comparing `zod-0.1.7/zod/visualization/polygon_utils.py` & `zod-0.1.8/zod/visualization/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.7/zod/zod_frames.py` & `zod-0.1.8/zod/_zod_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,91 +1,92 @@
 """ZOD Frames module."""
 import json
 import os.path as osp
+from abc import ABC, abstractmethod
 from functools import partial
-from itertools import repeat
-from pathlib import Path
-from typing import Dict, List, Set, Tuple, Union
+from itertools import chain
+from typing import Any, Dict, Set, Tuple, Union
 
 from tqdm.contrib.concurrent import process_map
 
-from zod.constants import FRAMES, FULL, TRAIN, TRAINVAL_FILES, VAL, VERSIONS
-from zod.data_classes.frame import ZodFrame
+from zod.constants import FULL, TRAIN, VAL, VERSIONS
 from zod.data_classes.info import Information
 from zod.utils.utils import zfill_id
 
 
 def _create_frame(frame: dict, dataset_root: str) -> Information:
     info = Information.from_dict(frame)
     info.convert_paths_to_absolute(dataset_root)
     return info
 
 
-class ZodFrames(object):
-    """ZOD Frames."""
+class ZodDataset(ABC):
+    """Base class for all ZOD sub-datasets (frames, sequences, drives)."""
 
-    def __init__(self, dataset_root: Union[Path, str], version: str, mp: bool = True):
+    def __init__(self, dataset_root: str, version: str, mp: bool = True):
         self._dataset_root = dataset_root
         self._version = version
         self._mp = mp
         assert version in VERSIONS, f"Unknown version: {version}, must be one of: {VERSIONS}"
-        self._train_frames, self._val_frames = self._load_frames()
-        self._frames: Dict[str, Information] = {**self._train_frames, **self._val_frames}
+        self._infos, self._train_ids, self._val_ids = self._load_infos()
 
     def __len__(self) -> int:
-        return len(self._frames)
+        return len(self._infos)
 
-    def __getitem__(self, frame_id: Union[int, str, slice]) -> ZodFrame:
-        """Get frame by id, which is a 6-digit zero-padded number. Ex: '000001'."""
+    def __iter__(self):
+        for frame_id in self._infos:
+            if frame_id not in self._train_ids and frame_id not in self._val_ids:
+                continue
+            yield self.__getitem__(frame_id)
+
+    @abstractmethod
+    def __getitem__(self, frame_id: Union[int, str, slice]) -> Any:
+        """Get item by id, which is a 6-digit zero-padded number. Ex: '000001'."""
         if isinstance(frame_id, slice):
             return [self.__getitem__(i) for i in range(*frame_id.indices(len(self)))]
         frame_id = zfill_id(frame_id)
-        return ZodFrame(self._frames[frame_id])
+        return self._infos[frame_id]
 
-    def __iter__(self):
-        for frame_id in self._frames:
-            yield self.__getitem__(frame_id)
+    @property
+    @abstractmethod
+    def trainval_files(self) -> Dict[str, str]:
+        """Mapping of version to trainval file."""
+        raise NotImplementedError
+
+    def get_split(self, split: str) -> Set[str]:
+        """Get split by name (e.g. train / val)."""
+        if split == TRAIN:
+            return self._train_ids
+        elif split == VAL:
+            return self._val_ids
+        else:
+            raise ValueError(f"Unknown split: {split}, should be {TRAIN} or {VAL}")
+
+    def get_all_infos(self) -> Dict[str, Information]:
+        """Get all infos (including blacklisted ones)."""
+        return self._infos
+
+    def get_all_ids(self) -> Set[str]:
+        """Get all frame ids (excluding blackisted ones)."""
+        return self._train_ids.union(self._val_ids)
 
-    def _load_frames(self) -> Tuple[Dict[str, Information], Dict[str, Information]]:
+    def _load_infos(self) -> Tuple[Dict[str, Information], Set[str], Set[str]]:
         """Load frames for the given version."""
-        filename = TRAINVAL_FILES[FRAMES][self._version]
+        filename = self.trainval_files[self._version]
         with open(osp.join(self._dataset_root, filename), "r") as f:
             all_ids = json.load(f)
 
         func = partial(_create_frame, dataset_root=self._dataset_root)
         if self._mp and self._version == FULL:
-            train_frames = process_map(
-                func,
-                all_ids[TRAIN],
-                desc="Loading train frames",
-                chunksize=50 if self._version == FULL else 1,
-            )
-            val_frames = process_map(
+            infos = process_map(
                 func,
-                all_ids[VAL],
-                desc="Loading val frames",
+                chain.from_iterable(all_ids.values()),
+                desc="Loading infos",
                 chunksize=50 if self._version == FULL else 1,
             )
-            train_frames = {frame.id: frame for frame in train_frames}
-            val_frames = {frame.id: frame for frame in val_frames}
+            infos = {frame.id: frame for frame in infos}
         else:
-            train_frames = {frame.id: frame for frame in map(func, all_ids[TRAIN])}
-            val_frames = {frame.id: frame for frame in map(func, all_ids[VAL])}
+            infos = {frame.id: frame for frame in map(func, chain.from_iterable(all_ids.values()))}
 
-        return train_frames, val_frames
-
-    def get_split(self, split: str) -> List[str]:
-        """Get split by name (e.g. train / val)."""
-        if split == TRAIN:
-            return list(self._train_frames.keys())
-        elif split == VAL:
-            return list(self._val_frames.keys())
-        else:
-            raise ValueError(f"Unknown split: {split}, should be {TRAIN} or {VAL}")
-
-    def get_all_frame_infos(self) -> Dict[str, Information]:
-        """Get all frames."""
-        return self._frames
-
-    def get_all_ids(self) -> Set[str]:
-        """Get all frame ids."""
-        return set(self._frames.keys())
+        train_ids = {f["id"] for f in all_ids[TRAIN]}
+        val_ids = {f["id"] for f in all_ids[VAL]}
+        return infos, train_ids, val_ids
```

### Comparing `zod-0.1.7/PKG-INFO` & `zod-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zod
-Version: 0.1.7
+Version: 0.1.8
 Summary: Zenseact Open Dataset
 Home-page: https://zod.zenseact.com
 License: MIT
 Author: Zenseact
 Author-email: opendataset@zenseact.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -62,35 +62,35 @@
 To install the full devkit, with the CLI and all dependencies, run:
 ```bash
 pip install "zod[all]"
 ```
 
 ## Download using the CLI
 
-This is an example of how to download the ZOD Frames mini-dataset using the CLI. Prerequisites are that you have applied for access and received a download link. To download the mini-dataset, run:
+This is an example of how to download the ZOD Frames mini-dataset using the CLI. Prerequisites are that you have applied for access and received a download link.
+The simplest way to download the dataset is to use the CLI interactively:
 ```bash
-zod download --url "<download-link>" --output-dir <path/to/outputdir> frames --mini
+zod download
 ```
-similarly, to download the full dataset (including all lidar scans before and after the keyframe), run:
+This will prompt you for the required information, present you with a summary of the download, and then ask for confirmation. You can of course also specify all the required information directly on the command line, and avoid the confirmation using `--no-confirm` or `-y`. For example:
 ```bash
-zod download --url "<download-link>" --output-dir <path/to/outputdir> frames --lidar --num-scans-before -1 --num-scans-after -1 --oxts --images --blur --dnat --calibrations --annotations
+zod download -y --url="<download-link>" --output-dir=<path/to/outputdir> --subset=frames --version=mini
 ```
-this will download all the previous and future lidar scans (as `num-scans-before=-1` and `num-scans-after=-1`), the OxTS data, the images (with both the blur and DNAT anonymization), the calibration files, the annotations, and all other necessary files. If you dont want any previous or future lidar scans, run:
+By default, all data streams are downloaded for ZodSequences and ZodDrives. For ZodFrames, DNAT versions of the images, and surrounding (non-keyframe) lidar scans are excluded. To download them as well, run:
 ```bash
-zod download --url "<download-link>" --output-dir <path/to/outputdir> frames --lidar --num-scans-before 0 --num-scans-after 0 --oxts --images --blur --dnat --calibrations --annotations
+zod download -y --url="<download-link>" --output-dir=<path/to/outputdir> --subset=frames --version=full --num-scans-before=-1 --num-scans-after=-1 --dnat
 ```
-
-For a full list of options for ZOD download, run:
+If you want to exclude some of the data streams, you can do so by specifying the `--no-<stream>` flag. For example, to download only the DNAT images, infos, and annotations, run:
+```bash
+zod download --dnat --no-blur --no-lidar --no-oxts --no-vehicle-data
+```
+Finally, for a full list of options you can of course run:
 ```bash
 zod download --help
-zod download --url="<url>" --output-dir=<dir> frames --help
-zod download --url="<url>" --output-dir=<dir> sequences --help
 ```
-depending on which dataset you want to download.
-
 
 ## Anonymization
 To preserve privacy, the dataset is anonymized. The anonymization is performed by [brighterAI](https://brighter.ai/), and we provide two separate modes of anonymization: deep fakes (DNAT) and blur. In our paper, we show that the performance of an object detector is not affected by the anonymization method. For more details regarding this experiment, please refer to our [coming soon]().
 
 ## Citation
 If you publish work that uses Zenseact Open Dataset, please cite: [coming soon]()
```

