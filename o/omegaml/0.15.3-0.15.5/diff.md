# Comparing `tmp/omegaml-0.15.3.tar.gz` & `tmp/omegaml-0.15.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegaml-0.15.3.tar", last modified: Thu Oct 27 19:07:50 2022, max compression
+gzip compressed data, was "omegaml-0.15.5.tar", last modified: Thu Apr 13 11:34:44 2023, max compression
```

## Comparing `omegaml-0.15.3.tar` & `omegaml-0.15.5.tar`

### file list

```diff
@@ -1,433 +1,436 @@
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:50.045386 omegaml-0.15.3/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    11353 2022-10-27 19:06:13.000000 omegaml-0.15.3/LICENSE
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      924 2022-10-27 19:06:13.000000 omegaml-0.15.3/LICENSE-NOSELLCLAUSE
--rw-rw-r--   0 circleci  (1000) circleci  (1000)   847986 2022-10-27 19:06:13.000000 omegaml-0.15.3/LICENSES-THIRDPARTY
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      490 2022-10-27 19:06:13.000000 omegaml-0.15.3/MANIFEST.in
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2893 2022-10-27 19:06:13.000000 omegaml-0.15.3/NOTICE
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5389 2022-10-27 19:07:50.045386 omegaml-0.15.3/PKG-INFO
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4025 2022-10-27 19:06:13.000000 omegaml-0.15.3/README.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    25564 2022-10-27 19:06:13.000000 omegaml-0.15.3/THIRDPARTY
--rw-rw-r--   0 circleci  (1000) circleci  (1000)   847986 2022-10-27 19:06:13.000000 omegaml-0.15.3/THIRDPARTY-LICENSES
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3710 2022-10-27 19:06:13.000000 omegaml-0.15.3/conda-requirements.txt
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2500 2022-10-27 19:06:13.000000 omegaml-0.15.3/docker-compose.yml
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.965386 omegaml-0.15.3/docs/
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.973386 omegaml-0.15.3/docs/source/
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.973386 omegaml-0.15.3/docs/source/_static/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       83 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/_static/custom.css
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.973386 omegaml-0.15.3/docs/source/admin/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3853 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/admin/configuration.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1735 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/admin/design.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      102 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/admin/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2462 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/admin/kickstart.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1024 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/admin/putget.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      299 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/admin/spark.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1305 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/admin/windows.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    10581 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/conf.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.973386 omegaml-0.15.3/docs/source/devguide/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4926 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/devguide/architecture.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1960 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/devguide/custom.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      126 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/devguide/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1890 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/devguide/metadata.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3875 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/devguide/mixins.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     7317 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/devguide/storage.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.973386 omegaml-0.15.3/docs/source/guide/
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.973386 omegaml-0.15.3/docs/source/guide/advanced/
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.977386 omegaml-0.15.3/docs/source/guide/advanced/customizing/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      789 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/advanced/customizing/custombackends.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       91 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/advanced/customizing/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      245 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/advanced/index.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.977386 omegaml-0.15.3/docs/source/guide/advanced/integration/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3673 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/advanced/integration/buckets.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      101 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/advanced/integration/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2074 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/advanced/integration/runtimes.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.977386 omegaml-0.15.3/docs/source/guide/advanced/scripts/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2729 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/advanced/scripts/apps.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       96 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/advanced/scripts/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3389 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/advanced/scripts/lambda.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2097 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/advanced/scripts/mlflow.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.977386 omegaml-0.15.3/docs/source/guide/advanced/streams/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       87 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/advanced/streams/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5938 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/advanced/streams/streams.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.977386 omegaml-0.15.3/docs/source/guide/cli/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4290 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/cli/cloud.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2350 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/cli/datasets.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      232 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/cli/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    11582 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/cli/intro.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4358 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/cli/jobs.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3320 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/cli/models.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     6655 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/cli/runtime.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     7228 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/cli/scripts.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.977386 omegaml-0.15.3/docs/source/guide/clusters/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      156 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/clusters/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     7882 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/clusters/intro.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5531 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/clusters/logging.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2464 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/clusters/mlops.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2093 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/clusters/monitoring.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    12586 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/clusters/restapi.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      795 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/clusters/runtimes.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.977386 omegaml-0.15.3/docs/source/guide/datasets/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3155 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/datasets/files.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1296 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/datasets/filterdf.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      127 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/datasets/index.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.977386 omegaml-0.15.3/docs/source/guide/datasets/outofcore/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      155 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/datasets/outofcore/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     7063 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/datasets/outofcore/mdataframe.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     7206 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/datasets/outofcore/mdfapply.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2428 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/datasets/outofcore/mdfdebug.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    10719 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/datasets/outofcore/mdfguide.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5323 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/datasets/store_retrieve.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      191 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/index.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.977386 omegaml-0.15.3/docs/source/guide/integration/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2588 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/integration/gitlab.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       66 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/integration/index.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.981386 omegaml-0.15.3/docs/source/guide/intro/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      491 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/intro/cli.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       73 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/intro/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3101 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/intro/install.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1763 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/intro/python.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     7864 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/intro/rsystem.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      126 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/intro/setup.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3026 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/intro/whatis.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.981386 omegaml-0.15.3/docs/source/guide/jobs/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      116 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/jobs/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    13230 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/jobs/parallel.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1485 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/jobs/scheduling.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2079 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/jobs/working.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.981386 omegaml-0.15.3/docs/source/guide/models/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      554 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/models/experiments.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.981386 omegaml-0.15.3/docs/source/guide/models/frameworks/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      122 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/models/frameworks/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3578 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/models/frameworks/mlflow.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2677 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/models/frameworks/tensorflow.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      120 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/models/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     7129 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/models/metrics.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     6750 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/guide/models/modelstore.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.981386 omegaml-0.15.3/docs/source/images/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)   113744 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/images/celery_events.png
--rw-rw-r--   0 circleci  (1000) circleci  (1000)   130422 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/images/celery_flower.png
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    10887 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/images/deployment.gif
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    62941 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/images/deployment.jpg
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    13014 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/images/deployment.png
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    20329 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/images/deployment.svg
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.981386 omegaml-0.15.3/docs/source/images/screenshots/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    90122 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/images/screenshots/dashboard.png
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    13014 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/images/screenshots/deployment.png
--rw-rw-r--   0 circleci  (1000) circleci  (1000)   202886 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/images/screenshots/help.png
--rw-rw-r--   0 circleci  (1000) circleci  (1000)   258904 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/images/screenshots/notebook.png
--rw-rw-r--   0 circleci  (1000) circleci  (1000)   132504 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/images/screenshots/restapi.png
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      363 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      629 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/moreinfo.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.981386 omegaml-0.15.3/docs/source/nb/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     8822 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/nb/a-snowflake-plugin-demo.ipynb
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      220 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/nb/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    64430 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/nb/omegaml sample code.ipynb
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    11424 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/nb/omegaml-mdataframe-guide.ipynb
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    30376 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/nb/omegaml-r-tutorial.ipynb
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    13490 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/nb/omegaml-tutorial.ipynb
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1687 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/nb/omx_iotools-tutorial.ipynb
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1620 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/nb/quickstart.ipynb
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     9675 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/nb/tfestimator-tutorial.ipynb
--rw-rw-r--   0 circleci  (1000) circleci  (1000)   888274 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/nb/tfkeras-tutorial.ipynb
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.981386 omegaml-0.15.3/docs/source/quickstart/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       96 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/quickstart/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     8738 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/quickstart/usp.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    11641 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/quickstart/whatisit.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.981386 omegaml-0.15.3/docs/source/reference/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      186 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/reference/core.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2093 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/reference/datasets.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      165 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/reference/index.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1085 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/reference/jobs.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      939 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/reference/mdataframe.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2726 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/reference/models.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1063 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/reference/public.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2013 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/reference/runtimes.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2094 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/reference/scripts.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      972 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/reference/tracking.rst
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      520 2022-10-27 19:06:13.000000 omegaml-0.15.3/docs/source/screenshots.rst
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.985386 omegaml-0.15.3/omegaml/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        7 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/VERSION
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2232 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      143 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/_version.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.985386 omegaml-0.15.3/omegaml/backends/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       41 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5783 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/basecommon.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2201 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/basedata.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    10404 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/basemodel.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2787 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/dashapp.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    26915 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/experiment.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5315 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/externaldata.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3651 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/keras.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.985386 omegaml-0.15.3/omegaml/backends/mlflow/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/mlflow/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1998 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/mlflow/gitprojects.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4441 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/mlflow/localprojects.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5007 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/mlflow/models.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2243 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/mlflow/registrymodels.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2405 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/npndarray.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.985386 omegaml-0.15.3/omegaml/backends/package/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       92 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/package/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3906 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/package/localpip.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2129 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/package/packager.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3649 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/package/remotepip.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3778 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/package/tasks.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2523 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/rawdict.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3075 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/rawfiles.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.985386 omegaml-0.15.3/omegaml/backends/restapi/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/restapi/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    13983 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/restapi/asyncrest.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1364 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/restapi/job.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4020 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/restapi/model.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      889 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/restapi/script.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     7801 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/restapi/service.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.989386 omegaml-0.15.3/omegaml/backends/rsystem/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/rsystem/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1595 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/rsystem/rmodels.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5270 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/rsystem/rscripts.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    14959 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/scikitlearn.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    22778 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/sqlalchemy.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.989386 omegaml-0.15.3/omegaml/backends/tensorflow/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1080 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/tensorflow/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1553 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/tensorflow/protobufobj.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      319 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/tensorflow/tfdataset.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     9476 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/tensorflow/tfestimatormodel.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3607 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/tensorflow/tfkeras.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      987 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/tensorflow/tfkerassavedmodel.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    10078 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/tensorflow/tfsavedmodel.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     6934 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/backends/virtualobj.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    11669 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/celery_util.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      729 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/celeryapp.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.989386 omegaml-0.15.3/omegaml/client/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        1 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    11173 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/auth.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.989386 omegaml-0.15.3/omegaml/client/cli/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2733 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/cli/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       76 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/cli/__main__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      557 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/cli/catchall.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    17126 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/cli/cloud.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3440 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/cli/datasets.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     9837 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/cli/deploy.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     6537 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/cli/jobs.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      928 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/cli/models.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    18866 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/cli/runtime.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1826 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/cli/scripts.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2148 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/cli/shell.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1772 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/cli/stores.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4778 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/cloud.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    34970 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/docoptparser.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     7507 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/userconf.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1040 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/client/util.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      886 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/datapipeline.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    18049 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/defaults.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5367 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/documents.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.989386 omegaml-0.15.3/omegaml/example/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/example/__init__.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.989386 omegaml-0.15.3/omegaml/example/demo/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/example/demo/__init__.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.989386 omegaml-0.15.3/omegaml/example/demo/callback/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/example/demo/callback/__init__.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.989386 omegaml-0.15.3/omegaml/example/demo/callback/callback/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      312 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/example/demo/callback/callback/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      240 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/example/demo/callback/setup.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.989386 omegaml-0.15.3/omegaml/example/demo/helloservice/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/example/demo/helloservice/__init__.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.989386 omegaml-0.15.3/omegaml/example/demo/helloservice/helloservice/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      305 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/example/demo/helloservice/helloservice/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      254 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/example/demo/helloservice/setup.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.989386 omegaml-0.15.3/omegaml/example/demo/helloworld/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/example/demo/helloworld/__init__.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.989386 omegaml-0.15.3/omegaml/example/demo/helloworld/helloworld/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      448 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/example/demo/helloworld/helloworld/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      249 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/example/demo/helloworld/setup.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      235 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/example/demo/modelfn.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    41617 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mdataframe.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.989386 omegaml-0.15.3/omegaml/mixins/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       43 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/__init__.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.989386 omegaml-0.15.3/omegaml/mixins/mdf/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      188 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/mdf/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    34180 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/mdf/apply.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2662 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/mdf/applyutil.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1051 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/mdf/filterops.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5840 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/mdf/iotools.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     8803 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/mdf/parallel.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.993386 omegaml-0.15.3/omegaml/mixins/store/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       72 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/store/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    13826 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/store/datarevision.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    19498 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/store/extdmeta.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    11020 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/store/imexport.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2201 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/store/lazyget.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     7831 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/store/modelversion.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      799 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/store/package.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4202 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/store/projected.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2141 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/store/promotion.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3352 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mixins/store/virtualobj.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1845 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/mongoshim.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.993386 omegaml-0.15.3/omegaml/notebook/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/notebook/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1657 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/notebook/checkpoints.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    21929 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/notebook/jobs.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    11739 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/notebook/jobschedule.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.993386 omegaml-0.15.3/omegaml/notebook/jupyter/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/notebook/jupyter/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      360 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/notebook/jupyter/ipystart.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      457 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/notebook/jupyter/ipython_config.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    23050 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/notebook/jupyter/jupyter_notebook_config.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    59901 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/notebook/jupyter/jupyter_server_config.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.993386 omegaml-0.15.3/omegaml/notebook/jupyterhub/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/notebook/jupyterhub/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    37170 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/notebook/jupyterhub/jupyterhub_config.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     6796 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/notebook/jupyterhub/logo.jpg
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    15674 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/notebook/omegacontentsmgr.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3461 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/notebook/tasks.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     7522 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/omega.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.993386 omegaml-0.15.3/omegaml/restapi/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      439 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/restapi/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      200 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/restapi/__main__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      910 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/restapi/app.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    11492 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/restapi/resources.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4063 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/restapi/util.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.993386 omegaml-0.15.3/omegaml/runtimes/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      193 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3856 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/daskruntime.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.993386 omegaml-0.15.3/omegaml/runtimes/envinstall/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/envinstall/__init__.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.993386 omegaml-0.15.3/omegaml/runtimes/envinstall/envinstall/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1701 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/envinstall/envinstall/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      213 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/envinstall/setup.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1671 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/jobproxy.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1394 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/loky.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.993386 omegaml-0.15.3/omegaml/runtimes/mixins/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       74 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/mixins/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      876 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/mixins/gridsearch.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     7426 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/mixins/modelmixin.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    10678 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/mixins/nbtasks.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.993386 omegaml-0.15.3/omegaml/runtimes/mixins/swagger/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2667 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/mixins/swagger/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    11525 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/mixins/swagger/helpers.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3867 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/mixins/taskcanvas.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2852 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/modelproxy.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.993386 omegaml-0.15.3/omegaml/runtimes/rsystem/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4076 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/rsystem/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      128 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/rsystem/install.R
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      527 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/rsystem/omegamlr.R
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      174 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/rsystem/omworker.R
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      239 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/rsystem/unittest.R
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    14877 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/runtime.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1239 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/scriptproxy.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3008 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/runtimes/trackingproxy.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1370 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/sklext.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:50.041386 omegaml-0.15.3/omegaml/store/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      172 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/store/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    50131 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/store/base.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2399 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/store/combined.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3732 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/store/fastinsert.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5723 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/store/filtered.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    16593 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/store/logging.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:50.041386 omegaml-0.15.3/omegaml/store/migrations/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      357 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/store/migrations/0001_upgrade_tracking.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      448 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/store/migrations/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    12463 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/store/query.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    12523 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/store/queryops.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4355 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/store/streams.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5301 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tasks.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:50.041386 omegaml-0.15.3/omegaml/tests/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       39 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/__init__.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:50.041386 omegaml-0.15.3/omegaml/tests/core/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/__init__.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:50.045386 omegaml-0.15.3/omegaml/tests/core/cli/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/cli/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     6449 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/cli/scenarios.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1596 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/cli/test_cli.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      486 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/cli/test_cli_cloud.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4507 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/cli/test_cli_datasets.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4248 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/cli/test_cli_jobs.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1837 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/cli/test_cli_models.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     8672 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/cli/test_cli_runtime.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2019 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/cli/test_cli_scripts.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:50.045386 omegaml-0.15.3/omegaml/tests/core/restapi/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/restapi/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1755 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/restapi/test_api_buckets.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4092 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/restapi/test_job_api.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     8301 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/restapi/test_model_api.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4005 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/restapi/test_model_api_async.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3436 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/restapi/test_script_api.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    15844 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/restapi/test_service_api.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1885 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/restapi/util.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2714 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_backendbase.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     8553 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_configs.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    13802 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_contentsmgr.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1115 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_dashapp_backend.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    11001 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_datarevision.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    13121 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_extdmeta.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2769 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_filtered_collection.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    11214 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_imexport.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1506 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_iotools.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    25669 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_jobs.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5043 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_logging.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    21429 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_mdataframe.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    18597 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_mdfmixins.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4335 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_mdfparallel.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2173 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_misc.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     6889 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_modelversions.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4563 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_nbtasks.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      938 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_npndarray.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5361 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_package.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2167 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_package_remote.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     7247 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_promotion.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4340 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_query.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1130 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_restauth.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    26998 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_runtime.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1651 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_sklext.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    10763 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_sqlalchemy.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    41868 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_store.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    12556 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_tracking.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     6002 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/core/test_virtualobj.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:50.045386 omegaml-0.15.3/omegaml/tests/features/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/features/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3345 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/features/environment.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:50.045386 omegaml-0.15.3/omegaml/tests/features/steps/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/features/steps/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/features/steps/cli.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1920 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/features/steps/notebook.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1781 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/features/steps/tftutorial.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1483 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/features/steps/tutorial.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1893 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/features/tutorial.feature
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     6368 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/features/util.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:50.045386 omegaml-0.15.3/omegaml/tests/mlflow/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/mlflow/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     8240 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/mlflow/test_mlflow_models.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5123 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/mlflow/test_mlflow_projects.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:50.045386 omegaml-0.15.3/omegaml/tests/rsystem/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/rsystem/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1127 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/rsystem/rtestutil.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     8469 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/rsystem/test_rmodels.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2056 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/rsystem/test_rscripts.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:50.045386 omegaml-0.15.3/omegaml/tests/streams/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/streams/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5567 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/streams/test_minibatch.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1148 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/streams/test_streams.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:50.045386 omegaml-0.15.3/omegaml/tests/tensorflow/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/tensorflow/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3473 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/tensorflow/test_kerasmodel.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3338 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/tensorflow/test_protobuf.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1859 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/tensorflow/test_tfdataset.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    16427 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/tensorflow/test_tfestimator.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     4651 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/tensorflow/test_tfkerasmodel.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     6532 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/tensorflow/test_tfsavedmodel.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2935 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/tensorflow/test_tftracking.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2554 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/tests/util.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    34679 2022-10-27 19:06:13.000000 omegaml-0.15.3/omegaml/util.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.985386 omegaml-0.15.3/omegaml.egg-info/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5389 2022-10-27 19:07:49.000000 omegaml-0.15.3/omegaml.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    12562 2022-10-27 19:07:49.000000 omegaml-0.15.3/omegaml.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        1 2022-10-27 19:07:49.000000 omegaml-0.15.3/omegaml.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       50 2022-10-27 19:07:49.000000 omegaml-0.15.3/omegaml.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1358 2022-10-27 19:07:49.000000 omegaml-0.15.3/omegaml.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        8 2022-10-27 19:07:49.000000 omegaml-0.15.3/omegaml.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       47 2022-10-27 19:06:13.000000 omegaml-0.15.3/requirements.txt
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.965386 omegaml-0.15.3/scripts/
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-10-27 19:07:49.973386 omegaml-0.15.3/scripts/runtime/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     8940 2022-10-27 19:06:13.000000 omegaml-0.15.3/scripts/runtime/easyoptions
--rwxrwxr-x   0 circleci  (1000) circleci  (1000)     1861 2022-10-27 19:06:13.000000 omegaml-0.15.3/scripts/runtime/omegajobs.sh
--rwxrwxr-x   0 circleci  (1000) circleci  (1000)      762 2022-10-27 19:06:13.000000 omegaml-0.15.3/scripts/runtime/setupnb.sh
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       38 2022-10-27 19:07:50.045386 omegaml-0.15.3/setup.cfg
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     5582 2022-10-27 19:06:13.000000 omegaml-0.15.3/setup.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.695625 omegaml-0.15.5/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    11353 2023-04-13 11:22:58.000000 omegaml-0.15.5/LICENSE
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      924 2023-04-13 11:22:58.000000 omegaml-0.15.5/LICENSE-NOSELLCLAUSE
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)   847986 2023-04-13 11:22:58.000000 omegaml-0.15.5/LICENSES-THIRDPARTY
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      490 2023-04-13 11:22:58.000000 omegaml-0.15.5/MANIFEST.in
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2893 2023-04-13 11:22:58.000000 omegaml-0.15.5/NOTICE
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5389 2023-04-13 11:34:44.695625 omegaml-0.15.5/PKG-INFO
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4025 2023-04-13 11:22:58.000000 omegaml-0.15.5/README.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    25564 2023-04-13 11:22:58.000000 omegaml-0.15.5/THIRDPARTY
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)   847986 2023-04-13 11:22:58.000000 omegaml-0.15.5/THIRDPARTY-LICENSES
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3710 2023-04-13 11:22:58.000000 omegaml-0.15.5/conda-requirements.txt
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2499 2023-04-13 11:22:58.000000 omegaml-0.15.5/docker-compose.yml
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.519625 omegaml-0.15.5/docs/
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.543625 omegaml-0.15.5/docs/source/
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.543625 omegaml-0.15.5/docs/source/_static/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       83 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/_static/custom.css
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.547625 omegaml-0.15.5/docs/source/admin/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3853 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/admin/configuration.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1735 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/admin/design.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      102 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/admin/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2462 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/admin/kickstart.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1024 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/admin/putget.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      299 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/admin/spark.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1305 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/admin/windows.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    10581 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/conf.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.551625 omegaml-0.15.5/docs/source/devguide/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4926 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/devguide/architecture.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1960 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/devguide/custom.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      126 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/devguide/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1890 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/devguide/metadata.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3875 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/devguide/mixins.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     7317 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/devguide/storage.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.551625 omegaml-0.15.5/docs/source/guide/
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.551625 omegaml-0.15.5/docs/source/guide/advanced/
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.551625 omegaml-0.15.5/docs/source/guide/advanced/customizing/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      789 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/advanced/customizing/custombackends.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       91 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/advanced/customizing/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      245 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/advanced/index.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.551625 omegaml-0.15.5/docs/source/guide/advanced/integration/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3673 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/advanced/integration/buckets.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      101 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/advanced/integration/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2074 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/advanced/integration/runtimes.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.555625 omegaml-0.15.5/docs/source/guide/advanced/scripts/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2729 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/advanced/scripts/apps.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       96 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/advanced/scripts/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3389 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/advanced/scripts/lambda.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2097 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/advanced/scripts/mlflow.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.555625 omegaml-0.15.5/docs/source/guide/advanced/streams/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       87 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/advanced/streams/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5938 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/advanced/streams/streams.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.559625 omegaml-0.15.5/docs/source/guide/cli/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4290 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/cli/cloud.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2350 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/cli/datasets.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      232 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/cli/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    11582 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/cli/intro.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4358 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/cli/jobs.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3320 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/cli/models.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     6655 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/cli/runtime.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     7228 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/cli/scripts.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.563625 omegaml-0.15.5/docs/source/guide/clusters/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      156 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/clusters/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     7882 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/clusters/intro.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5531 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/clusters/logging.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2464 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/clusters/mlops.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2093 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/clusters/monitoring.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    12596 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/clusters/restapi.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      795 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/clusters/runtimes.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.563625 omegaml-0.15.5/docs/source/guide/datasets/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3155 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/datasets/files.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1296 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/datasets/filterdf.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      127 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/datasets/index.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.567625 omegaml-0.15.5/docs/source/guide/datasets/outofcore/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      155 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/datasets/outofcore/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     7063 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/datasets/outofcore/mdataframe.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     7206 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/datasets/outofcore/mdfapply.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2428 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/datasets/outofcore/mdfdebug.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    10719 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/datasets/outofcore/mdfguide.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5323 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/datasets/store_retrieve.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      191 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/index.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.567625 omegaml-0.15.5/docs/source/guide/integration/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2588 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/integration/gitlab.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       66 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/integration/index.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.571625 omegaml-0.15.5/docs/source/guide/intro/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      491 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/intro/cli.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       73 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/intro/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3101 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/intro/install.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1763 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/intro/python.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     7864 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/intro/rsystem.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      126 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/intro/setup.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3026 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/intro/whatis.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.571625 omegaml-0.15.5/docs/source/guide/jobs/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      116 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/jobs/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    13230 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/jobs/parallel.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1485 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/jobs/scheduling.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2079 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/jobs/working.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.575625 omegaml-0.15.5/docs/source/guide/models/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      554 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/models/experiments.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.575625 omegaml-0.15.5/docs/source/guide/models/frameworks/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      122 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/models/frameworks/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3578 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/models/frameworks/mlflow.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2677 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/models/frameworks/tensorflow.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      120 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/models/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     7129 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/models/metrics.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     6750 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/guide/models/modelstore.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.583625 omegaml-0.15.5/docs/source/images/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)   113744 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/images/celery_events.png
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)   130422 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/images/celery_flower.png
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    10887 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/images/deployment.gif
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    62941 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/images/deployment.jpg
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    13014 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/images/deployment.png
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    20329 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/images/deployment.svg
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.587625 omegaml-0.15.5/docs/source/images/screenshots/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    90122 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/images/screenshots/dashboard.png
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    13014 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/images/screenshots/deployment.png
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)   202886 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/images/screenshots/help.png
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)   258904 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/images/screenshots/notebook.png
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)   132504 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/images/screenshots/restapi.png
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      363 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      629 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/moreinfo.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.591625 omegaml-0.15.5/docs/source/nb/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     8785 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/nb/a-snowflake-plugin-demo.ipynb
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      220 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/nb/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    64430 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/nb/omegaml sample code.ipynb
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    11424 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/nb/omegaml-mdataframe-guide.ipynb
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    30376 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/nb/omegaml-r-tutorial.ipynb
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    13448 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/nb/omegaml-tutorial.ipynb
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1687 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/nb/omx_iotools-tutorial.ipynb
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1620 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/nb/quickstart.ipynb
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     9675 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/nb/tfestimator-tutorial.ipynb
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)   888274 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/nb/tfkeras-tutorial.ipynb
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.591625 omegaml-0.15.5/docs/source/quickstart/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       96 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/quickstart/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     8738 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/quickstart/usp.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    11641 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/quickstart/whatisit.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.595625 omegaml-0.15.5/docs/source/reference/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      186 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/reference/core.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2093 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/reference/datasets.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      165 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/reference/index.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1085 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/reference/jobs.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      939 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/reference/mdataframe.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2726 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/reference/models.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1063 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/reference/public.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2013 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/reference/runtimes.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2094 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/reference/scripts.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      972 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/reference/tracking.rst
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      520 2023-04-13 11:22:58.000000 omegaml-0.15.5/docs/source/screenshots.rst
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.603625 omegaml-0.15.5/omegaml/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        7 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/VERSION
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2232 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      143 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/_version.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.611625 omegaml-0.15.5/omegaml/backends/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       41 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5783 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/basecommon.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2201 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/basedata.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    10404 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/basemodel.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2787 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/dashapp.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    29565 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/experiment.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5315 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/externaldata.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3651 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/keras.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.611625 omegaml-0.15.5/omegaml/backends/mlflow/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/mlflow/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1998 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/mlflow/gitprojects.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4441 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/mlflow/localprojects.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5007 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/mlflow/models.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2243 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/mlflow/registrymodels.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2405 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/npndarray.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.615625 omegaml-0.15.5/omegaml/backends/package/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       92 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/package/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3906 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/package/localpip.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2129 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/package/packager.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3649 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/package/remotepip.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3778 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/package/tasks.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2523 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/rawdict.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3075 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/rawfiles.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.615625 omegaml-0.15.5/omegaml/backends/restapi/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/restapi/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    13983 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/restapi/asyncrest.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1364 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/restapi/job.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4020 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/restapi/model.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      889 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/restapi/script.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     7801 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/restapi/service.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.619625 omegaml-0.15.5/omegaml/backends/rsystem/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/rsystem/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1595 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/rsystem/rmodels.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5270 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/rsystem/rscripts.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    14959 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/scikitlearn.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    28627 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/sqlalchemy.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.619625 omegaml-0.15.5/omegaml/backends/tensorflow/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1080 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/tensorflow/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1553 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/tensorflow/protobufobj.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      319 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/tensorflow/tfdataset.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     9476 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/tensorflow/tfestimatormodel.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3607 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/tensorflow/tfkeras.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      987 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/tensorflow/tfkerassavedmodel.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    10078 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/tensorflow/tfsavedmodel.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     7392 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/backends/virtualobj.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    12121 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/celery_util.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      729 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/celeryapp.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.623625 omegaml-0.15.5/omegaml/client/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        1 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    11474 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/auth.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.631625 omegaml-0.15.5/omegaml/client/cli/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2733 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/cli/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       76 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/cli/__main__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      557 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/cli/catchall.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    17126 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/cli/cloud.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3440 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/cli/datasets.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     9837 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/cli/deploy.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     6537 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/cli/jobs.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      928 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/cli/models.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    18808 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/cli/runtime.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1826 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/cli/scripts.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2148 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/cli/shell.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1772 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/cli/stores.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4778 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/cloud.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    34970 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/docoptparser.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     7531 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/userconf.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1057 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/client/util.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      886 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/datapipeline.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    18794 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/defaults.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5367 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/documents.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.631625 omegaml-0.15.5/omegaml/example/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/example/__init__.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.631625 omegaml-0.15.5/omegaml/example/demo/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/example/demo/__init__.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.631625 omegaml-0.15.5/omegaml/example/demo/callback/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/example/demo/callback/__init__.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.631625 omegaml-0.15.5/omegaml/example/demo/callback/callback/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      312 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/example/demo/callback/callback/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      240 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/example/demo/callback/setup.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.631625 omegaml-0.15.5/omegaml/example/demo/helloservice/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/example/demo/helloservice/__init__.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.631625 omegaml-0.15.5/omegaml/example/demo/helloservice/helloservice/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      305 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/example/demo/helloservice/helloservice/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      254 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/example/demo/helloservice/setup.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.631625 omegaml-0.15.5/omegaml/example/demo/helloworld/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/example/demo/helloworld/__init__.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.631625 omegaml-0.15.5/omegaml/example/demo/helloworld/helloworld/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      448 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/example/demo/helloworld/helloworld/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      249 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/example/demo/helloworld/setup.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      235 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/example/demo/modelfn.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    41617 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mdataframe.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.635625 omegaml-0.15.5/omegaml/mixins/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       43 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/__init__.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.635625 omegaml-0.15.5/omegaml/mixins/mdf/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      188 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/mdf/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    34180 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/mdf/apply.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2662 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/mdf/applyutil.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1051 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/mdf/filterops.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5840 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/mdf/iotools.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     8803 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/mdf/parallel.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.643625 omegaml-0.15.5/omegaml/mixins/store/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       72 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/store/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    13826 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/store/datarevision.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    19497 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/store/extdmeta.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    11020 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/store/imexport.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2209 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/store/lazyget.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     7831 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/store/modelversion.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      799 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/store/package.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3448 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/store/passthrough.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4202 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/store/projected.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2141 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/store/promotion.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4620 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/store/requests.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3352 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mixins/store/virtualobj.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2066 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/mongoshim.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.647625 omegaml-0.15.5/omegaml/notebook/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/notebook/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1663 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/notebook/checkpoints.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    22152 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/notebook/jobs.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    11739 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/notebook/jobschedule.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.647625 omegaml-0.15.5/omegaml/notebook/jupyter/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/notebook/jupyter/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      360 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/notebook/jupyter/ipystart.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      457 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/notebook/jupyter/ipython_config.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    23050 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/notebook/jupyter/jupyter_notebook_config.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    59901 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/notebook/jupyter/jupyter_server_config.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.651625 omegaml-0.15.5/omegaml/notebook/jupyterhub/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/notebook/jupyterhub/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    37170 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/notebook/jupyterhub/jupyterhub_config.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     6796 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/notebook/jupyterhub/logo.jpg
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    15680 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/notebook/omegacontentsmgr.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3461 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/notebook/tasks.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     7610 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/omega.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.651625 omegaml-0.15.5/omegaml/restapi/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      439 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/restapi/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      200 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/restapi/__main__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      910 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/restapi/app.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    11492 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/restapi/resources.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4063 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/restapi/util.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.655625 omegaml-0.15.5/omegaml/runtimes/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      193 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3856 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/daskruntime.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.655625 omegaml-0.15.5/omegaml/runtimes/envinstall/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/envinstall/__init__.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.655625 omegaml-0.15.5/omegaml/runtimes/envinstall/envinstall/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1701 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/envinstall/envinstall/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      213 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/envinstall/setup.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1671 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/jobproxy.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1394 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/loky.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.659625 omegaml-0.15.5/omegaml/runtimes/mixins/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       74 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/mixins/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      876 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/mixins/gridsearch.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     7921 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/mixins/modelmixin.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    10678 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/mixins/nbtasks.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.659625 omegaml-0.15.5/omegaml/runtimes/mixins/swagger/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2667 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/mixins/swagger/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    11525 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/mixins/swagger/helpers.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3867 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/mixins/taskcanvas.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2852 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/modelproxy.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.659625 omegaml-0.15.5/omegaml/runtimes/rsystem/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4076 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/rsystem/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      128 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/rsystem/install.R
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      527 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/rsystem/omegamlr.R
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      174 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/rsystem/omworker.R
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      239 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/rsystem/unittest.R
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    16150 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/runtime.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1239 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/scriptproxy.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3126 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/runtimes/trackingproxy.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1370 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/sklext.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.667625 omegaml-0.15.5/omegaml/store/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      172 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/store/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    51562 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/store/base.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2399 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/store/combined.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3732 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/store/fastinsert.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     6214 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/store/filtered.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    16707 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/store/logging.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.667625 omegaml-0.15.5/omegaml/store/migrations/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      357 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/store/migrations/0001_upgrade_tracking.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      448 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/store/migrations/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    12643 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/store/query.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    13637 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/store/queryops.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4355 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/store/streams.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5301 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tasks.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.667625 omegaml-0.15.5/omegaml/tests/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       39 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/__init__.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.679625 omegaml-0.15.5/omegaml/tests/core/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/__init__.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.683625 omegaml-0.15.5/omegaml/tests/core/cli/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/cli/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     6449 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/cli/scenarios.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1596 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/cli/test_cli.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      486 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/cli/test_cli_cloud.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4507 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/cli/test_cli_datasets.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4248 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/cli/test_cli_jobs.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1837 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/cli/test_cli_models.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     8672 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/cli/test_cli_runtime.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2019 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/cli/test_cli_scripts.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.687625 omegaml-0.15.5/omegaml/tests/core/restapi/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/restapi/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1755 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/restapi/test_api_buckets.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4092 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/restapi/test_job_api.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     8301 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/restapi/test_model_api.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4005 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/restapi/test_model_api_async.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3436 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/restapi/test_script_api.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    15844 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/restapi/test_service_api.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1885 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/restapi/util.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2714 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_backendbase.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     8553 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_configs.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    13802 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_contentsmgr.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1115 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_dashapp_backend.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    11001 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_datarevision.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    13121 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_extdmeta.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4214 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_filtered_collection.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    11214 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_imexport.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1506 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_iotools.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    25669 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_jobs.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5043 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_logging.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    23524 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_mdataframe.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    18597 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_mdfmixins.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4335 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_mdfparallel.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2173 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_misc.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     6889 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_modelversions.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4563 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_nbtasks.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      938 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_npndarray.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5361 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_package.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2167 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_package_remote.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1895 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_passthrough.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     7247 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_promotion.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4340 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_query.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1130 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_restauth.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    26998 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_runtime.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1651 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_sklext.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    14430 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_sqlalchemy.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    43752 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_store.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    13025 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_tracking.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     6002 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/core/test_virtualobj.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.687625 omegaml-0.15.5/omegaml/tests/features/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/features/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3848 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/features/environment.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.691624 omegaml-0.15.5/omegaml/tests/features/steps/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/features/steps/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/features/steps/cli.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1920 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/features/steps/notebook.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1781 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/features/steps/tftutorial.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1483 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/features/steps/tutorial.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1893 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/features/tutorial.feature
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     6370 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/features/util.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.691624 omegaml-0.15.5/omegaml/tests/mlflow/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/mlflow/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     8240 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/mlflow/test_mlflow_models.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5123 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/mlflow/test_mlflow_projects.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.691624 omegaml-0.15.5/omegaml/tests/rsystem/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/rsystem/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1127 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/rsystem/rtestutil.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     8469 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/rsystem/test_rmodels.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2056 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/rsystem/test_rscripts.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.691624 omegaml-0.15.5/omegaml/tests/streams/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/streams/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5567 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/streams/test_minibatch.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1148 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/streams/test_streams.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.695625 omegaml-0.15.5/omegaml/tests/tensorflow/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/tensorflow/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3473 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/tensorflow/test_kerasmodel.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3338 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/tensorflow/test_protobuf.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1859 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/tensorflow/test_tfdataset.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    16427 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/tensorflow/test_tfestimator.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     4651 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/tensorflow/test_tfkerasmodel.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     6532 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/tensorflow/test_tfsavedmodel.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2935 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/tensorflow/test_tftracking.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2554 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/tests/util.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    35430 2023-04-13 11:22:58.000000 omegaml-0.15.5/omegaml/util.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.603625 omegaml-0.15.5/omegaml.egg-info/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5389 2023-04-13 11:34:44.000000 omegaml-0.15.5/omegaml.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    12670 2023-04-13 11:34:44.000000 omegaml-0.15.5/omegaml.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        1 2023-04-13 11:34:44.000000 omegaml-0.15.5/omegaml.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       50 2023-04-13 11:34:44.000000 omegaml-0.15.5/omegaml.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1409 2023-04-13 11:34:44.000000 omegaml-0.15.5/omegaml.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        8 2023-04-13 11:34:44.000000 omegaml-0.15.5/omegaml.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       47 2023-04-13 11:22:58.000000 omegaml-0.15.5/requirements.txt
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.519625 omegaml-0.15.5/scripts/
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2023-04-13 11:34:44.543625 omegaml-0.15.5/scripts/runtime/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     8940 2023-04-13 11:22:58.000000 omegaml-0.15.5/scripts/runtime/easyoptions
+-rwxrwxr-x   0 circleci  (1000) circleci  (1000)     1861 2023-04-13 11:22:58.000000 omegaml-0.15.5/scripts/runtime/omegajobs.sh
+-rwxrwxr-x   0 circleci  (1000) circleci  (1000)      762 2023-04-13 11:22:58.000000 omegaml-0.15.5/scripts/runtime/setupnb.sh
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       38 2023-04-13 11:34:44.695625 omegaml-0.15.5/setup.cfg
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     5798 2023-04-13 11:22:58.000000 omegaml-0.15.5/setup.py
```

### Comparing `omegaml-0.15.3/LICENSE` & `omegaml-0.15.5/LICENSE`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/LICENSE-NOSELLCLAUSE` & `omegaml-0.15.5/LICENSE-NOSELLCLAUSE`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/LICENSES-THIRDPARTY` & `omegaml-0.15.5/LICENSES-THIRDPARTY`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/NOTICE` & `omegaml-0.15.5/NOTICE`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/PKG-INFO` & `omegaml-0.15.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegaml
-Version: 0.15.3
+Version: 0.15.5
 Summary: An open source DataOps, MLOps platform for humans
 Home-page: https://omegaml.io/
 Author: Patrick Senti
 Author-email: patrick.senti@omegaml.io
 License: Apache 2.0 + "No Sell, Consulting Yes" License Condition
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `omegaml-0.15.3/README.rst` & `omegaml-0.15.5/README.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/THIRDPARTY` & `omegaml-0.15.5/THIRDPARTY`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/THIRDPARTY-LICENSES` & `omegaml-0.15.5/THIRDPARTY-LICENSES`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/conda-requirements.txt` & `omegaml-0.15.5/conda-requirements.txt`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docker-compose.yml` & `omegaml-0.15.5/docker-compose.yml`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
        - pythonlib:/app/pylib
    rabbitmq:
        image: rabbitmq:3.7.17
        hostname: rabbitmq
        ports:
           - 5672:5672
    mongodb:
-       image: mongo:4.4.13-focal
+       image: mongo:5.0.9-focal
        hostname: mongodb
        ports:
           - 27017:27017
        environment:
           MONGO_INITDB_ROOT_USERNAME: admin
           MONGO_INITDB_ROOT_PASSWORD: foobar
```

### Comparing `omegaml-0.15.3/docs/source/admin/configuration.rst` & `omegaml-0.15.5/docs/source/admin/configuration.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/admin/design.rst` & `omegaml-0.15.5/docs/source/admin/design.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/admin/kickstart.rst` & `omegaml-0.15.5/docs/source/admin/kickstart.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/admin/putget.rst` & `omegaml-0.15.5/docs/source/admin/putget.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/admin/windows.rst` & `omegaml-0.15.5/docs/source/admin/windows.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/conf.py` & `omegaml-0.15.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/devguide/architecture.rst` & `omegaml-0.15.5/docs/source/devguide/architecture.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/devguide/custom.rst` & `omegaml-0.15.5/docs/source/devguide/custom.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/devguide/metadata.rst` & `omegaml-0.15.5/docs/source/devguide/metadata.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/devguide/mixins.rst` & `omegaml-0.15.5/docs/source/devguide/mixins.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/devguide/storage.rst` & `omegaml-0.15.5/docs/source/devguide/storage.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/advanced/customizing/custombackends.rst` & `omegaml-0.15.5/docs/source/guide/advanced/customizing/custombackends.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/advanced/integration/buckets.rst` & `omegaml-0.15.5/docs/source/guide/advanced/integration/buckets.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/advanced/integration/runtimes.rst` & `omegaml-0.15.5/docs/source/guide/advanced/integration/runtimes.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/advanced/scripts/apps.rst` & `omegaml-0.15.5/docs/source/guide/advanced/scripts/apps.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/advanced/scripts/lambda.rst` & `omegaml-0.15.5/docs/source/guide/advanced/scripts/lambda.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/advanced/scripts/mlflow.rst` & `omegaml-0.15.5/docs/source/guide/advanced/scripts/mlflow.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/advanced/streams/streams.rst` & `omegaml-0.15.5/docs/source/guide/advanced/streams/streams.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/cli/cloud.rst` & `omegaml-0.15.5/docs/source/guide/cli/cloud.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/cli/datasets.rst` & `omegaml-0.15.5/docs/source/guide/cli/datasets.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/cli/intro.rst` & `omegaml-0.15.5/docs/source/guide/cli/intro.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/cli/jobs.rst` & `omegaml-0.15.5/docs/source/guide/cli/jobs.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/cli/models.rst` & `omegaml-0.15.5/docs/source/guide/cli/models.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/cli/runtime.rst` & `omegaml-0.15.5/docs/source/guide/cli/runtime.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/cli/scripts.rst` & `omegaml-0.15.5/docs/source/guide/cli/scripts.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/clusters/intro.rst` & `omegaml-0.15.5/docs/source/guide/clusters/intro.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/clusters/logging.rst` & `omegaml-0.15.5/docs/source/guide/clusters/logging.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/clusters/mlops.rst` & `omegaml-0.15.5/docs/source/guide/clusters/mlops.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/clusters/monitoring.rst` & `omegaml-0.15.5/docs/source/guide/clusters/monitoring.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/clusters/restapi.rst` & `omegaml-0.15.5/docs/source/guide/clusters/restapi.rst`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 
 *Commercial Edition*
 
 From your omega-ml portal, get the userid and api key.
 
 .. code::
 
-    from omegacli.auth import OmegaRestApiAuth
+    from omegaml.client.cli.auth import OmegaRestApiAuth
     auth = OmegaRestApiAuth(userid, apikey)
 
 
 Working with data (REST API)
 ----------------------------
```

### Comparing `omegaml-0.15.3/docs/source/guide/clusters/runtimes.rst` & `omegaml-0.15.5/docs/source/guide/clusters/runtimes.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/datasets/files.rst` & `omegaml-0.15.5/docs/source/guide/datasets/files.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/datasets/filterdf.rst` & `omegaml-0.15.5/docs/source/guide/datasets/filterdf.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/datasets/outofcore/mdataframe.rst` & `omegaml-0.15.5/docs/source/guide/datasets/outofcore/mdataframe.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/datasets/outofcore/mdfapply.rst` & `omegaml-0.15.5/docs/source/guide/datasets/outofcore/mdfapply.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/datasets/outofcore/mdfdebug.rst` & `omegaml-0.15.5/docs/source/guide/datasets/outofcore/mdfdebug.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/datasets/outofcore/mdfguide.rst` & `omegaml-0.15.5/docs/source/guide/datasets/outofcore/mdfguide.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/datasets/store_retrieve.rst` & `omegaml-0.15.5/docs/source/guide/datasets/store_retrieve.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/integration/gitlab.rst` & `omegaml-0.15.5/docs/source/guide/integration/gitlab.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/intro/install.rst` & `omegaml-0.15.5/docs/source/guide/intro/install.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/intro/python.rst` & `omegaml-0.15.5/docs/source/guide/intro/python.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/intro/rsystem.rst` & `omegaml-0.15.5/docs/source/guide/intro/rsystem.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/intro/whatis.rst` & `omegaml-0.15.5/docs/source/guide/intro/whatis.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/jobs/parallel.rst` & `omegaml-0.15.5/docs/source/guide/jobs/parallel.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/jobs/scheduling.rst` & `omegaml-0.15.5/docs/source/guide/jobs/scheduling.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/jobs/working.rst` & `omegaml-0.15.5/docs/source/guide/jobs/working.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/models/experiments.rst` & `omegaml-0.15.5/docs/source/guide/models/experiments.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/models/frameworks/mlflow.rst` & `omegaml-0.15.5/docs/source/guide/models/frameworks/mlflow.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/models/frameworks/tensorflow.rst` & `omegaml-0.15.5/docs/source/guide/models/frameworks/tensorflow.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/models/metrics.rst` & `omegaml-0.15.5/docs/source/guide/models/metrics.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/guide/models/modelstore.rst` & `omegaml-0.15.5/docs/source/guide/models/modelstore.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/images/celery_events.png` & `omegaml-0.15.5/docs/source/images/celery_events.png`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/images/celery_flower.png` & `omegaml-0.15.5/docs/source/images/celery_flower.png`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/images/deployment.gif` & `omegaml-0.15.5/docs/source/images/deployment.gif`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/images/deployment.jpg` & `omegaml-0.15.5/docs/source/images/deployment.jpg`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/images/deployment.png` & `omegaml-0.15.5/docs/source/images/deployment.png`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/images/deployment.svg` & `omegaml-0.15.5/docs/source/images/deployment.svg`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/images/screenshots/dashboard.png` & `omegaml-0.15.5/docs/source/images/screenshots/dashboard.png`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/images/screenshots/deployment.png` & `omegaml-0.15.5/docs/source/images/screenshots/deployment.png`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/images/screenshots/help.png` & `omegaml-0.15.5/docs/source/images/screenshots/help.png`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/images/screenshots/notebook.png` & `omegaml-0.15.5/docs/source/images/screenshots/notebook.png`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/images/screenshots/restapi.png` & `omegaml-0.15.5/docs/source/images/screenshots/restapi.png`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/moreinfo.rst` & `omegaml-0.15.5/docs/source/moreinfo.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/nb/a-snowflake-plugin-demo.ipynb` & `omegaml-0.15.5/docs/source/nb/a-snowflake-plugin-demo.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992848020434227%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(10, '1. install dependencies: `pip install --user -U "*

 * *            "snowflake-sqlalchemy`\\n')], delete: [10]}}, 1: {'source': {insert: [(1, '!pip "*

 * *            "install --user -U snowflake-sqlalchemy\\n')], delete: [1]}}}"}*

```diff
@@ -10,15 +10,15 @@
                 "\n",
                 "* store & retrieve connections to snowflake for dynamic queries using SQL (dynamic: at runtime)\n",
                 "* store & retrieve views to snowflake (storing connection & static SQL)\n",
                 "* copy data from snowflake to omega-ml for further processing\n",
                 "\n",
                 "Installation\n",
                 "\n",
-                "1. install dependencies: `pip install --user -U snowflake-sqlalchemy==1.2.1 cffi==1.14`\n",
+                "1. install dependencies: `pip install --user -U snowflake-sqlalchemy`\n",
                 "2. register snow flake: \n",
                 "  \n",
                 "      from sqlalchemy.dialects import registry\n",
                 "      registry.register('snowflake', 'snowflake.sqlalchemy', 'dialect')\n",
                 "\n",
                 "Usage\n",
                 "\n",
@@ -37,15 +37,15 @@
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# install dependencies\n",
-                "!pip install --user -U snowflake-sqlalchemy==1.2.1 'cffi<1.14'\n",
+                "!pip install --user -U snowflake-sqlalchemy\n",
                 "from sqlalchemy.dialects import registry\n",
                 "registry.register('snowflake', 'snowflake.sqlalchemy', 'dialect')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
```

### Comparing `omegaml-0.15.3/docs/source/nb/omegaml sample code.ipynb` & `omegaml-0.15.5/docs/source/nb/omegaml sample code.ipynb`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/nb/omegaml-mdataframe-guide.ipynb` & `omegaml-0.15.5/docs/source/nb/omegaml-mdataframe-guide.ipynb`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/nb/omegaml-r-tutorial.ipynb` & `omegaml-0.15.5/docs/source/nb/omegaml-r-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/nb/omegaml-tutorial.ipynb` & `omegaml-0.15.5/docs/source/nb/omegaml-tutorial.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999936995967742%*

 * *Differences: {"'cells'": '{20: {\'source\': {insert: [(24, \'fig, ax = plt.subplots(subplot_kw={"projection": '*

 * *            '"3d"})\\n\'), (26, "               c=labels.astype(float), edgecolor=\'k\')\\n")], '*

 * *            'delete: [27, 25, 24]}}}'}*

```diff
@@ -324,18 +324,17 @@
                 "om.models.put(model, 'iris-model')\n",
                 "om.runtime.model('iris-model').fit(X, y).get()\n",
                 "\n",
                 "# get back remote fitted model and show results\n",
                 "model = om.models.get('iris-model')\n",
                 "labels = model.labels_\n",
                 "\n",
-                "fig = plt.figure(figsize=(4, 3))\n",
-                "ax = Axes3D(fig, rect=[0, 0, .95, 1], elev=48, azim=134)\n",
+                "fig, ax = plt.subplots(subplot_kw={\"projection\": \"3d\"})\n",
                 "ax.scatter(X[:, 3], X[:, 0], X[:, 2],\n",
-                "               c=labels.astype(np.float), edgecolor='k')\n",
+                "               c=labels.astype(float), edgecolor='k')\n",
                 "fig.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `omegaml-0.15.3/docs/source/nb/omx_iotools-tutorial.ipynb` & `omegaml-0.15.5/docs/source/nb/omx_iotools-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/nb/quickstart.ipynb` & `omegaml-0.15.5/docs/source/nb/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/nb/tfestimator-tutorial.ipynb` & `omegaml-0.15.5/docs/source/nb/tfestimator-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/nb/tfkeras-tutorial.ipynb` & `omegaml-0.15.5/docs/source/nb/tfkeras-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/quickstart/usp.rst` & `omegaml-0.15.5/docs/source/quickstart/usp.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/quickstart/whatisit.rst` & `omegaml-0.15.5/docs/source/quickstart/whatisit.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/reference/datasets.rst` & `omegaml-0.15.5/docs/source/reference/datasets.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/reference/jobs.rst` & `omegaml-0.15.5/docs/source/reference/jobs.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/reference/mdataframe.rst` & `omegaml-0.15.5/docs/source/reference/mdataframe.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/reference/models.rst` & `omegaml-0.15.5/docs/source/reference/models.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/reference/public.rst` & `omegaml-0.15.5/docs/source/reference/public.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/reference/runtimes.rst` & `omegaml-0.15.5/docs/source/reference/runtimes.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/reference/scripts.rst` & `omegaml-0.15.5/docs/source/reference/scripts.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/reference/tracking.rst` & `omegaml-0.15.5/docs/source/reference/tracking.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/docs/source/screenshots.rst` & `omegaml-0.15.5/docs/source/screenshots.rst`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/__init__.py` & `omegaml-0.15.5/omegaml/__init__.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/basecommon.py` & `omegaml-0.15.5/omegaml/backends/basecommon.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/basedata.py` & `omegaml-0.15.5/omegaml/backends/basedata.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/basemodel.py` & `omegaml-0.15.5/omegaml/backends/basemodel.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/dashapp.py` & `omegaml-0.15.5/omegaml/backends/dashapp.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/experiment.py` & `omegaml-0.15.5/omegaml/backends/experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import getpass
-
-import dill
 import os
-import pandas as pd
-import pkg_resources
 import platform
 from base64 import b64encode, b64decode
 from datetime import datetime
 from itertools import product
 from uuid import uuid4
 
+import dill
+import pandas as pd
+import pkg_resources
+import pymongo
+
 from omegaml.backends.basemodel import BaseModelBackend
 from omegaml.documents import Metadata
-from omegaml.util import _raise, settings
+from omegaml.util import _raise, settings, ensure_index
 
 
 class ExperimentBackend(BaseModelBackend):
     """ ExperimentBackend provides storage of tracker configurations
 
     Usage:
 
@@ -179,20 +180,32 @@
     def active_run(self):
         self._run = (self._run or 0) + 1
         return self._run
 
     def status(self, run=None):
         return 'STOPPED'
 
-    def start(self):
+    def start(self, run=None):
         raise NotImplementedError
 
     def stop(self):
         raise NotImplementedError
 
+    def start_runtime(self):
+        # hook to signal the runtime is starting a task inside a worker
+        # this is unlike the .start() method which is called to start a run
+        # which can happen in the client or in the runtime
+        pass
+
+    def stop_runtime(self):
+        # hook to signal the runtime has completed a task inside a worker
+        # this is unlike the .stop() method which is called to stop a run
+        # which can happen in the client or in the runtime
+        self.flush()
+
     def log_event(self, event, key, value, step=None, **extra):
         raise NotImplementedError
 
     def log_metric(self, key, value, step=None, **extra):
         raise NotImplementedError
 
     def log_artifact(self, obj, name, step=None, **extra):
@@ -207,23 +220,26 @@
 
     def tensorflow_callback(self):
         return TensorflowCallback(self)
 
     def data(self, experiment=None, run=None, event=None, step=None, key=None, raw=False):
         raise NotImplementedError
 
+    def flush(self):
+        pass
+
     @property
     def _data_name(self):
         return f'.experiments/{self._experiment}'
 
 
 class NoTrackTracker(TrackingProvider):
     """ A default tracker that does not record anything """
 
-    def start(self):
+    def start(self, run=None):
         pass
 
     def stop(self):
         pass
 
     def log_artifact(self, obj, name, step=None, **extra):
         pass
@@ -257,14 +273,20 @@
     _experiment = None
     _startdt = None
     _stopdt = None
 
     _ensure_active = lambda self, r: r if r is not None else _raise(
         ValueError('no active run, call .start() or .use() '))
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.log_buffer = []
+        self.max_buffer = 10
+        self._initialize_dataset()
+
     def active_run(self, run=None):
         """ set the lastest run as the active run
 
         Args:
             run (int|str): optional or unique task id, if None the
                latest active run will be set, or
 
@@ -289,54 +311,73 @@
             self
         """
         self.active_run(run=run)
         return self
 
     @property
     def _latest_run(self):
-        data = self.data(event='start', raw=True)
-        run = data[-1]['run'] if data is not None and len(data) > 0 else None
+        cursor = self.data(event='start', lazy=True)
+        data = list(cursor.sort('data.run', -1).limit(1)) if cursor else None
+        run = data[-1].get('data', {}).get('run') if data is not None and len(data) > 0 else None
         return run
 
     def status(self, run=None):
         """ status of a run
 
         Args:
             run (int): the run number, defaults to the currently active run
 
         Returns:
             status in 'STARTED', 'STOPPED'
         """
         self._run = run or self._run or self._latest_run
-        data = self.data(event=('start', 'stop'), run=self._run, raw=True)
+        data = self.data(event=['start', 'stop'], run=self._run, raw=True)
         no_runs = data is None or len(data) == 0
         has_stop = sum(1 for row in (data or []) if row.get('event') == 'stop')
         return 'PENDING' if no_runs else 'STOPPED' if has_stop else 'STARTED'
 
     def start(self, run=None):
         """ start a new run
 
         This starts a new run and logs the start event
         """
         self._run = run or (self._latest_run or 0) + 1
         self._startdt = datetime.utcnow()
         data = self._common_log_data('start', key=None, value=None, step=None, dt=self._startdt)
-        self._write_log(data)
+        self._write_log(data, immediate=True)
         return self._run
 
     def stop(self):
         """ stop the current run
 
         This stops the current run and records the stop event
         """
         self._stopdt = datetime.utcnow()
         data = self._common_log_data('stop', key=None, value=None, step=None, dt=self._stopdt)
         self._write_log(data)
+        self.flush()
+
+    def flush(self):
+        # passing list of list forces insert_many
+        if self.log_buffer:
+            self._store.put(self.log_buffer, self._data_name,
+                            noversion=True, as_many=True)
+            self.log_buffer.clear()
 
     def _common_log_data(self, event, key, value, step=None, dt=None, **extra):
+        if isinstance(value, dict):
+            # shortcut to resolve PassthroughDataset actual values
+            # -- enables storing the actual values of a dataset passed as a PassthroughDataset
+            # TODO: should this be the responsibility of SimpleTracker?
+            if isinstance(value.get('args'), (list, tuple)):
+                value['args'] = [getattr(arg, '_passthrough_data', arg) for arg in value['args']]
+            if isinstance(value.get('kwargs'), dict):
+                value['kwargs'] = {
+                    k: getattr(v, '_passthrough_data', v) for k, v in value['kwargs'].items()
+                }
         data = {
             'experiment': self._experiment,
             'run': self._ensure_active(self._run),
             'step': step,
             'event': event,
             'key': key or event,
             'value': value,
@@ -344,16 +385,18 @@
             'node': os.environ.get('HOSTNAME', platform.node()),
             'userid': self.userid,
         }
         data.update(extra)
         data.update(self._extra_log) if self._extra_log else None
         return data
 
-    def _write_log(self, data):
-        self._store.put(data, self._data_name, noversion=True)
+    def _write_log(self, data, immediate=False):
+        self.log_buffer.append(data)
+        if immediate or len(self.log_buffer) > self.max_buffer:
+            self.flush()
 
     def log_artifact(self, obj, name, step=None, **extra):
         """ log any object to the current run
 
         Usage::
 
             # log an artifact
@@ -382,15 +425,15 @@
             format = 'metadata'
             rawdata = obj.to_json()
         elif self._model_store.get_backend_byobj(obj) is not None:
             objname = uuid4().hex
             meta = self._model_store.put(obj, f'.experiments/.artefacts/{objname}')
             format = 'model'
             rawdata = meta.name
-        elif self._store.get_backend_by_obj(obj) is not None:
+        elif self._store.get_backend_byobj(obj) is not None:
             objname = uuid4().hex
             meta = self._store.put(obj, f'.experiments/.artefacts/{objname}')
             format = 'dataset'
             rawdata = meta.name
         else:
             try:
                 rawdata = b64encode(dill.dumps(obj)).decode('utf8')
@@ -471,24 +514,25 @@
             self._extra_log.update(kwargs)
         else:
             from collections import deque as consume
             deletions = (self._extra_log.pop(k, None) for k in kwargs)
             consume(deletions, maxlen=0)
 
     def data(self, experiment=None, run=None, event=None, step=None, key=None, raw=False,
-             **extra):
+             lazy=False, **extra):
         """ build a dataframe of all stored data
 
         Args:
-            experiment (str): the name of the experiment, defaults to its current value
+            experiment (str|list): the name of the experiment, defaults to its current value
             run (int|list): the run(s) to get data back, defaults to current run, use 'all' for all
             event (str|list): the event(s) to include
             step (int|list): the step(s) to include
             key (str|list): the key(s) to include
             raw (bool): if True returns the raw data instead of a DataFrame
+            lazy (bool): if True returns the Cursor instead of data, ignores raw
 
         Returns:
             * data (DataFrame) if raw == False
             * data (list of dicts) if raw == True
             * None if no data exists
         """
         filter = {}
@@ -505,20 +549,27 @@
         if valid(step):
             filter['data.step'] = op(step)
         if valid(key):
             filter['data.key'] = op(key)
         for k, v in extra.items():
             if valid(k):
                 filter[f'data.{k}'] = op(v)
-        data = self._store.get(self._data_name, filter=filter)
-        if data is not None and not raw:
+        data = self._store.get(self._data_name, filter=filter, lazy=lazy)
+        if data is not None and not raw and not lazy:
             data = pd.DataFrame.from_records(data)
             data.sort_values('dt', inplace=True) if 'dt' in data.columns else None
         return data
 
+    def _initialize_dataset(self, force=False):
+        # create indexes when the dataset is first created
+        if not force and self._store.exists(self._data_name):
+            return
+        coll = self._store.collection(self._data_name)
+        ensure_index(coll, {'data.run': pymongo.ASCENDING, 'data.event': pymongo.ASCENDING})
+
     def restore_artifact(self, key=None, experiment=None, run=None, step=None, value=None):
         """ restore a logged artificat
 
         Args:
             key (str): the name of the artifact as provided in log_artifact
             run (int): the run for which to query, defaults to current run
             step (int): the step for which to query, defaults to all steps in run
@@ -582,44 +633,49 @@
         - It usually sufficient to report system metrics in intervals > 10 seconds since machine
           learning algorithms tend to use CPU and memory over longer periods of time.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.profile_logs = []
-        self.max_buffer = 6
+        self.max_buffer = 10
 
     def log_profile(self, data):
         """ the callback for BackgroundProfiler """
         self.profile_logs.append(data)
         if len(self.profile_logs) >= (self.max_buffer or 1):
             self.flush()
 
     def flush(self):
-        for step, data in enumerate(self.profile_logs):
-            # record the actual time instead of logging time (avoid buffering delays)
-            dt = data.get('profile_dt')
-            for k, v in data.items():
-                self.log_event('profile', k, v, step=step, dt=dt)
-        self.profile_logs = []
+        def log_items():
+            for step, data in enumerate(self.profile_logs):
+                # record the actual time instead of logging time (avoid buffering delays)
+                dt = data.get('profile_dt')
+                for k, v in data.items():
+                    item = self._common_log_data('profile', k, v, step=step, dt=dt)
+                    yield item
+        if self.profile_logs:
+            self._store.put([item for item in log_items()], self._data_name,
+                            index=['event'], as_many=True, noversion=True)
+            self.profile_logs = []
 
-    def start(self):
+    def start_runtime(self):
         self.profiler = BackgroundProfiler(callback=self.log_profile)
         self.profiler.start()
-        super().start()
+        super().start_runtime()
 
-    def stop(self):
+    def stop_runtime(self):
         self.profiler.stop()
         self.flush()
-        super().stop()
+        super().stop_runtime()
 
 
 try:
     from tensorflow import keras
-except:
+except Exception:
     pass
 else:
     class TensorflowCallback(keras.callbacks.Callback):
         """ A callback for Tensorflow Keras models
 
         Implements the callback protocol according to Tensorflow Keras
         semantics and linking to a :class:`omegaml.backends.experiment.TrackingProvider`
```

### Comparing `omegaml-0.15.3/omegaml/backends/externaldata.py` & `omegaml-0.15.5/omegaml/backends/externaldata.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/keras.py` & `omegaml-0.15.5/omegaml/backends/keras.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/mlflow/gitprojects.py` & `omegaml-0.15.5/omegaml/backends/mlflow/gitprojects.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/mlflow/localprojects.py` & `omegaml-0.15.5/omegaml/backends/mlflow/localprojects.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/mlflow/models.py` & `omegaml-0.15.5/omegaml/backends/mlflow/models.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/mlflow/registrymodels.py` & `omegaml-0.15.5/omegaml/backends/mlflow/registrymodels.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/npndarray.py` & `omegaml-0.15.5/omegaml/backends/npndarray.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/package/localpip.py` & `omegaml-0.15.5/omegaml/backends/package/localpip.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/package/packager.py` & `omegaml-0.15.5/omegaml/backends/package/packager.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/package/remotepip.py` & `omegaml-0.15.5/omegaml/backends/package/remotepip.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/package/tasks.py` & `omegaml-0.15.5/omegaml/backends/package/tasks.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/rawdict.py` & `omegaml-0.15.5/omegaml/backends/rawdict.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/rawfiles.py` & `omegaml-0.15.5/omegaml/backends/rawfiles.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/restapi/asyncrest.py` & `omegaml-0.15.5/omegaml/backends/restapi/asyncrest.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/restapi/job.py` & `omegaml-0.15.5/omegaml/backends/restapi/job.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/restapi/model.py` & `omegaml-0.15.5/omegaml/backends/restapi/model.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/restapi/script.py` & `omegaml-0.15.5/omegaml/backends/restapi/script.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/restapi/service.py` & `omegaml-0.15.5/omegaml/backends/restapi/service.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/rsystem/rmodels.py` & `omegaml-0.15.5/omegaml/backends/rsystem/rmodels.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/rsystem/rscripts.py` & `omegaml-0.15.5/omegaml/backends/rsystem/rscripts.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/scikitlearn.py` & `omegaml-0.15.5/omegaml/backends/scikitlearn.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/tensorflow/__init__.py` & `omegaml-0.15.5/omegaml/backends/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/tensorflow/protobufobj.py` & `omegaml-0.15.5/omegaml/backends/tensorflow/protobufobj.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/tensorflow/tfestimatormodel.py` & `omegaml-0.15.5/omegaml/backends/tensorflow/tfestimatormodel.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/tensorflow/tfkeras.py` & `omegaml-0.15.5/omegaml/backends/tensorflow/tfkeras.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/tensorflow/tfkerassavedmodel.py` & `omegaml-0.15.5/omegaml/backends/tensorflow/tfkerassavedmodel.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/tensorflow/tfsavedmodel.py` & `omegaml-0.15.5/omegaml/backends/tensorflow/tfsavedmodel.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/backends/virtualobj.py` & `omegaml-0.15.5/omegaml/backends/virtualobj.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import sys
+
 import dill
 
 from omegaml.backends.basedata import BaseDataBackend
 
 
 class VirtualObjectBackend(BaseDataBackend):
     """
@@ -96,15 +98,25 @@
 
     def get(self, name, version=-1, force_python=False, lazy=False, **kwargs):
         meta = self.model_store.metadata(name)
         outf = meta.gridfile
         # compat: Python 3.8.x < 3.8.2
         # https://github.com/python/cpython/commit/b19f7ecfa3adc6ba1544225317b9473649815b38
         # https://docs.python.org/3.8/whatsnew/changelog.html#python-3-8-2-final
-        obj = dill.loads(outf.read())
+        try:
+            data = outf.read()
+            obj = dill.loads(data)
+        except ModuleNotFoundError as e:
+            # if the functions original module is not known, simulate it
+            # this is to deal with functions created outside of __main__
+            # see https://stackoverflow.com/q/26193102/890242
+            #     https://stackoverflow.com/a/70513630/890242
+            sys.modules[e.name] = sys.modules['__main__']
+            obj = dill.loads(data)
+
         outf.close()
         return obj
 
     def predict(self, modelname, xName, rName=None, **kwargs):
         # make this work as a model backend too
         meta = self.model_store.metadata(modelname)
         handler = self.get(modelname)
```

### Comparing `omegaml-0.15.3/omegaml/celery_util.py` & `omegaml-0.15.5/omegaml/celery_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,22 +72,22 @@
 
     def __init__(self, *args, **kwargs):
         super(OmegamlTask, self).__init__(*args, **kwargs)
         self.auth_env = AuthenticationEnv.active()
 
     @property
     def om(self):
-        # TODO do some more intelligent caching, i.e. by client/auth
         if not hasattr(self.request, '_om'):
             self.request._om = None
         if self.request._om is None:
             bucket = self.system_kwargs.get('__bucket')
             auth = self.system_kwargs.get('__auth')
             om = self.request._om = self.auth_env.get_omega_for_task(self, auth=auth)[bucket]
             self.auth_env.prepare_env(om.defaults)
+            self.request._auth = om.runtime.auth
         return self.request._om
 
     def get_delegate(self, name, kind='models', pass_as='model_store'):
         get_delegate_provider = getattr(self.om, kind)
         self.enable_delegate_tracking(name, kind, get_delegate_provider)
         kwargs = dict(data_store=self.om.datasets,
                       tracking=self.tracking)
@@ -102,15 +102,16 @@
         tracking = meta.attributes.setdefault('tracking', {})
         tracking['experiments'] = set(tracking.get('experiments', []) + [exp._experiment])
         meta.save()
         return meta
 
     @property
     def current_userid(self):
-        return getattr(self.om.runtime.auth, 'userid', getpass.getuser())
+        # TODO: move current_userid to authenenv
+        return getattr(self.request._auth, 'userid', getpass.getuser())
 
     @property
     def delegate_args(self):
         return self.request.args
 
     @property
     def delegate_kwargs(self):
@@ -182,15 +183,15 @@
                 if logger:
                     handler.flush()
                     handler.close()
                     logger.removeHandler(handler)
                     # reset stdout redirects
                     sys.stdout, sys.stderr = save_stdout, save_stderr
 
-        with task_logging():
+        with self.om.request(request=self.request), task_logging():
             # start experiment block, if required
             # -- this ensures we call exp.start() / exp.stop() if the task was started in context
             #    of this celery task
             with self.tracking as exp:
                 # log task call event
                 # -- only log delegate args, kwargs
                 # -- avoid logging internal arguments
@@ -209,52 +210,64 @@
                     # this may happen when calling tasks directly, such as in run_omega_callback_script
                     result = super().__call__(*args, **kwargs)
         return result
 
     def reset(self):
         # ensure next call will start over and get a new om instance
         self.request._om = None
+        self.request._om_tracking = None
         self.auth_env.prepare_env(None, clear=True)
+        # note we do not reset self.request._auth to preserve the user context for logging purpose
+
 
     def send_event(self, type, **fields):
         # ensure result masking in events
         if 'result' in fields:
             fields['result'] = AuthenticationEnv().active().resultauth(fields['result'])
         super().send_event(type, **fields)
 
     def on_failure(self, exc, task_id, args, kwargs, einfo):
-        with self.tracking as exp:
-            exp.log_event(f'task_failure', self.name, {
-                'exception': repr(exc),
-                'task_id': task_id,
-            })
-            exp.log_extra(taskid=None, remove=True)
-        self.reset()
-        return super().on_failure(exc, task_id, args, kwargs, einfo)
+        try:
+            with self.tracking as exp:
+                exp.log_event(f'task_failure', self.name, {
+                    'exception': repr(exc),
+                    'task_id': task_id,
+                })
+                exp.log_extra(taskid=None, remove=True)
+                exp.flush()
+        finally:
+            super().on_failure(exc, task_id, args, kwargs, einfo)
+            self.reset()
 
     def on_retry(self, exc, task_id, args, kwargs, einfo):
-        with self.tracking as exp:
-            exp.log_event(f'task_retry', self.name, {
-                'exception': repr(exc),
-                'task_id': task_id,
-            })
-            exp.log_extra(taskid=None, remove=True)
-        self.reset()
-        return super().on_retry(exc, task_id, args, kwargs)
+        try:
+            with self.tracking as exp:
+                exp.log_event(f'task_retry', self.name, {
+                    'exception': repr(exc),
+                    'task_id': task_id,
+                })
+                exp.log_extra(taskid=None, remove=True)
+                exp.flush()
+        finally:
+            super().on_retry(exc, task_id, args, kwargs)
+            self.reset()
 
     def on_success(self, retval, task_id, args, kwargs):
         # on task success the experiment is stopped already (if we started it)
-        exp = self.tracking
-        exp.log_event(f'task_success', self.name, {
-            'result': sanitized(retval),
-            'task_id': task_id,
-        })
-        exp.log_extra(taskid=None, remove=True)
-        self.reset()
-        return super().on_success(retval, task_id, args, kwargs)
+        try:
+            exp = self.tracking
+            exp.log_event(f'task_success', self.name, {
+                'result': sanitized(retval),
+                'task_id': task_id,
+            })
+            exp.log_extra(taskid=None, remove=True)
+            exp.flush()
+        finally:
+            super().on_success(retval, task_id, args, kwargs)
+            self.reset()
 
 
 def get_dataset_representations(items):
     """
     returns dict with x and y datasets
     """
     results = {}
```

### Comparing `omegaml-0.15.3/omegaml/celeryapp.py` & `omegaml-0.15.5/omegaml/celeryapp.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/client/auth.py` & `omegaml-0.15.5/omegaml/client/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,30 @@
 
     Usage:
         auth = OmegaRestApiAuth('jezdez',
                          '25fdd0d9d210acb78b5b845fe8284a3c93630252')
         response = requests.get('http://api.foo.bar/v1/spam/', auth=auth)
     """
 
-    def __init__(self, username, apikey, qualifier=None):
+    def __init__(self, username, apikey, qualifier=None, bucket=None):
         self.username = username
-        self.apikey = apikey
+        self.apikey = apikey.decode('utf8') if isinstance(apikey, bytes) else apikey
         self.qualifier = qualifier or 'default'
+        self.bucket = bucket
 
     def get_credentials(self):
         if self.kind == 'jwt':
             return 'Bearer %s' % (self.apikey,)
         return 'ApiKey %s:%s' % (self.username, self.apikey)
 
     def __call__(self, r):
         r.headers['Authorization'] = self.get_credentials()
         r.headers['Qualifier'] = self.qualifier
+        if self.bucket:
+            r.headers['Bucket'] = self.bucket
         return r
 
     def __repr__(self):
         return ('OmegaRestApiAuth(username={}, apikey="*****",'
                 'qualifier={})').format(self.username, self.qualifier)
 
     @property
@@ -167,16 +170,17 @@
                 os.environ[k] = envstr(defaults[k])
             else:
                 os.environ.pop(k, None)
 
 
 class CloudClientAuthenticationEnv(AuthenticationEnv):
     is_secure = True
-    env_keys = ['OMEGA_AUTH_ENV', 'OMEGA_RESTAPI_URL',
-                'OMEGA_USERID', 'OMEGA_APIKEY', 'OMEGA_QUALIFIER']
+    env_keys = ['OMEGA_AUTH_ENV', 'OMEGA_RESTAPI_URL', 'OMEGA_TEST_MODE',
+                'OMEGA_USERID', 'OMEGA_APIKEY', 'OMEGA_QUALIFIER',
+                'OMEGA_SERVICES_INCLUSTER']
 
     @classmethod
     @session_cache
     def get_omega_for_task(cls, task, auth=None):
         """
         Get Omega instance configured for user in auth
 
@@ -226,20 +230,21 @@
     @session_cache  # PERFTUNED
     def get_omega_from_apikey(cls, *args, **kwargs):
         from omegaml.client.userconf import _get_omega_from_apikey
         return _get_omega_from_apikey(*args, **kwargs)
 
     @classmethod
     def get_restapi_auth(cls, defaults=None, om=None,
-                         userid=None, apikey=None, qualifier=None):
+                         userid=None, apikey=None, qualifier=None, bucket=None):
         assert defaults or om, "require either defaults or om"
         defaults = defaults or om.defaults
         return OmegaRestApiAuth(userid or defaults.OMEGA_USERID,
                                 apikey or defaults.OMEGA_APIKEY,
-                                qualifier or defaults.OMEGA_QUALIFIER)
+                                qualifier=qualifier or defaults.OMEGA_QUALIFIER,
+                                bucket=bucket)
 
     @classmethod
     def get_runtime_auth(cls, defaults=None, om=None):
         assert defaults or om, "require either defaults or om"
         defaults = defaults or om.defaults
         return OmegaRuntimeAuthentication(defaults.OMEGA_USERID,
                                           defaults.OMEGA_APIKEY,
```

### Comparing `omegaml-0.15.3/omegaml/client/cli/__init__.py` & `omegaml-0.15.5/omegaml/client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/client/cli/catchall.py` & `omegaml-0.15.5/omegaml/client/cli/catchall.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/client/cli/cloud.py` & `omegaml-0.15.5/omegaml/client/cli/cloud.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/client/cli/datasets.py` & `omegaml-0.15.5/omegaml/client/cli/datasets.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/client/cli/deploy.py` & `omegaml-0.15.5/omegaml/client/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/client/cli/jobs.py` & `omegaml-0.15.5/omegaml/client/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/client/cli/models.py` & `omegaml-0.15.5/omegaml/client/cli/models.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/client/cli/runtime.py` & `omegaml-0.15.5/omegaml/client/cli/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,19 +277,17 @@
         result = om.runtime.require(label).job(name).run()
         if not is_async:
             self.logger.info(result.get())
         else:
             self.logger.info(result.task_id)
 
     def result(self):
-        from celery.result import AsyncResult
-
         om = get_omega(self.args)
         task_id = self.args.get('<taskid>')
-        result = AsyncResult(task_id, app=om.runtime.celeryapp).get()
+        result = om.runtime.result(task_id)
         self.logger.info(result)
 
     def log(self):
         import pandas as pd
         tail = self.args.get('-f')
         om = get_omega(self.args)
         if not tail:
@@ -305,40 +303,41 @@
         self.celery('inspect')
 
     def control(self):
         self.celery('control')
 
     def celery(self, action=None):
         om = get_omega(self.args)
-        # giving om command here changes celery help output
-        celery_cmds = ['om runtime celery']
+        celery_cmds = []
         if action:
             celery_cmds += action.split(' ')
         # convert omega terms into celery terms
         celery_opts = (
             # omega term, celery term, value|flag
             ('--worker', '--destination', 'value'),
             ('--queue', '--queue', 'value'),
             ('--celery-help', '--help', 'flag'),
         )
-        is_r_worker = 'rworker' in self.args.get('<celery-command>')
         for opt, celery_opt, kind in celery_opts:
             if self.args.get(opt):
                 celery_cmds += [celery_opt]
                 if kind == 'value':
                     celery_cmds += [self.args.get(opt)]
         # prepare celery command args, remove empty parts
-        celery_cmds += self.args.get('<celery-command>')
+        celery_command = self.args.get('<celery-command>')
+        celery_cmds += celery_command
         celery_cmds += (self.args.get('--flags') or '').split(' ')
         celery_cmds = [cmd for cmd in celery_cmds if cmd]
-        if len(celery_cmds) == 1 + int(action is not None):
+        if len(celery_command) == 1 and celery_command[0] in ('inspect', 'control'):
             celery_cmds += ['--help']
         # start in-process for speed
         # -- disable command logging to avoid curses problems in celery events
         self.logger.setLevel(logging.CRITICAL + 1)
+        # check for R worker
+        is_r_worker = 'rworker' in self.args.get('<celery-command>')
         if is_r_worker:
             # start r runtime
             from omegaml.runtimes import rsystem
             rworker = os.path.join(os.path.dirname(rsystem.__file__), 'omworker.R')
             rcmd = f'Rscript {rworker}'.split(' ')
             call(rcmd)
         else:
```

### Comparing `omegaml-0.15.3/omegaml/client/cli/scripts.py` & `omegaml-0.15.5/omegaml/client/cli/scripts.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/client/cli/shell.py` & `omegaml-0.15.5/omegaml/client/cli/shell.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/client/cli/stores.py` & `omegaml-0.15.5/omegaml/client/cli/stores.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/client/cloud.py` & `omegaml-0.15.5/omegaml/client/cloud.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/client/docoptparser.py` & `omegaml-0.15.5/omegaml/client/docoptparser.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/client/userconf.py` & `omegaml-0.15.5/omegaml/client/userconf.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,42 +30,43 @@
     s.mount('https://', HTTPAdapter(max_retries=retry))
     return s
 
 
 def _get_userconfig_from_api(api_auth, api_url=None, requested_userid=None, qualifier=None, view=False):
     # safe way to talk to either the remote API or the in-process test server
     from omegaml import settings
+    from omegaml import _base_config
     defaults = settings()
     api_url = ensure_api_url(api_url, defaults)
     api_url += '/api/v1/config/'
     api_url = api_url.replace('//api', '/api')
     query = []
     if requested_userid:
         query.append('user={}'.format(requested_userid))
     if view:
         query.append('view={}'.format(int(view)))
     if qualifier:
         query.append('qualifier={}'.format(qualifier))
     api_url += '?' + '&'.join(query)
     # -- setup appropriate client API
-    if api_url.startswith('http'):
-        import requests
-        server = session_backoff()
-        server_kwargs = dict(auth=api_auth)
-        deserialize = lambda resp: resp.json()
-    elif api_url.startswith('test') or any('test' in v for v in sys.argv):
+    if _base_config.is_test_run or api_url.startswith('/'):
         try:
             from tastypie.test import TestApiClient
         except ModuleNotFoundError as e:
             # we need omegaee environment to proceed
             raise
         server = TestApiClient()
         server.close = lambda: None
         server_kwargs = dict(authentication=api_auth.get_credentials())
         deserialize = lambda resp: json.loads(resp.content.decode('utf-8'))
+    elif api_url.startswith('http'):
+        import requests
+        server = session_backoff()
+        server_kwargs = dict(auth=api_auth)
+        deserialize = lambda resp: resp.json()
     else:
         raise ValueError('invalid api_url >{}<'.format(api_url))
     # -- actual logic to get configs
     fail_msg = ("omegaml hub refused authentication by {api_auth}, "
                 "status code={resp.status_code} "
                 "using {api_url}.")
     resp = server.get(api_url, **server_kwargs)
```

### Comparing `omegaml-0.15.3/omegaml/client/util.py` & `omegaml-0.15.5/omegaml/client/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             om = setup_from_config(config_file)
         except Exception as e:
             msg = (f'Config file could not be found due to {e}. Specify as --config or set '
                     'OMEGA_CONFIG_FILE env variable')
             raise ValueError(msg)
     else:
         om = setup()
-    if local:
+    if local or local_runtime:
         om.runtime.mode(local=True)
     return om[bucket] if bucket else om # for speed
 
 
 class AttrDict(dict):
     def __init__(self, *args, **kwargs):
         super(AttrDict, self).__init__(*args, **kwargs)
```

### Comparing `omegaml-0.15.3/omegaml/datapipeline.py` & `omegaml-0.15.5/omegaml/datapipeline.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/defaults.py` & `omegaml-0.15.5/omegaml/defaults.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 import shutil
 import sys
 from pathlib import Path
 
 from omegaml.util import tensorflow_available, keras_available, module_available, markup, dict_merge
 
 # determine how we're run
+test_runners = {'test', 'nosetest', 'pytest', '_jb_unittest_runner.py'}
+cmd_args = (basename(v) for v in sys.argv)
 truefalse = lambda v: (v if isinstance(v, bool) else
                        any(str(v).lower().startswith(c) for c in ('y', 't', '1')))
 is_cli_run = os.path.basename(sys.argv[0]) == 'om'
 is_test_run = truefalse(os.environ.get('OMEGA_TEST_MODE'))
-is_test_run |= any('test' in basename(v) for v in sys.argv[:3]) and 'omegaml-ce' in str(Path().cwd())
+is_test_run |= len(set(test_runners) & set(cmd_args)) and 'omegaml-ce' in str(Path().cwd())
 
 #: configuration file, by default will be searched in current directory, user config or site config
 OMEGA_CONFIG_FILE = os.environ.get('OMEGA_CONFIG_FILE') or 'config.yml'
 #: the temp directory used by omegaml processes
 OMEGA_TMP = os.environ.get('OMEGA_TMP', '/tmp')
 #: the fully qualified mongodb database URL, including the database name
 OMEGA_MONGO_URL = (os.environ.get('OMEGA_MONGO_URL') or
@@ -45,23 +47,27 @@
                 os.environ.get('RABBITMQ_URL') or
                 'amqp://admin:foobar@localhost:5672//')
 #: is the worker considered inside the same cluster as the client
 OMEGA_SERVICES_INCLUSTER = truefalse(os.environ.get('OMEGA_SERVICES_INCLUSTER', False))
 #: (deprecated) the collection used to store ipython notebooks
 OMEGA_NOTEBOOK_COLLECTION = 'ipynb'
 #: the celery backend name or URL
-OMEGA_RESULT_BACKEND = 'rpc://'
+OMEGA_RESULT_BACKEND = os.environ.get('OMEGA_RESULT_BACKEND', 'rpc://')
 #: the omega worker label
 OMEGA_WORKER_LABEL = os.environ.get('OMEGA_WORKER_LABEL') or os.environ.get('CELERY_Q', 'default')
 #: the celery configurations
 OMEGA_CELERY_CONFIG = {
     # FIXME should work with json (the default celery serializer)
     'CELERY_ACCEPT_CONTENT': ['pickle', 'json'],
     'CELERY_TASK_SERIALIZER': 'pickle',
     'CELERY_RESULT_SERIALIZER': 'pickle',
+    # according to docs, CELERY_RESULT_EXPIRES is the new setting
+    # however as of 5.2.7 celery still refers CELERY_TASK_RESULT_EXPIRES
+    # https://github.com/celery/celery/blob/7b585138af8318d62b8fe7086df7e85d110ac786/celery/app/defaults.py#L204
+    'CELERY_RESULT_EXPIRES': 3600,  # expire results within 1 hour
     'CELERY_TASK_RESULT_EXPIRES': 3600,  # expire results within 1 hour
     'CELERY_DEFAULT_QUEUE': OMEGA_WORKER_LABEL,
     'BROKER_URL': OMEGA_BROKER,
     'BROKER_HEARTBEAT': 0,  # due to https://github.com/celery/celery/issues/4980
     # TODO replace result backend with redis or mongodb
     'CELERY_RESULT_BACKEND': OMEGA_RESULT_BACKEND,
     'CELERY_ALWAYS_EAGER': True if OMEGA_LOCAL_RUNTIME else False,
@@ -134,17 +140,21 @@
     'omegaml.mixins.mdf.iotools.IOToolsStoreMixin',
     'omegaml.mixins.store.modelversion.ModelVersionMixin',
     'omegaml.mixins.store.datarevision.DataRevisionMixin',
     'omegaml.mixins.store.imexport.ObjectImportExportMixin',
     'omegaml.mixins.store.extdmeta.SignatureMixin',
     'omegaml.mixins.store.extdmeta.ScriptSignatureMixin',
     'omegaml.mixins.store.extdmeta.ModelSignatureMixin',
+    'omegaml.mixins.store.requests.RequestCache',
+    'omegaml.mixins.store.passthrough.PassthroughMixin',
 ]
 #: set hashed or clear names
 OMEGA_STORE_HASHEDNAMES = truefalse(os.environ.get('OMEGA_STORE_HASHEDNAMES', True))
+#: enable request caching for metadata
+OMEGA_STORE_CACHE = truefalse(os.environ.get('OMEGA_STORE_CACHE', False))
 #: runtimes mixins
 OMEGA_RUNTIME_MIXINS = [
     'omegaml.runtimes.mixins.ModelMixin',
     'omegaml.runtimes.mixins.GridSearchMixin',
 ]
 #: mdataframe mixins
 OMEGA_MDF_MIXINS = [
@@ -166,14 +176,16 @@
 OMEGA_JOBPROXY_MIXINS = [
     'omegaml.runtimes.mixins.nbtasks.JobTasks',
 ]
 #: user extensions
 OMEGA_USER_EXTENSIONS = os.environ.get('OMEGA_USER_EXTENSIONS') or None
 #: logging handler for om.logger
 OMEGA_LOG_HANDLER = 'omegaml.store.logging.OmegaLoggingHandler'
+#: route om.logger to python logger
+OMEGA_LOG_PYTHON = False
 #: log dataset
 OMEGA_LOG_DATASET = '.omega/logs'
 #: OmegaLoggingHandler log format
 OMEGA_LOG_FORMAT = '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 #: MongoClient ServerSelectionTimeoutMS
 OMEGA_MONGO_TIMEOUT = int(os.environ.get('OMEGA_MONGO_TIMEOUT') or 2500)
 #: tracking providers
```

### Comparing `omegaml-0.15.3/omegaml/documents.py` & `omegaml-0.15.5/omegaml/documents.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/mdataframe.py` & `omegaml-0.15.5/omegaml/mdataframe.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/mixins/mdf/apply.py` & `omegaml-0.15.5/omegaml/mixins/mdf/apply.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/mixins/mdf/applyutil.py` & `omegaml-0.15.5/omegaml/mixins/mdf/applyutil.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/mixins/mdf/filterops.py` & `omegaml-0.15.5/omegaml/mixins/mdf/filterops.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/mixins/mdf/iotools.py` & `omegaml-0.15.5/omegaml/mixins/mdf/iotools.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/mixins/mdf/parallel.py` & `omegaml-0.15.5/omegaml/mixins/mdf/parallel.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/mixins/store/datarevision.py` & `omegaml-0.15.5/omegaml/mixins/store/datarevision.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/mixins/store/extdmeta.py` & `omegaml-0.15.5/omegaml/mixins/store/extdmeta.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             actions = None
         existing = meta.attributes.setdefault('signature', {})
         # determine object or array
         is_many = lambda T: isinstance(T, list) or getattr(T, 'many', False)
         many_type = lambda T: T[0] if isinstance(T, list) else X
         Xmany, X = (True, many_type(X)) if is_many(X) else (False, X)
         Ymany, Y = (True, many_type(Y)) if is_many(Y) else (False, Y)
-        Rmany, result = (True, result[0]) if isinstance(result, list) else (False, result)
+        Rmany, result = (True, many_type(result)) if is_many(result) else (False, result)
         meta.attributes['signature'] = {
             'X': {
                 'datatype': f'{X.__module__}.{schema_name(X)}',
                 'schema': self._schema_from_datatype(X),
                 'many': Xmany,
             } if X is not None else existing.get('X'),
             'Y': {
```

### Comparing `omegaml-0.15.3/omegaml/mixins/store/imexport.py` & `omegaml-0.15.5/omegaml/mixins/store/imexport.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/mixins/store/lazyget.py` & `omegaml-0.15.5/omegaml/mixins/store/lazyget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import re
 
-from omegaml.mdataframe import MDataFrame
-
 
 class LazyGetMixin:
     """
     OmegaStore mixin to support chunked lazy get via name
 
     Usage:
 
@@ -53,14 +51,16 @@
         match = self.ops_pattern.match(name + ';') if '#' in name else None
         opspec = None
         if match is not None:
             name, opspec, _ = match.groups()
         return name, opspec
 
     def _default_op(self, name, lazy):
+        from omegaml.mdataframe import MDataFrame
+
         if isinstance(lazy, MDataFrame):
             op = 'iterchunks'
             opkwargs = {}
         else:
             op = '__repr__'
             opkwargs = {}
         return op, opkwargs
```

### Comparing `omegaml-0.15.3/omegaml/mixins/store/modelversion.py` & `omegaml-0.15.5/omegaml/mixins/store/modelversion.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/mixins/store/package.py` & `omegaml-0.15.5/omegaml/mixins/store/package.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/mixins/store/projected.py` & `omegaml-0.15.5/omegaml/mixins/store/projected.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/mixins/store/promotion.py` & `omegaml-0.15.5/omegaml/mixins/store/promotion.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/mixins/store/virtualobj.py` & `omegaml-0.15.5/omegaml/mixins/store/virtualobj.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/mongoshim.py` & `omegaml-0.15.5/omegaml/mongoshim.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,17 +29,22 @@
     if 'tlsCAFile' in kwargs and not kwargs.get('tls'):
         del kwargs['tlsCAFile']
     if 'ssl_ca_certs' in kwargs and not kwargs.get('tls'):
         del kwargs['ssl_ca_certs']
     return kwargs
 
 
-def mongo_url(om):
-    mongo_url = (om.datasets.mongo_url + '?authSource=admin&' +
-                 urlencode(sanitize_mongo_kwargs(om.defaults.OMEGA_MONGO_SSL_KWARGS)))
+def mongo_url(om, drop_kwargs=None):
+    url_kwargs = sanitize_mongo_kwargs(om.defaults.OMEGA_MONGO_SSL_KWARGS)
+    if drop_kwargs:
+        for kw in drop_kwargs:
+            url_kwargs.pop(kw, None)
+    url_kwargs = urlencode(url_kwargs)
+    url_kwargs = url_kwargs.replace('True', 'true').replace('False', 'false')
+    mongo_url = (om.datasets.mongo_url + '?authSource=admin&' + url_kwargs)
     return mongo_url
 
 
 def waitForConnection(client):
     _exc = None
     command = client.admin.command
     for i in range(100):
@@ -50,9 +55,7 @@
             sleep(0.01)
             _exc = e
         else:
             _exc = None
             break
     if _exc is not None:
         raise _exc
-
-
```

### Comparing `omegaml-0.15.3/omegaml/notebook/checkpoints.py` & `omegaml-0.15.5/omegaml/notebook/checkpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from notebook.services.contents.checkpoints import GenericCheckpointsMixin, Checkpoints
+from jupyter_server.services.contents.checkpoints import GenericCheckpointsMixin, Checkpoints
 
 
 class NoOpCheckpoints(GenericCheckpointsMixin, Checkpoints):
     # source https://jupyter-notebook.readthedocs.io/en/stable/extending/contents.html#customizing-checkpoints
     # © Copyright 2015, Jupyter Team, https://jupyter.org. Revision 775cb20d.
 
     def checkpoint_model(self):
```

### Comparing `omegaml-0.15.3/omegaml/notebook/jobs.py` & `omegaml-0.15.5/omegaml/notebook/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import datetime
 import gridfs
 import re
 import yaml
 from croniter import croniter
 from io import StringIO, BytesIO
+
+from jupyter_client import AsyncKernelManager
 from nbconvert.preprocessors import ClearOutputPreprocessor
 from nbconvert.preprocessors.execute import ExecutePreprocessor
 from nbformat import read as nbread, write as nbwrite, v4 as nbv4
 from uuid import uuid4
 
 from omegaml.backends.basecommon import BackendBaseCommon
 from omegaml.documents import MDREGISTRY
@@ -342,14 +344,17 @@
             # avoid kernel at exit functions
             # -- this stops ipykernel AttributeError 'send_multipart'
             'shutdown_kernel': 'immediate',
             # set kernel name, blank is default
             # -- e.g. python3, ir
             # -- see https://stackoverflow.com/a/47053020/890242
             'kernel_name': '',
+            # always use the async kernel manager
+            # -- see https://github.com/jupyter/nbconvert/issues/1964
+            'kernel_manager_class': AsyncKernelManager,
         }
         # overrides from metadata
         ep_kwargs.update(meta_job.kind_meta.get('ep_kwargs', {}))
         try:
             resources = {
                 'metadata': {
                     'path': self.defaults.OMEGA_TMP,
```

### Comparing `omegaml-0.15.3/omegaml/notebook/jobschedule.py` & `omegaml-0.15.5/omegaml/notebook/jobschedule.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/notebook/jupyter/jupyter_notebook_config.py` & `omegaml-0.15.5/omegaml/notebook/jupyter/jupyter_notebook_config.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/notebook/jupyter/jupyter_server_config.py` & `omegaml-0.15.5/omegaml/notebook/jupyter/jupyter_server_config.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/notebook/jupyterhub/jupyterhub_config.py` & `omegaml-0.15.5/omegaml/notebook/jupyterhub/jupyterhub_config.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/notebook/jupyterhub/logo.jpg` & `omegaml-0.15.5/omegaml/notebook/jupyterhub/logo.jpg`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/notebook/omegacontentsmgr.py` & `omegaml-0.15.5/omegaml/notebook/omegacontentsmgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import json
 import nbformat
 import os
 from datetime import datetime
 from io import BytesIO
 from notebook.base.handlers import HTTPError
-from notebook.services.contents.manager import ContentsManager
+from jupyter_server.services.contents.manager import ContentsManager
 from tornado import web
 from urllib.parse import unquote
 
 from omegaml.notebook.checkpoints import NoOpCheckpoints
 
 
 class OmegaStoreContentsManager(ContentsManager):
```

### Comparing `omegaml-0.15.3/omegaml/notebook/tasks.py` & `omegaml-0.15.5/omegaml/notebook/tasks.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/omega.py` & `omegaml-0.15.5/omegaml/omega.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 from uuid import uuid4
 
 from ._version import version
+from .mixins.store.requests import CombinedStoreRequestCache
 from .store.combined import CombinedOmegaStoreMixin
 from .store.logging import OmegaSimpleLogger
 
 
-class Omega(CombinedOmegaStoreMixin):
+class Omega(CombinedStoreRequestCache, CombinedOmegaStoreMixin):
     """
     Client API to omegaml
 
     Provides the following APIs:
 
     * :code:`datasets` - access to datasets stored in the cluster
     * :code:`models` - access to models stored in the cluster
```

### Comparing `omegaml-0.15.3/omegaml/restapi/app.py` & `omegaml-0.15.5/omegaml/restapi/app.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/restapi/resources.py` & `omegaml-0.15.5/omegaml/restapi/resources.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/restapi/util.py` & `omegaml-0.15.5/omegaml/restapi/util.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/runtimes/daskruntime.py` & `omegaml-0.15.5/omegaml/runtimes/daskruntime.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/runtimes/envinstall/envinstall/__init__.py` & `omegaml-0.15.5/omegaml/runtimes/envinstall/envinstall/__init__.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/runtimes/jobproxy.py` & `omegaml-0.15.5/omegaml/runtimes/jobproxy.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/runtimes/loky.py` & `omegaml-0.15.5/omegaml/runtimes/loky.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/runtimes/mixins/gridsearch.py` & `omegaml-0.15.5/omegaml/runtimes/mixins/gridsearch.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/runtimes/mixins/modelmixin.py` & `omegaml-0.15.5/omegaml/runtimes/mixins/modelmixin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import absolute_import
 
 import logging
+import sys
+import warnings
 from uuid import uuid4
 
 from omegaml.util import is_dataframe, is_ndarray, is_series
 
 logger = logging.getLogger(__file__)
 
 
@@ -163,25 +165,33 @@
         return omega_decision_function.delay(self.modelname, Xname, rName=rName, **kwargs)
 
     def reduce(self, rName=None, **kwargs):
         omega_reduce = self.task('omegaml.tasks.omega_reduce')
         return omega_reduce.delay(modelName=self.modelname, rName=rName, **kwargs)
 
     def _ensure_data_is_stored(self, name_or_data, prefix='_temp', as_payload=False):
+        from omegaml.mixins.store.passthrough import PassthroughDataset
+
         if as_payload:
+            return PassthroughDataset(name_or_data)
+        elif isinstance(name_or_data, str):
+            name = name_or_data
+        elif isinstance(name_or_data, PassthroughDataset):
             return name_or_data
-        if is_dataframe(name_or_data) or is_series(name_or_data):
+        elif isinstance(name_or_data, (list, tuple, dict)):
+            if sys.getsizeof(name_or_data) <= PassthroughDataset.MAX_SIZE:
+                return PassthroughDataset(name_or_data)
+            else:
+                warnings.warn(f'size of dataset is larger than {PassthroughDataset.MAX_SIZE} bytes, storing in om.datasets')
+                name = '%s_%s' % (prefix, uuid4().hex)
+                self.runtime.omega.datasets.put(name_or_data, name)
+        elif is_dataframe(name_or_data) or is_series(name_or_data):
             name = '%s_%s' % (prefix, uuid4().hex)
             self.runtime.omega.datasets.put(name_or_data, name)
         elif is_ndarray(name_or_data):
             name = '%s_%s' % (prefix, uuid4().hex)
             self.runtime.omega.datasets.put(name_or_data, name)
-        elif isinstance(name_or_data, (list, tuple, dict)):
-            name = '%s_%s' % (prefix, uuid4().hex)
-            self.runtime.omega.datasets.put(name_or_data, name)
-        elif isinstance(name_or_data, str):
-            name = name_or_data
         else:
             raise TypeError(
                 'invalid type for Xpath_or_data', type(name_or_data))
         return name
```

### Comparing `omegaml-0.15.3/omegaml/runtimes/mixins/nbtasks.py` & `omegaml-0.15.5/omegaml/runtimes/mixins/nbtasks.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/runtimes/mixins/swagger/__init__.py` & `omegaml-0.15.5/omegaml/runtimes/mixins/swagger/__init__.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/runtimes/mixins/swagger/helpers.py` & `omegaml-0.15.5/omegaml/runtimes/mixins/swagger/helpers.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/runtimes/mixins/taskcanvas.py` & `omegaml-0.15.5/omegaml/runtimes/mixins/taskcanvas.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/runtimes/modelproxy.py` & `omegaml-0.15.5/omegaml/runtimes/modelproxy.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/runtimes/rsystem/__init__.py` & `omegaml-0.15.5/omegaml/runtimes/rsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/runtimes/rsystem/omegamlr.R` & `omegaml-0.15.5/omegaml/runtimes/rsystem/omegamlr.R`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/runtimes/runtime.py` & `omegaml-0.15.5/omegaml/runtimes/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from __future__ import absolute_import
 
+import os
+
+import ssl
+
 import logging
 from celery import Celery
+
+from omegaml.mongoshim import mongo_url
 from socket import gethostname
 
 from omegaml.util import dict_merge
 
 logger = logging.getLogger(__name__)
 
 
@@ -85,25 +91,15 @@
         from omegaml.util import settings
 
         self.omega = omega
         defaults = defaults or settings()
         self.bucket = bucket
         self.pure_python = getattr(defaults, 'OMEGA_FORCE_PYTHON_CLIENT', False)
         self.pure_python = self.pure_python or self._client_is_pure_python()
-        # initialize celery as a runtimes
-        taskpkgs = defaults.OMEGA_CELERY_IMPORTS
-        celeryconf = celeryconf or defaults.OMEGA_CELERY_CONFIG
-        # ensure we use current value
-        celeryconf['CELERY_ALWAYS_EAGER'] = bool(defaults.OMEGA_LOCAL_RUNTIME)
-        self.celeryapp = Celery('omegaml')
-        self.celeryapp.config_from_object(celeryconf)
-        # needed to get it to actually load the tasks
-        # https://stackoverflow.com/a/35735471
-        self.celeryapp.autodiscover_tasks(taskpkgs, force=True)
-        self.celeryapp.finalize()
+        self._create_celery_app(defaults, celeryconf=celeryconf)
         # temporary requirements, use .require() to set
         self._require_kwargs = dict(task={}, routing={})
         # fixed default arguments, use .require(always=True) to set
         self._task_default_kwargs = dict(task={}, routing={})
         # default routing label
         self._default_label = self.celeryapp.conf.get('CELERY_DEFAULT_QUEUE')
 
@@ -157,14 +153,43 @@
             om.runtime.mode(logging=False)
         """
         if local is not None:
             self.celeryapp.conf['CELERY_ALWAYS_EAGER'] = local
         self._task_default_kwargs['task']['__logging'] = logging
         return self
 
+    def _create_celery_app(self, defaults, celeryconf=None):
+        # initialize celery as a runtimes
+        taskpkgs = defaults.OMEGA_CELERY_IMPORTS
+        celeryconf = dict(celeryconf or defaults.OMEGA_CELERY_CONFIG)
+        # ensure we use current value
+        celeryconf['CELERY_ALWAYS_EAGER'] = bool(defaults.OMEGA_LOCAL_RUNTIME)
+        if celeryconf['CELERY_RESULT_BACKEND'].startswith('mongodb://'):
+            celeryconf['CELERY_RESULT_BACKEND'] = mongo_url(self.omega, drop_kwargs=['uuidRepresentation'])
+        # initialize ssl configuration
+        if celeryconf.get('BROKER_USE_SSL'):
+            # celery > 5 requires ssl options to be specific
+            # https://docs.celeryq.dev/en/stable/userguide/configuration.html#std-setting-broker_use_ssl
+            # https://github.com/celery/kombu/issues/1493
+            # https://docs.python.org/dev/library/ssl.html#ssl.wrap_socket
+            # https://www.openssl.org/docs/man3.0/man3/SSL_CTX_set_default_verify_paths.html
+            # env variables:
+            # SSL_CERT_FILE, CA_CERTS_PATH
+            self._apply_broker_ssl(celeryconf)
+        self.celeryapp = Celery('omegaml')
+        self.celeryapp.config_from_object(celeryconf)
+        # needed to get it to actually load the tasks
+        # https://stackoverflow.com/a/35735471
+        self.celeryapp.autodiscover_tasks(taskpkgs, force=True)
+        self.celeryapp.finalize()
+
+    def _apply_broker_ssl(self, celeryconf):
+        # hook to apply broker ssl options
+        pass
+
     def _client_is_pure_python(self):
         try:
             import pandas as pd
             import numpy as np
             import sklearn
         except Exception as e:
             logging.getLogger().info(e)
@@ -296,14 +321,19 @@
         taskfn = self.celeryapp.tasks.get(name)
         assert taskfn is not None, "cannot find task {name} in Celery runtime".format(**locals())
         kwargs = dict_merge(self._common_kwargs, dict(routing=kwargs))
         task = CeleryTask(taskfn, kwargs)
         self._require_kwargs = dict(routing={}, task={})
         return task
 
+    def result(self, task_id, wait=True):
+        from celery.result import AsyncResult
+        promise = AsyncResult(task_id, app=self.celeryapp)
+        return promise.get() if wait else promise
+
     def settings(self, require=None):
         """ return the runtimes's cluster settings
         """
         self.require(**require) if require else None
         return self.task('omegaml.tasks.omega_settings').delay().get()
 
     def ping(self, *args, require=None, wait=True, **kwargs):
```

### Comparing `omegaml-0.15.3/omegaml/runtimes/scriptproxy.py` & `omegaml-0.15.5/omegaml/runtimes/scriptproxy.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/runtimes/trackingproxy.py` & `omegaml-0.15.5/omegaml/runtimes/trackingproxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,18 +69,21 @@
         OmegaTrackingProxy.__nested += 1
         self.runtime.require(task=dict(__experiment=self._experiment), always=True)
         self._with_experiment = experiment = self.experiment
         no_active_run = experiment.status() in ('STOPPED', 'PENDING')
         if self._implied_run or no_active_run:
             experiment.start()
             self._implied_run = True if no_active_run else self._implied_run
+        if OmegaTrackingProxy.__nested == 1:
+            experiment.start_runtime()
         return experiment
 
     def __exit__(self, exc_type, exc_val, exc_tb):
+        experiment = self._with_experiment or self.experiment
         if self._implied_run:
-            experiment = self._with_experiment or self.experiment
             experiment.stop()
         self._with_experiment = None
         OmegaTrackingProxy.__nested -= 1
         # remove task argument
         if OmegaTrackingProxy.__nested == 0:
             self.runtime.require(task=dict(__experiment=None), always=True)
+            experiment.stop_runtime()
```

### Comparing `omegaml-0.15.3/omegaml/sklext.py` & `omegaml-0.15.5/omegaml/sklext.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/store/base.py` & `omegaml-0.15.5/omegaml/store/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,23 +76,23 @@
 import bson
 import gridfs
 import os
 import tempfile
 import warnings
 from datetime import datetime
 from mongoengine.connection import disconnect, \
-    connect, _connections, get_db, _connection_settings
+    connect, _connections, get_db
 from mongoengine.errors import DoesNotExist
 from mongoengine.fields import GridFSProxy
 from mongoengine.queryset.visitor import Q
-from uuid import uuid4
-
 from omegaml.store.fastinsert import fast_insert, default_chunksize
 from omegaml.util import unravel_index, restore_index, make_tuple, jsonescape, \
     cursor_to_dataframe, convert_dtypes, load_class, extend_instance, ensure_index, PickableCollection, mongo_compatible
+from uuid import uuid4
+
 from ..documents import make_Metadata, MDREGISTRY
 from ..mongoshim import sanitize_mongo_kwargs, waitForConnection
 from ..util import (is_estimator, is_dataframe, is_ndarray, is_spark_mllib,
                     settings as omega_settings, urlparse, is_series)
 
 
 class OmegaStore(object):
@@ -611,35 +611,50 @@
         this requires the list, tuple or dict to be convertible into
         a dataframe
         """
         import pandas as pd
         df = pd.DataFrame(obj)
         return self.put_dataframe_as_hdf(df, name, attributes=attributes)
 
-    def put_pyobj_as_document(self, obj, name, attributes=None, append=True):
+    def put_pyobj_as_document(self, obj, name, attributes=None, append=True, index=None, as_many=None, **kwargs):
         """
         store a dict as a document
 
         similar to put_dataframe_as_documents no data will be replaced by
         default. that is, obj is appended as new documents into the objects'
         mongo collection. to replace the data, specify append=False.
         """
         collection = self.collection(name)
         if append is False:
             collection.drop()
         elif append is None and collection.esimated_document_count(limit=1):
             from warnings import warn
             warn('%s already exists, will append rows' % name)
-        if isinstance(obj, (list, tuple)) and isinstance(obj[0], (list, tuple)):
+        if index:
+            # create index with appropriate options
+            from omegaml.store import MongoQueryOps
+            if isinstance(index, dict):
+                idx_kwargs = index
+                index = index.pop('columns')
+            else:
+                idx_kwargs = {}
+            index = [f'data.{c}' for c in index]
+            keys, idx_kwargs = MongoQueryOps().make_index(index, **idx_kwargs)
+            ensure_index(collection, keys, **idx_kwargs)
+        if as_many is None:
+            as_many = isinstance(obj, (list, tuple)) and isinstance(obj[0], (list, tuple))
+        if as_many:
             # list of lists are inserted as many objects, as in pymongo < 4
-            result = collection.insert_many((mongo_compatible({'data': item}) for item in obj))
+            records = (mongo_compatible({'data': item}) for item in obj)
+            result = collection.insert_many(records)
             objid = result.inserted_ids[-1]
         else:
             result = collection.insert_one(mongo_compatible({'data': obj}))
             objid = result.inserted_id
+
         return self._make_metadata(name=name,
                                    prefix=self.prefix,
                                    bucket=self.bucket,
                                    kind=MDREGISTRY.PYTHON_DATA,
                                    collection=collection.name,
                                    attributes=attributes,
                                    objid=objid).save()
@@ -847,53 +862,61 @@
                 return self.get_python_data(name, version=version, **kwargs)
             elif meta.kind == MDREGISTRY.PANDAS_HDF:
                 return self.get_dataframe_hdf(name, version=version)
         return self.get_object_as_python(meta, version=version)
 
     def get_dataframe_documents(self, name, columns=None, lazy=False,
                                 filter=None, version=-1, is_series=False,
-                                chunksize=None,
+                                chunksize=None, sanitize=True,
                                 **kwargs):
         """
         Internal method to return DataFrame from documents
 
         :param name: the name of the object (str)
         :param columns: the column projection as a list of column names
         :param lazy: if True returns a lazy representation as an MDataFrame.
            If False retrieves all data and returns a DataFrame (default)
         :param filter: the filter to be applied as a column__op=value dict
+        :param sanitize: sanitize filter by removing all $op filter keys,
+          defaults to True. Specify False to allow $op filter keys. $where
+          is always removed as it is considered unsafe.
         :param version: the version to retrieve (not supported)
         :param is_series: if True retruns a Series instead of a DataFrame
         :param kwargs: remaining kwargs are used a filter. The filter kwarg
            overrides other kwargs.
         :return: the retrieved object (DataFrame, Series or MDataFrame)
 
         """
+        from omegaml.store.queryops import sanitize_filter
+        from omegaml.store.filtered import FilteredCollection
+
         collection = self.collection(name)
         meta = self.metadata(name)
         if lazy or chunksize:
             from ..mdataframe import MDataFrame
             filter = filter or kwargs
+            filter = sanitize_filter(filter, no_ops=sanitize)
             df = MDataFrame(collection,
                             metadata=meta.kind_meta,
                             columns=columns).query(**filter)
             if is_series:
                 df = df[0]
             if chunksize is not None and chunksize > 0:
                 return df.iterchunks(chunksize=chunksize)
         else:
             # TODO ensure the same processing is applied in MDataFrame
             # TODO this method should always use a MDataFrame disregarding lazy
             filter = filter or kwargs
             if filter:
                 from .query import Filter
+                filter = sanitize_filter(filter, no_ops=sanitize)
                 query = Filter(collection, **filter).query
-                cursor = collection.find(filter=query, projection=columns)
+                cursor = FilteredCollection(collection).find(filter=query, projection=columns)
             else:
-                cursor = collection.find(projection=columns)
+                cursor = FilteredCollection(collection).find(projection=columns)
             # restore dataframe
             df = cursor_to_dataframe(cursor)
             if '_id' in df.columns:
                 del df['_id']
             if hasattr(meta, 'kind_meta'):
                 df = convert_dtypes(df, meta.kind_meta.get('dtypes', {}))
             # -- restore columns
@@ -942,36 +965,41 @@
                 if item not in groupby_columns:
                     modified_query_param = '_data.' + item
                     modified_params[modified_query_param] = kwargs.get(item)
                 else:
                     modified_params[item] = kwargs.get(item)
         return modified_params
 
-    def get_dataframe_dfgroup(self, name, version=-1, kwargs=None):
+    def get_dataframe_dfgroup(self, name, version=-1, sanitize=True, kwargs=None):
         """
         Return a grouped dataframe
 
         :param name: the name of the object
         :param version: not supported
         :param kwargs: mongo db query arguments to be passed to
                collection.find() as a filter.
+        :param sanitize: remove any $op operators in kwargs
 
         """
         import pandas as pd
+        from omegaml.store.queryops import sanitize_filter
+        from omegaml.store.filtered import FilteredCollection
+
         def convert_doc_to_row(cursor):
             for doc in cursor:
                 data = doc.pop('_data', [])
                 for row in data:
                     doc.update(row)
                     yield doc
 
-        datastore = self.collection(name)
+        datastore = FilteredCollection(self.collection(name))
         kwargs = kwargs if kwargs else {}
         params = self.rebuild_params(kwargs, datastore)
-        cursor = datastore.find(params, {'_id': False})
+        params = sanitize_filter(params, no_ops=sanitize)
+        cursor = datastore.find(params, projection={'_id': False})
         df = pd.DataFrame(convert_doc_to_row(cursor))
         return df
 
     def get_dataframe_hdf(self, name, version=-1):
         """
         Retrieve dataframe from hdf
 
@@ -987,25 +1015,27 @@
             df = self._extract_dataframe_hdf(filename, version=version)
             return df
         else:
             raise gridfs.errors.NoFile(
                 "{0} does not exist in mongo collection '{1}'".format(
                     name, self.bucket))
 
-    def get_python_data(self, name, version=-1, **kwargs):
+    def get_python_data(self, name, version=-1, lazy=False, **kwargs):
         """
         Retrieve objects as python data
 
         :param name: The name of object
         :param version: The version of object
 
         :return: Returns the object as python list object
         """
         datastore = self.collection(name)
         cursor = datastore.find(**kwargs)
+        if lazy:
+            return cursor
         data = (d.get('data') for d in cursor)
         return list(data)
 
     def get_object_as_python(self, meta, version=-1):
         """
         Retrieve object as python object
```

### Comparing `omegaml-0.15.3/omegaml/store/combined.py` & `omegaml-0.15.5/omegaml/store/combined.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/store/fastinsert.py` & `omegaml-0.15.5/omegaml/store/fastinsert.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/store/filtered.py` & `omegaml-0.15.5/omegaml/store/filtered.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from __future__ import absolute_import
 
+import logging
+
+import warnings
+
 from omegaml.store import qops
 from omegaml.store.query import Filter
 from omegaml.util import PickableCollection, ensure_base_collection
 
+logger = logging.getLogger(__name__)
 
 class FilteredCollection:
     """
     A permanently filtered collection
 
     Supports all methods as a Collection does, however any filter or query
     argument is permanently set at instantiation
@@ -44,15 +49,16 @@
     Here expression will only apply to this particular method call. The
     global filter set by query= is unchanged.
 
     If no expression is given, the empty expression {} is assumed. To change
     the expression for the set fcoll.query = { expression }
     """
 
-    def __init__(self, collection, query=None, projection=None, **kwargs):
+    def __init__(self, collection, query=None, projection=None,
+                 **kwargs):
         if isinstance(collection, FilteredCollection):
             # avoid cascading of FilteredCollections
             query = query or collection._fixed_query
             projection = projection or collection.projection
             collection = ensure_base_collection(collection)
         else:
             query = query or {}
@@ -74,60 +80,60 @@
 
     @property
     def query(self):
         return Filter(self.collection, **self._fixed_query).query
 
     def aggregate(self, pipeline, filter=None, **kwargs):
         query = dict(self.query)
-        query.update(filter or {})
+        query.update(self._sanitize_filter(filter or {}))
         pipeline.insert(0, qops.MATCH(query))
         kwargs.update(allowDiskUse=True)
         return self.collection.aggregate(pipeline, **kwargs)
 
     def find(self, filter=None, **kwargs):
         query = dict(self.query)
-        query.update(filter or {})
+        query.update(self._sanitize_filter(filter or {}))
         return self.collection.find(filter=query, **kwargs)
 
     def find_one(self, filter=None, *args, **kwargs):
         query = dict(self.query)
-        query.update(filter or {})
+        query.update(self._sanitize_filter(filter or {}))
         return self.collection.find_one(query, *args, **kwargs)
 
     def find_one_and_delete(self, filter=None, **kwargs):
         query = dict(self.query)
-        query.update(filter or {})
+        query.update(self._sanitize_filter(filter or {}))
         return self.collection.find_one_and_delete(query,
                                                    **kwargs)
 
     def find_one_and_replace(self, replacement, filter=None, **kwargs):
         query = dict(self.query)
-        query.update(filter or {})
+        query.update(self._sanitize_filter(filter or {}))
         return self.collection.find_one_and_replace(query,
                                                     replacement,
                                                     **kwargs)
 
     def find_one_and_update(self, update, filter=None, **kwargs):
         query = dict(self.query)
-        query.update(filter or {})
+        query.update(self._sanitize_filter(filter or {}))
         return self.collection.find_one_and_update(query,
                                                    update,
                                                    **kwargs)
 
     def estimated_document_count(self, **kwargs):
         return self.collection.estimated_document_count(**kwargs)
 
     def count_documents(self, filter=None, **kwargs):
         query = dict(self.query)
-        query.update(filter or {})
+        query.update(self._sanitize_filter(filter or {}))
         return self.collection.count_documents(query, **kwargs)
 
     def distinct(self, key, filter=None, **kwargs):
         query = dict(self.query)
-        query.update(filter or {})
+        query.update(self._sanitize_filter(filter or {}))
         return self.collection.distinct(key, filter=query, **kwargs)
 
     def create_index(self, keys, **kwargs):
         return self.collection.create_index(keys, **kwargs)
 
     def list_indexes(self, **kwargs):
         return self.collection.list_indexes(**kwargs)
@@ -151,7 +157,14 @@
     def ensure_index(self, *args, **kwargs):
         raise NotImplementedError(
             "deprecated in Collection and not implemented in FilteredCollection")
 
     def save(self, *args, **kwargs):
         raise NotImplementedError(
             "deprecated in Collection and not implemented in FilteredCollection")
+
+    def _sanitize_filter(self, filter):
+        from omegaml.store.queryops import sanitize_filter
+        sanitize_filter(filter)
+        logger.debug(f'executing mongodb query filter {filter}')
+        return filter
+
```

### Comparing `omegaml-0.15.3/omegaml/store/logging.py` & `omegaml-0.15.5/omegaml/store/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,22 +232,23 @@
             return
         # insert a log message
         fmt = '{created} {level} {message}'
         log_entry = _make_log_entry(level, levelno, self._name, message, fmt=fmt,
                                     hostname=LOGGER_HOSTNAME, userid=self.userid)
         # log to dataset
         self.collection.insert_one(log_entry)
-        # log to system
+        # optionally log to system (e.g. external log aggregation)
         # -- we use extra to pass along the same information that we log in omega dataset
         #    see https://docs.python.org/3/library/logging.html#logging.debug
         # -- we mark this record to avoid double logging in case of an active OmegaLoggingHandler
-        pylogmeth = getattr(python_logger, level.lower(), 'INFO')
-        pylogmeth(message, extra=dict(userid=self.userid,
-                                      hostname=LOGGER_HOSTNAME,
-                                      _from_simplelogger=True))
+        if getattr(self.defaults, 'OMEGA_LOG_PYTHON', False) :
+            pylogmeth = getattr(python_logger, level.lower())
+            pylogmeth(message, extra=dict(userid=self.userid,
+                                          hostname=LOGGER_HOSTNAME,
+                                          _from_simplelogger=True))
 
     def info(self, message, **kwargs):
         self.log('INFO', message, **kwargs)
 
     def error(self, message, **kwargs):
         self.log('ERROR', message, **kwargs)
```

### Comparing `omegaml-0.15.3/omegaml/store/query.py` & `omegaml-0.15.5/omegaml/store/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import warnings
 
 from omegaml.store.queryops import MongoQueryOps, flatten_keys
 from omegaml.util import restore_index
 
 
 class MongoQ(object):
 
@@ -40,15 +41,15 @@
     Evaluation works as follows:
 
     1. for each Q object, apply the filters as collection.find(query)
     2. return the dataframe
 
     """
     def __init__(self, **kwargs):
-        self.conditions = kwargs
+        self.conditions = self._sanitize_filter(kwargs)
         self.qlist = [('', self)]
         # should we return ~(conditions)
         self._inv = False
         # is sorting implied by some operator
         self.sorted = False
 
     def __repr__(self):
@@ -228,14 +229,19 @@
     def __invert__(self):
         """
         return an inverted version of this object
         """
         notq = copy.deepcopy(self).negate()
         return notq
 
+    def _sanitize_filter(self, filter):
+        from omegaml.store.queryops import sanitize_filter
+        return sanitize_filter(filter)
+
+
 
 class Filter(object):
 
     """
     Filter for OmegaStore objects
 
     Allow keyword style filtering of dataframes:
@@ -396,7 +402,8 @@
              to the real data. makes more sense even though the results
              are somewhat different this way, but match better semantically
         """
         return self.value == self.value
 
     def __repr__(self):
         return ' '.join(f'Filter({self.q})'.replace('\n', ' ').split())
+
```

### Comparing `omegaml-0.15.3/omegaml/store/queryops.py` & `omegaml-0.15.5/omegaml/store/queryops.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import absolute_import
 
+import warnings
+
 import json
 import pymongo
 import sys
 from hashlib import md5
 
 from omegaml.util import make_tuple
 
@@ -404,10 +406,35 @@
     # avoid generating a name if already given
     if not 'name' in kwargs:
         name = md5(str(idx).encode('utf8')).hexdigest()
         kwargs.setdefault('name', name)
     return idx, kwargs
 
 
+def sanitize_filter(filter, no_ops=False):
+    """ sanitize mongodb filter statements """
+    injection_ops = ['$where', '$mapReduce']
+    user_ops = [k for k in filter if k.strip().startswith('$') and k not in injection_ops]
+    ops_to_remove = user_ops + injection_ops if no_ops else injection_ops
+    # sanitize user and default operators
+    if user_ops and not no_ops:
+        warnings.warn(f'Your MongoDB query contains operators {user_ops} which may be unsafe if not sanitized.')
+    for op in ops_to_remove:
+        value = filter.pop(op, None)
+        if value is not None:
+            repl_op = op.replace('$', '-')
+            warnings.warn(f'{op} clauses are not permitted and replaced by {repl_op} for security reasons.')
+            filter[repl_op] = value
+    # sanitize nested operators
+    for k, v in filter.items():
+        if isinstance(v, dict):
+            sanitize_filter(v, no_ops=no_ops)
+        elif isinstance(v, (list, tuple)):
+            for el in v:
+                if isinstance(el, dict):
+                    sanitize_filter(el, no_ops=no_ops)
+    return filter
+
+
 # convenience accessors
 x = MongoQueryOps()
 d = dict
```

### Comparing `omegaml-0.15.3/omegaml/store/streams.py` & `omegaml-0.15.5/omegaml/store/streams.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tasks.py` & `omegaml-0.15.5/omegaml/tasks.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/cli/scenarios.py` & `omegaml-0.15.5/omegaml/tests/core/cli/scenarios.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/cli/test_cli.py` & `omegaml-0.15.5/omegaml/tests/core/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/cli/test_cli_datasets.py` & `omegaml-0.15.5/omegaml/tests/core/cli/test_cli_datasets.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/cli/test_cli_jobs.py` & `omegaml-0.15.5/omegaml/tests/core/cli/test_cli_jobs.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/cli/test_cli_models.py` & `omegaml-0.15.5/omegaml/tests/core/cli/test_cli_models.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/cli/test_cli_runtime.py` & `omegaml-0.15.5/omegaml/tests/core/cli/test_cli_runtime.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/cli/test_cli_scripts.py` & `omegaml-0.15.5/omegaml/tests/core/cli/test_cli_scripts.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/restapi/test_api_buckets.py` & `omegaml-0.15.5/omegaml/tests/core/restapi/test_api_buckets.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/restapi/test_job_api.py` & `omegaml-0.15.5/omegaml/tests/core/restapi/test_job_api.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/restapi/test_model_api.py` & `omegaml-0.15.5/omegaml/tests/core/restapi/test_model_api.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/restapi/test_model_api_async.py` & `omegaml-0.15.5/omegaml/tests/core/restapi/test_model_api_async.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/restapi/test_script_api.py` & `omegaml-0.15.5/omegaml/tests/core/restapi/test_script_api.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/restapi/test_service_api.py` & `omegaml-0.15.5/omegaml/tests/core/restapi/test_service_api.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/restapi/util.py` & `omegaml-0.15.5/omegaml/tests/core/restapi/util.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_backendbase.py` & `omegaml-0.15.5/omegaml/tests/core/test_backendbase.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_configs.py` & `omegaml-0.15.5/omegaml/tests/core/test_configs.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_contentsmgr.py` & `omegaml-0.15.5/omegaml/tests/core/test_contentsmgr.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_dashapp_backend.py` & `omegaml-0.15.5/omegaml/tests/core/test_dashapp_backend.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_datarevision.py` & `omegaml-0.15.5/omegaml/tests/core/test_datarevision.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_extdmeta.py` & `omegaml-0.15.5/omegaml/tests/core/test_extdmeta.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_imexport.py` & `omegaml-0.15.5/omegaml/tests/core/test_imexport.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_iotools.py` & `omegaml-0.15.5/omegaml/tests/core/test_iotools.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_jobs.py` & `omegaml-0.15.5/omegaml/tests/core/test_jobs.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_logging.py` & `omegaml-0.15.5/omegaml/tests/core/test_logging.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_mdataframe.py` & `omegaml-0.15.5/omegaml/tests/core/test_mdataframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import absolute_import
 
+import warnings
+
 from datetime import datetime
 
 import random
 import string
 
 import numpy as np
 import os
@@ -547,7 +549,63 @@
     def test_items(self):
         om = self.om
         mdf = om.datasets.getl('sample')
         df = mdf.value
         for df_row, mdf_row in zip(mdf.items(), df.items()):
             self.assertEqual(type(df_row), type(mdf_row))
             assert_series_equal(df_row[1], mdf_row[1])
+
+    def test_filter_injection(self):
+        om = self.om
+        # check that where statements are not executed
+        injected = {
+            "$where": "function() { return true; }"
+        }
+        mdf = om.datasets.getl('sample', filter=injected)
+        self.assertEqual(len(mdf.value), 0)
+        # check that $operators are not executed by default
+        injected = {
+            "$or": [{
+                "x": -1,
+                "$where": "function() { return true; }"
+            }]
+        }
+        mdf = om.datasets.getl('sample', filter=injected, sanitize=False)
+        # if $where is executed we get rows back, else None (x == -1 is never true)
+        self.assertEqual(len(mdf.value), 0)
+        # check variable replacements that contain filters are detected
+        # -- lazy eval
+        injected = {
+            "$gt": 0
+        }
+        query = {
+            'x': injected
+        }
+        with self.assertLogs('omegaml', 'DEBUG') as cm:
+            mdf = om.datasets.getl('sample', filter=query)
+            result = mdf.value
+        # if injected condition is executed we get rows back, else None
+        # since x: "-gt: 0" is not a valid condition
+        self.assertIn("{'-gt': 0}", str(cm.output))
+        self.assertEqual(len(result), 0)
+        # -- direct eval
+        injected = {
+            "$gt": 0
+        }
+        query = {
+            'x': injected
+        }
+        with self.assertLogs('omegaml', 'DEBUG') as cm:
+            result = om.datasets.get('sample', filter=query)
+        # if injected condition is executed we get rows back, else None
+        # since x: "-gt: 0" is not a valid condition
+        self.assertIn("{'-gt': 0}", str(cm.output))
+        self.assertEqual(len(result), 0)
+        # check we can ask $operators other than $where to be executed
+        injected = {
+            "$and": [{
+                "x": {"$gte": 0},
+            }]
+        }
+        mdf = om.datasets.getl('sample', filter=injected, sanitize=False)
+        df = om.datasets.get('sample')
+        self.assertEqual(len(mdf.value), len(df))
```

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_mdfmixins.py` & `omegaml-0.15.5/omegaml/tests/core/test_mdfmixins.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_mdfparallel.py` & `omegaml-0.15.5/omegaml/tests/core/test_mdfparallel.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_misc.py` & `omegaml-0.15.5/omegaml/tests/core/test_misc.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_modelversions.py` & `omegaml-0.15.5/omegaml/tests/core/test_modelversions.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_nbtasks.py` & `omegaml-0.15.5/omegaml/tests/core/test_nbtasks.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_npndarray.py` & `omegaml-0.15.5/omegaml/tests/core/test_npndarray.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_package.py` & `omegaml-0.15.5/omegaml/tests/core/test_package.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_package_remote.py` & `omegaml-0.15.5/omegaml/tests/core/test_package_remote.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_promotion.py` & `omegaml-0.15.5/omegaml/tests/core/test_promotion.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_query.py` & `omegaml-0.15.5/omegaml/tests/core/test_query.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_restauth.py` & `omegaml-0.15.5/omegaml/tests/core/test_restauth.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_runtime.py` & `omegaml-0.15.5/omegaml/tests/core/test_runtime.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_sklext.py` & `omegaml-0.15.5/omegaml/tests/core/test_sklext.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_sqlalchemy.py` & `omegaml-0.15.5/omegaml/tests/core/test_sqlalchemy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import os
 from getpass import getuser
 from unittest import TestCase
 
+import os
 import pandas as pd
-from pandas.testing import assert_frame_equal
-from sqlalchemy.engine import Connection, create_engine, ResultProxy
-
 from omegaml import Omega
 from omegaml.backends.sqlalchemy import SQLAlchemyBackend
 from omegaml.tests.util import OmegaTestMixin
+from pandas.testing import assert_frame_equal
+from sqlalchemy.engine import Connection, create_engine, ResultProxy
 
 
 class SQLAlchemyBackendTests(OmegaTestMixin, TestCase):
     def setUp(self):
         self.om = Omega()
         self.om.models.register_backend(SQLAlchemyBackend.KIND, SQLAlchemyBackend)
         self.clean()
@@ -34,28 +33,51 @@
     def test_put_connection_with_secrets(self):
         """
         store generic sqlalchemy connection
         """
         om = self.om
         cnx = 'sqlite:///{user}.db'
         om.datasets.put(cnx, 'testsqlite', kind=SQLAlchemyBackend.KIND)
+        # -- test missing key values do not raise KeyError
+        om.datasets.defaults.OMEGA_FOOBAR = '{othervalue}'
         self.assertIn('testsqlite', om.datasets.list())
         meta = om.datasets.metadata('testsqlite')
         self.assertEqual(meta.kind, SQLAlchemyBackend.KIND)
         self.assertIn('secrets', meta.kind_meta)
         # no secrets
         with self.assertRaises(KeyError):
             om.datasets.get('testsqlite')
         # directly specified
         conn = om.datasets.get('testsqlite', raw=True, secrets=dict(user='user'))
         # via vault
         om.datasets.put(dict(userid=getuser(), user='foobar'), '.omega/vault', append=False)
         conn = om.datasets.get('testsqlite', raw=True)
         self.assertIsInstance(conn, Connection)
 
+    def test_connection_cache(self):
+        """ test connection caching
+        """
+        from omegaml.backends import sqlalchemy
+        om = self.om
+        cnx = 'sqlite:///{user}.db'
+        om.datasets.put(cnx, 'testsqlite', kind=SQLAlchemyBackend.KIND)
+        conn = om.datasets.get('testsqlite', raw=True, secrets=dict(user='user'), keep=True)
+        conn_ = om.datasets.get('testsqlite', raw=True, secrets=dict(user='user'), keep=True)
+        self.assertEqual(conn.engine, conn_.engine)
+        # drop should clear cache
+        om.datasets.drop('testsqlite', secrets=dict(user='user'))
+        conn_ = om.datasets.get('testsqlite', raw=True, secrets=dict(user='user'), keep=True)
+        self.assertIsNone(conn_)
+        self.assertTrue(len(sqlalchemy.SQLAlchemyBackend._SQLAlchemyBackend__CNX_CACHE) == 0)
+        # even if we drop without secrets, cache is cleared
+        om.datasets.put(cnx, 'testsqlite', kind=SQLAlchemyBackend.KIND)
+        om.datasets.get('testsqlite', raw=True, secrets=dict(user='user'), keep=True)
+        om.datasets.drop('testsqlite')
+        self.assertTrue(len(sqlalchemy.SQLAlchemyBackend._SQLAlchemyBackend__CNX_CACHE) == 0)
+
     def test_put_connection_with_sql(self):
         """
         store generic sqlalchemy connection with sql, same principle as a view
         """
         om = self.om
         cnx_str = 'sqlite:///test.db'
         engine = create_engine(cnx_str)
@@ -82,15 +104,15 @@
         engine = create_engine(cnx_str)
         cnx = engine.connect()
         df = pd.DataFrame({
             'x': range(10)
         })
         df.to_sql('foobar', cnx, if_exists='replace', index=False)
         om.datasets.put(cnx_str, 'foobar',
-                        sql='select {cols} from foobar',
+                        sql='select {{cols}} from foobar',
                         kind=SQLAlchemyBackend.KIND)
         self.assertIn('foobar', om.datasets.list())
         meta = om.datasets.metadata('foobar')
         self.assertEqual(meta.kind, SQLAlchemyBackend.KIND)
         with self.assertRaises(KeyError):
             # missing sqlvars
             dfx = om.datasets.get('foobar')
@@ -105,25 +127,27 @@
         cnx_str = 'sqlite:///test.db'
         engine = create_engine(cnx_str)
         cnx = engine.connect()
         df = pd.DataFrame({
             'x': range(10)
         })
         df.to_sql('foobar', cnx, if_exists='replace', index=False)
+        # using
         om.datasets.put(cnx_str, 'foobar',
-                        sql='select {cols} from foobar',
+                        sql='select {{cols}} from foobar',
                         kind=SQLAlchemyBackend.KIND)
         self.assertIn('foobar', om.datasets.list())
         meta = om.datasets.metadata('foobar')
         self.assertEqual(meta.kind, SQLAlchemyBackend.KIND)
         with self.assertRaises(KeyError):
             # missing sqlvars
             dfx = om.datasets.get('foobar')
-        dfx = om.datasets.getl('foobar', sqlvars=dict(cols='x'))
+        dfx = om.datasets.getl('foobar', sqlvars=dict(cols='x as x'))
         self.assertIsInstance(dfx, ResultProxy)
+        print(list(dfx))
 
     def test_put_copy_from_connection(self):
         """
         store generic sqlalchemy connection
         """
         om = self.om
         cnx_str = 'sqlite:///test.db'
@@ -272,7 +296,62 @@
         assert_frame_equal(df, dfx)
         # append
         om.datasets.put(raw, 'testsqlite', insert=True, append=False)
         om.datasets.put(raw, 'testsqlite', insert=True)
         dfx = om.datasets.get('testsqlite', sql='select * from foo')
         df_expected = df.append(df)
         assert_frame_equal(dfx, df_expected)
+
+    def test_query_in_clause(self):
+        om = self.om
+        cnx_str = 'sqlite:///test.db'
+        engine = create_engine(cnx_str)
+        cnx = engine.connect()
+        df = pd.DataFrame({
+            'x': range(10)
+        })
+        df.to_sql('foobar', cnx, if_exists='replace', index=False)
+        om.datasets.put(cnx_str, 'foobar',
+                        sql='select * from foobar where x in {x} or x in {y}',
+                        kind=SQLAlchemyBackend.KIND)
+        df_db = om.datasets.get('foobar', sqlvars={
+            'x': [1, 2, 3],
+            'y': [5, 6, 7]
+        })
+        fltx = df['x'].isin([1, 2, 3])
+        flty = df['x'].isin([5, 6, 7])
+        df_filtered = df[fltx | flty].reset_index(drop=True)
+        assert_frame_equal(df_db, df_filtered)
+
+    def test_put_connection_with_sql_injection(self):
+        """
+        attempt sql injection
+        """
+        om = self.om
+        cnx_str = 'sqlite:///test.db'
+        engine = create_engine(cnx_str)
+        cnx = engine.connect()
+        df = pd.DataFrame({
+            'x': range(10)
+        })
+        df.to_sql('foobar', cnx, if_exists='replace', index=False)
+        om.datasets.put(cnx_str, 'foobar',
+                        sql='select * from foobar where x={x} and x > 5',
+                        kind=SQLAlchemyBackend.KIND)
+        self.assertIn('foobar', om.datasets.list())
+        meta = om.datasets.metadata('foobar')
+        self.assertEqual(meta.kind, SQLAlchemyBackend.KIND)
+        # simulate sql injection
+        # -- if injection is executed, will return all rows
+        # -- if injection is not executed will return no rows
+        #    (because no row matches the {x}="-1 or 0=0" statement)
+        # -- the log statement prints the sql with {x} replaced as :x
+        #    (:notation denotes bound variables)
+        # -- the sqlvars are passed on to sqlalchemy.execute verbatim,
+        #    i.e. are not interpreted as part of the sql statement
+        injection = "-1 or 0=0 --"
+        sqlvars = {'x': injection}
+        with self.assertLogs('omegaml', level='DEBUG') as cm:
+            dfx = om.datasets.get('foobar', sqlvars=sqlvars)
+        self.assertEqual(len(dfx), 0)
+        self.assertIn("select * from foobar where x=:x", str(cm.output))
+        self.assertIn("{'x': '-1 or 0=0 --'}", str(cm.output))
```

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_store.py` & `omegaml-0.15.5/omegaml/tests/core/test_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from __future__ import absolute_import
 
+import warnings
+
 from io import BytesIO
 from unittest import skip
 
 import gridfs
 import joblib
 import pandas as pd
 import unittest
 import uuid
 from datetime import timedelta, datetime
+
+import pymongo
 from mongoengine.connection import disconnect
 from mongoengine.errors import DoesNotExist, FieldDoesNotExist
 from pandas.testing import assert_frame_equal, assert_series_equal
 from pymongo.errors import OperationFailure
 from sklearn.datasets import load_iris
 from sklearn.linear_model import LogisticRegression, LinearRegression
 
@@ -378,14 +382,34 @@
             'a': list(range(1, 10)),
             'b': list(range(1, 10))
         }
         store = OmegaStore(prefix='')
         store.put(data, 'mydata')
         data2 = store.get('mydata')
         self.assertEqual([data], data2)
+        # check we can get back a cursor instead of data
+        cursor = store.get('mydata', lazy=True)
+        self.assertIsInstance(cursor, pymongo.cursor.Cursor)
+        data = list(doc.get('data') for doc in cursor)
+        self.assertEqual(data, data2)
+
+
+    def test_put_python_dict_with_index(self):
+        # create some data
+        data = {
+            'a': list(range(1, 10)),
+            'b': list(range(1, 10))
+        }
+        store = OmegaStore(prefix='')
+        store.put(data, 'mydata', index=['a'])
+        coll = store.collection('mydata')
+        # SON(..., 'keys': { key: order, ...}) => ['key', ...]
+        idxs = [son.to_dict()['key'] for son in coll.list_indexes()]
+        idxs_keys = [list(sorted(d.keys())) for d in idxs]
+        self.assertTrue(any(keys == ['data.a'] for keys in idxs_keys))
 
     def test_put_python_dict_multiple(self):
         # create some data
         data = {
             'a': list(range(1, 10)),
             'b': list(range(1, 10))
         }
@@ -518,14 +542,42 @@
         df2 = store.get('dfgroup', kwargs={'b': 1})
         self.assertTrue(df2.equals(result_df[df2.columns]))
         df3 = store.get('dfgroup')
         self.assertTrue(df3.equals(df[df3.columns]))
         df4 = store.get('dfgroup', kwargs={'a': 1})
         self.assertTrue(df4.equals(result_df[df4.columns]))
 
+    def test_store_dataframe_as_dfgroup_injected(self):
+        data = {
+            'a': list(range(1, 10)),
+            'b': list(range(1, 10))
+        }
+        result_data = {
+            'a': list(range(1, 2)),
+            'b': 1,
+        }
+        df = pd.DataFrame(data)
+        result_df = pd.DataFrame(result_data)
+        store = OmegaStore()
+        groupby_columns = ['b']
+        meta = store.put(df, 'dfgroup', groupby=groupby_columns)
+        injected = {
+            '$gt': 0,
+        }
+        with warnings.catch_warnings(record=True) as wrn:
+            warnings.simplefilter('always')
+            df2 = store.get('dfgroup', kwargs={'b': injected})
+            warnlog = str(list(w.message for w in wrn))
+        self.assertIn('$gt clauses are not permitted', warnlog)
+        with self.assertLogs('omegaml', 'DEBUG') as cm:
+            df2 = store.get('dfgroup', kwargs={'b': injected})
+            log = cm.output
+        self.assertIn("{'b': {'-gt': 0}}", str(log))
+        self.assertEqual(len(df2), 0)
+
     def test_store_dataframe_as_hdf(self):
         data = {
             'a': list(range(1, 10)),
             'b': list(range(1, 10))
         }
         df = pd.DataFrame(data)
         store = OmegaStore()
```

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_tracking.py` & `omegaml-0.15.5/omegaml/tests/core/test_tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,32 @@
 
 class TrackingTestCases(OmegaTestMixin, unittest.TestCase):
     def setUp(self):
         self.om = om = Omega()
         self.clean()
         om.models.register_backend(ExperimentBackend.KIND, ExperimentBackend)
 
+    def test_initialize(self):
+        om = self.om
+        exp = om.runtime.experiment('test')
+        coll = om.datasets.collection(exp._data_name)
+        # SON(..., 'keys': { key: order, ...}) => ['key', ...]
+        idxs = [son.to_dict()['key'] for son in coll.list_indexes()]
+        idxs_keys = [list(sorted(d.keys())) for d in idxs]
+        self.assertTrue(any(keys == ['data.event', 'data.run'] for keys in idxs_keys))
+
     def test_ensure_active(self):
         # explicit start
         om = self.om
         exp = om.runtime.experiment('test')
         with self.assertRaises(ValueError):
             exp.log_param('foo', 'bar')
         run = exp.start()
         exp.log_param('foo', 'bar')
+        exp.flush()
         data = exp.data(run=run)
         self.assertIsNotNone(run)
         self.assertEqual(len(data), 2)
         # reuse latest run
         exp = om.runtime.experiment('test')
         with self.assertRaises(ValueError):
             exp.log_param('foo', 'bar')
@@ -275,14 +285,15 @@
         meta = om.models.metadata('experiments/foo')
         dataset = meta.attributes['tracking']['dataset']
         self.assertIsNotNone(dataset)
         self.assertIn(dataset, om.datasets.list(hidden=True))
         self.assertIn('experiments/foo', om.models.list())
         # add a metric, then clean
         exp.log_metric(5, 'accuracy')
+        exp.flush()
         self.assertEqual(len(exp.data()), 4)
         # explicit drop
         om.models.drop('experiments/foo', data_store=om.datasets)
         self.assertNotIn(dataset, om.datasets.list(hidden=True))
         # no more data present
         self.assertIsNone(exp.data())
```

### Comparing `omegaml-0.15.3/omegaml/tests/core/test_virtualobj.py` & `omegaml-0.15.5/omegaml/tests/core/test_virtualobj.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/features/environment.py` & `omegaml-0.15.5/omegaml/tests/features/environment.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 # -- FILE: features/environment.py
 # CONTAINS: Browser fixture setup and teardown
 import os
 
 import nbformat
 from behave import fixture, use_fixture
 from selenium.webdriver import ChromeOptions
-from splinter.browser import Browser
+from splinter import Browser
 
 from omegaml import settings
 from omegaml.tests.features.util import istrue
 from omegaml.tests.util import clear_om
 
 
 @fixture
 def splinter_browser(context):
     headless = istrue(os.environ.get('CHROME_HEADLESS'))
     screenshot_path = os.environ.get('CHROME_SCREENSHOTS', '/tmp/screenshots')
+    selenium_address = os.environ.get('SELENIUM_ADDRESS')
     os.makedirs(screenshot_path, exist_ok=True)
     options = None
-    if headless:
-        print("Running headless, debug at http://localhost:9222")
-        options = ChromeOptions()
-        options.add_argument('--no-sandbox')
-        options.add_argument('--headless')
-        options.add_argument('--disable-gpu')
-        options.add_argument('--remote-debugging-port=9222')
-        options.add_argument('--remote-debugging-address=0.0.0.0')
-        options.add_argument('--disable-dev-shm-usage')
-        options.add_argument('--disable-extensions')
-    context.browser = Browser('chrome', options=options)
-    context.browser.driver.set_window_size(1024, 768)
+    if selenium_address:
+        # start remote browser using selenium grid
+        caps = {
+            'browserName': 'chrome',
+            'screen_resolution': '1024x768',
+        }
+        context.browser = Browser('remote',
+                                  command_executor=selenium_address,
+                                  desired_capabilities=caps)
+    else:
+        # start local browser
+        if headless:
+            print("Running headless, debug at chrome://inspect/#devices")
+            options = ChromeOptions()
+            options.add_argument('--no-sandbox')
+            options.add_argument('--headless')
+            options.add_argument('--disable-gpu')
+            options.add_argument('--remote-debugging-port=4444')
+            options.add_argument('--remote-debugging-address=localhost')
+            options.add_argument('--disable-dev-shm-usage')
+            options.add_argument('--disable-extensions')
+        context.browser = Browser('chrome', options=options)
+        context.browser.driver.set_window_size(1024, 768)
     context.screenshot_path = screenshot_path
     yield context.browser
     context.browser.quit()
 
 
 def before_all(context):
     # setup omegaml
```

### Comparing `omegaml-0.15.3/omegaml/tests/features/steps/notebook.py` & `omegaml-0.15.5/omegaml/tests/features/steps/notebook.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/features/steps/tftutorial.py` & `omegaml-0.15.5/omegaml/tests/features/steps/tftutorial.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/features/steps/tutorial.py` & `omegaml-0.15.5/omegaml/tests/features/steps/tutorial.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/features/tutorial.feature` & `omegaml-0.15.5/omegaml/tests/features/tutorial.feature`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/features/util.py` & `omegaml-0.15.5/omegaml/tests/features/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             if login_required:
                 self.login_nb()
 
     def login_hub(self):
         br = self.browser
         br.find_by_id('username_input').first.fill(self.user)
         br.find_by_id('password_input').first.fill(self.password)
-        br.click_link_by_id('login_submit')
+        br.find_by_id('login_submit').click()
         br.visit(jburl(br.url, self.user, nbstyle='tree'))
         assert br.is_element_present_by_id('ipython-main-app', wait_time=60)
         # check that there is actually a connection
         assert not br.is_text_present('Server error: Traceback', wait_time=15)
         assert not br.is_text_present('Connection refuse', wait_time=15)
 
     def login_nb(self):
```

### Comparing `omegaml-0.15.3/omegaml/tests/mlflow/test_mlflow_models.py` & `omegaml-0.15.5/omegaml/tests/mlflow/test_mlflow_models.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/mlflow/test_mlflow_projects.py` & `omegaml-0.15.5/omegaml/tests/mlflow/test_mlflow_projects.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/rsystem/rtestutil.py` & `omegaml-0.15.5/omegaml/tests/rsystem/rtestutil.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/rsystem/test_rmodels.py` & `omegaml-0.15.5/omegaml/tests/rsystem/test_rmodels.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/rsystem/test_rscripts.py` & `omegaml-0.15.5/omegaml/tests/rsystem/test_rscripts.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/streams/test_minibatch.py` & `omegaml-0.15.5/omegaml/tests/streams/test_minibatch.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/streams/test_streams.py` & `omegaml-0.15.5/omegaml/tests/streams/test_streams.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/tensorflow/test_kerasmodel.py` & `omegaml-0.15.5/omegaml/tests/tensorflow/test_kerasmodel.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/tensorflow/test_protobuf.py` & `omegaml-0.15.5/omegaml/tests/tensorflow/test_protobuf.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/tensorflow/test_tfdataset.py` & `omegaml-0.15.5/omegaml/tests/tensorflow/test_tfdataset.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/tensorflow/test_tfestimator.py` & `omegaml-0.15.5/omegaml/tests/tensorflow/test_tfestimator.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/tensorflow/test_tfkerasmodel.py` & `omegaml-0.15.5/omegaml/tests/tensorflow/test_tfkerasmodel.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/tensorflow/test_tfsavedmodel.py` & `omegaml-0.15.5/omegaml/tests/tensorflow/test_tfsavedmodel.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/tensorflow/test_tftracking.py` & `omegaml-0.15.5/omegaml/tests/tensorflow/test_tftracking.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/tests/util.py` & `omegaml-0.15.5/omegaml/tests/util.py`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/omegaml/util.py` & `omegaml-0.15.5/omegaml/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -427,15 +427,15 @@
     should_create = not index_exists
     if should_drop or should_create:
         idx_specs, idx_kwargs = ensure_index_limit(idx_specs_SON, **kwargs)
     if should_drop:
         coll.drop_index(idx_specs, **idx_kwargs)
         should_create = True
     if should_create:
-        coll.create_index(idx_specs, **kwargs)
+        coll.create_index(idx_specs, **idx_kwargs)
         created = True
     return created
 
 
 def reshaped(data):
     """
     check if data is 1d and if so reshape to a column vector
@@ -1084,7 +1084,39 @@
     """
 
     def __str__(self):
         # on windows, return a posix path
         # on posix systems, this is a noop
         path = super().__str__()
         return path if os.name != 'nt' else path.replace('\\', '/')
+
+
+class ProcessLocal(dict):
+    def __init__(self, *args, **kwargs):
+        self._pid = os.getpid()
+        super().__init__(*args, **kwargs)
+
+    def _check_pid(self):
+        if self._pid != os.getpid():
+            self.clear()
+            self._pid = os.getpid()
+
+    def __getitem__(self, k):
+        self._check_pid()
+        return super().__getitem__(k)
+
+    def keys(self):
+        self._check_pid()
+        return super().keys()
+
+    def __contains__(self, item):
+        self._check_pid()
+        return super().__contains__(item)
+
+
+class KeepMissing(dict):
+    # a missing '{key}' is replaced by '{key}'
+    # in order to avoid raising KeyError
+    # see str.format_map
+    def __missing__(self, key):
+        return '{' + key + '}'
+
```

### Comparing `omegaml-0.15.3/omegaml.egg-info/PKG-INFO` & `omegaml-0.15.5/omegaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegaml
-Version: 0.15.3
+Version: 0.15.5
 Summary: An open source DataOps, MLOps platform for humans
 Home-page: https://omegaml.io/
 Author: Patrick Senti
 Author-email: patrick.senti@omegaml.io
 License: Apache 2.0 + "No Sell, Consulting Yes" License Condition
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `omegaml-0.15.3/omegaml.egg-info/SOURCES.txt` & `omegaml-0.15.5/omegaml.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -222,16 +222,18 @@
 omegaml/mixins/store/__init__.py
 omegaml/mixins/store/datarevision.py
 omegaml/mixins/store/extdmeta.py
 omegaml/mixins/store/imexport.py
 omegaml/mixins/store/lazyget.py
 omegaml/mixins/store/modelversion.py
 omegaml/mixins/store/package.py
+omegaml/mixins/store/passthrough.py
 omegaml/mixins/store/projected.py
 omegaml/mixins/store/promotion.py
+omegaml/mixins/store/requests.py
 omegaml/mixins/store/virtualobj.py
 omegaml/notebook/__init__.py
 omegaml/notebook/checkpoints.py
 omegaml/notebook/jobs.py
 omegaml/notebook/jobschedule.py
 omegaml/notebook/omegacontentsmgr.py
 omegaml/notebook/tasks.py
@@ -301,14 +303,15 @@
 omegaml/tests/core/test_mdfparallel.py
 omegaml/tests/core/test_misc.py
 omegaml/tests/core/test_modelversions.py
 omegaml/tests/core/test_nbtasks.py
 omegaml/tests/core/test_npndarray.py
 omegaml/tests/core/test_package.py
 omegaml/tests/core/test_package_remote.py
+omegaml/tests/core/test_passthrough.py
 omegaml/tests/core/test_promotion.py
 omegaml/tests/core/test_query.py
 omegaml/tests/core/test_restauth.py
 omegaml/tests/core/test_runtime.py
 omegaml/tests/core/test_sklext.py
 omegaml/tests/core/test_sqlalchemy.py
 omegaml/tests/core/test_store.py
```

### Comparing `omegaml-0.15.3/omegaml.egg-info/requires.txt` & `omegaml-0.15.5/omegaml.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-celery<5.0,>4.4
+celery<6.0,>5
 importlib-metadata<5.0
 joblib>=0.9.4
 jupyter-client>=4.1.1
 mongoengine~=0.24.1
 pymongo~=4.0.2
-pandas>1.1
+pandas<2,>1.1
 numpy>=1.16.4
 scipy>=0.17.0
 scikit-learn>=0.21
 PyYAML>=3.12
 flask-restx>=0.4.0
 werkzeug<2.1.0
 markupsafe==2.0.1
 croniter>=0.3.30
 nbformat>=4.0.1
 nbconvert>=6.4.0
+pygments>=2.7.4
 dill<0.3.6,>=0.3.2
 callable-pip>=1.0.0
 appdirs>=1.4.3
 cron-descriptor>=1.2.31
 docopt>=0.6.2
 requests>=2.20.0
 absl-py>=0.8.1
@@ -35,40 +36,44 @@
 [all]
 tables>=3.7
 matplotlib~=3.5
 seaborn~=0.11
 imageio~=2.6
 plotext~=1.0
 dashserve
+dash<2.9
 sqlalchemy
 ipython-sql
 boto>=2.49.0
 minibatch[all]>=0.5.0
 jupyterlab
 jupyterhub==2.2.1
-snowflake-sqlalchemy==1.2.3
+snowflake-sqlalchemy>1.2.3
 
 [all-client]
 tables>=3.7
 dashserve
+dash<2.9
 sqlalchemy
 ipython-sql
 boto>=2.49.0
 minibatch[all]>=0.5.0
 
 [client]
 tables>=3.7
 dashserve
+dash<2.9
 sqlalchemy
 ipython-sql
 boto>=2.49.0
 minibatch[all]>=0.5.0
 
 [dashserve]
 dashserve
+dash<2.9
 
 [dev]
 pytest
 twine
 flake8
 mock
 behave
@@ -92,15 +97,15 @@
 [keras]
 keras~=2.4.3
 
 [mlflow]
 mlflow~=1.21
 
 [snowflake]
-snowflake-sqlalchemy==1.2.3
+snowflake-sqlalchemy>1.2.3
 
 [sql]
 sqlalchemy
 ipython-sql
 
 [streaming]
 minibatch[all]>=0.5.0
```

### Comparing `omegaml-0.15.3/scripts/runtime/easyoptions` & `omegaml-0.15.5/scripts/runtime/easyoptions`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/scripts/runtime/omegajobs.sh` & `omegaml-0.15.5/scripts/runtime/omegajobs.sh`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/scripts/runtime/setupnb.sh` & `omegaml-0.15.5/scripts/runtime/setupnb.sh`

 * *Files identical despite different names*

### Comparing `omegaml-0.15.3/setup.py` & `omegaml-0.15.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 README = open(os.path.join(os.path.dirname(__file__), 'README.rst')).read()
 version = open(os.path.join(os.path.dirname(__file__), 'omegaml', 'VERSION')).read()
 
 # extras
 tables = ['tables>=3.7']
 graph_deps = ['matplotlib~=3.5', 'seaborn~=0.11', 'imageio~=2.6', 'plotext~=1.0']
-dashserve_deps = ['dashserve']
+dashserve_deps = ['dashserve', 'dash<2.9'] # dash 2.9 breaks dashserve due to required pages folder
 sql_deps = ['sqlalchemy', 'ipython-sql']
-snowflake_deps = ['snowflake-sqlalchemy==1.2.3']
+snowflake_deps = ['snowflake-sqlalchemy>1.2.3']
 iotools_deps = ['boto>=2.49.0']
 streaming_deps = ['minibatch[all]>=0.5.0']
 jupyter_deps = ['jupyterlab', 'jupyterhub==2.2.1']
 mlflow_deps = ['mlflow~=1.21']
 dev_deps = ['pytest', 'twine', 'flake8', 'mock', 'behave', 'splinter[selenium3]', 'ipdb', 'bumpversion']
 
 # -- tensorflow specifics
@@ -24,15 +24,15 @@
 tf_version = os.environ.get('TF_VERSION') or '2.3.1'
 tf_match = os.environ.get('TF_VERSION_MATCH', '==')
 if tf_version.startswith('1.15'):
     assert sys.version_info[:2] <= (3, 7), "TF < 2.x requires Python <= 3.7"
     tf_deps = ['tensorflow=={}'.format(tf_version)]
     tf_deps = tf_deps + ['tensorflow-gpu==1.15.0', 'h5py==2.10.0']
     keras_deps = ['keras==2.2.4']
-elif (3, 8) <= sys.version_info[:2] < (3, 9) :
+elif (3, 8) <= sys.version_info[:2] < (3, 9):
     major, minor, *_ = (int(v) for v in tf_version.split('.'))
     assert (major, minor) >= (2, 2), "Python version 3.8 only supported by TF >= 2.2"
     tf_deps = ['tensorflow{}{}'.format(tf_match, tf_version)]
     keras_deps = ['keras~=2.4.3']
 elif sys.version_info[:2] >= (3, 9):
     major, minor, *_ = (int(v) for v in tf_version.split('.'))
     tf_issue = "https://github.com/tensorflow/tensorflow/issues/44485"
@@ -75,49 +75,50 @@
         'Development Status :: 4 - Beta',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Software Development',
         'Operating System :: POSIX :: Linux',
         'License :: OSI Approved :: Apache Software License',
     ],
     install_requires=[
-        'celery>4.4,<5.0',
-        'importlib-metadata<5.0', # due to https://github.com/celery/kombu/pull/1601
+        'celery>5,<6.0',
+        'importlib-metadata<5.0',  # due to https://github.com/celery/kombu/pull/1601
         'joblib>=0.9.4',
         'jupyter-client>=4.1.1',
         'mongoengine~=0.24.1',
         'pymongo~=4.0.2',  # mongoengine 0.24.1 compatibility
-        'pandas>1.1',
+        'pandas>1.1,<2', # pandas 2.0 breaks some tests
         'numpy>=1.16.4',
         'scipy>=0.17.0',
         'scikit-learn>=0.21',
         'PyYAML>=3.12',
         'flask-restx>=0.4.0',
-        'werkzeug<2.1.0', # due to flask-restx, https://github.com/python-restx/flask-restx/issues/422
-        'markupsafe==2.0.1', # due to flask/markupsafe, https://github.com/pallets/markupsafe/issues/284
+        'werkzeug<2.1.0',  # due to flask-restx, https://github.com/python-restx/flask-restx/issues/422
+        'markupsafe==2.0.1',  # due to flask/markupsafe, https://github.com/pallets/markupsafe/issues/284
         'croniter>=0.3.30',
         'nbformat>=4.0.1',
         'nbconvert>=6.4.0',
-        'dill>=0.3.2,<0.3.6', # due to dill, https://github.com/uqfoundation/dill/issues/332
+        'pygments>=2.7.4',  # via nbconvert, due to snyk report https://github.com/omegaml/omegaml/pull/299
+        'dill>=0.3.2,<0.3.6',  # due to dill, https://github.com/uqfoundation/dill/issues/332
         'callable-pip>=1.0.0',
         'appdirs>=1.4.3',
         'cron-descriptor>=1.2.31',
         'docopt>=0.6.2',
         'requests>=2.20.0',
         # fix tensorflow pulling wrong version of absl-py,
         # https://github.com/tensorflow/tensorflow/issues/26691#issuecomment-525519742
         'absl-py>=0.8.1',
         'tqdm>=4.32.2',
         'honcho>=1.0.1',  # not strictly required, but used in docker compose
         'tabulate>=0.8.2',  # required in cli
-        'smart_open', # required in cli
-        'imageio>=2.3.0', # require to store images
-        'psutil>=5.8', # required for profiling tracker
-        'cachetools>=5.0.0', # required for session caching
-        'apispec>=5.2.2', # required for openapi generation
-        'marshmallow>=3.17.0', # required for openapi generation
+        'smart_open',  # required in cli
+        'imageio>=2.3.0',  # require to store images
+        'psutil>=5.8',  # required for profiling tracker
+        'cachetools>=5.0.0',  # required for session caching
+        'apispec>=5.2.2',  # required for openapi generation
+        'marshmallow>=3.17.0',  # required for openapi generation
     ],
     extras_require={
         'graph': graph_deps,
         'tables': tables,
         'tensorflow': tf_deps,
         'keras': keras_deps,
         'jupyter': jupyter_deps,
@@ -132,8 +133,7 @@
         'all-client': client_deps,
         'dev': dev_deps,
     },
     entry_points={
         'console_scripts': ['om=omegaml.client.cli:climain'],
     }
 )
-
```

