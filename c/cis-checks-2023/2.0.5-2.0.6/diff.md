# Comparing `tmp/cis_checks_2023-2.0.5.tar.gz` & `tmp/cis_checks_2023-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cis_checks_2023-2.0.5.tar", last modified: Thu Apr 13 06:34:53 2023, max compression
+gzip compressed data, was "cis_checks_2023-2.0.6.tar", last modified: Thu Apr 13 08:31:14 2023, max compression
```

## Comparing `cis_checks_2023-2.0.5.tar` & `cis_checks_2023-2.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 06:34:53.150341 cis_checks_2023-2.0.5/
--rw-rw-rw-   0        0        0      836 2023-04-13 06:34:53.147337 cis_checks_2023-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 cis_checks_2023-2.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 06:34:53.124414 cis_checks_2023-2.0.5/cis_checks_2023/
--rw-rw-rw-   0        0        0     6690 2023-04-13 06:34:22.000000 cis_checks_2023-2.0.5/cis_checks_2023/__init__.py
--rw-rw-rw-   0        0        0    35333 2023-04-07 14:21:10.000000 cis_checks_2023-2.0.5/cis_checks_2023/_security_control_5.py
--rw-rw-rw-   0        0        0    54565 2023-04-12 14:37:06.000000 cis_checks_2023-2.0.5/cis_checks_2023/iam_control_1.py
--rw-rw-rw-   0        0        0    25256 2023-04-13 06:34:22.000000 cis_checks_2023-2.0.5/cis_checks_2023/logging_control_3.py
--rw-rw-rw-   0        0        0    79813 2023-04-11 05:42:02.000000 cis_checks_2023-2.0.5/cis_checks_2023/monitoring_control_4.py
--rw-rw-rw-   0        0        0    25055 2023-04-11 07:00:11.000000 cis_checks_2023-2.0.5/cis_checks_2023/networking_control_5.py
--rw-rw-rw-   0        0        0    17716 2023-04-12 07:08:18.000000 cis_checks_2023-2.0.5/cis_checks_2023/storage_control_2.py
--rw-rw-rw-   0        0        0    20340 2023-04-10 07:28:15.000000 cis_checks_2023-2.0.5/cis_checks_2023/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:34:53.142342 cis_checks_2023-2.0.5/cis_checks_2023.egg-info/
--rw-rw-rw-   0        0        0      836 2023-04-13 06:34:52.000000 cis_checks_2023-2.0.5/cis_checks_2023.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-04-13 06:34:52.000000 cis_checks_2023-2.0.5/cis_checks_2023.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 06:34:52.000000 cis_checks_2023-2.0.5/cis_checks_2023.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 06:34:52.000000 cis_checks_2023-2.0.5/cis_checks_2023.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      557 2023-04-13 06:34:22.000000 cis_checks_2023-2.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 06:34:53.150341 cis_checks_2023-2.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 08:31:14.695237 cis_checks_2023-2.0.6/
+-rw-rw-rw-   0        0        0      836 2023-04-13 08:31:14.693260 cis_checks_2023-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 cis_checks_2023-2.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 08:31:14.673590 cis_checks_2023-2.0.6/cis_checks_2023/
+-rw-rw-rw-   0        0        0     6851 2023-04-13 08:30:38.000000 cis_checks_2023-2.0.6/cis_checks_2023/__init__.py
+-rw-rw-rw-   0        0        0    35333 2023-04-07 14:21:10.000000 cis_checks_2023-2.0.6/cis_checks_2023/_security_control_5.py
+-rw-rw-rw-   0        0        0    54565 2023-04-12 14:37:06.000000 cis_checks_2023-2.0.6/cis_checks_2023/iam_control_1.py
+-rw-rw-rw-   0        0        0    25256 2023-04-13 06:34:22.000000 cis_checks_2023-2.0.6/cis_checks_2023/logging_control_3.py
+-rw-rw-rw-   0        0        0    79813 2023-04-11 05:42:02.000000 cis_checks_2023-2.0.6/cis_checks_2023/monitoring_control_4.py
+-rw-rw-rw-   0        0        0    25055 2023-04-11 07:00:11.000000 cis_checks_2023-2.0.6/cis_checks_2023/networking_control_5.py
+-rw-rw-rw-   0        0        0    15823 2023-04-13 07:08:22.000000 cis_checks_2023-2.0.6/cis_checks_2023/storage_control_2.py
+-rw-rw-rw-   0        0        0    21541 2023-04-13 07:03:52.000000 cis_checks_2023-2.0.6/cis_checks_2023/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:31:14.689081 cis_checks_2023-2.0.6/cis_checks_2023.egg-info/
+-rw-rw-rw-   0        0        0      836 2023-04-13 08:31:14.000000 cis_checks_2023-2.0.6/cis_checks_2023.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-04-13 08:31:14.000000 cis_checks_2023-2.0.6/cis_checks_2023.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 08:31:14.000000 cis_checks_2023-2.0.6/cis_checks_2023.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-13 08:31:14.000000 cis_checks_2023-2.0.6/cis_checks_2023.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      557 2023-04-13 08:30:38.000000 cis_checks_2023-2.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 08:31:14.696230 cis_checks_2023-2.0.6/setup.cfg
```

### Comparing `cis_checks_2023-2.0.5/PKG-INFO` & `cis_checks_2023-2.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cis_checks_2023
-Version: 2.0.5
+Version: 2.0.6
 Summary: Provides AWS compliance details
 Author-email: Dheeraj Banodha <dheeraj.banodha@impetus.com>, Ravish Sharma <ravish.sharma@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cis_checks_2023-2.0.5/cis_checks_2023/__init__.py` & `cis_checks_2023-2.0.6/cis_checks_2023/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from cis_checks_2023.iam_control_1 import iam_control
 
 logging.basicConfig()
 logging.getLogger().setLevel(logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Dheeraj Banodha'
-__version__ = '2.0.5'
+__version__ = '2.0.6'
 
 
 class aws_client(iam_control, utils, storage_control, logging_control, monitoring_control, networking_control):
     def __init__(self, **kwargs):
         """
         @param str aws_access_key_id: AWS Access Key ID
         @param str aws_secret_access_key: AWS Secret Access Key
@@ -40,14 +40,16 @@
         """
         logger.info(" ---Inside get_compliance()")
 
         regions = self.get_regions()
         CloudTrail = self.get_cloudtrails(regions)
         creds_report = self.get_cred_report()
         password_policy = self.get_account_password_policy()
+        s3_buckets = self.list_s3_buckets()
+        rds_instances = self.list_rds_instances(regions)
 
         compliance = [
             # iam_control_1
 
             self.control_1_01_maintain_contact_details(),
             self.control_1_02_security_contact_information_registered(),
             self.control_1_03_security_questions_registered(),
@@ -68,23 +70,23 @@
             self.control_1_18_iam_instance_role_for_access_from_instances(),
             self.control_1_19_expired_ssl_tls_certificates_removed(regions),
             self.control_1_2_iam_access_analyzer_enabled(regions),
             self.control_1_21_iam_user_managed_centrally(),
 
             # storage_control_2
 
-            self.control_2_1_1_s3_default_encryption_at_rest(),
-            self.control_2_1_2_s3_deny_http_requests(),
-            self.control_2_1_3_s3_mfa_delete_enabled(),
+            self.control_2_1_1_s3_default_encryption_at_rest(s3_buckets),
+            self.control_2_1_2_s3_deny_http_requests(s3_buckets),
+            self.control_2_1_3_s3_mfa_delete_enabled(s3_buckets),
             self.control_2_1_4_ensure_all_data_discovered_classified_secured(),
-            self.control_2_1_5_s3_blocks_public_access(),
+            self.control_2_1_5_s3_blocks_public_access(s3_buckets),
             self.control_2_2_1_ebs_volumes_encrypted(regions),
-            self.control_2_3_1_rds_encryption_enabled(regions),
-            self.control_2_3_2_rds_auto_minor_version_upgrade_enabled(regions),
-            self.control_2_3_3_rds_publicly_accessible(regions),
+            self.control_2_3_1_rds_encryption_enabled(rds_instances),
+            self.control_2_3_2_rds_auto_minor_version_upgrade_enabled(rds_instances),
+            self.control_2_3_3_rds_publicly_accessible(rds_instances),
             self.control_2_4_1_encryption_enabled_for_efs(),
 
             # logging control 3
             self.control_3_01_ensure_cloud_trail_all_regions(CloudTrail),
             self.control_3_02_ensure_cloudtrail_validation(CloudTrail),
             self.control_3_03_ensure_cloudtrail_bucket_not_public(CloudTrail),
             self.control_3_04_ensure_cloudtrail_cloudwatch_logs_integration(CloudTrail),
```

### Comparing `cis_checks_2023-2.0.5/cis_checks_2023/_security_control_5.py` & `cis_checks_2023-2.0.6/cis_checks_2023/_security_control_5.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.5/cis_checks_2023/iam_control_1.py` & `cis_checks_2023-2.0.6/cis_checks_2023/iam_control_1.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.5/cis_checks_2023/logging_control_3.py` & `cis_checks_2023-2.0.6/cis_checks_2023/logging_control_3.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.5/cis_checks_2023/monitoring_control_4.py` & `cis_checks_2023-2.0.6/cis_checks_2023/monitoring_control_4.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.5/cis_checks_2023/networking_control_5.py` & `cis_checks_2023-2.0.6/cis_checks_2023/networking_control_5.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.5/cis_checks_2023/storage_control_2.py` & `cis_checks_2023-2.0.6/cis_checks_2023/storage_control_2.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,32 +27,29 @@
 # --- 2 Storage ---
 
 # --- 2.1 Simple Storage Service (S3) ---
 
 
 class storage_control:
     # 2.1.1 Ensure all S3 buckets employ encryption-at-rest
-    def control_2_1_1_s3_default_encryption_at_rest(self):
+    def control_2_1_1_s3_default_encryption_at_rest(self, buckets):
         logger.info(" ---Inside storage_control_2 :: control_2_1_1_s3_default_encryption_at_rest()--- ")
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
         offenders = []
         control = "2.1.1"
         description = "Ensure all S3 buckets employ encryption-at-rest"
         scored = True
-
         client = self.session.client('s3')
-        response = client.list_buckets()
-
-        for bucket in response['Buckets']:
+        for bucket in buckets:
             bucket_name = bucket['Name']
 
             try:
                 resp = client.get_bucket_encryption(
                     Bucket=bucket_name
                 )
                 rules = resp['ServerSideEncryptionConfiguration']['Rules']
@@ -72,32 +69,29 @@
             #     failReason = "The S3 buckets are not encrypted with AWS Key Management Service(AWS KMS)"
             #     offenders.append(bucket_name)
             #     continue
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 2.1.2 Ensure S3 Bucket Policy is set to deny HTTP requests
-    def control_2_1_2_s3_deny_http_requests(self):
+    def control_2_1_2_s3_deny_http_requests(self, buckets):
         logger.info(" ---Inside storage_control_2 :: control_2_1_2_s3_deny_http_requests()--- ")
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
         offenders = []
         control = "2.1.2"
         description = "Ensure S3 Bucket Policy is set to deny HTTP requests"
         scored = True
-
         client = self.session.client('s3')
-        response = client.list_buckets()
-
-        for bucket in response['Buckets']:
+        for bucket in buckets:
             bucket_name = bucket['Name']
 
             try:
                 resp = client.get_bucket_policy(
                     Bucket=bucket_name
                 )
                 ssl_requests_only = ""
@@ -125,32 +119,29 @@
                 offenders.append(bucket_name)
                 continue
 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 2.1.3 Ensure MFA Delete is enabled on S3 buckets
-    def control_2_1_3_s3_mfa_delete_enabled(self):
+    def control_2_1_3_s3_mfa_delete_enabled(self, buckets):
         logger.info(" ---Inside storage_control_2 :: control_2_1_3_s3_mfa_delete_enabled()--- ")
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
         offenders = []
         control = "2.1.3"
         description = "Ensure MFA Delete is enabled on S3 buckets"
         scored = True
-
         client = self.session.client('s3')
-        response = client.list_buckets()
-
-        for bucket in response['Buckets']:
+        for bucket in buckets:
             bucket_name = bucket['Name']
 
             try:
                 resp = client.get_bucket_versioning(
                     Bucket=bucket_name,
                 )
                 mfa_delete = resp['MFADelete']
@@ -183,32 +174,29 @@
                       "please verify manually"
         scored = True
         failReason = "Control not implemented using API, please verify manually"
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 2.1.5 Ensure that S3 Buckets are configured with 'Block public access (bucket settings)'
-    def control_2_1_5_s3_blocks_public_access(self):
+    def control_2_1_5_s3_blocks_public_access(self, buckets):
         logger.info(" ---Inside storage_control_2 :: control_2_1_5_s3_blocks_public_access()--- ")
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         offenders = []
         control = "2.1.5"
         description = "Ensure that S3 Buckets are configured with 'Block public access (bucket settings)"
         scored = True
         failReason = ""
-
         client = self.session.client('s3')
-        response = client.list_buckets()
-
-        for bucket in response['Buckets']:
+        for bucket in buckets:
             bucket_name = bucket['Name']
 
             try:
                 resp = client.get_public_access_block(
                     Bucket=bucket_name
                 )
 
@@ -290,15 +278,15 @@
             'Description': description,
             'ControlId': control
         }
 
     # --- 2.3 Relational Database Service (RDS) ---
     # 2.3.1 Ensure that encryption is enabled for RDS Instances
 
-    def control_2_3_1_rds_encryption_enabled(self, regions: list) -> dict:
+    def control_2_3_1_rds_encryption_enabled(self, rds_instances: dict) -> dict:
         logger.info(" ---Inside storage_control_2 :: control_2_3_1_rds_encryption_enabled()---")
 
         """Summary
         
         Args:
             regions TYPE: list
     
@@ -308,50 +296,34 @@
         result = "Compliant"
         failReason = ""
         offenders = []
         control = "2.3.1"
         description = "Ensure that encryption is enabled for RDS Instances"
         scored = True
 
-        for region in regions:
-            client = self.session.client('rds', region_name=region)
-            marker = ''
-            while True:
-                if marker == '':
-                    response = client.describe_db_instances()
-                else:
-                    response = client.describe_db_instances(
-                        Marker=marker
-                    )
-                for instance in response['DBInstances']:
-                    encrypted = instance['StorageEncrypted']
-                    if not encrypted:
-                        result = "Not Compliant"
-                        offenders.append(instance['DBInstanceIdentifier'])
-                        failReason = 'DB instance is not encrypted'
-
-                try:
-                    marker = response['Marker']
-                    if marker == '':
-                        break
-                except KeyError:
-                    break
+        for region, instances in rds_instances.items():
+            for instance in instances:
+                encrypted = instance['StorageEncrypted']
+                if not encrypted:
+                    result = "Not Compliant"
+                    offenders.append(instance['DBInstanceIdentifier'])
+                    failReason = 'DB instance is not encrypted'
 
         return {
             'Result': result,
             'failReason': failReason,
             'Offenders': offenders,
             'ScoredControl': scored,
             'Description': description,
             'ControlId': control
         }
 
     # 2.3.2 Ensure Auto Minor Version Upgrade feature is Enabled for RDS Instances
 
-    def control_2_3_2_rds_auto_minor_version_upgrade_enabled(self, regions: list) -> dict:
+    def control_2_3_2_rds_auto_minor_version_upgrade_enabled(self, rds_instances: dict) -> dict:
         logger.info(" ---Inside storage_control_2 :: control_2_3_2_rds_auto_minor_version_upgrade_enabled()---")
 
         """Summary
         
         Args:
             regions TYPE: list
     
@@ -361,49 +333,33 @@
         result = "Compliant"
         failReason = ""
         offenders = []
         control = "2.3.2"
         description = "Ensure Auto Minor Version Upgrade feature is Enabled for RDS Instances"
         scored = True
 
-        for region in regions:
-            client = self.session.client('rds', region_name=region)
-            marker = ''
-            while True:
-                if marker == '':
-                    response = client.describe_db_instances()
-                else:
-                    response = client.describe_db_instances(
-                        Marker=marker
-                    )
-                for instance in response['DBInstances']:
+        for region, instances in rds_instances.items():
+                for instance in instances:
                     version_upgrade = instance['AutoMinorVersionUpgrade']
                     if not version_upgrade:
                         result = "Not Compliant"
                         offenders.append(instance['DBInstanceIdentifier'])
                         failReason = 'Auto Minor Version Upgrade feature is not Enabled for RDS Instances'
 
-                try:
-                    marker = response['Marker']
-                    if marker == '':
-                        break
-                except KeyError:
-                    break
-
         return {
             'Result': result,
             'failReason': failReason,
             'Offenders': offenders,
             'ScoredControl': scored,
             'Description': description,
             'ControlId': control
         }
 
     # 2.3.3 Ensure that public access is not given to RDS Instance
-    def control_2_3_3_rds_publicly_accessible(self, regions: list) -> dict:
+    def control_2_3_3_rds_publicly_accessible(self, rds_instances: dict) -> dict:
         logger.info(" ---Inside storage_control_2 :: control_2_3_3_rds_publicly_accessible()")
 
         """Summary
         
         Args:
             regions TYPE: list
     
@@ -413,38 +369,21 @@
         result = "Compliant"
         failReason = ""
         offenders = []
         control = "2.3.3"
         description = "Ensure that public access is not given to RDS Instance"
         scored = True
 
-        for region in regions:
-            client = self.session.client('rds', region_name=region)
-            marker = ''
-            while True:
-                if marker == '':
-                    response = client.describe_db_instances()
-                else:
-                    response = client.describe_db_instances(
-                        Marker=marker
-                    )
-
-                for instance in response['DBInstances']:
-                    public = instance['PubliclyAccessible']
-                    if public:
-                        result = "Not Compliant"
-                        offenders.append(instance['DBInstanceIdentifier'])
-                        failReason = 'DB Instance is publicly accessible'
-
-                try:
-                    marker = response['Marker']
-                    if marker == '':
-                        break
-                except KeyError:
-                    break
+        for region, instances in rds_instances.items():
+            for instance in instances:
+                public = instance['PubliclyAccessible']
+                if public:
+                    result = "Not Compliant"
+                    offenders.append(instance['DBInstanceIdentifier'])
+                    failReason = 'DB Instance is publicly accessible'
 
         return {
             'Result': result,
             'failReason': failReason,
             'Offenders': offenders,
             'ScoredControl': scored,
             'Description': description,
```

### Comparing `cis_checks_2023-2.0.5/cis_checks_2023/utils.py` & `cis_checks_2023-2.0.6/cis_checks_2023/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -510,7 +510,51 @@
                 marker = response['Marker']
                 if marker == '':
                     break
             except:
                 break
 
         return elb_lst
+
+#     list s3 buckets
+    def list_s3_buckets(self) -> list:
+        """
+        :return:
+        """
+        logger.info(" ---Inside utils :: list_s3_buckets")
+
+        buckets = []
+
+        client = self.session.client('s3')
+        response = client.list_buckets()
+
+        return response['Buckets']
+
+#     list rds instances
+    def list_rds_instances(self, regions) -> dict:
+        """
+        :param regions:
+        :return:
+        """
+        logger.info(" ---Inside utils :: list_rds_instances()--- ")
+        rds_instance_lst = {}
+
+        for region in regions:
+            client = self.session.client('rds', region_name=region)
+            marker = ''
+            while True:
+                response = client.describe_db_instances(
+                    MaxRecords=100,
+                    Marker=marker
+                )
+                rds_instance_lst.setdefault(region, []).extend(response['DBInstances'])
+
+                try:
+                    marker = response['Marker']
+                    if marker == '':
+                        break
+                except KeyError:
+                    break
+        return rds_instance_lst
+
+
+
```

### Comparing `cis_checks_2023-2.0.5/cis_checks_2023.egg-info/PKG-INFO` & `cis_checks_2023-2.0.6/cis_checks_2023.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cis-checks-2023
-Version: 2.0.5
+Version: 2.0.6
 Summary: Provides AWS compliance details
 Author-email: Dheeraj Banodha <dheeraj.banodha@impetus.com>, Ravish Sharma <ravish.sharma@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cis_checks_2023-2.0.5/pyproject.toml` & `cis_checks_2023-2.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "cis_checks_2023"
-version = "2.0.5"
+version = "2.0.6"
 authors = [
   { name="Dheeraj Banodha", email="dheeraj.banodha@impetus.com" },
   { name="Ravish Sharma", email="ravish.sharma@impetus.com"}
 ]
 description = "Provides AWS compliance details"
 readme = "README.md"
 requires-python = ">=3.7"
```

