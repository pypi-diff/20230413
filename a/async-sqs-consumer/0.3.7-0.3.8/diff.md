# Comparing `tmp/async_sqs_consumer-0.3.7.tar.gz` & `tmp/async_sqs_consumer-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_sqs_consumer-0.3.7.tar", max compression
+gzip compressed data, was "async_sqs_consumer-0.3.8.tar", max compression
```

## Comparing `async_sqs_consumer-0.3.7.tar` & `async_sqs_consumer-0.3.8.tar`

### file list

```diff
@@ -1,16 +1,14 @@
--rw-r--r--   0        0        0     2410 2023-03-31 13:48:41.692048 async_sqs_consumer-0.3.7/README.md
--rw-r--r--   0        0        0        0 2023-03-31 14:08:47.294687 async_sqs_consumer-0.3.7/async_sqs_consumer/__init__.py
--rw-r--r--   0        0        0     4682 2023-04-11 18:06:55.645770 async_sqs_consumer-0.3.7/async_sqs_consumer/queue.py
--rw-r--r--   0        0        0     2254 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.7/async_sqs_consumer/resources.py
--rw-r--r--   0        0        0        0 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.7/async_sqs_consumer/test/__init__.py
--rw-r--r--   0        0        0      542 2023-04-02 17:24:04.634142 async_sqs_consumer-0.3.7/async_sqs_consumer/test/send_message.py
--rw-r--r--   0        0        0      543 2023-04-11 18:44:09.667026 async_sqs_consumer-0.3.7/async_sqs_consumer/test/server.py
--rw-r--r--   0        0        0      753 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.7/async_sqs_consumer/types.py
--rw-r--r--   0        0        0      486 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.7/async_sqs_consumer/utils/__init__.py
--rw-r--r--   0        0        0     1365 2023-03-31 15:12:56.460833 async_sqs_consumer-0.3.7/async_sqs_consumer/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5522 2023-04-11 14:12:54.911336 async_sqs_consumer-0.3.7/async_sqs_consumer/utils/__pycache__/retry.cpython-311.pyc
--rw-r--r--   0        0        0     3803 2023-04-11 12:49:23.872046 async_sqs_consumer-0.3.7/async_sqs_consumer/utils/retry.py
--rw-r--r--   0        0        0    10098 2023-04-11 22:05:33.291753 async_sqs_consumer-0.3.7/async_sqs_consumer/worker.py
--rw-r--r--   0        0        0      647 2023-04-11 22:06:08.746182 async_sqs_consumer-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.7/setup.py
--rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     2410 2023-03-31 13:48:41.692048 async_sqs_consumer-0.3.8/README.md
+-rw-r--r--   0        0        0        0 2023-03-31 14:08:47.294687 async_sqs_consumer-0.3.8/async_sqs_consumer/__init__.py
+-rw-r--r--   0        0        0     5040 2023-04-12 17:09:50.438085 async_sqs_consumer-0.3.8/async_sqs_consumer/queue.py
+-rw-r--r--   0        0        0     2254 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.8/async_sqs_consumer/resources.py
+-rw-r--r--   0        0        0        0 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.8/async_sqs_consumer/test/__init__.py
+-rw-r--r--   0        0        0      542 2023-04-02 17:24:04.634142 async_sqs_consumer-0.3.8/async_sqs_consumer/test/send_message.py
+-rw-r--r--   0        0        0      543 2023-04-11 18:44:09.667026 async_sqs_consumer-0.3.8/async_sqs_consumer/test/server.py
+-rw-r--r--   0        0        0      753 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.8/async_sqs_consumer/types.py
+-rw-r--r--   0        0        0      971 2023-04-12 22:14:17.319398 async_sqs_consumer-0.3.8/async_sqs_consumer/utils/__init__.py
+-rw-r--r--   0        0        0     3803 2023-04-11 12:49:23.872046 async_sqs_consumer-0.3.8/async_sqs_consumer/utils/retry.py
+-rw-r--r--   0        0        0    11296 2023-04-12 22:29:42.964531 async_sqs_consumer-0.3.8/async_sqs_consumer/worker.py
+-rw-r--r--   0        0        0      647 2023-04-12 22:39:16.715656 async_sqs_consumer-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.8/setup.py
+-rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.8/PKG-INFO
```

### Comparing `async_sqs_consumer-0.3.7/README.md` & `async_sqs_consumer-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.7/async_sqs_consumer/queue.py` & `async_sqs_consumer-0.3.8/async_sqs_consumer/queue.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,19 +50,24 @@
 @retry(exceptions=NETWORK_ERRORS, tries=3, delay=0.2)
 async def get_queue_messages(
     queue_url: str,
     credentials: Optional[AwsCredentials] = None,
     client: Optional[BaseClient] = None,
     visibility_timeout: Optional[int] = None,
     wait_time_seconds: Optional[int] = None,
+    max_number_of_messages: Optional[int] = None,
 ) -> list[dict[str, Any]]:
     client = await get_sqs_client(credentials)
+    max_number_of_messages = max_number_of_messages or 10
+    max_number_of_messages = (
+        10 if max_number_of_messages > 10 else max_number_of_messages
+    )
     response = await client.receive_message(
         QueueUrl=queue_url,
-        MaxNumberOfMessages=10,
+        MaxNumberOfMessages=max_number_of_messages,
         VisibilityTimeout=visibility_timeout or 60,
         WaitTimeSeconds=wait_time_seconds or 0,
     )
     return response.get("Messages", [])
 
 
 @retry(exceptions=NETWORK_ERRORS, tries=3, delay=0.2)
@@ -92,20 +97,23 @@
         self.priority = priority or 1
         self.authentication = authentication
         self.polling_interval = polling_interval or 1.0
         self.visibility_timeout = visibility_timeout or 60
         self._max_queue_parallel_messages = max_queue_parallel_messages
         self._polling = False
 
-    async def get_messages(self, sqs_client: Any) -> list[dict[str, Any]]:
+    async def get_messages(
+        self, sqs_client: Any, max_number_of_messages: Optional[int] = None
+    ) -> list[dict[str, Any]]:
         with suppress(asyncio.CancelledError):
             messages = await get_queue_messages(
                 self.url,
                 client=sqs_client,
                 visibility_timeout=self.visibility_timeout,
+                max_number_of_messages=max_number_of_messages,
             )
             return messages
         return []
 
     async def start_polling(
         self,
         callback: Callable[[dict[str, Any], str], Coroutine[Any, Any, None]],
```

### Comparing `async_sqs_consumer-0.3.7/async_sqs_consumer/resources.py` & `async_sqs_consumer-0.3.8/async_sqs_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.7/async_sqs_consumer/test/send_message.py` & `async_sqs_consumer-0.3.8/async_sqs_consumer/test/send_message.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.7/async_sqs_consumer/test/server.py` & `async_sqs_consumer-0.3.8/async_sqs_consumer/test/server.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.7/async_sqs_consumer/types.py` & `async_sqs_consumer-0.3.8/async_sqs_consumer/types.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.7/async_sqs_consumer/utils/retry.py` & `async_sqs_consumer-0.3.8/async_sqs_consumer/utils/retry.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.7/async_sqs_consumer/worker.py` & `async_sqs_consumer-0.3.8/async_sqs_consumer/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     Queue,
 )
 from async_sqs_consumer.resources import (
     RESOURCE_OPTIONS_SQS,
     SESSION,
 )
 from async_sqs_consumer.utils import (
+    inverse_proportional_distribution,
     TASK_NAME_PREFIX,
     validate_message,
 )
 from async_sqs_consumer.utils.retry import (
     retry_call,
 )
 import asyncio
@@ -20,26 +21,31 @@
     datetime,
 )
 from functools import (
     partial,
 )
 import json
 import logging
+import math
 import pytz
 import signal
 import sys
 from time import (
     sleep,
 )
+from traceback import (
+    print_tb,
+)
 from typing import (
     Any,
     Callable,
     Iterable,
     Literal,
     Optional,
+    Tuple,
 )
 from uuid import (
     uuid4,
 )
 
 logging.basicConfig(level=logging.INFO)
 
@@ -203,14 +209,31 @@
         queue_alias: str,
     ) -> None:
         asyncio.ensure_future(
             self.queues[queue_alias].delete_messages(receipt_handle),
             loop=self._loop,
         )
 
+    def _available_workers_to_consume(self) -> int:
+        current_tasks = [
+            task
+            for task in asyncio.all_tasks(asyncio.get_event_loop())
+            if task.get_name().startswith(TASK_NAME_PREFIX)
+        ]
+        return self._max_workers - len(current_tasks)
+
+    def _get_tasks_by_queue(
+        self, queue_alias: str
+    ) -> Tuple[asyncio.Task, ...]:
+        return tuple(
+            task
+            for task in asyncio.all_tasks(asyncio.get_event_loop())
+            if task.get_name().startswith(f"{TASK_NAME_PREFIX}_{queue_alias}")
+        )
+
     async def queue_message_to_worker(
         self,
         *,
         task_id: Optional[str] = None,
         task_name: Optional[str] = None,
         queue_alias: Optional[str] = None,
         retries: Optional[int] = None,
@@ -240,15 +263,15 @@
             retry_call(
                 handler,
                 fargs=tuple(args or []),
                 fkwargs=kwargs or {},
                 tries=retries or 1,
             ),
             name=(
-                f"{TASK_NAME_PREFIX}{queue_alias}"
+                f"{TASK_NAME_PREFIX}_{queue_alias}"
                 f"_{task_name}_{uuid4().hex[:8]}"
             ),
         )
         task.add_done_callback(
             partial(
                 self._finish_message,
                 receipt_handle=receipt_handler,
@@ -294,27 +317,35 @@
                     message["ReceiptHandle"]
                 )
 
     async def _poll_messages(self) -> None:
         queues = list(sorted(self.queues.items(), key=lambda x: x[1].priority))
         async with SESSION.client(**RESOURCE_OPTIONS_SQS) as sqs_client:
             while True:
-                if len(
-                    [
-                        task
-                        for task in asyncio.all_tasks(asyncio.get_event_loop())
-                        if task.get_name().startswith(TASK_NAME_PREFIX)
-                    ]
-                ) > (self._max_workers):
+                if self._available_workers_to_consume() < 1:
                     await asyncio.sleep(1)
                     continue
-
-                for queue_alias, queue in queues:
-                    messages = await queue.get_messages(sqs_client)
-                    await asyncio.gather(
-                        *[
-                            self._consumer_callback(message, queue_alias)
-                            for message in messages
-                        ]
+                for index, (queue_alias, queue) in enumerate(queues):
+                    required_messages = math.ceil(
+                        inverse_proportional_distribution(
+                            self._available_workers_to_consume(),
+                            [q[1].priority for q in queues[index:]],
+                        )[0]
                     )
-                    if messages:
-                        break
+
+                    # it is necessary to request the messages several times
+                    # because sqs only allows to obtain 10 messages at the
+                    # same time
+                    for _ in range(math.ceil(required_messages / 10)):
+                        messages = await queue.get_messages(
+                            sqs_client,
+                            max_number_of_messages=(required_messages),
+                        )
+
+                        if len(messages) == 0:
+                            break
+                        await asyncio.gather(
+                            *[
+                                self._consumer_callback(message, queue_alias)
+                                for message in messages
+                            ]
+                        )
```

### Comparing `async_sqs_consumer-0.3.7/pyproject.toml` & `async_sqs_consumer-0.3.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async_sqs_consumer"
-version = "0.3.7"
+version = "0.3.8"
 description = ""
 authors = ["Diego Restrepo <drestrepo@fluidattacks.com>"]
 repository = 'https://github.com/drestrepom/async_sqs_consumer'
 readme = "README.md"
 keywords = ["AWS", "AWS", "SQS", "sqs", "consumer", "async", "worker"]
 
 [tool.poetry.dependencies]
```

### Comparing `async_sqs_consumer-0.3.7/setup.py` & `async_sqs_consumer-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'aiohttp>=3.8.4,<4.0.0',
  'jsonschema>=4.17.3,<5.0.0',
  'pyrate-limiter>=2.10.0,<3.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'async-sqs-consumer',
-    'version': '0.3.7',
+    'version': '0.3.8',
     'description': '',
     'long_description': '# Async SQS consumer\n\nPython asynchronous (**async** / **await**) worker for consuming messages\nfrom AWS SQS.\n\nThis is a hobby project, if you find the project interesting\nany contribution is welcome.\n\n## Usage\n\nYou must create an instance of the worker with the url of the queue.\n\nAws credentials are taken from environment variables, you must set the\nfollowing environment variables. Or you can provide a Context object with the\naws credentials `async_sqs_consumer.types.Context`\n\n- `AWS_ACCESS_KEY_ID`\n- `AWS_SECRET_ACCESS_KEY`\n\nExample:\n\nYou can get the queue url with the follow aws cli command\n`aws sqs get-queue-url --queue-name xxxxxx`\n\n```python\n# test_worker.py\n\nfrom async_sqs_consumer.worker import (\n    Worker,\n)\n\nworker = Worker(\n    queue_url="https://sqs.us-east-1.amazonaws.com/xxxxxxx/queue_name"\n)\n\n\n@worker.task("report")\nasync def report(text: str) -> None:\n    print(text)\n\nif __name__: "__main__":\n    worker.start()\n```\n\nNow you can initialize the worker `python test_worker.py`\n\nNow you need to post a message for the worker to process\n\n```python\nimport json\nimport boto3\nimport uuid\n\nclient = boto3.client("sqs")\n\nclient.send_message(\n    QueueUrl="https://sqs.us-east-1.amazonaws.com/xxxxxxx/queue_name",\n    MessageBody=json.dumps(\n        {\n            "task": "report",\n            "id": uuid.uuid4().hex,\n            "args": ["hello world"],\n        }\n    ),\n)\n```\n\nOr you can use aioboto3\n\n```python\nimport asyncio\nimport json\nimport aioboto3\nimport uuid\n\n\nasync def main() -> None:\n    session = aioboto3.Session()\n    async with session.client("sqs") as client:\n        await client.send_message(\n            QueueUrl="https://sqs.us-east-1.amazonaws.com/xxxxxxx/queue_name",\n            MessageBody=json.dumps(\n                {\n                    "task": "report",\n                    "id": uuid.uuid4().hex,\n                    "args": ["hello world"],\n                }\n            ),\n        )\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nTo publish the messages they must have the following structure\n\n```json\n{\n    "type": "object",\n    "properties": {\n        "task": {"type": "string"},\n        "id": {"type": "string"},\n        "args": {"type": "array"},\n        "kwargs": {"type": "object"},\n        "retries": {"type": "number"},\n        "eta": {"type": "string"},\n        "expires": {"type": "string"},\n    },\n    "required": ["task", "id"],\n}\n```\n',
     'author': 'Diego Restrepo',
     'author_email': 'drestrepo@fluidattacks.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/drestrepom/async_sqs_consumer',
```

### Comparing `async_sqs_consumer-0.3.7/PKG-INFO` & `async_sqs_consumer-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-sqs-consumer
-Version: 0.3.7
+Version: 0.3.8
 Summary: 
 Home-page: https://github.com/drestrepom/async_sqs_consumer
 Keywords: AWS,AWS,SQS,sqs,consumer,async,worker
 Author: Diego Restrepo
 Author-email: drestrepo@fluidattacks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

