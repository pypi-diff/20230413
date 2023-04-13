# Comparing `tmp/vpc-img-inst-1.0.0b8.tar.gz` & `tmp/vpc-img-inst-1.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vpc-img-inst-1.0.0b8.tar", last modified: Mon Feb 13 15:01:39 2023, max compression
+gzip compressed data, was "vpc-img-inst-1.0.0b9.tar", last modified: Wed Feb 22 19:12:04 2023, max compression
```

## Comparing `vpc-img-inst-1.0.0b8.tar` & `vpc-img-inst-1.0.0b9.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-13 15:01:39.319863 vpc-img-inst-1.0.0b8/
--rw-r--r--   0 omer      (1000) omer      (1000)    11357 2022-11-15 16:30:30.000000 vpc-img-inst-1.0.0b8/LICENSE
--rw-r--r--   0 omer      (1000) omer      (1000)     4664 2023-02-13 15:01:39.318863 vpc-img-inst-1.0.0b8/PKG-INFO
--rw-r--r--   0 omer      (1000) omer      (1000)     4261 2023-02-11 14:20:49.000000 vpc-img-inst-1.0.0b8/README.md
--rw-r--r--   0 omer      (1000) omer      (1000)      104 2022-11-15 09:07:07.000000 vpc-img-inst-1.0.0b8/pyproject.toml
--rw-r--r--   0 omer      (1000) omer      (1000)       38 2023-02-13 15:01:39.319863 vpc-img-inst-1.0.0b8/setup.cfg
--rw-r--r--   0 omer      (1000) omer      (1000)     2941 2023-02-13 15:00:35.000000 vpc-img-inst-1.0.0b8/setup.py
-drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-13 15:01:39.309863 vpc-img-inst-1.0.0b8/src/
-drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-13 15:01:39.311863 vpc-img-inst-1.0.0b8/src/vpc_img_inst/
--rw-r--r--   0 omer      (1000) omer      (1000)        1 2022-12-07 12:30:57.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/__init__.py
-drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-13 15:01:39.313863 vpc-img-inst-1.0.0b8/src/vpc_img_inst/bin/
--rw-r--r--   0 omer      (1000) omer      (1000)        0 2022-12-07 12:30:57.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/bin/__init__.py
--rwxr-xr-x   0 omer      (1000) omer      (1000)      215 2022-12-07 12:30:57.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/bin/vpc_img_inst.py
--rw-r--r--   0 omer      (1000) omer      (1000)     5930 2022-12-19 12:56:05.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_builder.py
-drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-13 15:01:39.316863 vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/
--rw-r--r--   0 omer      (1000) omer      (1000)      832 2022-12-07 12:30:57.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/__init__.py
--rw-r--r--   0 omer      (1000) omer      (1000)     2223 2022-12-19 12:25:40.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/apikey_config.py
--rw-r--r--   0 omer      (1000) omer      (1000)     9947 2022-12-26 14:11:28.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/delete_resources.py
--rw-r--r--   0 omer      (1000) omer      (1000)     1921 2022-12-19 12:53:41.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/endpoint_config.py
--rw-r--r--   0 omer      (1000) omer      (1000)     2303 2022-12-13 13:01:54.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/image_config.py
--rw-r--r--   0 omer      (1000) omer      (1000)     4875 2022-12-08 10:10:40.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/image_create.py
--rw-r--r--   0 omer      (1000) omer      (1000)     4275 2022-12-08 17:02:56.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/install_feature.py
--rw-r--r--   0 omer      (1000) omer      (1000)     2668 2022-12-08 10:10:30.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/ip_config.py
--rw-r--r--   0 omer      (1000) omer      (1000)     4824 2022-12-08 10:10:26.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/ssh_config.py
--rw-r--r--   0 omer      (1000) omer      (1000)     8632 2022-12-19 12:33:37.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/vpc_config.py
--rw-r--r--   0 omer      (1000) omer      (1000)     3958 2022-12-08 10:10:11.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/vsi_config.py
--rw-r--r--   0 omer      (1000) omer      (1000)     1141 2023-02-06 18:44:09.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/constants.py
--rw-r--r--   0 omer      (1000) omer      (1000)      514 2022-12-07 12:30:57.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/defaults.yaml
-drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-13 15:01:39.310863 vpc-img-inst-1.0.0b8/src/vpc_img_inst/installation_scripts/
-drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-13 15:01:39.317863 vpc-img-inst-1.0.0b8/src/vpc_img_inst/installation_scripts/cuda/
--rwxr-xr-x   0 omer      (1000) omer      (1000)      928 2023-02-07 12:04:08.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/installation_scripts/cuda/install_cuda_rhel-8.sh
--rw-r--r--   0 omer      (1000) omer      (1000)      591 2023-02-07 12:03:38.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/installation_scripts/cuda/install_cuda_ubuntu-20.sh
--rw-r--r--   0 omer      (1000) omer      (1000)      591 2023-02-07 12:03:35.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/installation_scripts/cuda/install_cuda_ubuntu-22.sh
-drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-13 15:01:39.317863 vpc-img-inst-1.0.0b8/src/vpc_img_inst/installation_scripts/docker/
--rw-r--r--   0 omer      (1000) omer      (1000)      163 2022-12-07 12:30:57.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/installation_scripts/docker/install_docker_rhel.sh
--rw-r--r--   0 omer      (1000) omer      (1000)      569 2022-12-07 12:30:57.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/installation_scripts/docker/install_docker_ubuntu.sh
-drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-13 15:01:39.318863 vpc-img-inst-1.0.0b8/src/vpc_img_inst/installation_scripts/ray/
--rw-r--r--   0 omer      (1000) omer      (1000)      677 2022-12-18 17:25:07.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/installation_scripts/ray/install_ray_ubuntu.sh
--rw-r--r--   0 omer      (1000) omer      (1000)     6401 2022-12-08 10:09:49.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/main.py
--rw-r--r--   0 omer      (1000) omer      (1000)    17507 2022-12-08 10:09:47.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst/utils.py
-drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-13 15:01:39.313863 vpc-img-inst-1.0.0b8/src/vpc_img_inst.egg-info/
--rw-r--r--   0 omer      (1000) omer      (1000)     4664 2023-02-13 15:01:39.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst.egg-info/PKG-INFO
--rw-r--r--   0 omer      (1000) omer      (1000)     1461 2023-02-13 15:01:39.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst.egg-info/SOURCES.txt
--rw-r--r--   0 omer      (1000) omer      (1000)        1 2023-02-13 15:01:39.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst.egg-info/dependency_links.txt
--rw-r--r--   0 omer      (1000) omer      (1000)       59 2023-02-13 15:01:39.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst.egg-info/entry_points.txt
--rw-r--r--   0 omer      (1000) omer      (1000)      169 2023-02-13 15:01:39.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst.egg-info/requires.txt
--rw-r--r--   0 omer      (1000) omer      (1000)       13 2023-02-13 15:01:39.000000 vpc-img-inst-1.0.0b8/src/vpc_img_inst.egg-info/top_level.txt
+drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-22 19:12:04.177320 vpc-img-inst-1.0.0b9/
+-rw-r--r--   0 omer      (1000) omer      (1000)    11357 2022-11-15 16:30:30.000000 vpc-img-inst-1.0.0b9/LICENSE
+-rw-r--r--   0 omer      (1000) omer      (1000)     4664 2023-02-22 19:12:04.177320 vpc-img-inst-1.0.0b9/PKG-INFO
+-rw-r--r--   0 omer      (1000) omer      (1000)     4261 2023-02-11 14:20:49.000000 vpc-img-inst-1.0.0b9/README.md
+-rw-r--r--   0 omer      (1000) omer      (1000)      104 2022-11-15 09:07:07.000000 vpc-img-inst-1.0.0b9/pyproject.toml
+-rw-r--r--   0 omer      (1000) omer      (1000)       38 2023-02-22 19:12:04.177320 vpc-img-inst-1.0.0b9/setup.cfg
+-rw-r--r--   0 omer      (1000) omer      (1000)     2941 2023-02-22 19:09:48.000000 vpc-img-inst-1.0.0b9/setup.py
+drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-22 19:12:04.170320 vpc-img-inst-1.0.0b9/src/
+drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-22 19:12:04.172320 vpc-img-inst-1.0.0b9/src/vpc_img_inst/
+-rw-r--r--   0 omer      (1000) omer      (1000)        1 2022-12-07 12:30:57.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/__init__.py
+drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-22 19:12:04.174320 vpc-img-inst-1.0.0b9/src/vpc_img_inst/bin/
+-rw-r--r--   0 omer      (1000) omer      (1000)        0 2022-12-07 12:30:57.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/bin/__init__.py
+-rwxr-xr-x   0 omer      (1000) omer      (1000)      215 2022-12-07 12:30:57.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/bin/vpc_img_inst.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     5930 2022-12-19 12:56:05.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_builder.py
+drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-22 19:12:04.176320 vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/
+-rw-r--r--   0 omer      (1000) omer      (1000)      832 2022-12-07 12:30:57.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/__init__.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     2223 2022-12-19 12:25:40.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/apikey_config.py
+-rw-r--r--   0 omer      (1000) omer      (1000)    10405 2023-02-22 19:00:30.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/delete_resources.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     1921 2022-12-19 12:53:41.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/endpoint_config.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     2303 2022-12-13 13:01:54.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/image_config.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     4875 2022-12-08 10:10:40.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/image_create.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     4275 2023-02-22 18:28:09.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/install_feature.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     2668 2022-12-08 10:10:30.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/ip_config.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     4824 2022-12-08 10:10:26.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/ssh_config.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     8641 2023-02-22 18:57:40.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/vpc_config.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     3958 2022-12-08 10:10:11.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/vsi_config.py
+-rw-r--r--   0 omer      (1000) omer      (1000)     1138 2023-02-22 18:43:22.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/constants.py
+-rw-r--r--   0 omer      (1000) omer      (1000)      514 2022-12-07 12:30:57.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/defaults.yaml
+drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-22 19:12:04.170320 vpc-img-inst-1.0.0b9/src/vpc_img_inst/installation_scripts/
+drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-22 19:12:04.176320 vpc-img-inst-1.0.0b9/src/vpc_img_inst/installation_scripts/cuda/
+-rwxr-xr-x   0 omer      (1000) omer      (1000)      928 2023-02-22 16:57:40.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/installation_scripts/cuda/install_cuda_rhel.sh
+-rw-r--r--   0 omer      (1000) omer      (1000)      755 2023-02-22 16:57:10.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/installation_scripts/cuda/install_cuda_ubuntu.sh
+drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-22 19:12:04.177320 vpc-img-inst-1.0.0b9/src/vpc_img_inst/installation_scripts/docker/
+-rw-r--r--   0 omer      (1000) omer      (1000)      163 2022-12-07 12:30:57.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/installation_scripts/docker/install_docker_rhel.sh
+-rw-r--r--   0 omer      (1000) omer      (1000)      579 2023-02-22 17:00:22.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/installation_scripts/docker/install_docker_ubuntu.sh
+drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-22 19:12:04.177320 vpc-img-inst-1.0.0b9/src/vpc_img_inst/installation_scripts/ray/
+-rw-r--r--   0 omer      (1000) omer      (1000)      609 2023-02-22 19:10:12.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/installation_scripts/ray/install_ray_ubuntu.sh
+-rw-r--r--   0 omer      (1000) omer      (1000)     6401 2023-02-22 18:43:38.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/main.py
+-rw-r--r--   0 omer      (1000) omer      (1000)    17507 2022-12-08 10:09:47.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst/utils.py
+drwxr-xr-x   0 omer      (1000) omer      (1000)        0 2023-02-22 19:12:04.174320 vpc-img-inst-1.0.0b9/src/vpc_img_inst.egg-info/
+-rw-r--r--   0 omer      (1000) omer      (1000)     4664 2023-02-22 19:12:04.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst.egg-info/PKG-INFO
+-rw-r--r--   0 omer      (1000) omer      (1000)     1387 2023-02-22 19:12:04.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst.egg-info/SOURCES.txt
+-rw-r--r--   0 omer      (1000) omer      (1000)        1 2023-02-22 19:12:04.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst.egg-info/dependency_links.txt
+-rw-r--r--   0 omer      (1000) omer      (1000)       59 2023-02-22 19:12:04.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst.egg-info/entry_points.txt
+-rw-r--r--   0 omer      (1000) omer      (1000)      169 2023-02-22 19:12:04.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst.egg-info/requires.txt
+-rw-r--r--   0 omer      (1000) omer      (1000)       13 2023-02-22 19:12:04.000000 vpc-img-inst-1.0.0b9/src/vpc_img_inst.egg-info/top_level.txt
```

### Comparing `vpc-img-inst-1.0.0b8/LICENSE` & `vpc-img-inst-1.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/PKG-INFO` & `vpc-img-inst-1.0.0b9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpc-img-inst
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: vpc-img-inst is a lightweight script for quick-and-dirty generation of custom VSI images by installing features (software bundles) on base images.
 Home-page: https://github.com/IBM/vpc-img-inst
 Author:  Omer-J-Cohen
 Author-email: omer.cohen@ibm.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vpc-img-inst Version: 1.0.0b8 Summary: vpc-img-inst
+Metadata-Version: 2.1 Name: vpc-img-inst Version: 1.0.0b9 Summary: vpc-img-inst
 is a lightweight script for quick-and-dirty generation of custom VSI images by
 installing features (software bundles) on base images. Home-page: https://
 github.com/IBM/vpc-img-inst Author: Omer-J-Cohen Author-email:
 omer.cohen@ibm.com Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE # Image Installer For IBM-VPC vpc-img-inst is a
 lightweight script for quick-and-dirty generation of custom VSI images by
 installing features (software bundles) on base images. ## Setup Mostly tested
```

### Comparing `vpc-img-inst-1.0.0b8/README.md` & `vpc-img-inst-1.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/setup.py` & `vpc-img-inst-1.0.0b9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 find_packages(where='src',exclude=['logs'])
 
 setup(
     name='vpc-img-inst',
-    version='1.0.0b8',
+    version='1.0.0b9',
     author =' Omer-J-Cohen',
     author_email = 'omer.cohen@ibm.com',
     description = 'vpc-img-inst is a lightweight script for quick-and-dirty generation of custom VSI images by installing features (software bundles) on base images.',
     long_description=read('README.md'),
     long_description_content_type = "text/markdown",
     url = 'https://github.com/IBM/vpc-img-inst',
     install_requires=[
```

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_builder.py` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_builder.py`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/__init__.py` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/apikey_config.py` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/apikey_config.py`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/delete_resources.py` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/delete_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,22 +99,30 @@
                 os.remove(public_key)
                 logger.info(color_msg(f'Deleted public key: {public_key}', color=Color.PURPLE))
             except OSError as e:
                 logger.info(f"""Local public key: {public_key} doesn't exist""")
         
         # delete vpc
         if 'vpc_id' in self.base_config["node_config"] and self.base_config["node_config"]['vpc_id']:
-            try:
-                self.ibm_vpc_client.delete_vpc(self.base_config["node_config"]['vpc_id'])
-                logger.info(color_msg('Deleted VPC with id: {}'.format(self.base_config["node_config"]['vpc_id']), color=Color.PURPLE))
-            except ApiException as e:
-                if e.code == 404:
-                    logger.info(f"""VPC with id: "{self.base_config["node_config"]['vpc_id']}" doesn't exist""")
-                else:
-                    raise e
+            deleting_resources = True
+            sleep_duration = 10
+            while deleting_resources:
+                try:
+                    self.ibm_vpc_client.delete_vpc(self.base_config["node_config"]['vpc_id'])
+                    logger.info(color_msg('Deleted VPC with id: {}'.format(self.base_config["node_config"]['vpc_id']), color=Color.PURPLE))
+                    deleting_resources = False
+                except ApiException as e:
+                    if e.code == 404:
+                        logger.info(f"""VPC with id: "{self.base_config["node_config"]['vpc_id']}" doesn't exist""")
+                        deleting_resources = False
+                    elif e.code == 409:
+                        logger.info(f"""VPC with id: "{self.base_config["node_config"]['vpc_id']}" still in use. Retrying...""")
+                        time.sleep(sleep_duration)
+                    else:
+                        raise e
 
         # delete failed images
         failed_images = _get_failed_images(self.base_config['output_file'])
         for failed_image_id in failed_images:
             try:
                 self.ibm_vpc_client.delete_image(failed_image_id)
                 logger.info(color_msg('Deleted failed image with id: {}'.format(failed_image_id), color=Color.PURPLE))
```

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/endpoint_config.py` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/endpoint_config.py`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/image_config.py` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/image_config.py`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/image_create.py` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/image_create.py`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/install_feature.py` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/install_feature.py`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/ip_config.py` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/ip_config.py`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/ssh_config.py` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/ssh_config.py`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/vpc_config.py` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/vpc_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def __init__(self, base_config: Dict[str, Any]) -> None:
         super().__init__(base_config)
         self.base_config = base_config
 
         self.sg_rules = {'outbound_tcp_all': 'selected security group is missing rule permitting outbound TCP access\n',
                         'inbound_tcp_22': 'selected security group is missing rule permitting inbound traffic to tcp port 22 required for ssh\n',}  # security group rules.
-        self.vpc_name = 'temp-vpc'
+        self.vpc_name = 'temp-vpc-img-inst'
         
     def _get_region(self):
         region = None
         try:
             region = get_region_by_endpoint(self.ibm_vpc_client.service_url)
         except Exception:
             region = ConfigBuilder.region
```

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/config_modules/vsi_config.py` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/config_modules/vsi_config.py`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/constants.py` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 import tempfile
 from pathlib import Path
 DIR_PATH = os.path.dirname(os.path.realpath(__file__))  # absolute path to project's root folder.
 USER_SCRIPTS_FOLDER = str(Path.home())+os.sep+".vpc-img-inst" 
 
 DEFAULTS = {'base_image_name':'ibm-ubuntu-22-04',  
             'region':'eu-de',
-             'installation_type':"ubuntu-22",
+             'installation_type':"ubuntu",
              "feature":"cuda", 
              "image_create_retries":3, 
              "script_inst_retries":5,
              "input_file":f'{DIR_PATH}{os.sep}defaults.yaml',
              "output_folder":tempfile.mkdtemp()}
```

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/defaults.yaml` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/defaults.yaml`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/installation_scripts/cuda/install_cuda_rhel-8.sh` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/installation_scripts/cuda/install_cuda_rhel.sh`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/installation_scripts/cuda/install_cuda_ubuntu-20.sh` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/installation_scripts/cuda/install_cuda_ubuntu.sh`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/bin/bash
-#Ubuntu 20.04 CUDA 
+
 sudo apt-get install linux-headers-$(uname -r) gcc -y 
 sudo apt-key del 7fa2af80
-export distro="ubuntu2004"
+# extract ubuntu release version and parse the required format of: <OS><VERSION_ID_DIGITS_ONLY>, e.g. 'ubuntu2204'. 
+export distro="ubuntu$(awk -F'=' '/^VERSION_ID/ {print $2}' /etc/os-release | tr -d '[".]')"
 export arch="x86_64"
 wget https://developer.download.nvidia.com/compute/cuda/repos/$distro/$arch/cuda-keyring_1.0-1_all.deb
 sudo dpkg -i cuda-keyring_1.0-1_all.deb
 sudo apt-get update 
 sudo apt-get install cuda -y
 sudo apt-get install cuda-drivers-520 -y
 sudo systemctl enable nvidia-persistenced
```

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/installation_scripts/docker/install_docker_ubuntu.sh` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/installation_scripts/docker/install_docker_ubuntu.sh`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/bin/bash
 
-apt-get update
-apt-get -y install \
+sudo apt-get update
+sudo apt-get -y install \
     ca-certificates \
     curl \
     gnupg \
     lsb-release
 mkdir -p /etc/apt/keyrings
 curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
 echo \
```

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/main.py` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/main.py`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst/utils.py` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst/utils.py`

 * *Files identical despite different names*

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst.egg-info/PKG-INFO` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpc-img-inst
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: vpc-img-inst is a lightweight script for quick-and-dirty generation of custom VSI images by installing features (software bundles) on base images.
 Home-page: https://github.com/IBM/vpc-img-inst
 Author:  Omer-J-Cohen
 Author-email: omer.cohen@ibm.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vpc-img-inst Version: 1.0.0b8 Summary: vpc-img-inst
+Metadata-Version: 2.1 Name: vpc-img-inst Version: 1.0.0b9 Summary: vpc-img-inst
 is a lightweight script for quick-and-dirty generation of custom VSI images by
 installing features (software bundles) on base images. Home-page: https://
 github.com/IBM/vpc-img-inst Author: Omer-J-Cohen Author-email:
 omer.cohen@ibm.com Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE # Image Installer For IBM-VPC vpc-img-inst is a
 lightweight script for quick-and-dirty generation of custom VSI images by
 installing features (software bundles) on base images. ## Setup Mostly tested
```

### Comparing `vpc-img-inst-1.0.0b8/src/vpc_img_inst.egg-info/SOURCES.txt` & `vpc-img-inst-1.0.0b9/src/vpc_img_inst.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,13 +23,12 @@
 src/vpc_img_inst/config_modules/image_config.py
 src/vpc_img_inst/config_modules/image_create.py
 src/vpc_img_inst/config_modules/install_feature.py
 src/vpc_img_inst/config_modules/ip_config.py
 src/vpc_img_inst/config_modules/ssh_config.py
 src/vpc_img_inst/config_modules/vpc_config.py
 src/vpc_img_inst/config_modules/vsi_config.py
-src/vpc_img_inst/installation_scripts/cuda/install_cuda_rhel-8.sh
-src/vpc_img_inst/installation_scripts/cuda/install_cuda_ubuntu-20.sh
-src/vpc_img_inst/installation_scripts/cuda/install_cuda_ubuntu-22.sh
+src/vpc_img_inst/installation_scripts/cuda/install_cuda_rhel.sh
+src/vpc_img_inst/installation_scripts/cuda/install_cuda_ubuntu.sh
 src/vpc_img_inst/installation_scripts/docker/install_docker_rhel.sh
 src/vpc_img_inst/installation_scripts/docker/install_docker_ubuntu.sh
 src/vpc_img_inst/installation_scripts/ray/install_ray_ubuntu.sh
```

