# Comparing `tmp/vdk-meta-jobs-0.1.833741966.tar.gz` & `tmp/vdk-meta-jobs-0.1.836044868.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-meta-jobs-0.1.833741966.tar", last modified: Tue Apr 11 12:13:05 2023, max compression
+gzip compressed data, was "vdk-meta-jobs-0.1.836044868.tar", last modified: Thu Apr 13 09:30:52 2023, max compression
```

## Comparing `vdk-meta-jobs-0.1.833741966.tar` & `vdk-meta-jobs-0.1.836044868.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.888825 vdk-meta-jobs-0.1.833741966/
--rw-r--r--   0 root         (0) root         (0)     6645 2023-04-11 12:13:05.888825 vdk-meta-jobs-0.1.833741966/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6072 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 12:13:05.888825 vdk-meta-jobs-0.1.833741966/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1457 2023-04-11 12:12:57.000000 vdk-meta-jobs-0.1.833741966/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.884825 vdk-meta-jobs-0.1.833741966/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.884825 vdk-meta-jobs-0.1.833741966/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.884825 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.888825 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.888825 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/api/
--rw-rw-rw-   0 root         (0) root         (0)      738 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/api/meta_job.py
--rw-rw-rw-   0 root         (0) root         (0)     8320 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/cached_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     7948 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/dag_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2082 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     4522 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/meta_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5710 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/meta_dag.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/meta_job_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/plugin_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     9041 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/remote_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1663 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/remote_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     2332 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/time_based_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.888825 vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6645 2023-04-11 12:13:05.000000 vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      859 2023-04-11 12:13:05.000000 vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 12:13:05.000000 vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-11 12:13:05.000000 vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-11 12:13:05.000000 vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-11 12:13:05.000000 vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.888825 vdk-meta-jobs-0.1.833741966/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2624 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/tests/test_meta_dag.py
--rw-rw-rw-   0 root         (0) root         (0)    15107 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/tests/test_meta_job.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/tests/test_time_based_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2303 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/tests/test_tracking_job_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.977267 vdk-meta-jobs-0.1.836044868/
+-rw-r--r--   0 root         (0) root         (0)     6645 2023-04-13 09:30:52.977267 vdk-meta-jobs-0.1.836044868/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6072 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 09:30:52.977267 vdk-meta-jobs-0.1.836044868/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2023-04-13 09:30:42.000000 vdk-meta-jobs-0.1.836044868/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.973267 vdk-meta-jobs-0.1.836044868/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.973267 vdk-meta-jobs-0.1.836044868/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.973267 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.977267 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.977267 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1402 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/api/meta_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     9347 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/cached_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7949 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/dag_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/dags_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2269 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     6713 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/meta_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     6148 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/meta_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/meta_job_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     9344 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/remote_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1743 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/remote_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2579 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/time_based_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.977267 vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6645 2023-04-13 09:30:52.000000 vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      858 2023-04-13 09:30:52.000000 vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 09:30:52.000000 vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-13 09:30:52.000000 vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-13 09:30:52.000000 vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-13 09:30:52.000000 vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.977267 vdk-meta-jobs-0.1.836044868/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/tests/test_meta_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)    15096 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/tests/test_meta_job.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/tests/test_time_based_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2303 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/tests/test_tracking_job_executor.py
```

### Comparing `vdk-meta-jobs-0.1.833741966/PKG-INFO` & `vdk-meta-jobs-0.1.836044868/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-meta-jobs
-Version: 0.1.833741966
+Version: 0.1.836044868
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-meta-jobs-0.1.833741966/README.md` & `vdk-meta-jobs-0.1.836044868/README.md`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.833741966/setup.py` & `vdk-meta-jobs-0.1.836044868/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.833741966"
+__version__ = "0.1.836044868"
 
 setuptools.setup(
     name="vdk-meta-jobs",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Express dependecies between data jobs.",
     long_description=pathlib.Path("README.md").read_text(),
@@ -25,15 +25,15 @@
         "vdk-control-service-api",
         "urllib3",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_namespace_packages(where="src"),
     # This is the only vdk plugin specifc part
     # Define entry point called "vdk.plugin.run" with name of plugin and module to act as entry point.
-    entry_points={"vdk.plugin.run": ["meta-jobs = vdk.plugin.meta_jobs.plugin_entry"]},
+    entry_points={"vdk.plugin.run": ["meta-jobs = vdk.plugin.meta_jobs.dags_plugin"]},
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/cached_data_job_executor.py` & `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/cached_data_job_executor.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,31 +18,49 @@
 
 ACTIVE_JOB_STATUSES = [JobStatus.SUBMITTED.value, JobStatus.RUNNING.value]
 SLEEP_TIME = 10
 ALLOWED_RETRIES = 3
 
 
 class TrackingDataJobExecutor:
+    """
+    The purpose of this class is to execute Data Jobs, track them and change their
+    statuses accordingly.
+    """
+
     def __init__(
         self, executor: IDataJobExecutor, time_between_status_check_seconds: int
     ):
+        """
+
+        :param executor: the Data Job executor
+        :param time_between_status_check_seconds: the number of seconds between status check
+        """
         self._executor = executor
         self._jobs_cache: Dict[str, TrackableJob] = dict()
         self._time_between_status_check_seconds = time_between_status_check_seconds
 
     def register_job(self, job: TrackableJob):
+        """
+        Registers a Data Job by adding it to the cache.
+
+        :param job: the job to be added to the cache
+        :return:
+        """
         if job.job_name in self._jobs_cache:
             log.warning(
-                f"Job with name {job.job_name} aleady exists. Details: {self._jobs_cache[job.job_name]}. "
+                f"Job with name {job.job_name} already exists. Details: {self._jobs_cache[job.job_name]}. "
                 f"Will overwrite it."
             )
         self._jobs_cache[job.job_name] = job
 
     def start_job(self, job_name: str) -> None:
         """
+        Starts a Data Job.
+
         :param job_name: the job to start and track
         """
         job = self.__get_job(job_name)
         job.start_attempt += 1
         execution_id = self.start_new_job_execution(
             job_name=job.job_name, team_name=job.team_name, arguments=job.arguments
         )
@@ -53,14 +71,20 @@
             job.job_name, job.team_name, job.execution_id
         )
         log.info(
             f"Started data job {job_name}:\n{self.__get_printable_details(job.details)}"
         )
 
     def finalize_job(self, job_name):
+        """
+        Finalizes a finished job by updating its details and logging them or raising an error.
+
+        :param job_name: the name of the job
+        :return:
+        """
         job = self.__get_job(job_name)
         details = self._executor.details_job(
             job.job_name, job.team_name, job.execution_id
         )
         job.details = details
         log.info(
             f"Finished data job {job_name}:\n"
@@ -96,23 +120,32 @@
         return job
 
     @staticmethod
     def __is_job_submitted(job: TrackableJob):
         return job.status is not None
 
     def status(self, job_name: str) -> str:
+        """
+        Gets the status of a job.
+
+        :param job_name: the name of the job
+        :return: the job status
+        """
         job = self.__get_job(job_name)
         if job.status in ACTIVE_JOB_STATUSES:
             job.status = self._executor.status_job(
                 job.job_name, job.team_name, job.execution_id
             )
         log.debug(f"Job status: {job}")
         return job.status
 
     def get_finished_job_names(self):
+        """
+        :return: list of the names of all the finalized jobs
+        """
         finalized_jobs = []
         # TODO: optimize
         # Do not call the status every time (use TTL caching)
         # Do not call all status at the same time - stagger them in time
         # Or use GraphQL API to get status at once (batch)
         for job in self._jobs_cache.values():
             if (
@@ -126,17 +159,23 @@
 
         for job in self._jobs_cache.values():
             if self.__is_job_submitted(job) and job.status not in ACTIVE_JOB_STATUSES:
                 finalized_jobs.append(job.job_name)
         return finalized_jobs
 
     def get_all_jobs(self):
+        """
+        :return: list of all jobs
+        """
         return list(self._jobs_cache.values())
 
     def get_currently_running_jobs(self):
+        """
+        :return: list of jobs with current status SUBMITTED or RUNNING
+        """
         return [j for j in self._jobs_cache.values() if j.status in ACTIVE_JOB_STATUSES]
 
     def start_new_job_execution(
         self, job_name: str, team_name: str, arguments: IJobArguments = None
     ) -> str:
         """
         Start a new data job execution.
```

### Comparing `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/dag_validator.py` & `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/dag_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     The purpose of this class is to validate the DAG structure and jobs.
     It is being used right before the DAG is built.
     """
 
     def validate(self, jobs: List[Dict]):
         """
         Validate the structure and the order of the DAG of Data Jobs.
+
         :param jobs: List of Data Jobs (DAG vertices) to be validated
         :return:
         """
         self._validate_no_duplicates(jobs)
         for job in jobs:
             self._validate_job(job)
         self._check_dag_cycles(jobs)
```

### Comparing `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/meta.py` & `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 from taurus_datajob_api import DataJobExecution
 from vdk.api.job_input import IJobArguments
 from vdk.plugin.meta_jobs.api import meta_job
 
 
 class IDataJobExecutor(abc.ABC):
+    """
+    This module is responsible for the execution of Data Jobs.
+    """
+
     @abc.abstractmethod
     def start_job(self, job_name: str, team_name: str, arguments: IJobArguments = None):
         """
         Start an execution of a data job and returns its execution id
         :param arguments:
         :param job_name:
         :param team_name:
@@ -56,12 +60,16 @@
         :return: A list of DataJobExecution objects.
         """
         pass
 
 
 @dataclass
 class TrackableJob(meta_job.SingleJob):
+    """
+    This class provides the ability to track status details of Data Job during execution.
+    """
+
     status: str = None
     execution_id: str = None
     details: dict = None
     start_attempt = 0
     last_status_time = 0
```

### Comparing `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/meta_configuration.py` & `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/meta_configuration.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,34 +17,75 @@
 
 
 class MetaPluginConfiguration:
     def __init__(self, config: Configuration):
         self.__config = config
 
     def meta_jobs_delayed_jobs_min_delay_seconds(self):
+        """
+        Returns the minimum delay time for a delayed job to be executed in seconds.
+
+        :return: the number of seconds for the minimum delay of a delayed job
+
+        :seealso: `META_JOBS_DELAYED_JOBS_MIN_DELAY_SECONDS <https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-meta-jobs/src/vdk/plugin/meta_jobs/meta_configuration.py#L90>`
+        """
         return self.__config.get_value(META_JOBS_DELAYED_JOBS_MIN_DELAY_SECONDS)
 
     def meta_jobs_delayed_jobs_randomized_added_delay_seconds(self):
+        """
+        Returns the additional randomized delay time in seconds to the minimum delay time of a delayed job.
+
+        :return: the number of seconds for the additional randomized delay of the delayed jobs
+
+        :seealso: `META_JOBS_DELAYED_JOBS_RANDOMIZED_ADDED_DELAY_SECONDS <https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-meta-jobs/src/vdk/plugin/meta_jobs/meta_configuration.py#L100>`
+        """
         return self.__config.get_value(
             META_JOBS_DELAYED_JOBS_RANDOMIZED_ADDED_DELAY_SECONDS
         )
 
     def meta_jobs_dag_execution_check_time_period_seconds(self):
+        """
+        Returns the frequency at which the system checks a DAG execution's status.
+
+        :return: the frequency in seconds at which the system checks a DAG execution's status
+
+        :seealso: `META_JOBS_DAG_EXECUTION_CHECK_TIME_PERIOD_SECONDS <https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-meta-jobs/src/vdk/plugin/meta_jobs/meta_configuration.py#L111>`
+        """
         return self.__config.get_value(
             META_JOBS_DAG_EXECUTION_CHECK_TIME_PERIOD_SECONDS
         )
 
     def meta_jobs_time_between_status_check_seconds(self):
+        """
+        Returns the time interval in seconds between status checks for a job.
+
+        :return: the number of seconds between status checks for a job.
+
+        :seealso: `META_JOBS_TIME_BETWEEN_STATUS_CHECK_SECONDS <https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-meta-jobs/src/vdk/plugin/meta_jobs/meta_configuration.py#L121>`
+        """
         return self.__config.get_value(META_JOBS_TIME_BETWEEN_STATUS_CHECK_SECONDS)
 
     def meta_jobs_max_concurrent_running_jobs(self):
+        """
+        Returns the limit of concurrent running jobs.
+
+        :return: the number of maximum concurrent running jobs
+
+        :seealso: `META_JOBS_MAX_CONCURRENT_RUNNING_JOBS <https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-meta-jobs/src/vdk/plugin/meta_jobs/meta_configuration.py#L132>`
+        """
         return self.__config.get_value(META_JOBS_MAX_CONCURRENT_RUNNING_JOBS)
 
 
 def add_definitions(config_builder: ConfigurationBuilder):
+    """
+    Defines what configuration settings are needed for the DAGs plugin with reasonable defaults.
+
+    :param config_builder: the builder used to add the configuration variables
+    :return:
+    """
     config_builder.add(
         key=META_JOBS_DELAYED_JOBS_MIN_DELAY_SECONDS,
         default_value=30,
         description=(
             "This sets the minimum delay time for a delayed job to be executed. "
             "Delayed jobs are not scheduled to run immediately due to issues such as "
             "server errors or concurrent job limits. For instance, a delay time of 30 "
```

### Comparing `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/meta_dag.py` & `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/meta_dag.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,21 @@
 from vdk.plugin.meta_jobs.remote_data_job_executor import RemoteDataJobExecutor
 from vdk.plugin.meta_jobs.time_based_queue import TimeBasedQueue
 
 log = logging.getLogger(__name__)
 
 
 class MetaJobsDag:
-    def __init__(
-        self,
-        team_name: str,
-        meta_config: MetaPluginConfiguration,
-    ):
+    def __init__(self, team_name: str, meta_config: MetaPluginConfiguration):
+        """
+        This module deals with all the DAG-related operations such as build and execute.
+
+        :param team_name: the name of the owning team
+        :param meta_config: the DAG job configuration
+        """
         self._team_name = team_name
         self._topological_sorter = TopologicalSorter()
         self._delayed_starting_jobs = TimeBasedQueue(
             min_ready_time_seconds=meta_config.meta_jobs_delayed_jobs_min_delay_seconds(),
             randomize_delay_seconds=meta_config.meta_jobs_delayed_jobs_randomized_added_delay_seconds(),
         )
         self._max_concurrent_running_jobs = (
@@ -43,26 +45,37 @@
         self._job_executor = TrackingDataJobExecutor(
             executor=RemoteDataJobExecutor(),
             time_between_status_check_seconds=meta_config.meta_jobs_time_between_status_check_seconds(),
         )
         self._dag_validator = DagValidator()
 
     def build_dag(self, jobs: List[Dict]):
+        """
+        Validate the jobs and build a DAG based on their dependency lists.
+
+        :param jobs: the jobs that are part of the DAG
+        :return:
+        """
         self._dag_validator.validate(jobs)
         for job in jobs:
             trackable_job = TrackableJob(
                 job["job_name"],
                 job.get("team_name", self._team_name),
                 job.get("fail_meta_job_on_error", True),
                 job.get("arguments", None),
             )
             self._job_executor.register_job(trackable_job)
             self._topological_sorter.add(trackable_job.job_name, *job["depends_on"])
 
     def execute_dag(self):
+        """
+        Execute the DAG of jobs.
+
+        :return:
+        """
         self._topological_sorter.prepare()
         while self._topological_sorter.is_active():
             for node in self._topological_sorter.get_ready():
                 self._start_job(node)
             self._start_delayed_jobs()
             finished_jobs = self._get_finished_jobs()
             self._finalize_jobs(finished_jobs)
```

### Comparing `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/plugin_entry.py` & `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/dags_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,13 +23,16 @@
         meta_job_runner.META_CONFIG = MetaPluginConfiguration(
             context.core_context.configuration
         )
 
     @staticmethod
     @hookimpl
     def vdk_configure(config_builder: ConfigurationBuilder) -> None:
+        """
+        Here we define what configuration settings are needed for DAGs with reasonable defaults.
+        """
         add_definitions(config_builder)
 
 
 @hookimpl
 def vdk_start(plugin_registry: IPluginRegistry, command_line_args: List):
     plugin_registry.load_plugin_with_hooks_impl(MetaJobsPlugin(), "MetaJobsPlugin")
```

### Comparing `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/remote_data_job.py` & `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/remote_data_job.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,26 +38,35 @@
     SKIPPED = "skipped"
     USER_ERROR = "user_error"
     PLATFORM_ERROR = "platform_error"
 
 
 class RemoteDataJob:
     """
-    Interact with Verstile Data Kit (VDK) Control Service
+    Interact with Versatile Data Kit (VDK) Control Service
     """
 
     def __init__(
         self,
         job_name: str,
         team_name: str,
         rest_api_url: str,
         arguments: IJobArguments = None,
         timeout: int = 5,  # TODO: Set reasonable default
         **kwargs,
     ) -> None:
+        """
+
+        :param job_name: the name of the job
+        :param team_name: the name of the owning team
+        :param rest_api_url: the Control Service REST API URL
+        :param arguments: the job arguments
+        :param timeout: timeout
+        :param kwargs: extra parameters
+        """
         self.__job_name = job_name
         self.__team_name = team_name
         self.__rest_api_url = rest_api_url
         self.__arguments = arguments
         self.timeout = timeout
         self.deployment_id = "production"  # currently multiple deployments are not supported so this remains hardcoded
         self.auth: Optional[Authentication] = kwargs.pop("auth", None)
```

### Comparing `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/remote_data_job_executor.py` & `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/remote_data_job_executor.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from vdk.api.job_input import IJobArguments
 from vdk.internal.control.configuration.vdk_config import VDKConfig
 from vdk.plugin.meta_jobs.meta import IDataJobExecutor
 from vdk.plugin.meta_jobs.remote_data_job import RemoteDataJob
 
 
 class RemoteDataJobExecutor(IDataJobExecutor):
+    """
+    This module is responsible for executing remote Data Jobs.
+    """
+
     def start_job(self, job_name: str, team_name: str, arguments: IJobArguments = None):
         vdk_cfg = VDKConfig()
         job = RemoteDataJob(
             job_name, team_name, vdk_cfg.control_service_rest_api_url, arguments
         )
         return job.start_job_execution()
         # catch error on 409
```

### Comparing `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/time_based_queue.py` & `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/time_based_queue.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,21 @@
         """
         self._elements: deque[_QueueEntry] = deque()
         self._min_ready_time_seconds = min_ready_time_seconds
         self._randomize_delay_seconds = randomize_delay_seconds
         self._dequeue_timeout_seconds = dequeue_timeout_seconds
 
     def enqueue(self, element):
+        """
+        Adds an element to the queue.
+
+        :param element: the element to be added to the queue
+        :type typing.Any
+        :return:
+        """
         ready_time = self._min_ready_time_seconds + randint(
             0, self._randomize_delay_seconds
         )
         self._elements.append(_QueueEntry(element, time.time() + ready_time))
 
     def dequeue(self):
         """
@@ -54,13 +61,18 @@
             else:
                 self.__wait_for_entry_to_be_ready(entry.ready_time)
                 if entry.ready_time <= time.time():
                     return self._elements.popleft().element
         return None
 
     def size(self):
+        """
+        Returns the size of the queue.
+
+        :return:
+        """
         return len(self._elements)
 
     def __wait_for_entry_to_be_ready(self, ready_time: float):
         sleep_time_seconds = ready_time - time.time()
         sleep_time_seconds = min(sleep_time_seconds, self._dequeue_timeout_seconds)
         time.sleep(sleep_time_seconds)
```

### Comparing `vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/PKG-INFO` & `vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-meta-jobs
-Version: 0.1.833741966
+Version: 0.1.836044868
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/SOURCES.txt` & `vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 README.md
 setup.py
 src/vdk/plugin/meta_jobs/cached_data_job_executor.py
 src/vdk/plugin/meta_jobs/dag_validator.py
+src/vdk/plugin/meta_jobs/dags_plugin.py
 src/vdk/plugin/meta_jobs/meta.py
 src/vdk/plugin/meta_jobs/meta_configuration.py
 src/vdk/plugin/meta_jobs/meta_dag.py
 src/vdk/plugin/meta_jobs/meta_job_runner.py
-src/vdk/plugin/meta_jobs/plugin_entry.py
 src/vdk/plugin/meta_jobs/remote_data_job.py
 src/vdk/plugin/meta_jobs/remote_data_job_executor.py
 src/vdk/plugin/meta_jobs/time_based_queue.py
 src/vdk/plugin/meta_jobs/api/meta_job.py
 src/vdk_meta_jobs.egg-info/PKG-INFO
 src/vdk_meta_jobs.egg-info/SOURCES.txt
 src/vdk_meta_jobs.egg-info/dependency_links.txt
```

### Comparing `vdk-meta-jobs-0.1.833741966/tests/test_meta_dag.py` & `vdk-meta-jobs-0.1.836044868/tests/test_meta_dag.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.833741966/tests/test_meta_job.py` & `vdk-meta-jobs-0.1.836044868/tests/test_meta_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from unittest import mock
 
 from click.testing import Result
 from pytest_httpserver.pytest_plugin import PluginHTTPServer
 from taurus_datajob_api import DataJobDeployment
 from taurus_datajob_api import DataJobExecution
 from vdk.internal.core.errors import UserCodeError
-from vdk.plugin.meta_jobs import plugin_entry
+from vdk.plugin.meta_jobs import dags_plugin
 from vdk.plugin.test_utils.util_funcs import cli_assert_equal
 from vdk.plugin.test_utils.util_funcs import CliEntryBasedTestRunner
 from vdk.plugin.test_utils.util_funcs import jobs_path_from_caller_directory
 from werkzeug import Request
 from werkzeug import Response
 
 
@@ -146,15 +146,15 @@
 
     def test_meta_job(self):
         self._set_up()
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
-            self.runner = CliEntryBasedTestRunner(plugin_entry)
+            self.runner = CliEntryBasedTestRunner(dags_plugin)
             result = self._run_meta_job("meta-job")
             cli_assert_equal(0, result)
             self.httpserver.stop()
 
     def test_meta_job_error(self):
         jobs = [
             ("job1", [200], "succeeded"),
@@ -163,15 +163,15 @@
             ("job4", [200], "succeeded"),
         ]
         self._set_up(jobs)
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
-            self.runner = CliEntryBasedTestRunner(plugin_entry)
+            self.runner = CliEntryBasedTestRunner(dags_plugin)
             result = self._run_meta_job("meta-job")
             cli_assert_equal(1, result)
             self.httpserver.stop()
 
     def test_meta_job_fail_false(self):
         jobs = [
             ("job1", [200], "succeeded"),
@@ -180,15 +180,15 @@
             ("job4", [200], "succeeded"),
         ]
         self._set_up(jobs)
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
-            self.runner = CliEntryBasedTestRunner(plugin_entry)
+            self.runner = CliEntryBasedTestRunner(dags_plugin)
             result = self._run_meta_job("meta-job")
             cli_assert_equal(0, result)
             self.httpserver.stop()
 
     def test_meta_job_conflict(self):
         jobs = [
             ("job1", [409, 200], "succeeded"),
@@ -201,15 +201,15 @@
             "VDK_META_JOBS_DELAYED_JOBS_MIN_DELAY_SECONDS": "0",
         }
         self._set_up(jobs, env_vars)
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
-            self.runner = CliEntryBasedTestRunner(plugin_entry)
+            self.runner = CliEntryBasedTestRunner(dags_plugin)
             result = self._run_meta_job("meta-job")
             cli_assert_equal(0, result)
             self.httpserver.stop()
 
     def test_meta_job_cannot_start_job(self):
         jobs = [
             ("job1", [401, 200], "succeeded"),
@@ -218,15 +218,15 @@
             ("job4", [200], "succeeded"),
         ]
         self._set_up(jobs)
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
-            self.runner = CliEntryBasedTestRunner(plugin_entry)
+            self.runner = CliEntryBasedTestRunner(dags_plugin)
             result = self._run_meta_job("meta-job")
             cli_assert_equal(1, result)
             # we should have 2 requests in the log, one to get a list
             # of all executions, and one for the failing data job
             # no other request should be tried as the meta job fails
             assert len(self.httpserver.log) == 2
             self.httpserver.stop()
@@ -244,15 +244,15 @@
             "VDK_META_JOBS_DAG_EXECUTION_CHECK_TIME_PERIOD_SECONDS": "0",
         }
         self._set_up(jobs, env_vars)
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
-            self.runner = CliEntryBasedTestRunner(plugin_entry)
+            self.runner = CliEntryBasedTestRunner(dags_plugin)
             result = self._run_meta_job("meta-job")
             cli_assert_equal(0, result)
             job1_requests = [
                 req
                 for req, res in self.httpserver.log
                 if req.method == "GET" and req.base_url.endswith("job1")
             ]
@@ -278,15 +278,15 @@
             "VDK_META_JOBS_TIME_BETWEEN_STATUS_CHECK_SECONDS": "1",
         }
         self._set_up(jobs, env_vars)
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
-            self.runner = CliEntryBasedTestRunner(plugin_entry)
+            self.runner = CliEntryBasedTestRunner(dags_plugin)
             result = self._run_meta_job("meta-job-exceed-limit")
             expected_max_running_jobs = int(
                 os.getenv("VDK_META_JOBS_MAX_CONCURRENT_RUNNING_JOBS", "2")
             )
             # keep track of the number of running jobs at any given time
             running_jobs = set()
             for request, response in self.httpserver.log:
@@ -308,15 +308,15 @@
 
     def _test_meta_job_validation(self, meta_job_name):
         self._set_up()
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
-            self.runner = CliEntryBasedTestRunner(plugin_entry)
+            self.runner = CliEntryBasedTestRunner(dags_plugin)
             result = self._run_meta_job(meta_job_name)
             cli_assert_equal(1, result)
             self._assert_meta_job_fails_with_error(result, UserCodeError)
             self.httpserver.stop()
 
     def test_meta_job_circular_dependency(self):
         self._test_meta_job_validation("meta-job-circular-dep")
@@ -335,29 +335,29 @@
 
     def test_meta_job_arguments(self):
         self._set_up()
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
-            self.runner = CliEntryBasedTestRunner(plugin_entry)
+            self.runner = CliEntryBasedTestRunner(dags_plugin)
             result = self._run_meta_job("dag-arguments")
             cli_assert_equal(0, result)
             job2_arguments = self._get_job_arguments("job2")
             assert len(job2_arguments) == 2
             assert job2_arguments == {"table_name": "test_table", "counter": 123}
             self.httpserver.stop()
 
     def test_meta_job_empty_arguments(self):
         self._set_up()
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
-            self.runner = CliEntryBasedTestRunner(plugin_entry)
+            self.runner = CliEntryBasedTestRunner(dags_plugin)
             result = self._run_meta_job("dag-empty-arguments")
             cli_assert_equal(0, result)
             job2_arguments = self._get_job_arguments("job2")
             assert len(job2_arguments) == 0
             self.httpserver.stop()
 
     def test_meta_job_wrong_job_key_type(self):
```

### Comparing `vdk-meta-jobs-0.1.833741966/tests/test_time_based_queue.py` & `vdk-meta-jobs-0.1.836044868/tests/test_time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.833741966/tests/test_tracking_job_executor.py` & `vdk-meta-jobs-0.1.836044868/tests/test_tracking_job_executor.py`

 * *Files identical despite different names*

