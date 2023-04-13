# Comparing `tmp/cis_checks_2023-2.0.6.tar.gz` & `tmp/cis_checks_2023-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cis_checks_2023-2.0.6.tar", last modified: Thu Apr 13 08:31:14 2023, max compression
+gzip compressed data, was "cis_checks_2023-2.0.7.tar", last modified: Thu Apr 13 09:07:27 2023, max compression
```

## Comparing `cis_checks_2023-2.0.6.tar` & `cis_checks_2023-2.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 08:31:14.695237 cis_checks_2023-2.0.6/
--rw-rw-rw-   0        0        0      836 2023-04-13 08:31:14.693260 cis_checks_2023-2.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 cis_checks_2023-2.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 08:31:14.673590 cis_checks_2023-2.0.6/cis_checks_2023/
--rw-rw-rw-   0        0        0     6851 2023-04-13 08:30:38.000000 cis_checks_2023-2.0.6/cis_checks_2023/__init__.py
--rw-rw-rw-   0        0        0    35333 2023-04-07 14:21:10.000000 cis_checks_2023-2.0.6/cis_checks_2023/_security_control_5.py
--rw-rw-rw-   0        0        0    54565 2023-04-12 14:37:06.000000 cis_checks_2023-2.0.6/cis_checks_2023/iam_control_1.py
--rw-rw-rw-   0        0        0    25256 2023-04-13 06:34:22.000000 cis_checks_2023-2.0.6/cis_checks_2023/logging_control_3.py
--rw-rw-rw-   0        0        0    79813 2023-04-11 05:42:02.000000 cis_checks_2023-2.0.6/cis_checks_2023/monitoring_control_4.py
--rw-rw-rw-   0        0        0    25055 2023-04-11 07:00:11.000000 cis_checks_2023-2.0.6/cis_checks_2023/networking_control_5.py
--rw-rw-rw-   0        0        0    15823 2023-04-13 07:08:22.000000 cis_checks_2023-2.0.6/cis_checks_2023/storage_control_2.py
--rw-rw-rw-   0        0        0    21541 2023-04-13 07:03:52.000000 cis_checks_2023-2.0.6/cis_checks_2023/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:31:14.689081 cis_checks_2023-2.0.6/cis_checks_2023.egg-info/
--rw-rw-rw-   0        0        0      836 2023-04-13 08:31:14.000000 cis_checks_2023-2.0.6/cis_checks_2023.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-04-13 08:31:14.000000 cis_checks_2023-2.0.6/cis_checks_2023.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 08:31:14.000000 cis_checks_2023-2.0.6/cis_checks_2023.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 08:31:14.000000 cis_checks_2023-2.0.6/cis_checks_2023.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      557 2023-04-13 08:30:38.000000 cis_checks_2023-2.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 08:31:14.696230 cis_checks_2023-2.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 09:07:27.047910 cis_checks_2023-2.0.7/
+-rw-rw-rw-   0        0        0      836 2023-04-13 09:07:27.046409 cis_checks_2023-2.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 cis_checks_2023-2.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 09:07:27.013757 cis_checks_2023-2.0.7/cis_checks_2023/
+-rw-rw-rw-   0        0        0     6897 2023-04-13 09:06:51.000000 cis_checks_2023-2.0.7/cis_checks_2023/__init__.py
+-rw-rw-rw-   0        0        0    35333 2023-04-07 14:21:10.000000 cis_checks_2023-2.0.7/cis_checks_2023/_security_control_5.py
+-rw-rw-rw-   0        0        0    54565 2023-04-12 14:37:06.000000 cis_checks_2023-2.0.7/cis_checks_2023/iam_control_1.py
+-rw-rw-rw-   0        0        0    25256 2023-04-13 06:34:22.000000 cis_checks_2023-2.0.7/cis_checks_2023/logging_control_3.py
+-rw-rw-rw-   0        0        0    79813 2023-04-11 05:42:02.000000 cis_checks_2023-2.0.7/cis_checks_2023/monitoring_control_4.py
+-rw-rw-rw-   0        0        0    25055 2023-04-11 07:00:11.000000 cis_checks_2023-2.0.7/cis_checks_2023/networking_control_5.py
+-rw-rw-rw-   0        0        0    16019 2023-04-13 09:03:31.000000 cis_checks_2023-2.0.7/cis_checks_2023/storage_control_2.py
+-rw-rw-rw-   0        0        0    21541 2023-04-13 07:03:52.000000 cis_checks_2023-2.0.7/cis_checks_2023/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:07:27.039382 cis_checks_2023-2.0.7/cis_checks_2023.egg-info/
+-rw-rw-rw-   0        0        0      836 2023-04-13 09:07:26.000000 cis_checks_2023-2.0.7/cis_checks_2023.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-04-13 09:07:26.000000 cis_checks_2023-2.0.7/cis_checks_2023.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 09:07:26.000000 cis_checks_2023-2.0.7/cis_checks_2023.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-13 09:07:26.000000 cis_checks_2023-2.0.7/cis_checks_2023.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      557 2023-04-13 09:06:51.000000 cis_checks_2023-2.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 09:07:27.048910 cis_checks_2023-2.0.7/setup.cfg
```

### Comparing `cis_checks_2023-2.0.6/PKG-INFO` & `cis_checks_2023-2.0.7/cis_checks_2023.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cis_checks_2023
-Version: 2.0.6
+Name: cis-checks-2023
+Version: 2.0.7
 Summary: Provides AWS compliance details
 Author-email: Dheeraj Banodha <dheeraj.banodha@impetus.com>, Ravish Sharma <ravish.sharma@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cis_checks_2023-2.0.6/cis_checks_2023/__init__.py` & `cis_checks_2023-2.0.7/cis_checks_2023/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from cis_checks_2023.iam_control_1 import iam_control
 
 logging.basicConfig()
 logging.getLogger().setLevel(logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Dheeraj Banodha'
-__version__ = '2.0.6'
+__version__ = '2.0.7'
 
 
 class aws_client(iam_control, utils, storage_control, logging_control, monitoring_control, networking_control):
     def __init__(self, **kwargs):
         """
         @param str aws_access_key_id: AWS Access Key ID
         @param str aws_secret_access_key: AWS Secret Access Key
@@ -46,40 +46,40 @@
         password_policy = self.get_account_password_policy()
         s3_buckets = self.list_s3_buckets()
         rds_instances = self.list_rds_instances(regions)
 
         compliance = [
             # iam_control_1
 
-            self.control_1_01_maintain_contact_details(),
-            self.control_1_02_security_contact_information_registered(),
-            self.control_1_03_security_questions_registered(),
-            self.control_1_04_root_key_exists(creds_report),
-            self.control_1_05_root_mfa_enabled(),
-            self.control_1_06_root_hardware_mfa_enabled(),
-            self.control_1_07_root_use(creds_report),
-            self.control_1_08_password_policy_length(password_policy),
-            self.control_1_09_password_policy_reuse(password_policy),
-            self.control_1_10_mfa_on_password_enabled_iam(creds_report),
-            self.control_1_11_no_accesskey_on_initial_setup(creds_report),
-            self.control_1_12_unused_credentials(creds_report),
-            self.control_1_13_one_active_key(creds_report),
-            self.control_1_14_ensure_access_keys_are_rotated_90_days(),
-            self.control_1_15_no_policies_on_iam_users(),
-            self.control_1_16_no_policies_with_full_administrative_privileges(),
-            self.control_1_17_AWS_support_role_created(),
-            self.control_1_18_iam_instance_role_for_access_from_instances(),
-            self.control_1_19_expired_ssl_tls_certificates_removed(regions),
-            self.control_1_2_iam_access_analyzer_enabled(regions),
-            self.control_1_21_iam_user_managed_centrally(),
+            # self.control_1_01_maintain_contact_details(),
+            # self.control_1_02_security_contact_information_registered(),
+            # self.control_1_03_security_questions_registered(),
+            # self.control_1_04_root_key_exists(creds_report),
+            # self.control_1_05_root_mfa_enabled(),
+            # self.control_1_06_root_hardware_mfa_enabled(),
+            # self.control_1_07_root_use(creds_report),
+            # self.control_1_08_password_policy_length(password_policy),
+            # self.control_1_09_password_policy_reuse(password_policy),
+            # self.control_1_10_mfa_on_password_enabled_iam(creds_report),
+            # self.control_1_11_no_accesskey_on_initial_setup(creds_report),
+            # self.control_1_12_unused_credentials(creds_report),
+            # self.control_1_13_one_active_key(creds_report),
+            # self.control_1_14_ensure_access_keys_are_rotated_90_days(),
+            # self.control_1_15_no_policies_on_iam_users(),
+            # self.control_1_16_no_policies_with_full_administrative_privileges(),
+            # self.control_1_17_AWS_support_role_created(),
+            # self.control_1_18_iam_instance_role_for_access_from_instances(),
+            # self.control_1_19_expired_ssl_tls_certificates_removed(regions),
+            # self.control_1_2_iam_access_analyzer_enabled(regions),
+            # self.control_1_21_iam_user_managed_centrally(),
 
             # storage_control_2
 
-            self.control_2_1_1_s3_default_encryption_at_rest(s3_buckets),
-            self.control_2_1_2_s3_deny_http_requests(s3_buckets),
+            # self.control_2_1_1_s3_default_encryption_at_rest(s3_buckets),
+            # self.control_2_1_2_s3_deny_http_requests(s3_buckets),
             self.control_2_1_3_s3_mfa_delete_enabled(s3_buckets),
             self.control_2_1_4_ensure_all_data_discovered_classified_secured(),
             self.control_2_1_5_s3_blocks_public_access(s3_buckets),
             self.control_2_2_1_ebs_volumes_encrypted(regions),
             self.control_2_3_1_rds_encryption_enabled(rds_instances),
             self.control_2_3_2_rds_auto_minor_version_upgrade_enabled(rds_instances),
             self.control_2_3_3_rds_publicly_accessible(rds_instances),
```

### Comparing `cis_checks_2023-2.0.6/cis_checks_2023/_security_control_5.py` & `cis_checks_2023-2.0.7/cis_checks_2023/_security_control_5.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.6/cis_checks_2023/iam_control_1.py` & `cis_checks_2023-2.0.7/cis_checks_2023/iam_control_1.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.6/cis_checks_2023/logging_control_3.py` & `cis_checks_2023-2.0.7/cis_checks_2023/logging_control_3.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.6/cis_checks_2023/monitoring_control_4.py` & `cis_checks_2023-2.0.7/cis_checks_2023/monitoring_control_4.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.6/cis_checks_2023/networking_control_5.py` & `cis_checks_2023-2.0.7/cis_checks_2023/networking_control_5.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.6/cis_checks_2023/storage_control_2.py` & `cis_checks_2023-2.0.7/cis_checks_2023/storage_control_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """storage_control_2.py"""
-
-import botocore.errorfactory
-import botocore.exceptions
+from botocore.exceptions import ClientError
 
 from cis_checks_2023.utils import *
 
 global logger
 logging.basicConfig(level=logging.INFO)
 
 
@@ -146,14 +144,19 @@
                 )
                 mfa_delete = resp['MFADelete']
             except KeyError:
                 result = "Not Compliant"
                 failReason = "Either bucket versioning is not enabled or configuration not found"
                 offenders.append(bucket_name)
                 continue
+            except ClientError as e:
+                result = "Not Compliant"
+                failReason = e.response['Error']['Code']
+                offenders.append(bucket_name)
+                continue
 
             if not mfa_delete == 'Enabled':
                 result = "Not Compliant"
                 failReason = "MFA Delete is not enabled on S3 buckets"
                 offenders.append(bucket_name)
 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
```

### Comparing `cis_checks_2023-2.0.6/cis_checks_2023/utils.py` & `cis_checks_2023-2.0.7/cis_checks_2023/utils.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.6/cis_checks_2023.egg-info/PKG-INFO` & `cis_checks_2023-2.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cis-checks-2023
-Version: 2.0.6
+Name: cis_checks_2023
+Version: 2.0.7
 Summary: Provides AWS compliance details
 Author-email: Dheeraj Banodha <dheeraj.banodha@impetus.com>, Ravish Sharma <ravish.sharma@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cis_checks_2023-2.0.6/pyproject.toml` & `cis_checks_2023-2.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "cis_checks_2023"
-version = "2.0.6"
+version = "2.0.7"
 authors = [
   { name="Dheeraj Banodha", email="dheeraj.banodha@impetus.com" },
   { name="Ravish Sharma", email="ravish.sharma@impetus.com"}
 ]
 description = "Provides AWS compliance details"
 readme = "README.md"
 requires-python = ">=3.7"
```

