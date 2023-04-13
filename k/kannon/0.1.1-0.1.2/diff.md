# Comparing `tmp/kannon-0.1.1.tar.gz` & `tmp/kannon-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kannon-0.1.1.tar", max compression
+gzip compressed data, was "kannon-0.1.2.tar", max compression
```

## Comparing `kannon-0.1.1.tar` & `kannon-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-03-14 05:35:42.219510 kannon-0.1.1/LICENSE
--rw-r--r--   0        0        0     2933 2023-03-14 05:35:42.219510 kannon-0.1.1/README.md
--rw-r--r--   0        0        0       70 2023-03-14 05:35:42.219510 kannon-0.1.1/kannon/__init__.py
--rw-r--r--   0        0        0     1321 2023-03-14 05:35:42.219510 kannon-0.1.1/kannon/kube_util.py
--rw-r--r--   0        0        0     7302 2023-03-14 05:35:42.219510 kannon-0.1.1/kannon/master.py
--rw-r--r--   0        0        0       64 2023-03-14 05:35:42.219510 kannon-0.1.1/kannon/task.py
--rw-r--r--   0        0        0     1662 2023-03-14 05:35:56.667539 kannon-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3771 1970-01-01 00:00:00.000000 kannon-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-13 01:33:16.999551 kannon-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5988 2023-04-13 01:33:16.999551 kannon-0.1.2/README.md
+-rw-r--r--   0        0        0       70 2023-04-13 01:33:16.999551 kannon-0.1.2/kannon/__init__.py
+-rw-r--r--   0        0        0     1229 2023-04-13 01:33:16.999551 kannon-0.1.2/kannon/kube_util.py
+-rw-r--r--   0        0        0     6850 2023-04-13 01:33:16.999551 kannon-0.1.2/kannon/master.py
+-rw-r--r--   0        0        0       64 2023-04-13 01:33:16.999551 kannon-0.1.2/kannon/task.py
+-rw-r--r--   0        0        0     1173 2023-04-13 01:33:32.055549 kannon-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6826 1970-01-01 00:00:00.000000 kannon-0.1.2/PKG-INFO
```

### Comparing `kannon-0.1.1/LICENSE` & `kannon-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kannon-0.1.1/kannon/kube_util.py` & `kannon-0.1.2/kannon/kube_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,35 @@
 import enum
-from time import sleep
-from kubernetes import client
-from datetime import datetime
+import logging
 import random
+from datetime import datetime
 
-import logging
+from kubernetes import client
 
 logger = logging.getLogger(__name__)
 
 
 class JobStatus(enum.Enum):
     RUNNING = 0
     SUCCEEDED = 1
     FAILED = 2
 
 
-def create_job(
-    api_instance: client.BatchV1Api, job: client.V1Job, namespace: str
-) -> None:
+def create_job(api_instance: client.BatchV1Api, job: client.V1Job, namespace: str) -> None:
     api_response = api_instance.create_namespaced_job(
         body=job,
         namespace=namespace,
     )
     logger.debug(f"Job created. status={api_response.status}")
 
-def get_job_status(
-    api_instance: client.BatchV1Api, job_name: str, namespace: str
-) -> JobStatus:
-    api_response = api_instance.read_namespaced_job_status(
-        name=job_name, namespace=namespace
-    )
-    if (
-        api_response.status.succeeded is not None
-        or api_response.status.failed is not None
-    ):
-        final_status = (
-            JobStatus.SUCCEEDED if api_response.status.succeeded else JobStatus.FAILED
-        )
+
+def get_job_status(api_instance: client.BatchV1Api, job_name: str, namespace: str) -> JobStatus:
+    api_response = api_instance.read_namespaced_job_status(name=job_name, namespace=namespace)
+    if (api_response.status.succeeded is not None or api_response.status.failed is not None):
+        final_status = (JobStatus.SUCCEEDED if api_response.status.succeeded else JobStatus.FAILED)
         return final_status
     return JobStatus.RUNNING
 
 
 def gen_job_name(job_prefix: str) -> str:
     job_name = f"{job_prefix}-{str(random.randint(0, 255)).zfill(3)}-{datetime.now().strftime('%Y%m%d%H%M%S')}"
     # TODO: validate job_name more precisely
```

### Comparing `kannon-0.1.1/kannon/master.py` & `kannon-0.1.2/kannon/master.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,203 +1,171 @@
-from collections import deque
+import logging
 import os
+from collections import deque
+from copy import deepcopy
 from time import sleep
-from typing import Deque, Dict, List, Set
-import logging
+from typing import Deque, Dict, List, Optional, Set
 
 import gokart
 from kubernetes import client
+from luigi.task import flatten
 
+from .kube_util import JobStatus, create_job, gen_job_name, get_job_status
 from .task import TaskOnBullet
-from .kube_util import create_job, JobStatus, gen_job_name, get_job_status
-
 
 logger = logging.getLogger(__name__)
 
 
 class Kannon:
+
     def __init__(
         self,
+        # k8s resources
         api_instance: client.BatchV1Api,
-        namespace: str,
-        image_name: str,
-        container_name: str,
-        service_account_name: str,
+        template_job: client.V1Job,
+        # kannon resources
         job_prefix: str,
-        path_child_script: str,
-        env_to_inherit: List[str],
-        backoff_limit: int = 0,
+        path_child_script: str = "./run_child.py",
+        env_to_inherit: Optional[List[str]] = None,
     ) -> None:
         # validation
         if not os.path.exists(path_child_script):
             raise FileNotFoundError(f"Child script {path_child_script} does not exist.")
-        if backoff_limit < 0:
-            raise ValueError(f"backoff_limit should be >= 0")
+
+        self.template_job = template_job
         self.api_instance = api_instance
-        self.namespace = namespace
-        self.image_name = image_name
-        self.container_name = container_name
-        self.service_account_name = service_account_name
+        self.namespace = template_job.metadata.namespace
         self.job_prefix = job_prefix
         self.path_child_script = path_child_script
+        if env_to_inherit is None:
+            env_to_inherit = ["TASK_WORKSPACE_DIRECTORY"]
         self.env_to_inherit = env_to_inherit
-        self.backoff_limit = backoff_limit
 
         self.task_id_to_job_name: Dict[str, str] = dict()
 
     def build(self, root_task: gokart.TaskOnKart):
         # push tasks into queue
         logger.info("Creating task queue...")
         task_queue = self._create_task_queue(root_task)
 
         # consume task queue
         launched_task_ids: Set[str] = set()
         logger.info("Consuming task queue...")
         while task_queue:
             task = task_queue.popleft()
             if task.complete():
-                logger.info(f"Task {self._gen_task_info(task)} is already done.")
+                logger.info(f"Task {self._gen_task_info(task)} is already completed.")
                 continue
             if task.make_unique_id() in launched_task_ids:
-                logger.info(f"Task {self._gen_task_info(task)} is already running.")
+                logger.info(f"Task {self._gen_task_info(task)} is still running on child job.")
+                task_queue.append(task)
                 continue
 
-            logger.info(
-                f"Checking if task {self._gen_task_info(task)} is executable..."
-            )
             # TODO: enable user to specify duration to sleep for each task
             sleep(1.0)
+            logger.info(f"Checking if task {self._gen_task_info(task)} is executable...")
             if not self._is_executable(task):
-                task_queue.append(task)
+                task_queue.append(task)  # re-enqueue task to check if it's executable later
+                logger.debug("Task is not executable yet. Re-enqueue task.")
                 continue
             # execute task
             if isinstance(task, TaskOnBullet):
-                logger.info(
-                    f"Trying to run task {self._gen_task_info(task)} on child job..."
-                )
+                logger.info(f"Trying to run task {self._gen_task_info(task)} on child job...")
                 self._exec_bullet_task(task)
+                launched_task_ids.add(task.make_unique_id())  # mark as already launched task
+                task_queue.append(task)  # re-enqueue task to check if it is done
             elif isinstance(task, gokart.TaskOnKart):
-                logger.info(
-                    f"Executing task {self._gen_task_info(task)} on master job..."
-                )
+                logger.info(f"Executing task {self._gen_task_info(task)} on master job...")
                 self._exec_gokart_task(task)
-                logger.info(
-                    f"Completed task {self._gen_task_info(task)} on master job."
-                )
+                logger.info(f"Completed task {self._gen_task_info(task)} on master job.")
             else:
                 raise TypeError(f"Invalid task type: {type(task)}")
-            launched_task_ids.add(task.make_unique_id())
 
-        logger.info(f"All tasks completed!")
+        logger.info("All tasks completed!")
 
-    def _create_task_queue(
-        self, root_task: gokart.TaskOnKart
-    ) -> Deque[gokart.TaskOnKart]:
+    def _create_task_queue(self, root_task: gokart.TaskOnKart) -> Deque[gokart.TaskOnKart]:
         task_queue: Deque[gokart.TaskOnKart] = deque()
 
         def _rec_enqueue_task(task: gokart.TaskOnKart) -> None:
             """Traversal task tree in post-order to push tasks into task queue."""
             nonlocal task_queue
             # run children
-            children = task.requires()
-            if isinstance(children, dict):
-                children = children.values()
+            children = flatten(task.requires())
             for child in children:
                 _rec_enqueue_task(child)
 
             task_queue.append(task)
             logger.info(f"Task {self._gen_task_info(task)} is pushed to task queue")
 
         _rec_enqueue_task(root_task)
         return task_queue
 
     def _exec_gokart_task(self, task: gokart.TaskOnKart) -> None:
         # Run on master job
         try:
             gokart.build(task)
         except Exception:
-            raise RuntimeError(
-                f"Task {self._gen_task_info(task)} on job master has failed."
-            )
+            raise RuntimeError(f"Task {self._gen_task_info(task)} on job master has failed.")
 
     def _exec_bullet_task(self, task: TaskOnBullet) -> None:
         # Run on child job
         serialized_task = gokart.TaskInstanceParameter().serialize(task)
         job_name = gen_job_name(f"{self.job_prefix}-{task.get_task_family()}")
-        job = self._create_job_object(
+        job = self._create_child_job_object(
             job_name=job_name,
             serialized_task=serialized_task,
         )
         create_job(self.api_instance, job, self.namespace)
-        logger.info(
-            f"Created child job {job_name} with task {self._gen_task_info(task)}"
-        )
+        logger.info(f"Created child job {job_name} with task {self._gen_task_info(task)}")
         task_unique_id = task.make_unique_id()
         self.task_id_to_job_name[task_unique_id] = job_name
 
-    @staticmethod
-    def _gen_task_info(task: gokart.TaskOnKart) -> str:
-        return f"{task.get_task_family()}_{task.make_unique_id()}"
-
-    def _create_job_object(self, serialized_task: str, job_name: str) -> client.V1Job:
+    def _create_child_job_object(self, job_name: str, serialized_task: str) -> client.V1Job:
         # TODO: use python -c to avoid dependency to execute_task.py
         cmd = [
             "python",
             self.path_child_script,
             "--serialized-task",
             f"'{serialized_task}'",
         ]
-        child_envs = []
+        job = deepcopy(self.template_job)
+        # replace command
+        assert job.spec.template.spec.containers[0].command is None, \
+            "command will be replaced by kannon, so you shouldn't set any command and args"
+        job.spec.template.spec.containers[0].command = cmd
+        # replace env
+        child_envs = job.spec.template.spec.containers[0].env
+        if not child_envs:
+            child_envs = []
         for env_name in self.env_to_inherit:
             if env_name not in os.environ:
                 raise ValueError(f"Envvar {env_name} does not exist.")
             child_envs.append({"name": env_name, "value": os.environ.get(env_name)})
-        container = client.V1Container(
-            name=self.container_name,
-            image=self.image_name,
-            command=cmd,
-            env=child_envs,
-        )
-        template = client.V1PodTemplateSpec(
-            metadata=client.V1ObjectMeta(labels={"app": "kannon"}),
-            spec=client.V1PodSpec(
-                restart_policy="Never",
-                containers=[container],
-                service_account_name=self.service_account_name,
-            ),
-        )
-        spec = client.V1JobSpec(template=template, backoff_limit=self.backoff_limit)
-        job = client.V1Job(
-            api_version="batch/v1",
-            kind="Job",
-            metadata=client.V1ObjectMeta(
-                name=job_name,
-                namespace=self.namespace,
-            ),
-            spec=spec,
-        )
+        job.spec.template.spec.containers[0].env = child_envs
+        # replace job name
+        job.metadata.name = job_name
 
         return job
 
+    @staticmethod
+    def _gen_task_info(task: gokart.TaskOnKart) -> str:
+        return f"{task.get_task_family()}_{task.make_unique_id()}"
+
     def _is_executable(self, task: gokart.TaskOnKart) -> bool:
-        children = task.requires()
-        if isinstance(children, dict):
-            children = children.values()
+        children = flatten(task.requires())
 
         for child in children:
             if not child.complete():
                 return False
             if child.make_unique_id() not in self.task_id_to_job_name:
                 continue
             job_name = self.task_id_to_job_name[child.make_unique_id()]
             job_status = get_job_status(
                 self.api_instance,
                 job_name,
                 self.namespace,
             )
             if job_status == JobStatus.FAILED:
-                raise RuntimeError(
-                    f"Task {self._gen_task_info(child)} on job {job_name} has failed."
-                )
+                raise RuntimeError(f"Task {self._gen_task_info(child)} on job {job_name} has failed.")
             if job_status == JobStatus.RUNNING:
                 return False
         return True
```

