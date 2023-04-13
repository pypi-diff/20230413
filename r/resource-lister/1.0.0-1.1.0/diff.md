# Comparing `tmp/resource-lister-1.0.0.tar.gz` & `tmp/resource-lister-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Abhijit\AWS\GIT-Publishing\repository\resource-lister\dist\.tmp-tntdplej\resource-lister-1.0.0.tar", last modified: Thu Apr 13 01:32:01 2023, max compression
+gzip compressed data, was "C:\Abhijit\AWS\GIT-Publishing\repository\resource-lister\dist\.tmp-suubc6e6\resource-lister-1.1.0.tar", last modified: Thu Apr 13 03:08:47 2023, max compression
```

## Comparing `resource-lister-1.0.0.tar` & `resource-lister-1.1.0.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 01:32:01.825929 resource-lister-1.0.0/
--rw-rw-rw-   0        0        0    11525 2023-03-20 16:57:45.000000 resource-lister-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      122 2023-02-18 03:26:18.000000 resource-lister-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0       68 2023-04-11 18:33:31.000000 resource-lister-1.0.0/NOTICE
--rw-rw-rw-   0        0        0    10284 2023-04-13 01:32:01.818138 resource-lister-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     9724 2023-04-12 19:06:59.000000 resource-lister-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 01:32:01.406422 resource-lister-1.0.0/cfn/
--rw-rw-rw-   0        0        0     4006 2023-03-03 17:37:23.000000 resource-lister-1.0.0/cfn/cfn_s3_bucket_master_account.json
--rw-rw-rw-   0        0        0     3949 2023-03-03 03:24:49.000000 resource-lister-1.0.0/cfn/master_account_IAM_role.json
--rw-rw-rw-   0        0        0      688 2023-04-12 16:22:33.000000 resource-lister-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 01:32:01.826665 resource-lister-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 01:32:01.320850 resource-lister-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 01:32:01.424207 resource-lister-1.0.0/src/resource_lister/
--rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.0.0/src/resource_lister/__init__.py
--rw-rw-rw-   0        0        0       64 2023-03-25 17:10:45.000000 resource-lister-1.0.0/src/resource_lister/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:32:01.465531 resource-lister-1.0.0/src/resource_lister/boto_formatter/
--rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/__init__.py
--rw-rw-rw-   0        0        0     7595 2023-02-27 03:30:46.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/core_formatter.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:32:01.473558 resource-lister-1.0.0/src/resource_lister/boto_formatter/json_util/
--rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/json_util/__init__.py
--rw-rw-rw-   0        0        0    10769 2023-01-30 03:32:28.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/json_util/json_util.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:32:01.485513 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/
--rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/__init__.py
--rw-rw-rw-   0        0        0     5848 2022-12-29 03:55:50.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_config.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:32:01.648465 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/
--rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/__init__.py
--rw-rw-rw-   0        0        0     2064 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/accessanalyzer.json
--rw-rw-rw-   0        0        0     1086 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/apigateway.json
--rw-rw-rw-   0        0        0     2104 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/budgets.json
--rw-rw-rw-   0        0        0     1037 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudformation.json
--rw-rw-rw-   0        0        0    10697 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudfront.json
--rw-rw-rw-   0        0        0      623 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudtrail.json
--rw-rw-rw-   0        0        0     1350 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudwatch.json
--rw-rw-rw-   0        0        0      643 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/codecommit.json
--rw-rw-rw-   0        0        0       73 2023-01-27 22:09:30.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/describe_cache_clusters.json
--rw-rw-rw-   0        0        0      555 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/dynamodb.json
--rw-rw-rw-   0        0        0    34336 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ec2.json
--rw-rw-rw-   0        0        0     1510 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ecs.json
--rw-rw-rw-   0        0        0     1464 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/efs.json
--rw-rw-rw-   0        0        0     3576 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/eks.json
--rw-rw-rw-   0        0        0     4475 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elasticache.json
--rw-rw-rw-   0        0        0     1594 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elbv2.json
--rw-rw-rw-   0        0        0     1795 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr-serverless.json
--rw-rw-rw-   0        0        0     5490 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr.json
--rw-rw-rw-   0        0        0     7276 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/iam.json
--rw-rw-rw-   0        0        0      585 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/kms.json
--rw-rw-rw-   0        0        0     3425 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/lambda.json
--rw-rw-rw-   0        0        0     1447 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/organizations.json
--rw-rw-rw-   0        0        0    17897 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/rds.json
--rw-rw-rw-   0        0        0     2630 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift-serverless.json
--rw-rw-rw-   0        0        0     7405 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift.json
--rw-rw-rw-   0        0        0     3129 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53.json
--rw-rw-rw-   0        0        0     1753 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53domains.json
--rw-rw-rw-   0        0        0     2526 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/s3.json
--rw-rw-rw-   0        0        0     3480 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sagemaker.json
--rw-rw-rw-   0        0        0     1212 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sns.json
--rw-rw-rw-   0        0        0      548 2023-03-13 03:17:54.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sqs.json
--rw-rw-rw-   0        0        0     7440 2023-02-27 03:30:45.000000 resource-lister-1.0.0/src/resource_lister/boto_formatter/service_formatter.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:32:01.671481 resource-lister-1.0.0/src/resource_lister/config_mgr/
--rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.0.0/src/resource_lister/config_mgr/__init__.py
--rw-rw-rw-   0        0        0      129 2023-02-21 16:45:05.000000 resource-lister-1.0.0/src/resource_lister/config_mgr/config.json
--rw-rw-rw-   0        0        0     4276 2023-03-22 01:14:18.000000 resource-lister-1.0.0/src/resource_lister/config_mgr/config_menu_processor.py
--rw-rw-rw-   0        0        0     2264 2023-03-22 01:14:33.000000 resource-lister-1.0.0/src/resource_lister/config_mgr/config_util.py
--rw-rw-rw-   0        0        0      103 2023-03-25 16:15:33.000000 resource-lister-1.0.0/src/resource_lister/main.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:32:01.707586 resource-lister-1.0.0/src/resource_lister/menu/
--rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.0.0/src/resource_lister/menu/__init__.py
--rw-rw-rw-   0        0        0     3888 2023-03-22 01:19:46.000000 resource-lister-1.0.0/src/resource_lister/menu/batch_processing.py
--rw-rw-rw-   0        0        0    34834 2023-03-13 03:36:33.000000 resource-lister-1.0.0/src/resource_lister/menu/menu_config.json
--rw-rw-rw-   0        0        0    12825 2023-04-12 16:26:38.000000 resource-lister-1.0.0/src/resource_lister/menu/menu_processor.py
--rw-rw-rw-   0        0        0     6134 2023-03-14 16:30:15.000000 resource-lister-1.0.0/src/resource_lister/menu/menu_util.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:32:01.755180 resource-lister-1.0.0/src/resource_lister/processor/
--rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.0.0/src/resource_lister/processor/__init__.py
--rw-rw-rw-   0        0        0     3635 2023-03-22 01:23:29.000000 resource-lister-1.0.0/src/resource_lister/processor/_global_no_paginate.py
--rw-rw-rw-   0        0        0     3771 2023-02-27 03:30:43.000000 resource-lister-1.0.0/src/resource_lister/processor/_global_paginate.py
--rw-rw-rw-   0        0        0     4502 2023-02-27 04:04:32.000000 resource-lister-1.0.0/src/resource_lister/processor/_regional_no_paginate.py
--rw-rw-rw-   0        0        0     4877 2023-02-27 04:06:31.000000 resource-lister-1.0.0/src/resource_lister/processor/_regional_paginate.py
--rw-rw-rw-   0        0        0      426 2023-03-22 01:21:21.000000 resource-lister-1.0.0/src/resource_lister/processor/core_processor.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:32:01.779303 resource-lister-1.0.0/src/resource_lister/session_mgr/
--rw-rw-rw-   0        0        0        0 2023-01-25 16:19:16.000000 resource-lister-1.0.0/src/resource_lister/session_mgr/__init__.py
--rw-rw-rw-   0        0        0      242 2023-04-11 14:46:14.000000 resource-lister-1.0.0/src/resource_lister/session_mgr/account_config.json
--rw-rw-rw-   0        0        0     8919 2023-04-11 14:55:49.000000 resource-lister-1.0.0/src/resource_lister/session_mgr/account_config_util.py
--rw-rw-rw-   0        0        0     4805 2023-04-11 15:24:28.000000 resource-lister-1.0.0/src/resource_lister/session_mgr/accounts_menu_processor.py
--rw-rw-rw-   0        0        0    10969 2023-04-11 15:22:16.000000 resource-lister-1.0.0/src/resource_lister/session_mgr/iam_session_mgr.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:32:01.808811 resource-lister-1.0.0/src/resource_lister/util/
--rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.0.0/src/resource_lister/util/__init__.py
--rw-rw-rw-   0        0        0     7075 2023-04-11 14:42:54.000000 resource-lister-1.0.0/src/resource_lister/util/menu_configs.py
--rw-rw-rw-   0        0        0     9176 2023-03-23 14:48:06.000000 resource-lister-1.0.0/src/resource_lister/util/menu_util.py
--rw-rw-rw-   0        0        0      231 2023-03-23 13:53:26.000000 resource-lister-1.0.0/src/resource_lister/util/resource_lister_exceptions.py
--rw-rw-rw-   0        0        0     2297 2023-04-11 13:25:41.000000 resource-lister-1.0.0/src/resource_lister/util/s3_util.py
--rw-rw-rw-   0        0        0     1264 2023-04-11 15:21:36.000000 resource-lister-1.0.0/src/resource_lister/util/session_util.py
--rw-rw-rw-   0        0        0      670 2023-02-24 02:30:16.000000 resource-lister-1.0.0/src/resource_lister/util/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:32:01.445328 resource-lister-1.0.0/src/resource_lister.egg-info/
--rw-rw-rw-   0        0        0    10284 2023-04-13 01:32:01.000000 resource-lister-1.0.0/src/resource_lister.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4769 2023-04-13 01:32:01.000000 resource-lister-1.0.0/src/resource_lister.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 01:32:01.000000 resource-lister-1.0.0/src/resource_lister.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-04-13 01:32:01.000000 resource-lister-1.0.0/src/resource_lister.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 01:32:01.000000 resource-lister-1.0.0/src/resource_lister.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.482880 resource-lister-1.1.0/
+-rw-rw-rw-   0        0        0    11525 2023-03-20 16:57:45.000000 resource-lister-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      122 2023-02-18 03:26:18.000000 resource-lister-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0       68 2023-04-11 18:33:31.000000 resource-lister-1.1.0/NOTICE
+-rw-rw-rw-   0        0        0    10284 2023-04-13 03:08:47.477078 resource-lister-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9724 2023-04-12 19:06:59.000000 resource-lister-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 03:08:46.892903 resource-lister-1.1.0/cfn/
+-rw-rw-rw-   0        0        0     4006 2023-03-03 17:37:23.000000 resource-lister-1.1.0/cfn/cfn_s3_bucket_master_account.json
+-rw-rw-rw-   0        0        0     3949 2023-03-03 03:24:49.000000 resource-lister-1.1.0/cfn/master_account_IAM_role.json
+-rw-rw-rw-   0        0        0      732 2023-04-13 02:53:53.000000 resource-lister-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 03:08:47.484486 resource-lister-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 03:08:46.865393 resource-lister-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 03:08:46.901448 resource-lister-1.1.0/src/resource_lister/
+-rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.1.0/src/resource_lister/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-03-25 17:10:45.000000 resource-lister-1.1.0/src/resource_lister/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:08:46.975969 resource-lister-1.1.0/src/resource_lister/boto_formatter/
+-rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/__init__.py
+-rw-rw-rw-   0        0        0     7595 2023-02-27 03:30:46.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/core_formatter.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:08:46.990001 resource-lister-1.1.0/src/resource_lister/boto_formatter/json_util/
+-rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/json_util/__init__.py
+-rw-rw-rw-   0        0        0    10769 2023-01-30 03:32:28.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/json_util/json_util.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.006600 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/
+-rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/__init__.py
+-rw-rw-rw-   0        0        0     5848 2022-12-29 03:55:50.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_config.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.281917 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/
+-rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/__init__.py
+-rw-rw-rw-   0        0        0     2064 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/accessanalyzer.json
+-rw-rw-rw-   0        0        0     1086 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/apigateway.json
+-rw-rw-rw-   0        0        0     2104 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/budgets.json
+-rw-rw-rw-   0        0        0     1037 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudformation.json
+-rw-rw-rw-   0        0        0    10697 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudfront.json
+-rw-rw-rw-   0        0        0      623 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudtrail.json
+-rw-rw-rw-   0        0        0     1350 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudwatch.json
+-rw-rw-rw-   0        0        0      643 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/codecommit.json
+-rw-rw-rw-   0        0        0       73 2023-01-27 22:09:30.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/describe_cache_clusters.json
+-rw-rw-rw-   0        0        0      555 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/dynamodb.json
+-rw-rw-rw-   0        0        0    34336 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ec2.json
+-rw-rw-rw-   0        0        0     1510 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ecs.json
+-rw-rw-rw-   0        0        0     1464 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/efs.json
+-rw-rw-rw-   0        0        0     3576 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/eks.json
+-rw-rw-rw-   0        0        0     4475 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elasticache.json
+-rw-rw-rw-   0        0        0     1594 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elbv2.json
+-rw-rw-rw-   0        0        0     1795 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr-serverless.json
+-rw-rw-rw-   0        0        0     5490 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr.json
+-rw-rw-rw-   0        0        0     7276 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/iam.json
+-rw-rw-rw-   0        0        0      585 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/kms.json
+-rw-rw-rw-   0        0        0     3425 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/lambda.json
+-rw-rw-rw-   0        0        0     1447 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/organizations.json
+-rw-rw-rw-   0        0        0    17897 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/rds.json
+-rw-rw-rw-   0        0        0     2630 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift-serverless.json
+-rw-rw-rw-   0        0        0     7405 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift.json
+-rw-rw-rw-   0        0        0     3129 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53.json
+-rw-rw-rw-   0        0        0     1753 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53domains.json
+-rw-rw-rw-   0        0        0     2526 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/s3.json
+-rw-rw-rw-   0        0        0     3480 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sagemaker.json
+-rw-rw-rw-   0        0        0     1212 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sns.json
+-rw-rw-rw-   0        0        0      548 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sqs.json
+-rw-rw-rw-   0        0        0     7440 2023-02-27 03:30:45.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_formatter.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.305704 resource-lister-1.1.0/src/resource_lister/config_mgr/
+-rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.1.0/src/resource_lister/config_mgr/__init__.py
+-rw-rw-rw-   0        0        0      129 2023-02-21 16:45:05.000000 resource-lister-1.1.0/src/resource_lister/config_mgr/config.json
+-rw-rw-rw-   0        0        0     4276 2023-03-22 01:14:18.000000 resource-lister-1.1.0/src/resource_lister/config_mgr/config_menu_processor.py
+-rw-rw-rw-   0        0        0     2264 2023-03-22 01:14:33.000000 resource-lister-1.1.0/src/resource_lister/config_mgr/config_util.py
+-rw-rw-rw-   0        0        0      103 2023-03-25 16:15:33.000000 resource-lister-1.1.0/src/resource_lister/main.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.341962 resource-lister-1.1.0/src/resource_lister/menu/
+-rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.1.0/src/resource_lister/menu/__init__.py
+-rw-rw-rw-   0        0        0     3888 2023-03-22 01:19:46.000000 resource-lister-1.1.0/src/resource_lister/menu/batch_processing.py
+-rw-rw-rw-   0        0        0    34834 2023-03-13 03:36:33.000000 resource-lister-1.1.0/src/resource_lister/menu/menu_config.json
+-rw-rw-rw-   0        0        0    12825 2023-04-12 16:26:38.000000 resource-lister-1.1.0/src/resource_lister/menu/menu_processor.py
+-rw-rw-rw-   0        0        0     6134 2023-03-14 16:30:15.000000 resource-lister-1.1.0/src/resource_lister/menu/menu_util.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.379737 resource-lister-1.1.0/src/resource_lister/processor/
+-rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.1.0/src/resource_lister/processor/__init__.py
+-rw-rw-rw-   0        0        0     3635 2023-03-22 01:23:29.000000 resource-lister-1.1.0/src/resource_lister/processor/_global_no_paginate.py
+-rw-rw-rw-   0        0        0     3771 2023-02-27 03:30:43.000000 resource-lister-1.1.0/src/resource_lister/processor/_global_paginate.py
+-rw-rw-rw-   0        0        0     4502 2023-02-27 04:04:32.000000 resource-lister-1.1.0/src/resource_lister/processor/_regional_no_paginate.py
+-rw-rw-rw-   0        0        0     4877 2023-02-27 04:06:31.000000 resource-lister-1.1.0/src/resource_lister/processor/_regional_paginate.py
+-rw-rw-rw-   0        0        0      426 2023-03-22 01:21:21.000000 resource-lister-1.1.0/src/resource_lister/processor/core_processor.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.419504 resource-lister-1.1.0/src/resource_lister/session_mgr/
+-rw-rw-rw-   0        0        0        0 2023-01-25 16:19:16.000000 resource-lister-1.1.0/src/resource_lister/session_mgr/__init__.py
+-rw-rw-rw-   0        0        0      242 2023-04-11 14:46:14.000000 resource-lister-1.1.0/src/resource_lister/session_mgr/account_config.json
+-rw-rw-rw-   0        0        0     8919 2023-04-11 14:55:49.000000 resource-lister-1.1.0/src/resource_lister/session_mgr/account_config_util.py
+-rw-rw-rw-   0        0        0     4805 2023-04-11 15:24:28.000000 resource-lister-1.1.0/src/resource_lister/session_mgr/accounts_menu_processor.py
+-rw-rw-rw-   0        0        0    10969 2023-04-11 15:22:16.000000 resource-lister-1.1.0/src/resource_lister/session_mgr/iam_session_mgr.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.468175 resource-lister-1.1.0/src/resource_lister/util/
+-rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.1.0/src/resource_lister/util/__init__.py
+-rw-rw-rw-   0        0        0     7075 2023-04-11 14:42:54.000000 resource-lister-1.1.0/src/resource_lister/util/menu_configs.py
+-rw-rw-rw-   0        0        0     9176 2023-03-23 14:48:06.000000 resource-lister-1.1.0/src/resource_lister/util/menu_util.py
+-rw-rw-rw-   0        0        0      231 2023-03-23 13:53:26.000000 resource-lister-1.1.0/src/resource_lister/util/resource_lister_exceptions.py
+-rw-rw-rw-   0        0        0     2297 2023-04-11 13:25:41.000000 resource-lister-1.1.0/src/resource_lister/util/s3_util.py
+-rw-rw-rw-   0        0        0     1264 2023-04-11 15:21:36.000000 resource-lister-1.1.0/src/resource_lister/util/session_util.py
+-rw-rw-rw-   0        0        0      670 2023-02-24 02:30:16.000000 resource-lister-1.1.0/src/resource_lister/util/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:08:46.943965 resource-lister-1.1.0/src/resource_lister.egg-info/
+-rw-rw-rw-   0        0        0    10284 2023-04-13 03:08:46.000000 resource-lister-1.1.0/src/resource_lister.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4811 2023-04-13 03:08:46.000000 resource-lister-1.1.0/src/resource_lister.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 03:08:46.000000 resource-lister-1.1.0/src/resource_lister.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-04-13 03:08:46.000000 resource-lister-1.1.0/src/resource_lister.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-04-13 03:08:46.000000 resource-lister-1.1.0/src/resource_lister.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-13 03:08:46.000000 resource-lister-1.1.0/src/resource_lister.egg-info/top_level.txt
```

### Comparing `resource-lister-1.0.0/LICENSE` & `resource-lister-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/PKG-INFO` & `resource-lister-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resource-lister
-Version: 1.0.0
+Version: 1.1.0
 Summary: Resource Lister
 Author-email: Abhijit Rajeshirke <rajeabh@amazon.com>
 Project-URL: Homepage, https://github.com/awslabs/resource-lister
 Project-URL: Bug Tracker, https://github.com/awslabs/resource-lister/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `resource-lister-1.0.0/README.md` & `resource-lister-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/cfn/cfn_s3_bucket_master_account.json` & `resource-lister-1.1.0/cfn/cfn_s3_bucket_master_account.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/cfn/master_account_IAM_role.json` & `resource-lister-1.1.0/cfn/master_account_IAM_role.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/pyproject.toml` & `resource-lister-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "resource-lister"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Abhijit Rajeshirke", email="rajeabh@amazon.com" },
 ]
 description = "Resource Lister"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
+dependencies = [
+    "boto3>=1.15.0"
+]
+
 [project.scripts]
 resource_lister = "resource_lister.main:main"
 
 [project.urls]
 "Homepage" = "https://github.com/awslabs/resource-lister"
 "Bug Tracker" = "https://github.com/awslabs/resource-lister/issues"
```

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/core_formatter.py` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/core_formatter.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/json_util/json_util.py` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/json_util/json_util.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_config.py` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_config.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/accessanalyzer.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/accessanalyzer.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/apigateway.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/apigateway.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/budgets.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/budgets.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudformation.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudformation.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudfront.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudfront.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudtrail.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudtrail.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudwatch.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudwatch.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/codecommit.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/codecommit.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/dynamodb.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/dynamodb.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ec2.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ec2.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ecs.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ecs.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/efs.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/efs.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/eks.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/eks.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elasticache.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elasticache.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elbv2.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elbv2.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr-serverless.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr-serverless.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/iam.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/iam.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/kms.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/kms.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/lambda.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/lambda.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/organizations.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/organizations.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/rds.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/rds.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift-serverless.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift-serverless.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53domains.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53domains.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/s3.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/s3.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sagemaker.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sagemaker.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sns.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sns.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sqs.json` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sqs.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/boto_formatter/service_formatter.py` & `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_formatter.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/config_mgr/config_menu_processor.py` & `resource-lister-1.1.0/src/resource_lister/config_mgr/config_menu_processor.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/config_mgr/config_util.py` & `resource-lister-1.1.0/src/resource_lister/config_mgr/config_util.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/menu/batch_processing.py` & `resource-lister-1.1.0/src/resource_lister/menu/batch_processing.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/menu/menu_config.json` & `resource-lister-1.1.0/src/resource_lister/menu/menu_config.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/menu/menu_processor.py` & `resource-lister-1.1.0/src/resource_lister/menu/menu_processor.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/menu/menu_util.py` & `resource-lister-1.1.0/src/resource_lister/menu/menu_util.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/processor/_global_no_paginate.py` & `resource-lister-1.1.0/src/resource_lister/processor/_global_no_paginate.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/processor/_global_paginate.py` & `resource-lister-1.1.0/src/resource_lister/processor/_global_paginate.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/processor/_regional_no_paginate.py` & `resource-lister-1.1.0/src/resource_lister/processor/_regional_no_paginate.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/processor/_regional_paginate.py` & `resource-lister-1.1.0/src/resource_lister/processor/_regional_paginate.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/session_mgr/account_config_util.py` & `resource-lister-1.1.0/src/resource_lister/session_mgr/account_config_util.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/session_mgr/accounts_menu_processor.py` & `resource-lister-1.1.0/src/resource_lister/session_mgr/accounts_menu_processor.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/session_mgr/iam_session_mgr.py` & `resource-lister-1.1.0/src/resource_lister/session_mgr/iam_session_mgr.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/util/menu_configs.py` & `resource-lister-1.1.0/src/resource_lister/util/menu_configs.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/util/menu_util.py` & `resource-lister-1.1.0/src/resource_lister/util/menu_util.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/util/s3_util.py` & `resource-lister-1.1.0/src/resource_lister/util/s3_util.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/util/session_util.py` & `resource-lister-1.1.0/src/resource_lister/util/session_util.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister/util/setup.py` & `resource-lister-1.1.0/src/resource_lister/util/setup.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.0.0/src/resource_lister.egg-info/PKG-INFO` & `resource-lister-1.1.0/src/resource_lister.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resource-lister
-Version: 1.0.0
+Version: 1.1.0
 Summary: Resource Lister
 Author-email: Abhijit Rajeshirke <rajeabh@amazon.com>
 Project-URL: Homepage, https://github.com/awslabs/resource-lister
 Project-URL: Bug Tracker, https://github.com/awslabs/resource-lister/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `resource-lister-1.0.0/src/resource_lister.egg-info/SOURCES.txt` & `resource-lister-1.1.0/src/resource_lister.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/resource_lister/__init__.py
 src/resource_lister/__main__.py
 src/resource_lister/main.py
 src/resource_lister.egg-info/PKG-INFO
 src/resource_lister.egg-info/SOURCES.txt
 src/resource_lister.egg-info/dependency_links.txt
 src/resource_lister.egg-info/entry_points.txt
+src/resource_lister.egg-info/requires.txt
 src/resource_lister.egg-info/top_level.txt
 src/resource_lister/boto_formatter/__init__.py
 src/resource_lister/boto_formatter/core_formatter.py
 src/resource_lister/boto_formatter/service_formatter.py
 src/resource_lister/boto_formatter/json_util/__init__.py
 src/resource_lister/boto_formatter/json_util/json_util.py
 src/resource_lister/boto_formatter/service_config_mgr/__init__.py
```

