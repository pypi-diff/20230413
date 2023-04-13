# Comparing `tmp/endgame-0.0.0.tar.gz` & `tmp/endgame-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/endgame-0.0.0.tar", last modified: Wed Feb 17 02:51:34 2021, max compression
+gzip compressed data, was "endgame-0.3.0.tar", last modified: Thu Apr 13 21:19:32 2023, max compression
```

## Comparing `endgame-0.0.0.tar` & `endgame-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,63 @@
-drwxr-xr-x   0 kmcquade   (502) staff       (20)        0 2021-02-17 02:51:34.952210 endgame-0.0.0/
--rw-r--r--   0 kmcquade   (502) staff       (20)      260 2021-02-17 02:51:34.951920 endgame-0.0.0/PKG-INFO
--rw-r--r--   0 kmcquade   (502) staff       (20)        4 2021-02-17 02:45:44.000000 endgame-0.0.0/README.md
-drwxr-xr-x   0 kmcquade   (502) staff       (20)        0 2021-02-17 02:51:34.951243 endgame-0.0.0/endgame.egg-info/
--rw-r--r--   0 kmcquade   (502) staff       (20)      260 2021-02-17 02:51:34.000000 endgame-0.0.0/endgame.egg-info/PKG-INFO
--rw-r--r--   0 kmcquade   (502) staff       (20)      168 2021-02-17 02:51:34.000000 endgame-0.0.0/endgame.egg-info/SOURCES.txt
--rw-r--r--   0 kmcquade   (502) staff       (20)        1 2021-02-17 02:51:34.000000 endgame-0.0.0/endgame.egg-info/dependency_links.txt
--rw-r--r--   0 kmcquade   (502) staff       (20)        1 2021-02-17 02:51:34.000000 endgame-0.0.0/endgame.egg-info/top_level.txt
--rw-r--r--   0 kmcquade   (502) staff       (20)        1 2021-02-17 02:45:33.000000 endgame-0.0.0/endgame.egg-info/zip-safe
--rw-r--r--   0 kmcquade   (502) staff       (20)       38 2021-02-17 02:51:34.952310 endgame-0.0.0/setup.cfg
--rw-r--r--   0 kmcquade   (502) staff       (20)      364 2021-02-17 02:50:20.000000 endgame-0.0.0/setup.py
+drwxr-xr-x   0 kmcquade   (501) staff       (20)        0 2023-04-13 21:19:32.496071 endgame-0.3.0/
+-rw-r--r--   0 kmcquade   (501) staff       (20)     1053 2023-04-13 21:15:45.000000 endgame-0.3.0/LICENSE
+-rw-r--r--   0 kmcquade   (501) staff       (20)    26541 2023-04-13 21:19:32.496614 endgame-0.3.0/PKG-INFO
+-rw-r--r--   0 kmcquade   (501) staff       (20)    25957 2023-04-13 21:15:45.000000 endgame-0.3.0/README.md
+drwxr-xr-x   0 kmcquade   (501) staff       (20)        0 2023-04-13 21:19:32.424393 endgame-0.3.0/endgame/
+-rw-r--r--   0 kmcquade   (501) staff       (20)     1908 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/__init__.py
+drwxr-xr-x   0 kmcquade   (501) staff       (20)        0 2023-04-13 21:19:32.432822 endgame-0.3.0/endgame/bin/
+-rw-r--r--   0 kmcquade   (501) staff       (20)        0 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/bin/__init__.py
+-rwxr-xr-x   0 kmcquade   (501) staff       (20)      794 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/bin/cli.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)       22 2023-04-13 21:19:19.000000 endgame-0.3.0/endgame/bin/version.py
+drwxr-xr-x   0 kmcquade   (501) staff       (20)        0 2023-04-13 21:19:32.438174 endgame-0.3.0/endgame/command/
+-rw-r--r--   0 kmcquade   (501) staff       (20)      112 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/command/__init__.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)    10663 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/command/expose.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     4287 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/command/list_resources.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     7335 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/command/smash.py
+drwxr-xr-x   0 kmcquade   (501) staff       (20)        0 2023-04-13 21:19:32.439463 endgame-0.3.0/endgame/exposure_via_aws_ram/
+-rw-r--r--   0 kmcquade   (501) staff       (20)        0 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_aws_ram/__init__.py
+drwxr-xr-x   0 kmcquade   (501) staff       (20)        0 2023-04-13 21:19:32.476509 endgame-0.3.0/endgame/exposure_via_resource_policies/
+-rw-r--r--   0 kmcquade   (501) staff       (20)        0 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/__init__.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)    10023 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/acm_pca.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)    10223 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/cloudwatch_logs.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     5467 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/common.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     4893 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/ecr.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     4761 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/efs.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     4762 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/elasticsearch.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     4767 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/glacier_vault.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     5023 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/iam.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     7804 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/kms.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     7371 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/lambda_function.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     9059 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/lambda_layer.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     4450 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/s3.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     4293 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/secrets_manager.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     7768 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/ses.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     9016 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/sns.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     9076 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_resource_policies/sqs.py
+drwxr-xr-x   0 kmcquade   (501) staff       (20)        0 2023-04-13 21:19:32.480788 endgame-0.3.0/endgame/exposure_via_sharing_apis/
+-rw-r--r--   0 kmcquade   (501) staff       (20)        0 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_sharing_apis/__init__.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     3435 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_sharing_apis/common.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)    10647 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_sharing_apis/ebs_snapshots.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)    10135 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_sharing_apis/ec2_amis.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     9215 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/exposure_via_sharing_apis/rds_snapshots.py
+drwxr-xr-x   0 kmcquade   (501) staff       (20)        0 2023-04-13 21:19:32.494925 endgame-0.3.0/endgame/shared/
+-rw-r--r--   0 kmcquade   (501) staff       (20)        0 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/shared/__init__.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     1574 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/shared/aws_login.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     1546 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/shared/constants.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)      543 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/shared/list_resources_response.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     7626 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/shared/policy_document.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)    13164 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/shared/resource_results.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     2489 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/shared/response_message.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     2909 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/shared/scary_warnings.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     5081 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/shared/statement_detail.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     5416 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/shared/utils.py
+-rw-r--r--   0 kmcquade   (501) staff       (20)     3216 2023-04-13 21:15:45.000000 endgame-0.3.0/endgame/shared/validate.py
+drwxr-xr-x   0 kmcquade   (501) staff       (20)        0 2023-04-13 21:19:32.430595 endgame-0.3.0/endgame.egg-info/
+-rw-r--r--   0 kmcquade   (501) staff       (20)    26541 2023-04-13 21:19:32.000000 endgame-0.3.0/endgame.egg-info/PKG-INFO
+-rw-r--r--   0 kmcquade   (501) staff       (20)     1934 2023-04-13 21:19:32.000000 endgame-0.3.0/endgame.egg-info/SOURCES.txt
+-rw-r--r--   0 kmcquade   (501) staff       (20)        1 2023-04-13 21:19:32.000000 endgame-0.3.0/endgame.egg-info/dependency_links.txt
+-rw-r--r--   0 kmcquade   (501) staff       (20)       49 2023-04-13 21:19:32.000000 endgame-0.3.0/endgame.egg-info/entry_points.txt
+-rw-r--r--   0 kmcquade   (501) staff       (20)       52 2023-04-13 21:19:32.000000 endgame-0.3.0/endgame.egg-info/requires.txt
+-rw-r--r--   0 kmcquade   (501) staff       (20)        8 2023-04-13 21:19:32.000000 endgame-0.3.0/endgame.egg-info/top_level.txt
+-rw-r--r--   0 kmcquade   (501) staff       (20)        1 2023-04-13 21:19:32.000000 endgame-0.3.0/endgame.egg-info/zip-safe
+-rw-r--r--   0 kmcquade   (501) staff       (20)      369 2023-04-13 21:19:32.514081 endgame-0.3.0/setup.cfg
+-rw-r--r--   0 kmcquade   (501) staff       (20)     1535 2023-04-13 21:15:45.000000 endgame-0.3.0/setup.py
```

