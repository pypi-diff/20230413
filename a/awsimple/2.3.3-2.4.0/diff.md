# Comparing `tmp/awsimple-2.3.3-py3-none-any.whl.zip` & `tmp/awsimple-2.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 32261 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat      849 b- defN 23-Apr-10 03:01 awsimple/__init__.py
--rw-rw-rw-  2.0 fat      323 b- defN 23-Apr-10 06:10 awsimple/__version__.py
--rw-rw-rw-  2.0 fat     6365 b- defN 23-Mar-14 23:35 awsimple/aws.py
+Zip file size: 32561 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat      871 b- defN 23-Apr-12 19:14 awsimple/__init__.py
+-rw-rw-rw-  2.0 fat      323 b- defN 23-Apr-12 19:14 awsimple/__version__.py
+-rw-rw-rw-  2.0 fat     6952 b- defN 23-Apr-12 23:17 awsimple/aws.py
 -rw-rw-rw-  2.0 fat     7137 b- defN 23-Mar-14 23:35 awsimple/cache.py
--rw-rw-rw-  2.0 fat    35658 b- defN 23-Apr-10 06:09 awsimple/dynamodb.py
+-rw-rw-rw-  2.0 fat    35771 b- defN 23-Apr-10 06:56 awsimple/dynamodb.py
 -rw-rw-rw-  2.0 fat     4619 b- defN 23-Mar-14 23:35 awsimple/dynamodb_miv.py
 -rw-rw-rw-  2.0 fat     4278 b- defN 23-Mar-14 23:10 awsimple/logs.py
 -rw-rw-rw-  2.0 fat      199 b- defN 23-Mar-14 23:10 awsimple/mock.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 23:10 awsimple/py.typed
 -rw-rw-rw-  2.0 fat    23243 b- defN 23-Mar-14 23:35 awsimple/s3.py
 -rw-rw-rw-  2.0 fat     3266 b- defN 23-Mar-14 23:10 awsimple/sns.py
--rw-rw-rw-  2.0 fat    13007 b- defN 23-Mar-14 23:35 awsimple/sqs.py
--rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-10 06:16 awsimple-2.3.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-10 06:16 awsimple-2.3.3.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     4815 b- defN 23-Apr-10 06:16 awsimple-2.3.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 06:16 awsimple-2.3.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-10 06:16 awsimple-2.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1376 b- defN 23-Apr-10 06:16 awsimple-2.3.3.dist-info/RECORD
-18 files, 107422 bytes uncompressed, 30047 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat    13260 b- defN 23-Apr-12 23:34 awsimple/sqs.py
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-13 00:13 awsimple-2.4.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-13 00:13 awsimple-2.4.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     4815 b- defN 23-Apr-13 00:13 awsimple-2.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 00:13 awsimple-2.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-13 00:13 awsimple-2.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1376 b- defN 23-Apr-13 00:13 awsimple-2.4.0.dist-info/RECORD
+18 files, 108397 bytes uncompressed, 30347 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: awsimple/sns.py
 Comment: 
 
 Filename: awsimple/sqs.py
 Comment: 
 
-Filename: awsimple-2.3.3.dist-info/LICENSE
+Filename: awsimple-2.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: awsimple-2.3.3.dist-info/LICENSE.txt
+Filename: awsimple-2.4.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: awsimple-2.3.3.dist-info/METADATA
+Filename: awsimple-2.4.0.dist-info/METADATA
 Comment: 
 
-Filename: awsimple-2.3.3.dist-info/WHEEL
+Filename: awsimple-2.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: awsimple-2.3.3.dist-info/top_level.txt
+Filename: awsimple-2.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: awsimple-2.3.3.dist-info/RECORD
+Filename: awsimple-2.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awsimple/__init__.py

```diff
@@ -1,10 +1,10 @@
 from .__version__ import __application_name__, __version__, __author__, __title__
 from .mock import use_moto_mock_env_var, is_mock
-from .aws import AWSAccess, AWSimpleException
+from .aws import AWSAccess, AWSimpleException, boto_error_to_string
 from .cache import get_disk_free, get_directory_size, lru_cache_write, CacheAccess, CACHE_DIR_ENV_VAR
 from .dynamodb import DynamoDBAccess, dict_to_dynamodb, DBItemNotFound, DynamoDBTableNotFound, dynamodb_to_json, dynamodb_to_dict, QuerySelection, DictKey, convert_serializable_special_cases
 from .dynamodb import KeyType, aws_name_to_key_type
 from .dynamodb_miv import DynamoDBMIVUI, miv_string, get_time_us, miv_us_to_timestamp
 from .s3 import S3Access, S3DownloadStatus, S3ObjectMetadata, BucketNotFound
 from .sqs import SQSAccess, SQSPollAccess, aws_sqs_long_poll_max_wait_time, aws_sqs_max_messages
 from .sns import SNSAccess
```

## awsimple/__version__.py

```diff
@@ -1,8 +1,8 @@
 __application_name__ = "awsimple"
 __title__ = __application_name__
 __author__ = "abel"
-__version__ = "2.3.3"
+__version__ = "2.4.0"
 __author_email__ = "j@abel.co"
 __url__ = "https://github.com/jamesabel/awsimple"
 __download_url__ = "https://github.com/jamesabel/awsimple"
 __description__ = "Simple AWS API for S3, DynamoDB, SNS, and SQS"
```

## awsimple/aws.py

```diff
@@ -9,14 +9,25 @@
 log = getLogger(__application_name__)
 
 
 class AWSimpleException(Exception):
     pass
 
 
+def boto_error_to_string(boto_error) -> Union[str, None]:
+    if (response := boto_error.response) is None:
+        most_recent_error = str(boto_error)
+    else:
+        if (response_error := response.get("Error")) is None:
+            most_recent_error = None
+        else:
+            most_recent_error = response_error.get("Code")
+    return most_recent_error
+
+
 class AWSAccess:
     @typechecked()
     def __init__(
         self,
         resource_name: str = None,
         profile_name: str = None,
         aws_access_key_id: str = None,
@@ -40,14 +51,17 @@
 
         self.resource_name = resource_name
         self.profile_name = profile_name
         self.aws_access_key_id = aws_access_key_id
         self.aws_secret_access_key = aws_secret_access_key
         self.region_name = region_name
 
+        # string representation of AWS most recent error code
+        self.most_recent_error = None  # type: Union[str, None]
+
         self._moto_mock = None
         self._aws_keys_save = {}
 
         # use keys in AWS config
         # https://docs.aws.amazon.com/cli/latest/userguide/cli-config-files.html
         kwargs = {}
         for k in ["profile_name", "aws_access_key_id", "aws_secret_access_key", "region_name"]:
@@ -151,14 +165,17 @@
         """
         Return True if currently mocking the AWS interface (e.g. for testing).
 
         :return: True if mocked
         """
         return self._moto_mock is not None
 
+    def clear_most_recent_error(self):
+        self.most_recent_error = None
+
     def __del__(self):
         if self._moto_mock is not None:
             # if mocking, put everything back
 
             for aws_key, value in self._aws_keys_save.items():
                 if value is None:
                     del os.environ[aws_key]
```

## awsimple/dynamodb.py

```diff
@@ -190,14 +190,18 @@
         super().__init__(self.message)
 
     def __str__(self):
         return f"{self.key=} {self.message}"
 
 
 class DynamoDBTableNotFound(AWSimpleException):
+    """
+    DynamoDB Table Not Found exception (doesn't require access to a boto3 client instance).
+    """
+
     def __init__(self, table_name: str):
         self.table_name = table_name
         self.message = f'Table "{self.table_name}" not found'
         super().__init__(self.message)
 
 
 @typechecked()
```

## awsimple/sqs.py

```diff
@@ -7,19 +7,19 @@
 import time
 import statistics
 from datetime import timedelta
 from pathlib import Path
 import json
 from logging import getLogger
 
-from botocore.exceptions import ClientError
+from botocore.exceptions import ClientError, HTTPClientError
 from typeguard import typechecked
 import appdirs
 
-from awsimple import AWSAccess, __application_name__, __author__
+from awsimple import AWSAccess, __application_name__, __author__, boto_error_to_string
 
 log = getLogger(__application_name__)
 
 
 @dataclass
 class SQSMessage:
     """
@@ -200,17 +200,18 @@
                             for handle, start_finish in self.response_history.items():
                                 if oldest is None or start_finish[0] < self.response_history[oldest][0]:
                                     oldest = handle
                             del self.response_history[oldest]
 
                     messages.append(SQSMessage(m.body, m, self))
 
-            except ClientError as e:
-                # should happen very infrequently
-                log.warning(f"{self.queue_name=} {e}")
+            except (ClientError, HTTPClientError) as e:
+                # Usually we don't catch boto3 exceptions, but during a long poll a quick internet disruption can raise an exception that we'd like to avoid.
+                log.debug(f"{self.queue_name=} {e}")
+                self.most_recent_error = boto_error_to_string(e)
 
             call_wait_time = 0  # now, short polls
 
             if aws_messages is None or len(aws_messages) == 0 or (max_number_of_messages_parameter is not None and len(messages) >= max_number_of_messages_parameter):
                 continue_to_receive = False
 
         return messages
@@ -264,15 +265,16 @@
     @typechecked()
     def send(self, message: str):
         """
         send SQS message
 
         :param message: message string
         """
-        self._get_queue().send_message(MessageBody=message)
+        queue = self._get_queue()
+        queue.send_message(MessageBody=message)
 
     @typechecked()
     def get_arn(self) -> str:
         """
         get SQS ARN
 
         :return: ARN string
```

## Comparing `awsimple-2.3.3.dist-info/LICENSE` & `awsimple-2.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awsimple-2.3.3.dist-info/LICENSE.txt` & `awsimple-2.4.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `awsimple-2.3.3.dist-info/METADATA` & `awsimple-2.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsimple
-Version: 2.3.3
+Version: 2.4.0
 Summary: Simple AWS API for S3, DynamoDB, SNS, and SQS
 Home-page: https://github.com/jamesabel/awsimple
 Download-URL: https://github.com/jamesabel/awsimple
 Author: abel
 Author-email: j@abel.co
 License: MIT License
 Project-URL: Documentation, https://awsimple.readthedocs.io/
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: awsimple Version: 2.3.3 Summary: Simple AWS API for
+Metadata-Version: 2.1 Name: awsimple Version: 2.4.0 Summary: Simple AWS API for
 S3, DynamoDB, SNS, and SQS Home-page: https://github.com/jamesabel/awsimple
 Download-URL: https://github.com/jamesabel/awsimple Author: abel Author-email:
 j@abel.co License: MIT License Project-URL: Documentation, https://
 awsimple.readthedocs.io/ Keywords: aws,cloud,storage,database,dynamodb,s3
 Description-Content-Type: text/markdown License-File: LICENSE License-File:
 LICENSE.txt Requires-Dist: boto3 Requires-Dist: typeguard (<3) Requires-Dist:
 hashy (>=0.1.1) Requires-Dist: dictim Requires-Dist: appdirs Requires-Dist:
```

