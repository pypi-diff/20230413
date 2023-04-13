# Comparing `tmp/cis_checks_2023-2.0.4.tar.gz` & `tmp/cis_checks_2023-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cis_checks_2023-2.0.4.tar", last modified: Wed Apr 12 14:39:28 2023, max compression
+gzip compressed data, was "cis_checks_2023-2.0.5.tar", last modified: Thu Apr 13 06:34:53 2023, max compression
```

## Comparing `cis_checks_2023-2.0.4.tar` & `cis_checks_2023-2.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 14:39:28.319993 cis_checks_2023-2.0.4/
--rw-rw-rw-   0        0        0      836 2023-04-12 14:39:28.319993 cis_checks_2023-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 cis_checks_2023-2.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 14:39:28.304354 cis_checks_2023-2.0.4/cis_checks_2023/
--rw-rw-rw-   0        0        0     6690 2023-04-12 14:38:35.000000 cis_checks_2023-2.0.4/cis_checks_2023/__init__.py
--rw-rw-rw-   0        0        0    35333 2023-04-07 14:21:10.000000 cis_checks_2023-2.0.4/cis_checks_2023/_security_control_5.py
--rw-rw-rw-   0        0        0    54565 2023-04-12 14:37:06.000000 cis_checks_2023-2.0.4/cis_checks_2023/iam_control_1.py
--rw-rw-rw-   0        0        0    24792 2023-04-12 14:37:06.000000 cis_checks_2023-2.0.4/cis_checks_2023/logging_control_3.py
--rw-rw-rw-   0        0        0    79813 2023-04-11 05:42:02.000000 cis_checks_2023-2.0.4/cis_checks_2023/monitoring_control_4.py
--rw-rw-rw-   0        0        0    25055 2023-04-11 07:00:11.000000 cis_checks_2023-2.0.4/cis_checks_2023/networking_control_5.py
--rw-rw-rw-   0        0        0    17716 2023-04-12 07:08:18.000000 cis_checks_2023-2.0.4/cis_checks_2023/storage_control_2.py
--rw-rw-rw-   0        0        0    20340 2023-04-10 07:28:15.000000 cis_checks_2023-2.0.4/cis_checks_2023/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:39:28.319993 cis_checks_2023-2.0.4/cis_checks_2023.egg-info/
--rw-rw-rw-   0        0        0      836 2023-04-12 14:39:28.000000 cis_checks_2023-2.0.4/cis_checks_2023.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-04-12 14:39:28.000000 cis_checks_2023-2.0.4/cis_checks_2023.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 14:39:28.000000 cis_checks_2023-2.0.4/cis_checks_2023.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-12 14:39:28.000000 cis_checks_2023-2.0.4/cis_checks_2023.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      557 2023-04-12 14:38:35.000000 cis_checks_2023-2.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 14:39:28.335613 cis_checks_2023-2.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 06:34:53.150341 cis_checks_2023-2.0.5/
+-rw-rw-rw-   0        0        0      836 2023-04-13 06:34:53.147337 cis_checks_2023-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 cis_checks_2023-2.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 06:34:53.124414 cis_checks_2023-2.0.5/cis_checks_2023/
+-rw-rw-rw-   0        0        0     6690 2023-04-13 06:34:22.000000 cis_checks_2023-2.0.5/cis_checks_2023/__init__.py
+-rw-rw-rw-   0        0        0    35333 2023-04-07 14:21:10.000000 cis_checks_2023-2.0.5/cis_checks_2023/_security_control_5.py
+-rw-rw-rw-   0        0        0    54565 2023-04-12 14:37:06.000000 cis_checks_2023-2.0.5/cis_checks_2023/iam_control_1.py
+-rw-rw-rw-   0        0        0    25256 2023-04-13 06:34:22.000000 cis_checks_2023-2.0.5/cis_checks_2023/logging_control_3.py
+-rw-rw-rw-   0        0        0    79813 2023-04-11 05:42:02.000000 cis_checks_2023-2.0.5/cis_checks_2023/monitoring_control_4.py
+-rw-rw-rw-   0        0        0    25055 2023-04-11 07:00:11.000000 cis_checks_2023-2.0.5/cis_checks_2023/networking_control_5.py
+-rw-rw-rw-   0        0        0    17716 2023-04-12 07:08:18.000000 cis_checks_2023-2.0.5/cis_checks_2023/storage_control_2.py
+-rw-rw-rw-   0        0        0    20340 2023-04-10 07:28:15.000000 cis_checks_2023-2.0.5/cis_checks_2023/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:34:53.142342 cis_checks_2023-2.0.5/cis_checks_2023.egg-info/
+-rw-rw-rw-   0        0        0      836 2023-04-13 06:34:52.000000 cis_checks_2023-2.0.5/cis_checks_2023.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-04-13 06:34:52.000000 cis_checks_2023-2.0.5/cis_checks_2023.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:34:52.000000 cis_checks_2023-2.0.5/cis_checks_2023.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-13 06:34:52.000000 cis_checks_2023-2.0.5/cis_checks_2023.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      557 2023-04-13 06:34:22.000000 cis_checks_2023-2.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:34:53.150341 cis_checks_2023-2.0.5/setup.cfg
```

### Comparing `cis_checks_2023-2.0.4/PKG-INFO` & `cis_checks_2023-2.0.5/cis_checks_2023.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cis_checks_2023
-Version: 2.0.4
+Name: cis-checks-2023
+Version: 2.0.5
 Summary: Provides AWS compliance details
 Author-email: Dheeraj Banodha <dheeraj.banodha@impetus.com>, Ravish Sharma <ravish.sharma@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cis_checks_2023-2.0.4/cis_checks_2023/__init__.py` & `cis_checks_2023-2.0.5/cis_checks_2023/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from cis_checks_2023.iam_control_1 import iam_control
 
 logging.basicConfig()
 logging.getLogger().setLevel(logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Dheeraj Banodha'
-__version__ = '2.0.4'
+__version__ = '2.0.5'
 
 
 class aws_client(iam_control, utils, storage_control, logging_control, monitoring_control, networking_control):
     def __init__(self, **kwargs):
         """
         @param str aws_access_key_id: AWS Access Key ID
         @param str aws_secret_access_key: AWS Secret Access Key
```

### Comparing `cis_checks_2023-2.0.4/cis_checks_2023/_security_control_5.py` & `cis_checks_2023-2.0.5/cis_checks_2023/_security_control_5.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.4/cis_checks_2023/iam_control_1.py` & `cis_checks_2023-2.0.5/cis_checks_2023/iam_control_1.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.4/cis_checks_2023/logging_control_3.py` & `cis_checks_2023-2.0.5/cis_checks_2023/logging_control_3.py`

 * *Files 6% similar despite different names*

```diff
@@ -423,15 +423,14 @@
         offenders = []
         control = "3.1"
         description = "Ensure that Object-level logging for write events is enabled for S3 bucket"
         scored = True
 
         for region in regions:
             try:
-
                 paginator = self.session.client('cloudtrail', region_name=region).get_paginator('list_trails')
                 response_iterator = paginator.paginate()
                 pagedResult = []
                 for page in response_iterator:
                     for n in page['Trails']:
                         pagedResult.append(n)
 
@@ -457,14 +456,20 @@
                     except:
                         KeyError
             except botocore.exceptions.ClientError as error:
                 logger.error(f" Exception while listing trails: {error}")
                 result = "Not Compliant"
                 failReason = "Exception while listing trails "+str(error)
                 offenders.append(region)
+            except Exception as e:
+                logger.error(str(e))
+                result = "Not Compliant"
+                failReason = "Exception while listing trails " + str(e)
+                offenders.append(region)
+
             
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 3.11 Ensure that Object-level logging for read events is enabled for S3 bucket
 
     def control_3_1_1_ensure_logging_enabled_for_s3_read(self, regions):
@@ -512,10 +517,16 @@
                     except:
                         KeyError
             except botocore.exceptions.ClientError as error:
                 logger.error(f" Exception while listing trails: {error}")
                 result = "Not Compliant"
                 failReason = "Exception while listing trails "+str(error)
                 offenders.append(region)
+
+            except Exception as e:
+                logger.error(str(e))
+                result = "Not Compliant"
+                failReason = "Exception while listing trails " + str(e)
+                offenders.append(region)
                 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
```

### Comparing `cis_checks_2023-2.0.4/cis_checks_2023/monitoring_control_4.py` & `cis_checks_2023-2.0.5/cis_checks_2023/monitoring_control_4.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.4/cis_checks_2023/networking_control_5.py` & `cis_checks_2023-2.0.5/cis_checks_2023/networking_control_5.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.4/cis_checks_2023/storage_control_2.py` & `cis_checks_2023-2.0.5/cis_checks_2023/storage_control_2.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.4/cis_checks_2023/utils.py` & `cis_checks_2023-2.0.5/cis_checks_2023/utils.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.4/pyproject.toml` & `cis_checks_2023-2.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "cis_checks_2023"
-version = "2.0.4"
+version = "2.0.5"
 authors = [
   { name="Dheeraj Banodha", email="dheeraj.banodha@impetus.com" },
   { name="Ravish Sharma", email="ravish.sharma@impetus.com"}
 ]
 description = "Provides AWS compliance details"
 readme = "README.md"
 requires-python = ">=3.7"
```

