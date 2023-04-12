# Comparing `tmp/django_google_cloud_tasks-2.1.4.tar.gz` & `tmp/django_google_cloud_tasks-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_google_cloud_tasks-2.1.4.tar", max compression
+gzip compressed data, was "django_google_cloud_tasks-2.1.5.tar", max compression
```

## Comparing `django_google_cloud_tasks-2.1.4.tar` & `django_google_cloud_tasks-2.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11358 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/LICENSE.md
--rw-r--r--   0        0        0      153 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/__init__.py
--rw-r--r--   0        0        0     6245 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/apps.py
--rw-r--r--   0        0        0      446 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/context.py
--rw-r--r--   0        0        0      373 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/exceptions.py
--rw-r--r--   0        0        0     1389 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/field.py
--rw-r--r--   0        0        0        0 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/management/__init__.py
--rw-r--r--   0        0        0      860 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/management/commands/__init__.py
--rw-r--r--   0        0        0      490 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/management/commands/initialize_subscribers.py
--rw-r--r--   0        0        0      394 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/management/commands/initialize_tasks.py
--rw-r--r--   0        0        0      501 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/management/commands/schedule_tasks.py
--rw-r--r--   0        0        0      252 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/middleware/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/middleware/headers_context_middlware.py
--rw-r--r--   0        0        0     1650 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/middleware/pubsub_headers_middleware.py
--rw-r--r--   0        0        0     3888 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/migrations/0001_initial.py
--rw-r--r--   0        0        0     1024 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
--rw-r--r--   0        0        0        0 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/migrations/__init__.py
--rw-r--r--   0        0        0     4364 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/models.py
--rw-r--r--   0        0        0      925 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/serializers.py
--rw-r--r--   0        0        0     2704 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/signals.py
--rw-r--r--   0        0        0      667 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/tasks/__init__.py
--rw-r--r--   0        0        0     1118 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/tasks/periodic_task.py
--rw-r--r--   0        0        0     4775 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/tasks/publisher_task.py
--rw-r--r--   0        0        0     2522 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/tasks/routine_task.py
--rw-r--r--   0        0        0     2382 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/tasks/subscriber_task.py
--rw-r--r--   0        0        0     8812 2023-04-10 12:32:03.850621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/tasks/task.py
--rw-r--r--   0        0        0        0 2023-04-10 12:32:03.854621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/tests/__init__.py
--rw-r--r--   0        0        0      985 2023-04-10 12:32:03.854621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/tests/factories.py
--rw-r--r--   0        0        0      871 2023-04-10 12:32:03.854621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/tests/tests_base.py
--rw-r--r--   0        0        0      291 2023-04-10 12:32:03.854621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/urls.py
--rw-r--r--   0        0        0     2897 2023-04-10 12:32:03.854621 django_google_cloud_tasks-2.1.4/django_cloud_tasks/views.py
--rw-r--r--   0        0        0      772 2023-04-10 12:32:03.854621 django_google_cloud_tasks-2.1.4/pyproject.toml
--rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/LICENSE.md
+-rw-r--r--   0        0        0      153 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/__init__.py
+-rw-r--r--   0        0        0     6245 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/apps.py
+-rw-r--r--   0        0        0      446 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/context.py
+-rw-r--r--   0        0        0      373 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/exceptions.py
+-rw-r--r--   0        0        0     1389 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/field.py
+-rw-r--r--   0        0        0        0 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/management/__init__.py
+-rw-r--r--   0        0        0      860 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/management/commands/__init__.py
+-rw-r--r--   0        0        0      490 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/management/commands/initialize_subscribers.py
+-rw-r--r--   0        0        0      394 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/management/commands/initialize_tasks.py
+-rw-r--r--   0        0        0      501 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/management/commands/schedule_tasks.py
+-rw-r--r--   0        0        0      252 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/middleware/__init__.py
+-rw-r--r--   0        0        0     1179 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/middleware/headers_context_middlware.py
+-rw-r--r--   0        0        0     1870 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/middleware/pubsub_headers_middleware.py
+-rw-r--r--   0        0        0     3888 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1024 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
+-rw-r--r--   0        0        0        0 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/migrations/__init__.py
+-rw-r--r--   0        0        0     4364 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/models.py
+-rw-r--r--   0        0        0      925 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/serializers.py
+-rw-r--r--   0        0        0     2704 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/signals.py
+-rw-r--r--   0        0        0      667 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/__init__.py
+-rw-r--r--   0        0        0     1118 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/periodic_task.py
+-rw-r--r--   0        0        0     4775 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/publisher_task.py
+-rw-r--r--   0        0        0     2522 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/routine_task.py
+-rw-r--r--   0        0        0     2610 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/subscriber_task.py
+-rw-r--r--   0        0        0     8812 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/task.py
+-rw-r--r--   0        0        0        0 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tests/__init__.py
+-rw-r--r--   0        0        0      985 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tests/factories.py
+-rw-r--r--   0        0        0      871 2023-04-12 23:18:32.993646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tests/tests_base.py
+-rw-r--r--   0        0        0      291 2023-04-12 23:18:32.993646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/urls.py
+-rw-r--r--   0        0        0     3014 2023-04-12 23:18:32.993646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/views.py
+-rw-r--r--   0        0        0      772 2023-04-12 23:18:32.993646 django_google_cloud_tasks-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.1.5/PKG-INFO
```

### Comparing `django_google_cloud_tasks-2.1.4/LICENSE.md` & `django_google_cloud_tasks-2.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/apps.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/apps.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/field.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/field.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/management/commands/__init__.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/middleware/headers_context_middlware.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/middleware/headers_context_middlware.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/middleware/pubsub_headers_middleware.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/middleware/pubsub_headers_middleware.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from json import JSONDecodeError
 from typing import Any
 
 from django.apps import apps
 from django.urls import reverse
 from gcp_pilot.pubsub import Message
 
 from django_cloud_tasks.apps import DjangoCloudTasksAppConfig
@@ -37,14 +38,18 @@
         if not task_name:
             return False
 
         expected_url = reverse(self.url_name, args=(task_name,))
         return request.path == expected_url
 
     def extract_headers(self, request) -> dict[str, Any]:
-        message = Message.load(body=request.body)
+        try:
+            message = Message.load(body=request.body)
+        except JSONDecodeError:
+            logger.warning("Message received through PubSub is not a valid JSON. Ignoring PubSub headers feature.")
+            return {}
 
         headers = {}
         for key, value in message.attributes.items():
             if key.startswith(self.pubsub_header_prefix):
                 headers[key.removeprefix(self.pubsub_header_prefix)] = value
         return headers
```

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/migrations/0001_initial.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/models.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/models.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/serializers.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/serializers.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/signals.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/signals.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/tasks/__init__.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/tasks/periodic_task.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/periodic_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/tasks/publisher_task.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/publisher_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/tasks/routine_task.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/routine_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/tasks/subscriber_task.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/subscriber_task.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import abc
+import json
 from urllib.parse import urljoin
+from typing import Callable
 
 from cachetools.func import lru_cache
 from django.urls import reverse
 from gcp_pilot.pubsub import CloudSubscriber
 
 from django_cloud_tasks import UNSET
 from django_cloud_tasks.tasks.task import Task, get_config
@@ -18,14 +20,20 @@
     use_cloud_tasks: bool = False
 
     @abc.abstractmethod
     def run(self, content: dict, attributes: dict[str, str] | None = None):
         raise NotImplementedError()
 
     @classmethod
+    def message_parser(cls) -> Callable:
+        # The callable used to parse the message content
+        # By default, we handle JSON messages
+        return json.loads
+
+    @classmethod
     def set_up(cls):
         return cls._get_subscriber_client().create_or_update_subscription(
             topic_id=cls.topic_name(),
             subscription_id=cls.subscription_name(),
             push_to_url=cls.subscription_url(),
             use_oidc_auth=cls._use_oidc_auth,
             dead_letter_topic_id=cls.dead_letter_topic_name(),
```

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/tasks/task.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/tests/factories.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/tests/tests_base.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tests/tests_base.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.4/django_cloud_tasks/views.py` & `django_google_cloud_tasks-2.1.5/django_cloud_tasks/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def post(self, request, task_name, *args, **kwargs):
         try:
             task_class = self.get_task(name=task_name)
         except TaskNotFound:
             result = {"error": f"Task {task_name} not found"}
             return JsonResponse(status=404, data=result)
 
-        task_kwargs = self.parse_input(request=request)
+        task_kwargs = self.parse_input(request=request, task_class=task_class)
         task_metadata = self.parse_metadata(request=request)
         try:
             output = self.execute_task(task_class=task_class, task_metadata=task_metadata, task_kwargs=task_kwargs)
             data = {"result": output, "status": "executed"}
             status = 200
         except exceptions.DiscardTaskException:
             data = {"status": "discarded"}
@@ -35,25 +35,25 @@
     def get_task(self, name: str) -> Type[Task]:
         app = apps.get_app_config("django_cloud_tasks")
         return app.get_task(name=name)
 
     def execute_task(self, task_class: type[Task], task_metadata: TaskMetadata, task_kwargs: dict) -> Any:
         return task_class(metadata=task_metadata).process(**task_kwargs)
 
-    def parse_input(self, request) -> dict:
+    def parse_input(self, request, task_class: Type[Task]) -> dict:
         return deserialize(value=request.body)
 
     def parse_metadata(self, request) -> TaskMetadata:
         return TaskMetadata.from_headers(headers=dict(request.headers))
 
 
 # More info: https://cloud.google.com/pubsub/docs/push#receiving_messages
 class GoogleCloudSubscribeView(GoogleCloudTaskView):
-    def parse_input(self, request) -> dict:
-        message = Message.load(body=request.body)
+    def parse_input(self, request, task_class: Type[SubscriberTask]) -> dict:
+        message = Message.load(body=request.body, parser=task_class.message_parser())
         return {
             "content": message.data,
             "attributes": message.attributes,
         }
 
     def get_task(self, name: str) -> Type[SubscriberTask]:
         app = apps.get_app_config("django_cloud_tasks")
```

### Comparing `django_google_cloud_tasks-2.1.4/pyproject.toml` & `django_google_cloud_tasks-2.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-google-cloud-tasks"
-version = "2.1.4"
+version = "2.1.5"
 description = "Async Tasks with HTTP endpoints"
 authors = ["Joao Daher <joao@daher.dev>"]
 packages = [
     { include = "django_cloud_tasks" },
 ]
 
 [tool.poetry.dependencies]
```

