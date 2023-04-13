# Comparing `tmp/dpdispatcher-0.5.5.tar.gz` & `tmp/dpdispatcher-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpdispatcher-0.5.5.tar", last modified: Fri Mar 24 03:42:44 2023, max compression
+gzip compressed data, was "dpdispatcher-0.5.6.tar", last modified: Thu Apr 13 04:21:20 2023, max compression
```

## Comparing `dpdispatcher-0.5.5.tar` & `dpdispatcher-0.5.6.tar`

### file list

```diff
@@ -1,297 +1,297 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.911996 dpdispatcher-0.5.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.835991 dpdispatcher-0.5.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.859992 dpdispatcher-0.5.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/.github/workflows/ci-docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/.github/workflows/machines.yml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/.github/workflows/mirror_gitee.yml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/.github/workflows/publish_conda.yml
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/.github/workflows/pyright.yml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-03-24 03:42:44.911996 dpdispatcher-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.863993 dpdispatcher-0.5.5/ci/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/ci/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/ci/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.863993 dpdispatcher-0.5.5/ci/pbs/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/ci/pbs/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/ci/pbs/start-pbs.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/ci/pbs.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.863993 dpdispatcher-0.5.5/ci/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/ci/slurm/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/ci/slurm/register_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/ci/slurm/start-slurm.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/ci/slurm.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.863993 dpdispatcher-0.5.5/ci/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/ci/ssh/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/ci/ssh/start-ssh.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      411 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/ci/ssh.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/ci/ssh_rsync.sh
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.867993 dpdispatcher-0.5.5/conda/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/conda/conda_build_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.871993 dpdispatcher-0.5.5/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/batch.md
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/context.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/credits.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/dpdispatcher_on_yarn.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.875994 dpdispatcher-0.5.5/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/examples/expanse.md
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/examples/g16.md
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/examples/shell.md
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/install.md
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/machine.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/resources.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/doc/task.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.883994 dpdispatcher-0.5.5/dpdispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/JobStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-24 03:42:44.000000 dpdispatcher-0.5.5/dpdispatcher/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/arginfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/base_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/distributed_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/dp_cloud_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/dp_cloud_server_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.883994 dpdispatcher-0.5.5/dpdispatcher/dpcloudserver/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/dpcloudserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/dpcloudserver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/dpcloudserver/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/dpcloudserver/retcode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/dpcloudserver/temp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/dpcloudserver/zip_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/dpdisp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/hdfs_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/hdfs_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/lazy_local_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/local_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    12935 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    34271 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/ssh_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    41870 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/dpdispatcher/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.883994 dpdispatcher-0.5.5/dpdispatcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-03-24 03:42:44.000000 dpdispatcher-0.5.5/dpdispatcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-03-24 03:42:44.000000 dpdispatcher-0.5.5/dpdispatcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 03:42:44.000000 dpdispatcher-0.5.5/dpdispatcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-24 03:42:44.000000 dpdispatcher-0.5.5/dpdispatcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-24 03:42:44.000000 dpdispatcher-0.5.5/dpdispatcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-24 03:42:44.000000 dpdispatcher-0.5.5/dpdispatcher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.839991 dpdispatcher-0.5.5/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.883994 dpdispatcher-0.5.5/examples/machine/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/examples/machine/expanse.json
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/examples/machine/lazy_local.json
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/examples/machine/mandu.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.883994 dpdispatcher-0.5.5/examples/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/examples/resources/expanse_cpu.json
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/examples/resources/mandu.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.887994 dpdispatcher-0.5.5/examples/task/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/examples/task/deepmd-kit.json
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/examples/task/g16.json
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.887994 dpdispatcher-0.5.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/scripts/script_gen_dargs_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/scripts/script_gen_dargs_json.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 03:42:44.911996 dpdispatcher-0.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.891995 dpdispatcher-0.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/batch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/context.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1843 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/debug_test_class_submission_init.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3256 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/devel_test_ali_ehpc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/devel_test_dp_cloud_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/devel_test_lazy_ali_ehpc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1408 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/devel_test_lsf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2460 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/devel_test_shell.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2744 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/devel_test_slurm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2639 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/devel_test_ssh_ali_ehpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.895995 dpdispatcher-0.5.5/tests/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/job.json
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/machine.json
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/machine_ali_ehpc.json
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/machine_center.json
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/machine_diffenert.json
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/machine_dp_cloud_server.json
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/machine_if_cuda_multi_devices.json
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/machine_lazy_local_lsf.json
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/machine_lazy_local_slurm.json
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/machine_lazylocal_shell.json
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/machine_local_shell.json
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/machine_lsf.json
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/machine_slurm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/machine_yarn.json
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/resources.json
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/submission.json
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/jsons/task.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.895995 dpdispatcher-0.5.5/tests/lsf/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/lsf/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/lsf/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/lsf/test_lsf_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.895995 dpdispatcher-0.5.5/tests/old/
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/old/test_dispatcher_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/old/test_lazy_local_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/old/test_local_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/old/test_local_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/old/test_ssh_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.899995 dpdispatcher-0.5.5/tests/pbs/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/pbs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/pbs/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/pbs/test_pbs_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/sample_class.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/script_gen_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.899995 dpdispatcher-0.5.5/tests/shell/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/shell/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/shell/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/shell/test_shell_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/shell/test_shell_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.899995 dpdispatcher-0.5.5/tests/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/slurm/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/slurm/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/slurm/test_dispatcher_lazy_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/slurm/test_slurm_lazy_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/slurm/test_slurm_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/slurm/test_slurm_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/slurm_test.env
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_argcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_class_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_class_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_class_machine_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_class_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_class_submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_class_submission_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_class_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.843991 dpdispatcher-0.5.5/tests/test_context_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.899995 dpdispatcher-0.5.5/tests/test_context_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.899995 dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.899995 dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-1/some_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-1/some_dir/some_file
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.899995 dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.899995 dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.899995 dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-4/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.899995 dpdispatcher-0.5.5/tests/test_context_dir/0_md/dir with space/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_context_dir/0_md/dir with space/file with space
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_context_dir/0_md/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.903996 dpdispatcher-0.5.5/tests/test_context_dir/0_md/some_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_context_dir/0_md/some_dir/some_file
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_group_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_hdfs_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.843991 dpdispatcher-0.5.5/tests/test_hdfs_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.903996 dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.903996 dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.903996 dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.903996 dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.903996 dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.847992 dpdispatcher-0.5.5/tests/test_if_cuda_multi_devices/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.903996 dpdispatcher-0.5.5/tests/test_if_cuda_multi_devices/test_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_if_cuda_multi_devices/test_dir/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_import_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_lazy_local_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_local_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.847992 dpdispatcher-0.5.5/tests/test_lsf_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.903996 dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.903996 dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.903996 dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.903996 dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.903996 dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/graph.pb
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/submission.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     4112 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_lsf_script_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.847992 dpdispatcher-0.5.5/tests/test_pbs_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.907996 dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.907996 dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.907996 dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.907996 dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.907996 dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/graph.pb
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_run_submission.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1925 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_shell_cuda_multi_devices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4921 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_shell_trival.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.851992 dpdispatcher-0.5.5/tests/test_shell_trival_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.907996 dpdispatcher-0.5.5/tests/test_shell_trival_dir/fail_dir/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_shell_trival_dir/fail_dir/mock_fail_task.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.907996 dpdispatcher-0.5.5/tests/test_shell_trival_dir/parent_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.907996 dpdispatcher-0.5.5/tests/test_shell_trival_dir/parent_dir/dir with space/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_shell_trival_dir/parent_dir/dir with space/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.907996 dpdispatcher-0.5.5/tests/test_shell_trival_dir/parent_dir/dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_shell_trival_dir/parent_dir/dir1/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.907996 dpdispatcher-0.5.5/tests/test_shell_trival_dir/parent_dir/dir2/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_shell_trival_dir/parent_dir/dir2/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.907996 dpdispatcher-0.5.5/tests/test_shell_trival_dir/parent_dir/dir3/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_shell_trival_dir/parent_dir/dir3/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.907996 dpdispatcher-0.5.5/tests/test_shell_trival_dir/parent_dir/dir4/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_shell_trival_dir/parent_dir/dir4/example.txt
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_shell_trival_dir/parent_dir/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.907996 dpdispatcher-0.5.5/tests/test_shell_trival_dir/recover_dir/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_shell_trival_dir/recover_dir/mock_recover_task.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.851992 dpdispatcher-0.5.5/tests/test_slurm_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.907996 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.907996 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.911996 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.911996 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.911996 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/graph.pb
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/submission.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     2393 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_slurm_script_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_ssh_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:44.911996 dpdispatcher-0.5.5/tests/test_work_path/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 03:42:34.000000 dpdispatcher-0.5.5/tests/test_work_path/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.671903 dpdispatcher-0.5.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.679903 dpdispatcher-0.5.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/.github/workflows/ci-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/.github/workflows/machines.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/.github/workflows/mirror_gitee.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/.github/workflows/publish_conda.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/.github/workflows/pyright.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.679903 dpdispatcher-0.5.6/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/ci/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/ci/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.679903 dpdispatcher-0.5.6/ci/pbs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/ci/pbs/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/ci/pbs/start-pbs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/ci/pbs.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.679903 dpdispatcher-0.5.6/ci/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/ci/slurm/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/ci/slurm/register_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/ci/slurm/start-slurm.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/ci/slurm.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.679903 dpdispatcher-0.5.6/ci/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/ci/ssh/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/ci/ssh/start-ssh.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      411 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/ci/ssh.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/ci/ssh_rsync.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.679903 dpdispatcher-0.5.6/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/conda/conda_build_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.683903 dpdispatcher-0.5.6/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/batch.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/context.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/dpdispatcher_on_yarn.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.683903 dpdispatcher-0.5.6/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/examples/expanse.md
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/examples/g16.md
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/examples/shell.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/machine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/doc/task.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.683903 dpdispatcher-0.5.6/dpdispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/JobStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 04:21:20.000000 dpdispatcher-0.5.6/dpdispatcher/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/arginfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/base_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/distributed_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/dp_cloud_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/dp_cloud_server_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.687903 dpdispatcher-0.5.6/dpdispatcher/dpcloudserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/dpcloudserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/dpcloudserver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/dpcloudserver/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/dpcloudserver/retcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/dpcloudserver/temp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/dpcloudserver/zip_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/dpdisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/hdfs_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/hdfs_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/lazy_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/local_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14949 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/ssh_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41960 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/dpdispatcher/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.687903 dpdispatcher-0.5.6/dpdispatcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-04-13 04:21:20.000000 dpdispatcher-0.5.6/dpdispatcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-04-13 04:21:20.000000 dpdispatcher-0.5.6/dpdispatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 04:21:20.000000 dpdispatcher-0.5.6/dpdispatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 04:21:20.000000 dpdispatcher-0.5.6/dpdispatcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 04:21:20.000000 dpdispatcher-0.5.6/dpdispatcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 04:21:20.000000 dpdispatcher-0.5.6/dpdispatcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.671903 dpdispatcher-0.5.6/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.687903 dpdispatcher-0.5.6/examples/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/examples/machine/expanse.json
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/examples/machine/lazy_local.json
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/examples/machine/mandu.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.687903 dpdispatcher-0.5.6/examples/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/examples/resources/expanse_cpu.json
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/examples/resources/mandu.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.687903 dpdispatcher-0.5.6/examples/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/examples/task/deepmd-kit.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/examples/task/g16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.687903 dpdispatcher-0.5.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/scripts/script_gen_dargs_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/scripts/script_gen_dargs_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.691903 dpdispatcher-0.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1843 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/debug_test_class_submission_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3228 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/devel_test_ali_ehpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2669 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/devel_test_dp_cloud_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1752 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/devel_test_lazy_ali_ehpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/devel_test_lsf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2357 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/devel_test_shell.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2673 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/devel_test_slurm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2629 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/devel_test_ssh_ali_ehpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/graph.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.695903 dpdispatcher-0.5.6/tests/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/job.json
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/machine.json
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/machine_ali_ehpc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/machine_center.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/machine_diffenert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/machine_dp_cloud_server.json
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/machine_if_cuda_multi_devices.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/machine_lazy_local_lsf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/machine_lazy_local_slurm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/machine_lazylocal_shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/machine_local_shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/machine_lsf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/machine_slurm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/machine_yarn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/resources.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/submission.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/jsons/task.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.695903 dpdispatcher-0.5.6/tests/lsf/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/lsf/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/lsf/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/lsf/test_lsf_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.695903 dpdispatcher-0.5.6/tests/old/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/old/test_dispatcher_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/old/test_lazy_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/old/test_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/old/test_local_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/old/test_ssh_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.695903 dpdispatcher-0.5.6/tests/pbs/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/pbs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/pbs/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/pbs/test_pbs_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/sample_class.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1074 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/script_gen_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.695903 dpdispatcher-0.5.6/tests/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/shell/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/shell/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/shell/test_shell_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/shell/test_shell_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.695903 dpdispatcher-0.5.6/tests/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/slurm/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/slurm/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/slurm/test_dispatcher_lazy_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/slurm/test_slurm_lazy_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/slurm/test_slurm_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/slurm/test_slurm_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/slurm_test.env
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_argcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_class_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_class_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_class_machine_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_class_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_class_submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_class_submission_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_class_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.671903 dpdispatcher-0.5.6/tests/test_context_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.695903 dpdispatcher-0.5.6/tests/test_context_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.695903 dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.695903 dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-1/some_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-1/some_dir/some_file
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.695903 dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.695903 dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-4/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_context_dir/0_md/dir with space/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_context_dir/0_md/dir with space/file with space
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_context_dir/0_md/graph.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_context_dir/0_md/some_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_context_dir/0_md/some_dir/some_file
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_group_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_hdfs_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.675903 dpdispatcher-0.5.6/tests/test_hdfs_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/graph.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.675903 dpdispatcher-0.5.6/tests/test_if_cuda_multi_devices/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_if_cuda_multi_devices/test_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_if_cuda_multi_devices/test_dir/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_import_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_lazy_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_local_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.675903 dpdispatcher-0.5.6/tests/test_lsf_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/graph.pb
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/submission.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4068 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_lsf_script_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.675903 dpdispatcher-0.5.6/tests/test_pbs_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.699903 dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/graph.pb
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_run_submission.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1913 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_shell_cuda_multi_devices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4895 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_shell_trival.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.675903 dpdispatcher-0.5.6/tests/test_shell_trival_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/tests/test_shell_trival_dir/fail_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_shell_trival_dir/fail_dir/mock_fail_task.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/tests/test_shell_trival_dir/parent_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/tests/test_shell_trival_dir/parent_dir/dir with space/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_shell_trival_dir/parent_dir/dir with space/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/tests/test_shell_trival_dir/parent_dir/dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_shell_trival_dir/parent_dir/dir1/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/tests/test_shell_trival_dir/parent_dir/dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_shell_trival_dir/parent_dir/dir2/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/tests/test_shell_trival_dir/parent_dir/dir3/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_shell_trival_dir/parent_dir/dir3/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/tests/test_shell_trival_dir/parent_dir/dir4/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_shell_trival_dir/parent_dir/dir4/example.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_shell_trival_dir/parent_dir/graph.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/tests/test_shell_trival_dir/recover_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_shell_trival_dir/recover_dir/mock_recover_task.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.675903 dpdispatcher-0.5.6/tests/test_slurm_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/graph.pb
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/submission.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2349 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_slurm_script_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_ssh_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:20.703903 dpdispatcher-0.5.6/tests/test_work_path/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 04:21:11.000000 dpdispatcher-0.5.6/tests/test_work_path/.gitkeep
```

### Comparing `dpdispatcher-0.5.5/.github/workflows/ci-docker.yml` & `dpdispatcher-0.5.6/.github/workflows/ci-docker.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/.github/workflows/test.yml` & `dpdispatcher-0.5.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/.pre-commit-config.yaml` & `dpdispatcher-0.5.6/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -13,22 +13,23 @@
     -   id: check-json
     -   id: check-added-large-files
     -   id: check-merge-conflict
     -   id: check-symlinks
     -   id: check-toml
 # Python
 -   repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
     -   id: black-jupyter
--   repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
+-   repo: https://github.com/charliermarsh/ruff-pre-commit
+    # Ruff version.
+    rev: v0.0.260
     hooks:
-    - id: isort
-    files: \.py$
+    - id: ruff
+      args: ["--fix"]
 # numpydoc
 -   repo: https://github.com/Carreau/velin
     rev: 0.0.12
     hooks:
     - id: velin
       args: ["--write"]
 # Python inside docs
```

### Comparing `dpdispatcher-0.5.5/CONTRIBUTING.md` & `dpdispatcher-0.5.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/LICENSE` & `dpdispatcher-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/PKG-INFO` & `dpdispatcher-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpdispatcher
-Version: 0.5.5
+Version: 0.5.6
 Summary: Generate HPC scheduler systems jobs input scripts, submit these scripts to HPC systems, and poke until they finish
 Author: DeepModeling
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `dpdispatcher-0.5.5/README.md` & `dpdispatcher-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/ci/LICENSE` & `dpdispatcher-0.5.6/ci/LICENSE`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/ci/pbs/docker-compose.yml` & `dpdispatcher-0.5.6/ci/pbs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/ci/pbs.sh` & `dpdispatcher-0.5.6/ci/pbs.sh`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/ci/slurm/docker-compose.yml` & `dpdispatcher-0.5.6/ci/slurm/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/ci/slurm/start-slurm.sh` & `dpdispatcher-0.5.6/ci/slurm/start-slurm.sh`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/ci/ssh/docker-compose.yml` & `dpdispatcher-0.5.6/ci/ssh/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/ci/ssh_rsync.sh` & `dpdispatcher-0.5.6/ci/ssh_rsync.sh`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/conda/meta.yaml` & `dpdispatcher-0.5.6/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/doc/.gitignore` & `dpdispatcher-0.5.6/doc/.gitignore`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/doc/Makefile` & `dpdispatcher-0.5.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/doc/batch.md` & `dpdispatcher-0.5.6/doc/batch.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/doc/conf.py` & `dpdispatcher-0.5.6/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
-import subprocess
 import sys
 from datetime import date
 
 # sys.path.insert(0, os.path.abspath('.'))
 
 
 # -- Project information -----------------------------------------------------
```

### Comparing `dpdispatcher-0.5.5/doc/context.md` & `dpdispatcher-0.5.6/doc/context.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/doc/dpdispatcher_on_yarn.md` & `dpdispatcher-0.5.6/doc/dpdispatcher_on_yarn.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/doc/examples/expanse.md` & `dpdispatcher-0.5.6/doc/examples/expanse.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/doc/examples/shell.md` & `dpdispatcher-0.5.6/doc/examples/shell.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/doc/getting-started.md` & `dpdispatcher-0.5.6/doc/getting-started.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/doc/index.rst` & `dpdispatcher-0.5.6/doc/index.rst`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/doc/make.bat` & `dpdispatcher-0.5.6/doc/make.bat`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/dpdispatcher/__init__.py` & `dpdispatcher-0.5.6/dpdispatcher/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 dlog.setLevel(logging.INFO)
 try:
     dlogf = logging.FileHandler(
         os.getcwd() + os.sep + "dpdispatcher" + ".log", delay=True
     )
 except PermissionError:
     warnings.warn(
-        f"dpdispatcher.log meet permission error. redirect the log to ~/dpdispatcher.log"
+        "dpdispatcher.log meet permission error. redirect the log to ~/dpdispatcher.log"
     )
     dlogf = logging.FileHandler(
         os.path.join(os.path.expanduser("~"), "dpdispatcher.log")
     )
 
 # dlogf = logging.FileHandler('./'+os.sep+SHORT_CMD+'.log')
 # dlogf = logging.FileHandler(os.path.join(os.environ['HOME'], SHORT_CMD+'.log'))
@@ -52,24 +52,46 @@
 from .shell import Shell
 from .slurm import Slurm
 from .ssh_context import SSHContext
 from .submission import Job, Resources, Submission, Task
 
 
 def info():
-    """
-    Show basic information about dpdispatcher, its location and version.
-    """
-
+    """Show basic information about dpdispatcher, its location and version."""
     print("DeepModeling\n------------")
     print("Version: " + __version__)
     print("Path:    " + ROOT_PATH)
     print("")
     print("Dependency")
     print("------------")
     for modui in ["psutil", "paramiko", "dargs", "oss2"]:
         try:
             mm = __import__(modui)
             print("%10s %10s   %s" % (modui, mm.__version__, mm.__path__[0]))
         except ImportError:
             print("%10s %10s Not Found" % (modui, ""))
     print()
+
+
+__all__ = [
+    "__version__",
+    "DistributedShell",
+    "DpCloudServer",
+    "DpCloudServerContext",
+    "HDFSContext",
+    "LazyLocalContext",
+    "LocalContext",
+    "LSF",
+    "Machine",
+    "PBS",
+    "Shell",
+    "Slurm",
+    "SSHContext",
+    "Submission",
+    "Task",
+    "Torque",
+    "info",
+    "Lebesgue",
+    "LebesgueContext",
+    "Job",
+    "Resources",
+]
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/base_context.py` & `dpdispatcher-0.5.6/dpdispatcher/base_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABCMeta, abstractmethod
-from typing import List, Optional, Tuple
+from typing import List, Tuple
 
 from dargs import Argument
 
 from dpdispatcher import dlog
 
 
 class BaseContext(metaclass=ABCMeta):
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/distributed_shell.py` & `dpdispatcher-0.5.6/dpdispatcher/distributed_shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import subprocess as sp
-
 from dpdispatcher import dlog
 from dpdispatcher.JobStatus import JobStatus
 from dpdispatcher.machine import Machine
 from dpdispatcher.utils import run_cmd_with_all_output
 
 shell_script_header_template = """
 #!/bin/bash -l
@@ -114,27 +112,26 @@
         return script_end
 
     def gen_script_header(self, job):
         shell_script_header = shell_script_header_template
         return shell_script_header
 
     def do_submit(self, job):
-        """submit th job to yarn using distributed shell
+        """Submit th job to yarn using distributed shell.
 
         Parameters
         ----------
         job : Job class instance
             job to be submitted
 
         Returns
         -------
         job_id: string
             submit process id
         """
-
         script_str = self.gen_script(job)
         script_file_name = job.script_file_name
         job_id_name = job.job_hash + "_job_id"
         output_name = job.job_hash + ".out"
         self.context.write_file(fname=script_file_name, write_str=script_str)
 
         resources = job.resources
@@ -157,15 +154,15 @@
                 resources.kwargs.get("img_name", ""),
                 resources.kwargs.get("mem_limit", 1) * 1024,
                 resources.cpu_per_node,
                 script_file_name,
             )
         )
 
-        cmd = "{ nohup %s 1>%s 2>%s & } && echo $!" % (
+        cmd = "{{ nohup {} 1>{} 2>{} & }} && echo $!".format(
             submit_command,
             output_name,
             output_name,
         )
         ret, stdout, stderr = run_cmd_with_all_output(cmd)
 
         if ret != 0:
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/dp_cloud_server.py` & `dpdispatcher-0.5.6/dpdispatcher/dp_cloud_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     def _gen_backward_files_list(self, job):
         result_file_list = []
         # result_file_list.extend(job.backward_common_files)
         for task in job.job_task_list:
             result_file_list.extend(
                 [os.path.join(task.task_work_path, b_f) for b_f in task.backward_files]
             )
+        result_file_list = list(set(result_file_list))
         return result_file_list
 
     def _gen_oss_path(self, job, zip_filename):
         if hasattr(job, "upload_path") and job.upload_path:
             return job.upload_path
         else:
             program_id = self.context.remote_profile.get("program_id")
@@ -103,15 +104,16 @@
         oss_task_zip = self._gen_oss_path(job, zip_filename)
         job_resources = ALI_OSS_BUCKET_URL + oss_task_zip
 
         input_data = self.input_data.copy()
 
         input_data["job_resources"] = job_resources
         input_data["command"] = f"bash {job.script_file_name}"
-        input_data["backward_files"] = self._gen_backward_files_list(job)
+        if not input_data.get("backward_files"):
+            input_data["backward_files"] = self._gen_backward_files_list(job)
         input_data["logFiles"] = os.path.join(
             job.job_task_list[0].task_work_path, job.job_task_list[0].outlog
         )
         program_id = self.context.remote_profile.get("program_id")
         program_id = self.context.remote_profile.get("project_id", program_id)
         if program_id is None:
             warnings.warn("program_id is compulsory.")
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/dp_cloud_server_context.py` & `dpdispatcher-0.5.6/dpdispatcher/dp_cloud_server_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 #!/usr/bin/env python
-# coding: utf-8
 # %%
 import os
 import shutil
-import time
 import uuid
 from typing import List
 
 import tqdm
 from dargs.dargs import Argument
 
 from dpdispatcher import dlog
 from dpdispatcher.base_context import BaseContext
 
 # from dpdispatcher.submission import Machine
 # from . import dlog
 from .dpcloudserver import Client, zip_file
 
 # from zip_file import zip_files
-from .dpcloudserver.config import ALI_OSS_BUCKET_URL
 
 DP_CLOUD_SERVER_HOME_DIR = os.path.join(
     os.path.expanduser("~"), ".dpdispatcher/", "dp_cloud_server/"
 )
 ENDPOINT = "http://oss-cn-shenzhen.aliyuncs.com"
 BUCKET_NAME = "dpcloudserver"
 
@@ -243,15 +240,15 @@
     def write_home_file(self, fname, write_str):
         # os.makedirs(self.remote_root, exist_ok = True)
         with open(os.path.join(DP_CLOUD_SERVER_HOME_DIR, fname), "w") as fp:
             fp.write(write_str)
         return True
 
     def read_home_file(self, fname):
-        with open(os.path.join(DP_CLOUD_SERVER_HOME_DIR, fname), "r") as fp:
+        with open(os.path.join(DP_CLOUD_SERVER_HOME_DIR, fname)) as fp:
             ret = fp.read()
         return ret
 
     def check_file_exists(self, fname):
         result = self.check_home_file_exits(fname)
         return result
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/dpcloudserver/client.py` & `dpdispatcher-0.5.6/dpdispatcher/dpcloudserver/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import os
 import re
 import time
 import urllib.parse
 from urllib.parse import urljoin
 
 import requests
@@ -281,15 +280,15 @@
         return None, 0
 
     def get_tasks_list(self, group_id, per_page=30):
         result = []
         page = 0
         while True:
             ret = self.get(
-                f"/brm/v1/job/list",
+                "/brm/v1/job/list",
                 params={
                     "groupId": group_id,
                     "page": page,
                     "pageSize": per_page,
                 },
             )
             if len(ret["items"]) == 0:
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/dpcloudserver/config.py` & `dpdispatcher-0.5.6/dpdispatcher/dpcloudserver/config.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/dpdispatcher/dpcloudserver/retcode.py` & `dpdispatcher-0.5.6/dpdispatcher/dpcloudserver/retcode.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/dpdispatcher/dpcloudserver/temp_test.py` & `dpdispatcher-0.5.6/dpdispatcher/dpcloudserver/temp_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,17 @@
     def setUp(self):
         print("execute", sys._getframe().f_code.co_name)
         api.login(self.username, self.password)
 
     def test_commit_job(self):
         print("----------", sys._getframe().f_code.co_name)
         file_uuid = uuid.uuid1().hex
-        oss_task_zip = os.path.join("%s/%s/%s.zip" % ("indicate", file_uuid, file_uuid))
+        oss_task_zip = os.path.join(
+            "{}/{}/{}.zip".format("indicate", file_uuid, file_uuid)
+        )
         zip_path = "/home/felix/workplace/22_dpdispatcher/dpdispatcher-yfb/dpdispatcher/dpcloudserver/t.txt"
         zip_task_file = zip_path + ".zip"
         zip_files(zip_path, zip_task_file, [])
         api.upload(oss_task_zip, zip_task_file, self.ENDPOINT, self.BUCKET_NAME)
         job_id = api.job_create(
             self.test_data["job_type"], self.test_data["job_resources"], self.test_data
         )
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/dpcloudserver/zip_file.py` & `dpdispatcher-0.5.6/dpdispatcher/dpcloudserver/zip_file.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/dpdispatcher/hdfs_cli.py` & `dpdispatcher-0.5.6/dpdispatcher/hdfs_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # /usr/bin/python
-# -*- encoding=utf-8 -*-
 
 import os
-import sys
 
 from dpdispatcher.utils import run_cmd_with_all_output
 
 
-class HDFS(object):
-    """Fundamental class for HDFS basic manipulation"""
+class HDFS:
+    """Fundamental class for HDFS basic manipulation."""
 
     @staticmethod
     def exists(uri):
         """Check existence of hdfs uri
         Returns: True on exists
-        Raises: RuntimeError
+        Raises: RuntimeError.
         """
-        cmd = "hadoop fs -test -e {uri}".format(uri=uri)
+        cmd = f"hadoop fs -test -e {uri}"
         try:
             ret, out, err = run_cmd_with_all_output(cmd)
             if ret == 0:
                 return True
             elif ret == 1:
                 return False
             else:
@@ -36,18 +34,17 @@
                 "with cmd[{}]".format(uri, cmd)
             ) from e
 
     @staticmethod
     def remove(uri):
         """Check existence of hdfs uri
         Returns: True on exists
-        Raises: RuntimeError
+        Raises: RuntimeError.
         """
-
-        cmd = "hadoop fs -rm -r {uri}".format(uri=uri)
+        cmd = f"hadoop fs -rm -r {uri}"
         try:
             ret, out, err = run_cmd_with_all_output(cmd)
             if ret == 0:
                 return True
             else:
                 raise RuntimeError(
                     "Cannot remove hdfs uri[{}] "
@@ -60,17 +57,17 @@
                 "Cannot remove hdfs uri[{}] " "with cmd[{}]".format(uri, cmd)
             ) from e
 
     @staticmethod
     def mkdir(uri):
         """Make new hdfs directory
         Returns: True on success
-        Raises: RuntimeError
+        Raises: RuntimeError.
         """
-        cmd = "hadoop fs -mkdir -p {uri}".format(uri=uri)
+        cmd = f"hadoop fs -mkdir -p {uri}"
         try:
             ret, out, err = run_cmd_with_all_output(cmd)
             if ret == 0:
                 return True
             else:
                 raise RuntimeError(
                     "Cannot mkdir of hdfs uri[{}] "
@@ -81,17 +78,16 @@
         except Exception as e:
             raise RuntimeError(
                 "Cannot mkdir of hdfs uri[{}] " "with cmd[{}]".format(uri, cmd)
             ) from e
 
     @staticmethod
     def copy_from_local(local_path, to_uri):
-        """
-        Returns: True on success
-        Raises: on unexpected error
+        """Returns: True on success
+        Raises: on unexpected error.
         """
         # Make sure local_path is accessible
         if not os.path.exists(local_path) or not os.access(local_path, os.R_OK):
             raise RuntimeError(
                 "try to access local_path[{}] " "but failed".format(local_path)
             )
         cmd = "hadoop fs -copyFromLocal -f {local} {remote}".format(
@@ -142,15 +138,15 @@
                 "Cannot copy remote[{}] to local[{}] with cmd[{}]".format(
                     from_uri, local_path, cmd
                 )
             ) from e
 
     @staticmethod
     def read_hdfs_file(uri):
-        cmd = "hadoop fs -text {uri}".format(uri=uri)
+        cmd = f"hadoop fs -text {uri}"
         try:
             ret, out, err = run_cmd_with_all_output(cmd)
             if ret == 0:
                 return out
             else:
                 raise RuntimeError(
                     "Cannot read text from uri[{}]"
@@ -161,15 +157,15 @@
         except Exception as e:
             raise RuntimeError(
                 "Cannot read text from uri[{}]" "cmd [{}]".format(uri, cmd)
             ) from e
 
     @staticmethod
     def move(from_uri, to_uri):
-        cmd = "hadoop fs -mv {furi} {turi}".format(furi=from_uri, turi=to_uri)
+        cmd = f"hadoop fs -mv {from_uri} {to_uri}"
         try:
             ret, out, err = run_cmd_with_all_output(cmd)
             if ret == 0:
                 return True
             else:
                 raise RuntimeError(
                     "Cannot move from_uri[{}] to "
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/hdfs_context.py` & `dpdispatcher-0.5.6/dpdispatcher/hdfs_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import hashlib
 import os
 import shutil
 import tarfile
 from glob import glob
 
 from dpdispatcher import dlog
 from dpdispatcher.base_context import BaseContext
@@ -65,26 +64,27 @@
         from_f = os.path.join(self.local_root, of)
         HDFS.copy_from_local(os.path.join(self.local_root, of), self.remote_root)
 
         # clean up
         os.remove(from_f)
 
     def upload(self, submission, dereference=True):
-        """upload forward files and forward command files to HDFS root dir
+        """Upload forward files and forward command files to HDFS root dir.
 
         Parameters
         ----------
         submission : Submission class instance
             represents a collection of tasks, such as forward file names
+        dereference : bool
+            whether to dereference symbolic links
 
         Returns
         -------
         none
         """
-
         file_list = []
 
         for task in submission.belonging_tasks:
             local_job = os.path.join(self.local_root, task.task_work_path)
             for ff in task.forward_files:
                 abs_file_list = glob(os.path.join(local_job, ff))
                 if not abs_file_list:
@@ -109,34 +109,39 @@
             file_list.extend(rel_file_list)
 
         self._put_files(file_list, dereference=dereference)
 
     def download(
         self, submission, check_exists=False, mark_failure=True, back_error=False
     ):
-        """download backward files from HDFS root dir
+        """Download backward files from HDFS root dir.
 
         Parameters
         ----------
         submission : Submission class instance
             represents a collection of tasks, such as backward file names
+        check_exists : bool
+            whether to check if the file exists
+        mark_failure : bool
+            whether to mark the task as failed if the file does not exist
+        back_error : bool
+            whether to download error files
 
         Returns
         -------
         none
         """
-
         cwd = os.getcwd()
 
         # download all hdfs files to tmp dir
         gz_dir = os.path.join(self.local_root, "tmp")
         if os.path.exists(gz_dir):
             shutil.rmtree(gz_dir, ignore_errors=True)
         os.mkdir(os.path.join(self.local_root, "tmp"))
-        rfile_tgz = "%s/%s_*_download.tar.gz" % (
+        rfile_tgz = "{}/{}_*_download.tar.gz".format(
             self.remote_root,
             submission.submission_hash,
         )
         lfile_tgz = "%s/tmp/" % (self.local_root)
         HDFS.copy_to_local(rfile_tgz, lfile_tgz)
 
         tgz_file_list = glob(os.path.join(self.local_root, "tmp/*_download.tar.gz"))
@@ -169,15 +174,15 @@
                                 pass
                         else:
                             raise RuntimeError("do not find download file " + rfile)
                     else:
                         raise RuntimeError("do not find download file " + rfile)
                 else:
                     if os.path.exists(lfile):
-                        dlog.info("find existing %s, replacing by %s" % (lfile, rfile))
+                        dlog.info(f"find existing {lfile}, replacing by {rfile}")
                         if os.path.isdir(lfile):
                             shutil.rmtree(lfile, ignore_errors=True)
                         elif os.path.isfile(lfile):
                             os.remove(lfile)
                     shutil.move(rfile, lfile)
 
         local_job = self.local_root
@@ -202,26 +207,26 @@
                             pass
                     else:
                         raise RuntimeError("do not find download file " + rfile)
                 else:
                     raise RuntimeError("do not find download file " + rfile)
             else:
                 if os.path.exists(lfile):
-                    dlog.info("find existing %s, replacing by %s" % (lfile, rfile))
+                    dlog.info(f"find existing {lfile}, replacing by {rfile}")
                     if os.path.isdir(lfile):
                         shutil.rmtree(lfile, ignore_errors=True)
                     elif os.path.isfile(lfile):
                         os.remove(lfile)
                 shutil.move(rfile, lfile)
 
         # remove tmp dir
         shutil.rmtree(gz_dir, ignore_errors=True)
 
     def check_file_exists(self, fname):
-        """check whether the given file exists, often used in checking whether the belonging job has finished
+        """Check whether the given file exists, often used in checking whether the belonging job has finished.
 
         Parameters
         ----------
         fname : string
             file name to be checked
 
         Returns
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/lazy_local_context.py` & `dpdispatcher-0.5.6/dpdispatcher/lazy_local_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import signal
 import subprocess as sp
 
 from dpdispatcher.base_context import BaseContext
 
 
-class SPRetObj(object):
+class SPRetObj:
     def __init__(self, ret):
         self.data = ret
 
     def read(self):
         return self.data
 
     def readlines(self):
@@ -17,27 +17,38 @@
         ret = []
         for aa in lines:
             ret.append(aa + "\n")
         return ret
 
 
 class LazyLocalContext(BaseContext):
+    """Run jobs in the local server and local directory.
+
+    Parameters
+    ----------
+    local_root : str
+        The local directory to store the jobs.
+    remote_root : str, optional
+        The argument takes no effect.
+    remote_profile : dict, optional
+        The remote profile. The default is {}.
+    *args
+        The arguments.
+    **kwargs
+        The keyword arguments.
+    """
+
     def __init__(
         self,
         local_root,
         remote_root=None,
         remote_profile={},
         *args,
         **kwargs,
     ):
-        """
-        local_root:
-        remote_root:
-        remote_profile:
-        """
         assert type(local_root) == str
         self.init_local_root = local_root
         self.init_remote_root = remote_root
         self.temp_local_root = os.path.abspath(local_root)
         self.temp_remote_root = os.path.abspath(local_root)
         self.remote_profile = remote_profile
         # self.job_uuid = None
@@ -134,15 +145,15 @@
 
     def write_file(self, fname, write_str):
         os.makedirs(self.remote_root, exist_ok=True)
         with open(os.path.join(self.remote_root, fname), "w") as fp:
             fp.write(write_str)
 
     def read_file(self, fname):
-        with open(os.path.join(self.remote_root, fname), "r") as fp:
+        with open(os.path.join(self.remote_root, fname)) as fp:
             ret = fp.read()
         return ret
 
     def check_file_exists(self, fname):
         # submission_work_base = os.path.join(self.local_root, self.submission.work_base)
         # file_to_be_checked = os.path.join(submission_work_base, fname)
         # print('debug:dpdispatcher.LazyLocalContext().check_file_exists:file_to_be_checked', file_to_be_checked)
@@ -156,15 +167,15 @@
         )
         return proc
 
     def kill(self, job_id):
         os.kill(job_id, signal.SIGTERM)
 
     def check_finish(self, proc):
-        return proc.poll() != None
+        return proc.poll() is not None
 
     def get_return(self, proc):
         ret = proc.poll()
         if ret is None:
             return None, None, None
         else:
             try:
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/local_context.py` & `dpdispatcher-0.5.6/dpdispatcher/local_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from glob import glob
 from subprocess import TimeoutExpired
 
 from dpdispatcher import dlog
 from dpdispatcher.base_context import BaseContext
 
 
-class SPRetObj(object):
+class SPRetObj:
     def __init__(self, ret):
         self.data = ret
 
     def read(self):
         return self.data
 
     def readlines(self):
@@ -36,27 +36,38 @@
         code0 = hashlib.sha1(fp.read().encode("utf-8")).hexdigest()
     with open(fname1) as fp:
         code1 = hashlib.sha1(fp.read().encode("utf-8")).hexdigest()
     return code0 == code1
 
 
 class LocalContext(BaseContext):
+    """Run jobs in the local server and remote directory.
+
+    Parameters
+    ----------
+    local_root : str
+        The local directory to store the jobs.
+    remote_root : str
+        The remote directory to store the jobs.
+    remote_profile : dict, optional
+        The remote profile. The default is {}.
+    *args
+        The arguments.
+    **kwargs
+        The keyword arguments.
+    """
+
     def __init__(
         self,
         local_root,
         remote_root,
         remote_profile={},
         *args,
         **kwargs,
     ):
-        """
-        local_root:
-        remote_root:
-        remote_profile:
-        """
         assert type(local_root) == str
         self.init_local_root = local_root
         self.init_remote_root = remote_root
         self.temp_local_root = os.path.abspath(local_root)
         self.temp_remote_root = os.path.abspath(remote_root)
         self.remote_profile = remote_profile
 
@@ -171,15 +182,15 @@
                         # for links, copy instead of moving (default behavior of copyfile is following symlinks)
                         if not os.path.islink(rfile):
                             shutil.move(rfile, lfile)
                         else:
                             shutil.copyfile(rfile, lfile)
                     elif (os.path.exists(rfile)) and (os.path.exists(lfile)):
                         # both exists, replace!
-                        dlog.info("find existing %s, replacing by %s" % (lfile, rfile))
+                        dlog.info(f"find existing {lfile}, replacing by {rfile}")
                         if os.path.isdir(lfile):
                             shutil.rmtree(lfile, ignore_errors=True)
                         elif os.path.isfile(lfile) or os.path.islink(lfile):
                             os.remove(lfile)
                         shutil.copyfile(rfile, lfile)
                     else:
                         raise RuntimeError("should not reach here!")
@@ -217,15 +228,15 @@
                     if not os.path.islink(rfile):
                         shutil.move(rfile, lfile)
                     else:
                         shutil.copyfile(rfile, lfile)
                 elif (os.path.exists(rfile)) and (os.path.exists(lfile)):
                     dlog.info(f"both exist rfile:{rfile}; lfile:{lfile}")
                     # both exists, replace!
-                    dlog.info("find existing %s, replacing by %s" % (lfile, rfile))
+                    dlog.info(f"find existing {lfile}, replacing by {rfile}")
                     if os.path.isdir(lfile):
                         shutil.rmtree(lfile, ignore_errors=True)
                     elif os.path.isfile(lfile) or os.path.islink(lfile):
                         os.remove(lfile)
                     shutil.copyfile(rfile, lfile)
                 else:
                     raise RuntimeError("should not reach here!")
@@ -263,15 +274,15 @@
 
     def write_file(self, fname, write_str):
         os.makedirs(self.remote_root, exist_ok=True)
         with open(os.path.join(self.remote_root, fname), "w") as fp:
             fp.write(write_str)
 
     def read_file(self, fname):
-        with open(os.path.join(self.remote_root, fname), "r") as fp:
+        with open(os.path.join(self.remote_root, fname)) as fp:
             ret = fp.read()
         return ret
 
     def check_file_exists(self, fname):
         return os.path.isfile(os.path.join(self.remote_root, fname))
 
     def call(self, cmd):
@@ -280,15 +291,15 @@
         )
         return proc
 
     def kill(self, job_id):
         os.kill(job_id, signal.SIGTERM)
 
     def check_finish(self, proc):
-        return proc.poll() != None
+        return proc.poll() is not None
 
     def get_return(self, proc):
         ret = proc.poll()
         if ret is None:
             return None, None, None
         else:
             try:
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/lsf.py` & `dpdispatcher-0.5.6/dpdispatcher/lsf.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,18 @@
 {lsf_nodes_line}
 {lsf_ptile_line}
 {lsf_partition_line}
 {lsf_number_gpu_line}"""
 
 
 class LSF(Machine):
-    """
-    LSF batch
-    """
+    """LSF batch."""
 
     def gen_script(self, job):
-        lsf_script = super(LSF, self).gen_script(job)
+        lsf_script = super().gen_script(job)
         return lsf_script
 
     def gen_script_header(self, job):
         resources = job.resources
         script_header_dict = {
             "lsf_nodes_line": "#BSUB -n {number_cores}".format(
                 number_cores=resources.number_node * resources.cpu_per_node
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/machine.py` & `dpdispatcher-0.5.6/dpdispatcher/machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import pathlib
 import shlex
 from abc import ABCMeta, abstractmethod
-from typing import List, Optional, Tuple
+from typing import List, Tuple
 
 from dargs import Argument, Variant
 
 from dpdispatcher import dlog
 from dpdispatcher.base_context import BaseContext
 
 script_template = """\
@@ -115,15 +115,15 @@
             cls.subclasses_dict[aa] = cls
             cls.subclasses_dict[aa.lower()] = cls
         cls.options.add(cls.__name__)
         # cls.subclasses.append(cls)
 
     @classmethod
     def load_from_json(cls, json_path):
-        with open(json_path, "r") as f:
+        with open(json_path) as f:
             machine_dict = json.load(f)
         machine = cls.load_from_dict(machine_dict=machine_dict)
         return machine
 
     @classmethod
     def load_from_dict(cls, machine_dict):
         batch_type = machine_dict["batch_type"]
@@ -182,17 +182,15 @@
     def sub_script_cmd(self, res):
         raise NotImplementedError(
             "abstract method sub_script_cmd should be implemented by derived class"
         )
 
     @abstractmethod
     def do_submit(self, job):
-        """
-        submit a single job, assuming that no job is running there.
-        """
+        """Submit a single job, assuming that no job is running there."""
         raise NotImplementedError(
             "abstract method do_submit should be implemented by derived class"
         )
 
     def gen_script(self, job):
         script_header = self.gen_script_header(job)
         script_custom_flags = self.gen_script_custom_flags_lines(job)
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/pbs.py` & `dpdispatcher-0.5.6/dpdispatcher/pbs.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 #PBS -j oe
 {queue_name_line}
 """
 
 
 class PBS(Machine):
     def gen_script(self, job):
-        pbs_script = super(PBS, self).gen_script(job)
+        pbs_script = super().gen_script(job)
         return pbs_script
 
     def gen_script_header(self, job):
         resources = job.resources
         pbs_script_header_dict = {}
         pbs_script_header_dict[
             "select_node_line"
         ] = "#PBS -l select={number_node}:ncpus={cpu_per_node}".format(
             number_node=resources.number_node, cpu_per_node=resources.cpu_per_node
         )
         if resources.gpu_per_node != 0:
             pbs_script_header_dict[
                 "select_node_line"
-            ] += ":ngpus={gpu_per_node}".format(gpu_per_node=resources.gpu_per_node)
+            ] += f":ngpus={resources.gpu_per_node}"
         pbs_script_header_dict["queue_name_line"] = "#PBS -q {queue_name}".format(
             queue_name=resources.queue_name
         )
         pbs_script_header = pbs_script_header_template.format(**pbs_script_header_dict)
         return pbs_script_header
 
     def do_submit(self, job):
@@ -60,18 +60,15 @@
     def check_status(self, job):
         job_id = job.job_id
         if job_id == "":
             return JobStatus.unsubmitted
         ret, stdin, stdout, stderr = self.context.block_call("qstat -x " + job_id)
         err_str = stderr.read().decode("utf-8")
         if ret != 0:
-            if (
-                str("qstat: Unknown Job Id") in err_str
-                or str("Job has finished") in err_str
-            ):
+            if "qstat: Unknown Job Id" in err_str or "Job has finished" in err_str:
                 if self.check_finish_tag(job=job):
                     return JobStatus.finished
                 else:
                     return JobStatus.terminated
             else:
                 raise RuntimeError(
                     "status command qstat fails to execute. erro info: %s return code %d"
@@ -102,18 +99,15 @@
     def check_status(self, job):
         job_id = job.job_id
         if job_id == "":
             return JobStatus.unsubmitted
         ret, stdin, stdout, stderr = self.context.block_call("qstat -l " + job_id)
         err_str = stderr.read().decode("utf-8")
         if ret != 0:
-            if (
-                str("qstat: Unknown Job Id") in err_str
-                or str("Job has finished") in err_str
-            ):
+            if "qstat: Unknown Job Id" in err_str or "Job has finished" in err_str:
                 if self.check_finish_tag(job=job):
                     return JobStatus.finished
                 else:
                     return JobStatus.terminated
             else:
                 raise RuntimeError(
                     "status command qstat fails to execute. erro info: %s return code %d"
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/shell.py` & `dpdispatcher-0.5.6/dpdispatcher/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 shell_script_header_template = """
 #!/bin/bash -l
 """
 
 
 class Shell(Machine):
     def gen_script(self, job):
-        shell_script = super(Shell, self).gen_script(job)
+        shell_script = super().gen_script(job)
         return shell_script
 
     def gen_script_header(self, job):
         shell_script_header = shell_script_header_template
         return shell_script_header
 
     def do_submit(self, job):
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/slurm.py` & `dpdispatcher-0.5.6/dpdispatcher/slurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 {slurm_ntasks_per_node_line}
 {slurm_number_gpu_line}
 {slurm_partition_line}"""
 
 
 class Slurm(Machine):
     def gen_script(self, job):
-        slurm_script = super(Slurm, self).gen_script(job)
+        slurm_script = super().gen_script(job)
         return slurm_script
 
     def gen_script_header(self, job):
         resources = job.resources
         script_header_dict = {}
         script_header_dict["slurm_nodes_line"] = "#SBATCH --nodes {number_node}".format(
             number_node=resources.number_node
@@ -43,15 +43,15 @@
             ] = "#SBATCH --gres=gpu:{gpu_per_node}".format(
                 gpu_per_node=resources.gpu_per_node
             )
         else:
             script_header_dict["slurm_number_gpu_line"] = custom_gpu_line
         script_header_dict[
             "slurm_partition_line"
-        ] = "#SBATCH --partition {queue_name}".format(queue_name=resources.queue_name)
+        ] = f"#SBATCH --partition {resources.queue_name}"
         slurm_script_header = slurm_script_header_template.format(**script_header_dict)
         return slurm_script_header
 
     @retry()
     def do_submit(self, job):
         script_file_name = job.script_file_name
         script_str = self.gen_script(job)
@@ -102,15 +102,15 @@
         if job_id == "":
             return JobStatus.unsubmitted
         ret, stdin, stdout, stderr = self.context.block_call(
             'squeue -o "%.18i %.2t" -j ' + job_id
         )
         if ret != 0:
             err_str = stderr.read().decode("utf-8")
-            if str("Invalid job id specified") in err_str:
+            if "Invalid job id specified" in err_str:
                 if self.check_finish_tag(job):
                     dlog.info(f"job: {job.job_hash} {job.job_id} finished")
                     return JobStatus.finished
                 else:
                     return JobStatus.terminated
             elif (
                 "Socket timed out on send/recv operation" in err_str
@@ -192,15 +192,15 @@
                 optional=True,
                 doc="Extra arguments.",
             )
         ]
 
 
 class SlurmJobArray(Slurm):
-    """Slurm with job array enabled for multiple tasks in a job"""
+    """Slurm with job array enabled for multiple tasks in a job."""
 
     def gen_script_header(self, job):
         if job.fail_count > 0:
             # resubmit jobs, check if some of tasks have been finished
             job_array = []
             for ii, task in enumerate(job.job_task_list):
                 task_tag_finished = (
@@ -261,15 +261,15 @@
         if job_id == "":
             return JobStatus.unsubmitted
         ret, stdin, stdout, stderr = self.context.block_call(
             'squeue -h -o "%.18i %.2t" -j ' + job_id
         )
         if ret != 0:
             err_str = stderr.read().decode("utf-8")
-            if str("Invalid job id specified") in err_str:
+            if "Invalid job id specified" in err_str:
                 if self.check_finish_tag(job):
                     dlog.info(f"job: {job.job_hash} {job.job_id} finished")
                     return JobStatus.finished
                 else:
                     return JobStatus.terminated
             elif (
                 "Socket timed out on send/recv operation" in err_str
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/ssh_context.py` & `dpdispatcher-0.5.6/dpdispatcher/ssh_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# coding: utf-8
 
 import os
 import pathlib
 import shlex
 import shutil
 import socket
 import tarfile
@@ -20,15 +19,15 @@
 from dpdispatcher import dlog
 from dpdispatcher.base_context import BaseContext
 
 # from dpdispatcher.submission import Machine
 from dpdispatcher.utils import RetrySignal, generate_totp, get_sha256, retry, rsync
 
 
-class SSHSession(object):
+class SSHSession:
     def __init__(
         self,
         hostname,
         username,
         password=None,
         port=22,
         key_filename=None,
@@ -217,16 +216,15 @@
         ts.open_session(timeout=self.timeout)
         ts.set_keepalive(60)
         self.ssh._transport = ts  # type: ignore
         # reset sftp
         self._sftp = None
 
     def inter_handler(self, title, instructions, prompt_list):
-        """
-        inter_handler: the callback for paramiko.transport.auth_interactive
+        """inter_handler: the callback for paramiko.transport.auth_interactive.
 
         The prototype for this function is defined by Paramiko, so all of the
         arguments need to be there, even though we don't use 'title' or
         'instructions'.
 
         The function is expected to return a tuple of data containing the
         responses to the provided prompts. Experimental results suggests that
@@ -237,15 +235,14 @@
         Since tuples can't really be built on the fly, the responses are
         collected in a list which is then converted to a tuple when it's time
         to return a value.
 
         Experiments suggest that the username prompt never happens. This makes
         sense, but the Username prompt is included here just in case.
         """
-
         resp = []  # Initialize the response container
 
         # Walk the list of prompts that the server sent that we need to answer
         for pr in prompt_list:
             # str() used to to make sure that we're dealing with a string rather than a unicode string
             # strip() used to get rid of any padding spaces sent by the server
             pr_str = str(pr[0]).strip().lower()
@@ -389,15 +386,15 @@
             and self.exec_command("rsync --version")[1].channel.recv_exit_status() == 0
             and self.totp_secret is None
             and self.passphrase is None
         )
 
     @property
     def remote(self) -> str:
-        return "%s@%s" % (self.username, self.hostname)
+        return f"{self.username}@{self.hostname}"
 
 
 class SSHContext(BaseContext):
     def __init__(
         self,
         local_root,
         remote_root,
@@ -406,15 +403,15 @@
         *args,
         **kwargs,
     ):
         assert type(local_root) == str
         self.init_local_root = local_root
         self.init_remote_root = remote_root
         self.temp_local_root = os.path.abspath(local_root)
-        assert os.path.isabs(remote_root), f"remote_root must be a abspath"
+        assert os.path.isabs(remote_root), "remote_root must be a abspath"
         self.temp_remote_root = remote_root
         self.remote_profile = remote_profile
         self.remote_root = None
 
         # self.job_uuid = None
         self.clean_asynchronously = clean_asynchronously
         # self.job_uuid = job_uuid
@@ -564,26 +561,29 @@
             if len(self.ssh_session.sftp.listdir(os.path.basename(self.remote_root))):
                 recover = True
         self.ssh_session.sftp.chdir(None)
 
         file_list = []
         directory_list = []
         for task in submission.belonging_tasks:
-            directory_list.append(task.task_work_path)
+            directory_list.append(os.path.join(self.local_root, task.task_work_path))
             #     file_list.append(ii)
             self._walk_directory(
                 task.forward_files,
                 os.path.join(self.local_root, task.task_work_path),
                 file_list,
                 directory_list,
             )
         self._walk_directory(
             submission.forward_common_files, self.local_root, file_list, directory_list
         )
 
+        # convert to relative path to local_root
+        directory_list = [os.path.relpath(jj, self.local_root) for jj in directory_list]
+
         # check if the same file exists on the remote file
         # only check sha256 when the job is recovered
         if recover:
             # generate local sha256 file
             sha256_list = []
             for jj in file_list:
                 sha256 = get_sha256(jj)
@@ -669,14 +669,18 @@
 
         Parameters
         ----------
         cmd : str
             The command to run.
         asynchronously : bool, optional, default=False
             Run command asynchronously. If True, `nohup` will be used to run the command.
+        stderr_whitelist : list of str, optional, default=None
+            If not None, the stderr will be checked against the whitelist. If the stderr
+            contains any of the strings in the whitelist, the command will be considered
+            successful.
         """
         assert self.remote_root is not None
         self.ssh_session.ensure_alive()
         if asynchronously:
             cmd = "nohup %s >/dev/null &" % cmd
         stdin, stdout, stderr = self.ssh_session.exec_command(
             ("cd %s ;" % shlex.quote(self.remote_root)) + cmd
@@ -713,15 +717,15 @@
         fname = pathlib.PurePath(os.path.join(self.remote_root, fname)).as_posix()
         # to prevent old file from being overwritten but cancelled, create a temporary file first
         # when it is fully written, rename it to the original file name
         with self.sftp.open(fname + "~", "w") as fp:
             fp.write(write_str)
         # sftp.rename may throw OSError
         self.block_checkcall(
-            "mv %s %s" % (shlex.quote(fname + "~"), shlex.quote(fname))
+            "mv {} {}".format(shlex.quote(fname + "~"), shlex.quote(fname))
         )
 
     def read_file(self, fname):
         assert self.remote_root is not None
         self.ssh_session.ensure_alive()
         with self.sftp.open(
             pathlib.PurePath(os.path.join(self.remote_root, fname)).as_posix(), "r"
@@ -733,15 +737,15 @@
         assert self.remote_root is not None
         self.ssh_session.ensure_alive()
         try:
             self.sftp.stat(
                 pathlib.PurePath(os.path.join(self.remote_root, fname)).as_posix()
             )
             ret = True
-        except IOError:
+        except OSError:
             ret = False
         return ret
 
     def call(self, cmd):
         stdin, stdout, stderr = self.ssh_session.exec_command(cmd)
         # stdin, stdout, stderr = self.ssh.exec_command('echo $$; exec ' + cmd)
         # pid = stdout.readline().strip()
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/submission.py` & `dpdispatcher-0.5.6/dpdispatcher/submission.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from dpdispatcher.machine import Machine
 
 # from dpdispatcher.slurm import SlurmResources
 # %%
 default_strategy = dict(if_cuda_multi_devices=False, ratio_unfinished=0.0)
 
 
-class Submission(object):
+class Submission:
     """A submission represents a collection of tasks.
     These tasks usually locate at a common directory.
     And these Tasks may share common files to be uploaded and downloaded.
 
     Parameters
     ----------
     work_base : Path
@@ -87,20 +87,22 @@
         )
 
     def __getitem__(self, key):
         return self.serialize()[key]
 
     @classmethod
     def deserialize(cls, submission_dict, machine=None):
-        """convert the submission_dict to a Submission class object
+        """Convert the submission_dict to a Submission class object.
 
         Parameters
         ----------
         submission_dict : dict
             path-like, the base directory of the local tasks
+        machine : Machine
+            Machine class Object to execute the jobs
 
         Returns
         -------
         submission : Submission
             the Submission class instance converted from the submission_dict
         """
         submission = cls(
@@ -120,15 +122,15 @@
             submission.bind_machine(machine=machine)
         else:
             machine = Machine.deserialize(machine_dict=submission_dict["machine"])
             submission.bind_machine(machine)
         return submission
 
     def serialize(self, if_static=False):
-        """convert the Submission class instance to a dictionary.
+        """Convert the Submission class instance to a dictionary.
 
         Parameters
         ----------
         if_static : bool
             whether dump the job runtime infomation (like job_id, job_state, fail_count) to the dictionary.
 
         Returns
@@ -176,15 +178,15 @@
 
     def get_hash(self):
         return sha1(
             json.dumps(self.serialize(if_static=True)).encode("utf-8")
         ).hexdigest()
 
     def bind_machine(self, machine):
-        """bind this submission to a machine. update the machine's context remote_root and local_root.
+        """Bind this submission to a machine. update the machine's context remote_root and local_root.
 
         Parameters
         ----------
         machine : Machine
             the machine to bind with
         """
         self.submission_hash = self.get_hash()
@@ -193,15 +195,15 @@
             job.machine = machine
         if machine is not None:
             self.machine.context.bind_submission(self)
             self.local_root = machine.context.temp_local_root
         return self
 
     def run_submission(self, *, dry_run=False, exit_on_submit=False, clean=True):
-        """main method to execute the submission.
+        """Main method to execute the submission.
         First, check whether old Submission exists on the remote machine, and try to recover from it.
         Second, upload the local files to the remote machine where the tasks to be executed.
         Third, run the submission defined previously.
         Forth, wait until the tasks in the submission finished and download the result file to local directory.
         If dry_run is True, submission will be uploaded but not be executed and exit.
         If exit_on_submit is True, submission will exit.
         """
@@ -254,15 +256,15 @@
         self.download_jobs()
         self.submission_to_json()
         if clean:
             self.clean_jobs()
         return self.serialize()
 
     def update_submission_state(self):
-        """check whether all the jobs in the submission.
+        """Check whether all the jobs in the submission.
 
         Notes
         -----
         this method will not handle unexpected (like resubmit terminated) job state in the submission.
         """
         for job in self.belonging_jobs:
             if job.job_state == JobStatus.finished:
@@ -271,15 +273,15 @@
             job.get_job_state()
             dlog.debug(
                 f"debug:update_submission_state: job: {job.job_hash}, {job.job_id}, {job.job_state}"
             )
         # self.submission_to_json()
 
     def handle_unexpected_submission_state(self):
-        """handle unexpected job state of the submission.
+        """Handle unexpected job state of the submission.
         If the job state is unsubmitted, submit the job.
         If the job state is terminated (killed unexpectly), resubmit the job.
         If the job state is unknown, raise an error.
         """
         try:
             for job in self.belonging_jobs:
                 job.handle_unexpected_job_state()
@@ -338,15 +340,15 @@
                     ignore_errors=True,
                 )
             self.belonging_tasks = [
                 task for task in self.belonging_tasks if task not in job.job_task_list
             ]
 
     def check_all_finished(self):
-        """check whether all the jobs in the submission.
+        """Check whether all the jobs in the submission.
 
         Notes
         -----
         This method will not handle unexpected job state in the submission.
         """
         # self.update_submission_state()
         if any(
@@ -433,15 +435,15 @@
         submission_file_name = "{submission_hash}.json".format(
             submission_hash=self.submission_hash
         )
         self.machine.context.write_file(submission_file_name, write_str=write_str)
 
     @classmethod
     def submission_from_json(cls, json_file_name="submission.json"):
-        with open(json_file_name, "r") as f:
+        with open(json_file_name) as f:
             submission_dict = json.load(f)
         # submission_dict = machine.context.read_file(json_file_name)
         submission = cls.deserialize(submission_dict=submission_dict, machine=None)
         return submission
 
     # def check_if_recover()
 
@@ -471,15 +473,15 @@
                 # self = submission.bind_machine(machine=self.machine)
             else:
                 print(self.serialize())
                 print(submission.serialize())
                 raise RuntimeError("Recover failed.")
 
 
-class Task(object):
+class Task:
     """A task is a sequential command to be executed,
     as well as the files it depends on to transmit forward and backward.
 
     Parameters
     ----------
     command : Str
         the command to be executed.
@@ -527,15 +529,15 @@
         return self.serialize()[key]
 
     def get_hash(self):
         return sha1(json.dumps(self.serialize()).encode("utf-8")).hexdigest()
 
     @classmethod
     def load_from_json(cls, json_file):
-        with open(json_file, "r") as f:
+        with open(json_file) as f:
             task_dict = json.load(f)
         return cls.load_from_dict(task_dict)
 
     @classmethod
     def load_from_dict(cls, task_dict: dict) -> "Task":
         # check dict
         base = cls.arginfo()
@@ -543,15 +545,15 @@
         base.check_value(task_dict, strict=False)
 
         task = cls.deserialize(task_dict=task_dict)
         return task
 
     @classmethod
     def deserialize(cls, task_dict):
-        """convert the task_dict to a Task class object
+        """Convert the task_dict to a Task class object.
 
         Parameters
         ----------
         task_dict : dict
             the dictionary which contains the task information
 
         Returns
@@ -606,15 +608,15 @@
                 "errlog", [None, str], optional=False, doc=doc_errlog, default="err"
             ),
         ]
         task_format = Argument("task", dict, task_args)
         return task_format
 
 
-class Job(object):
+class Job:
     """Job is generated by Submission automatically.
     A job ususally has many tasks and it may request computing resources from job scheduler systems.
     Each Job can generate a script file to be submitted to the job scheduler system or executed locally.
 
     Parameters
     ----------
     job_task_list : list of Task
@@ -655,20 +657,22 @@
         """
         return json.dumps(self.serialize(if_static=True)) == json.dumps(
             other.serialize(if_static=True)
         )
 
     @classmethod
     def deserialize(cls, job_dict, machine=None):
-        """convert the  job_dict to a Submission class object
+        """Convert the  job_dict to a Submission class object.
 
         Parameters
         ----------
-        submission_dict : dict
-            path-like, the base directory of the local tasks
+        job_dict : dict
+            the dictionary which contains the job information
+        machine : Machine
+            the machine object to execute the job
 
         Returns
         -------
         submission : Job
             the Job class instance converted from the job_dict
         """
         if len(job_dict.keys()) != 1:
@@ -695,15 +699,15 @@
         job.job_state = job_dict[job_hash]["job_state"]
         job.job_id = job_dict[job_hash]["job_id"]
         job.fail_count = job_dict[job_hash]["fail_count"]
         # job.job_uuid = job_dict[job_hash]['job_uuid']
         return job
 
     def get_job_state(self):
-        """get the jobs. Usually, this method will query the database of slurm or pbs job scheduler system and get the results.
+        """Get the jobs. Usually, this method will query the database of slurm or pbs job scheduler system and get the results.
 
         Notes
         -----
         this method will not submit or resubmit the jobs if the job is unsubmitted.
         """
         dlog.debug(
             f"debug:query database; self.job_hash:{self.job_hash}; self.job_id:{self.job_id}"
@@ -712,15 +716,15 @@
         job_state = self.machine.check_status(self)
         self.job_state = job_state
 
     def handle_unexpected_job_state(self):
         job_state = self.job_state
 
         if job_state == JobStatus.unknown:
-            raise RuntimeError("job_state for job {job} is unknown".format(job=self))
+            raise RuntimeError(f"job_state for job {self} is unknown")
 
         if job_state == JobStatus.terminated:
             self.fail_count += 1
             dlog.info(
                 f"job: {self.job_hash} {self.job_id} terminated;"
                 f"fail_cout is {self.fail_count}; resubmitting job"
             )
@@ -759,15 +763,15 @@
                 time.sleep(self.resources.wait_time)
             # self.get_job_state()
 
     def get_hash(self):
         return str(list(self.serialize(if_static=True).keys())[0])
 
     def serialize(self, if_static=False):
-        """convert the Task class instance to a dictionary.
+        """Convert the Task class instance to a dictionary.
 
         Parameters
         ----------
         if_static : bool
             whether dump the job runtime infomation (job_id, job_state, fail_count, job_uuid etc.) to the dictionary.
 
         Returns
@@ -806,15 +810,15 @@
         write_str = json.dumps(self.serialize(), indent=2, default=str)
         assert self.machine is not None
         self.machine.context.write_file(
             self.job_hash + "_job.json", write_str=write_str
         )
 
 
-class Resources(object):
+class Resources:
     """Resources is used to describe the machine resources we need to do calculations.
 
     Parameters
     ----------
     number_node : int
         The number of node need for each `job`.
     cpu_per_node : int
@@ -960,15 +964,15 @@
         return resources
 
     def __getitem__(self, key):
         return self.serialize()[key]
 
     @classmethod
     def load_from_json(cls, json_file):
-        with open(json_file, "r") as f:
+        with open(json_file) as f:
             resources_dict = json.load(f)
         resources = cls.deserialize(resources_dict=resources_dict)
         return resources
 
     @classmethod
     def load_from_dict(cls, resources_dict):
         # check dict
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher/utils.py` & `dpdispatcher-0.5.6/dpdispatcher/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import hashlib
 import hmac
 import struct
 import subprocess
 import time
-from typing import Callable, Iterable, Optional, Type, Union
+from typing import Callable, Optional, Type, Union
 
 from dpdispatcher import dlog
 
 
 def get_sha256(filename):
     """Get sha256 of a file.
 
@@ -129,15 +129,15 @@
         " ".join(ssh_cmd),
         "-q",
         from_file,
         to_file,
     ]
     ret, out, err = run_cmd_with_all_output(cmd, shell=False)
     if ret != 0:
-        raise RuntimeError("Failed to run %s: %s" % (cmd, err))
+        raise RuntimeError(f"Failed to run {cmd}: {err}")
 
 
 class RetrySignal(Exception):
     """Exception to give a signal to retry the function."""
 
 
 def retry(
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher.egg-info/PKG-INFO` & `dpdispatcher-0.5.6/dpdispatcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpdispatcher
-Version: 0.5.5
+Version: 0.5.6
 Summary: Generate HPC scheduler systems jobs input scripts, submit these scripts to HPC systems, and poke until they finish
 Author: DeepModeling
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `dpdispatcher-0.5.5/dpdispatcher.egg-info/SOURCES.txt` & `dpdispatcher-0.5.6/dpdispatcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/examples/resources/expanse_cpu.json` & `dpdispatcher-0.5.6/examples/resources/expanse_cpu.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/scripts/script_gen_dargs_docs.py` & `dpdispatcher-0.5.6/scripts/script_gen_dargs_docs.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/context.py` & `dpdispatcher-0.5.6/tests/context.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 import hashlib
 import os
 import pathlib
 import sys
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 # sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..')))
-import dpdispatcher
-from dpdispatcher.base_context import BaseContext
-from dpdispatcher.distributed_shell import DistributedShell
-from dpdispatcher.dp_cloud_server import Lebesgue
-from dpdispatcher.hdfs_cli import HDFS
-from dpdispatcher.hdfs_context import HDFSContext
+
+import dpdispatcher  # noqa: F401
+from dpdispatcher.base_context import BaseContext  # noqa: F401
+from dpdispatcher.distributed_shell import DistributedShell  # noqa: F401
+from dpdispatcher.dp_cloud_server import Lebesgue  # noqa: F401
+from dpdispatcher.hdfs_cli import HDFS  # noqa: F401
+from dpdispatcher.hdfs_context import HDFSContext  # noqa: F401
 
 # from dpgen.dispatcher.Dispatcher import FinRecord
-from dpdispatcher.JobStatus import JobStatus
+from dpdispatcher.JobStatus import JobStatus  # noqa: F401
 
 # from dpdispatcher.local_context import local_context
-from dpdispatcher.lazy_local_context import LazyLocalContext
+from dpdispatcher.lazy_local_context import LazyLocalContext  # noqa: F401
 
 # from dpdispatcher.local_context import LocalSession
-from dpdispatcher.local_context import LocalContext, _identical_files
-from dpdispatcher.lsf import LSF
-from dpdispatcher.pbs import PBS
-from dpdispatcher.shell import Shell
-from dpdispatcher.slurm import Slurm
-from dpdispatcher.ssh_context import SSHContext, SSHSession
+from dpdispatcher.local_context import LocalContext, _identical_files  # noqa: F401
+from dpdispatcher.lsf import LSF  # noqa: F401
+from dpdispatcher.pbs import PBS  # noqa: F401
+from dpdispatcher.shell import Shell  # noqa: F401
+from dpdispatcher.slurm import Slurm  # noqa: F401
+from dpdispatcher.ssh_context import SSHContext, SSHSession  # noqa: F401
 
 try:
-    from dpdispatcher.dp_cloud_server import DpCloudServer
-    from dpdispatcher.dp_cloud_server_context import DpCloudServerContext
+    from dpdispatcher.dp_cloud_server import DpCloudServer  # noqa: F401
+    from dpdispatcher.dp_cloud_server_context import DpCloudServerContext  # noqa: F401
 except Exception:
     pass
-import dargs
+import dargs  # noqa: F401
 
-from dpdispatcher.machine import Machine
-from dpdispatcher.submission import Job, Resources, Submission, Task
-from dpdispatcher.utils import RetrySignal, retry
+from dpdispatcher.machine import Machine  # noqa: F401
+from dpdispatcher.submission import Job, Resources, Submission, Task  # noqa: F401
+from dpdispatcher.utils import RetrySignal, retry  # noqa: F401
 
 
 def setUpModule():
     os.chdir(os.path.abspath(os.path.dirname(__file__)))
 
 
 def get_file_md5(file_path):
```

### Comparing `dpdispatcher-0.5.5/tests/debug_test_class_submission_init.py` & `dpdispatcher-0.5.6/tests/debug_test_class_submission_init.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/devel_test_ali_ehpc.py` & `dpdispatcher-0.5.6/tests/devel_test_ali_ehpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # from .context import Machine
 # from .context import Resources
 # from dpdispatcher.local_context import LocalSession
 # from dpdispatcher.local_context import LocalContext
 # from dpdispatcher.lazy_local_context import LazyLocalContext
 
 from dpdispatcher.machine import Machine
-from dpdispatcher.submission import Job, Resources, Submission, Task
+from dpdispatcher.submission import Resources
 from tests.sample_class import SampleClass
 
 # from dpdispatcher.pbs import PBS
 
 # local_session = LocalSession({'work_path':'test_work_path/'})
 # local_context = LocalContext(local_root='test_pbs_dir/', work_profile=local_session)
 
@@ -28,15 +28,15 @@
 # pbs = PBS(context=local_context)
 # pbs = PBS(context=lazy_local_context)
 
 submission = SampleClass.get_sample_submission()
 # pbs = SampleClass.get_sample_pbs_local_context()
 # slurm = SampleClass.get_sample_slurm_local_context()
 
-with open("jsons/machine_ali_ehpc.json", "r") as f:
+with open("jsons/machine_ali_ehpc.json") as f:
     compute_dict = json.load(f)
 
 machine = Machine.load_from_dict(compute_dict["machine"])
 resources = Resources.load_from_dict(compute_dict["resources"])
 
 submission.resouces = resources
 submission.bind_machine(machine=machine)
```

### Comparing `dpdispatcher-0.5.5/tests/devel_test_dp_cloud_server.py` & `dpdispatcher-0.5.6/tests/devel_test_dp_cloud_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import json
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
-from dpdispatcher.dp_cloud_server import DpCloudServer
-from dpdispatcher.dp_cloud_server_context import DpCloudServerContext
 
 # from dpdispatcher.batch_object import BatchObject
 from dpdispatcher.machine import Machine
-from dpdispatcher.submission import Job, Resources, Submission, Task
+from dpdispatcher.submission import Resources, Submission, Task
 
 # from dpdispatcher.slurm import SlurmResources, Slurm
 
 # local_session = LocalSession({'work_path':'temp2'})
 # local_context = LocalContext(local_root='test_slurm_dir/', work_profile=local_session)
 # lazy_local_context = LazyLocalContext(local_root='./')
 
@@ -32,15 +30,15 @@
 # dp_cloud_server_context = DpCloudServerContext(
 #     local_root='test_context_dir/',
 #     username='yfb222333',
 #     password='yfb222333')
 # dp_cloud_server = DpCloudServer(context=dp_cloud_server_context)
 # with open('test_dp_cloud_server.json', 'r') as f:
 #     jdata = json.load(f)
-with open("jsons/machine_dp_cloud_server.json", "r") as f:
+with open("jsons/machine_dp_cloud_server.json") as f:
     compute_dict = json.load(f)
 
 machine = Machine.load_from_dict(compute_dict["machine"])
 resources = Resources.load_from_dict(compute_dict["resources"])
 
 task1 = Task(
     command="lmp    -i input.lammps",
```

### Comparing `dpdispatcher-0.5.5/tests/devel_test_lazy_ali_ehpc.py` & `dpdispatcher-0.5.6/tests/devel_test_lazy_ali_ehpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
-from dpdispatcher.batch import Batch
 from dpdispatcher.lazy_local_context import LazyLocalContext
-from dpdispatcher.local_context import LocalContext, LocalSession
 from dpdispatcher.pbs import PBS
-from dpdispatcher.submission import Job, Resources, Submission, Task
+from dpdispatcher.submission import Resources, Submission, Task
 
 # local_session = LocalSession({'work_path':'temp2'})
 # local_context = LocalContext(local_root='temp1/0_md', work_profile=local_session)
 lazy_local_context = LazyLocalContext(
     local_root="/home/fengbo/10_dpdispatcher/dpdispatcher/tests/temp3",
     work_profile=None,
 )
```

### Comparing `dpdispatcher-0.5.5/tests/devel_test_lsf.py` & `dpdispatcher-0.5.6/tests/devel_test_lsf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import os
 import sys
 
 from dpdispatcher.machine import Machine
-from dpdispatcher.submission import Job, Resources, Submission, Task
+from dpdispatcher.submission import Resources, Submission, Task
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
 # task_need_resources has no effect
-with open("jsons/machine_lsf.json", "r") as f:
+with open("jsons/machine_lsf.json") as f:
     mdata = json.load(f)
 
 machine = Machine.load_from_dict(mdata["machine"])
 resources = Resources.load_from_dict(mdata["resources"])
 
 submission = Submission(
     work_base="0_md/",
```

### Comparing `dpdispatcher-0.5.5/tests/devel_test_shell.py` & `dpdispatcher-0.5.6/tests/devel_test_shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
-from dpdispatcher.batch import Batch
-from dpdispatcher.lazy_local_context import LazyLocalContext
 from dpdispatcher.local_context import LocalContext, LocalSession
 
 # from dpdispatcher.pbs import PBS
 from dpdispatcher.shell import Shell
-from dpdispatcher.submission import Job, Resources, Submission, Task
+from dpdispatcher.submission import Resources, Submission, Task
 
 local_session = LocalSession({"work_path": "temp2"})
 local_context = LocalContext(local_root="test_shell_dir/", work_profile=local_session)
 # lazy_local_context = LazyLocalContext(local_root='/home/fengbo/10_dpdispatcher/dpdispatcher/tests/temp3/0_md', work_profile=None)
 shell = Shell(context=local_context)
 # pbs = PBS(context=lazy_local_context)
```

### Comparing `dpdispatcher-0.5.5/tests/devel_test_slurm.py` & `dpdispatcher-0.5.6/tests/devel_test_slurm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import json
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 # from .context import dpdispatcher
 # from dpdispatcher.local_context import LocalContext
-from dpdispatcher.lazy_local_context import LazyLocalContext
 from dpdispatcher.machine import Machine
-from dpdispatcher.submission import Job, Resources, Submission, Task
+from dpdispatcher.submission import Resources, Submission, Task
 
 # from dpdispatcher.ssh_context import SSHContext
 
 
 # from dpdispatcher.submission import
 # from dpdispatcher.slurm import Slurm
 
@@ -30,15 +29,15 @@
 # resources = Resources(number_node=1, cpu_per_node=4, gpu_per_node=2, queue_name="GPU_2080Ti", group_size=4,
 #     custom_flags=['#SBATCH --exclude=2080ti000,2080ti001,2080ti002,2080ti004,2080ti005,2080ti006'],
 #     para_deg=2,
 #     strategy={"if_cuda_multi_devices":True})
 # slurm_sbatch_dict={'mem': '10G', 'cpus_per_task':1, 'time': "120:0:0"}
 # slurm_resources = SlurmResources(resources=resources, slurm_sbatch_dict=slurm_sbatch_dict)
 
-with open("jsons/machine_slurm.json", "r") as f:
+with open("jsons/machine_slurm.json") as f:
     mdata = json.load(f)
 
 machine = Machine.load_from_dict(mdata["machine"])
 resources = Resources.load_from_dict(mdata["resources"])
 
 submission = Submission(
     work_base="0_md/",
```

### Comparing `dpdispatcher-0.5.5/tests/devel_test_ssh_ali_ehpc.py` & `dpdispatcher-0.5.6/tests/devel_test_ssh_ali_ehpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # from dpdispatcher.local_context import LocalSession
 # from dpdispatcher.local_context import LocalContext
 
 # from dpdispatcher.batch import Batch
 # from dpdispatcher.pbs import PBS
 from dpdispatcher.batch_object import BatchObject
-from dpdispatcher.submission import Job, Resources, Submission, Task
+from dpdispatcher.submission import Resources, Submission, Task
 
-with open("ssh_machine.json", "r") as f:
+with open("ssh_machine.json") as f:
     jdata = json.load(f)
 
 batch = BatchObject(jdata=jdata)
 # local_session = LocalSession({'work_path':'temp2'})
 # local_context = LocalContext(local_root='temp1/', work_profile=local_session)
 # lazy_local_context = LazyLocalContext(local_root='/home/fengbo/10_dpdispatcher/dpdispatcher/tests/temp3/0_md', work_profile=None)
 # pbs = PBS(context=lazy_local_context)
```

### Comparing `dpdispatcher-0.5.5/tests/jsons/job.json` & `dpdispatcher-0.5.6/tests/jsons/job.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/jsons/machine_center.json` & `dpdispatcher-0.5.6/tests/jsons/machine_center.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/jsons/machine_diffenert.json` & `dpdispatcher-0.5.6/tests/jsons/machine_diffenert.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/jsons/machine_dp_cloud_server.json` & `dpdispatcher-0.5.6/tests/jsons/machine_dp_cloud_server.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/jsons/machine_lazy_local_lsf.json` & `dpdispatcher-0.5.6/tests/jsons/machine_lazy_local_lsf.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/jsons/machine_lazy_local_slurm.json` & `dpdispatcher-0.5.6/tests/jsons/machine_lazy_local_slurm.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/jsons/machine_lsf.json` & `dpdispatcher-0.5.6/tests/jsons/machine_lsf.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/jsons/machine_slurm.json` & `dpdispatcher-0.5.6/tests/jsons/machine_slurm.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/jsons/machine_yarn.json` & `dpdispatcher-0.5.6/tests/jsons/machine_yarn.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/jsons/submission.json` & `dpdispatcher-0.5.6/tests/jsons/submission.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/lsf/context.py` & `dpdispatcher-0.5.6/tests/lsf/context.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import sys
 
 sys.path.insert(
     0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..", "..", ".."))
 )
 
-from dpgen.dispatcher.Dispatcher import Dispatcher
-from dpgen.dispatcher.JobStatus import JobStatus
-from dpgen.dispatcher.LocalContext import LocalContext, LocalSession
-from dpgen.dispatcher.LSF import LSF
-from dpgen.dispatcher.SSHContext import SSHContext, SSHSession
+from dpgen.dispatcher.Dispatcher import Dispatcher  # noqa: F401
+from dpgen.dispatcher.JobStatus import JobStatus  # noqa: F401
+from dpgen.dispatcher.LocalContext import LocalContext, LocalSession  # noqa: F401
+from dpgen.dispatcher.LSF import LSF  # noqa: F401
+from dpgen.dispatcher.SSHContext import SSHContext, SSHSession  # noqa: F401
 
 
 def my_file_cmp(test, f0, f1):
     with open(f0) as fp0:
         with open(f1) as fp1:
             test.assertTrue(fp0.read() == fp1.read())
```

### Comparing `dpdispatcher-0.5.5/tests/lsf/test_dispatcher.py` & `dpdispatcher-0.5.6/tests/lsf/test_dispatcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,18 @@
-import glob
-import json
 import os
 import shutil
 import sys
-import time
 import unittest
-import uuid
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "lsf"
 from .context import (
-    LSF,
     Dispatcher,
-    JobStatus,
-    LocalContext,
-    LocalSession,
     my_file_cmp,
-    setUpModule,
+    setUpModule,  # noqa: F401
 )
 
 
 class TestDispatcher(unittest.TestCase):
     def setUp(self):
         os.makedirs("loc", exist_ok=True)
         os.makedirs("rmt", exist_ok=True)
```

### Comparing `dpdispatcher-0.5.5/tests/lsf/test_lsf_local.py` & `dpdispatcher-0.5.6/tests/lsf/test_lsf_local.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-import glob
-import json
 import os
 import shutil
 import sys
 import time
 import unittest
 import uuid
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "lsf"
-from .context import LSF, JobStatus, LocalContext, LocalSession, setUpModule
+from .context import (
+    LSF,
+    JobStatus,
+    LocalContext,
+    LocalSession,
+)
 
 
 class TestLSF(unittest.TestCase):
     def setUp(self):
         os.makedirs("loc", exist_ok=True)
         os.makedirs("rmt", exist_ok=True)
         os.makedirs("loc/task0", exist_ok=True)
```

### Comparing `dpdispatcher-0.5.5/tests/old/test_dispatcher_utils.py` & `dpdispatcher-0.5.6/tests/old/test_dispatcher_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-import glob
-import json
 import os
-import shutil
 import sys
-import time
 import unittest
-import uuid
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
 # from .context import FinRecord
-from .context import _split_tasks, setUpModule
+from .context import _split_tasks
 
 # class TestFinRecord(unittest.TestCase):
 #     def setUp(self):
 #         self.njobs = 10
 #         self.fr = FinRecord('.', self.njobs)
 
 #     def tearDown(self):
```

### Comparing `dpdispatcher-0.5.5/tests/old/test_lazy_local_context.py` & `dpdispatcher-0.5.6/tests/old/test_lazy_local_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-import glob
-import json
 import os
 import shutil
 import sys
 import time
 import unittest
 import uuid
-from pathlib import Path
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
-from .context import LazyLocalContext, setUpModule
+from .context import LazyLocalContext
 
 
 class TestLazyLocalContext(unittest.TestCase):
     def setUp(self):
         os.makedirs("loc", exist_ok=True)
         os.makedirs("loc/task0", exist_ok=True)
         os.makedirs("loc/task1", exist_ok=True)
@@ -80,15 +77,15 @@
                         os.path.exists(
                             os.path.join("loc", ii, "tag_failure_download_%s" % jj)
                         ),
                         msg="failed to find "
                         + os.path.join("loc", ii, "tag_failure_download_%s" % jj),
                     )
                     continue
-                with open(os.path.join("loc", ii, jj), "r") as fp:
+                with open(os.path.join("loc", ii, jj)) as fp:
                     tmp = fp.read()
                     self.assertEqual(tmp, record_uuid[cc])
                     cc += 1
         for ii in tasks:
             for jj in ["dir1"]:
                 self.assertFalse(os.path.exists(os.path.join("loc", ii, jj)))
                 self.assertTrue(
@@ -132,15 +129,15 @@
                         os.path.exists(
                             os.path.join("loc", ii, "tag_failure_download_%s" % jj)
                         ),
                         msg="found "
                         + os.path.join("loc", ii, "tag_failure_download_%s" % jj),
                     )
                     continue
-                with open(os.path.join("loc", ii, jj), "r") as fp:
+                with open(os.path.join("loc", ii, jj)) as fp:
                     tmp = fp.read()
                     self.assertEqual(tmp, record_uuid[cc])
                     cc += 1
         for ii in tasks:
             for jj in ["dir1"]:
                 self.assertFalse(os.path.exists(os.path.join("loc", ii, jj)))
                 self.assertFalse(
```

### Comparing `dpdispatcher-0.5.5/tests/old/test_local_context.py` & `dpdispatcher-0.5.6/tests/old/test_local_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-import glob
-import json
 import os
 import shutil
 import sys
 import time
 import unittest
 import uuid
-from pathlib import Path
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
-from .context import LocalContext, LocalSession, _identical_files, setUpModule
+from .context import LocalContext, LocalSession, _identical_files
 
 
 class TestIdFile(unittest.TestCase):
     def test_id(self):
         with open("f0", "w") as fp:
             fp.write("foo")
         with open("f1", "w") as fp:
@@ -116,15 +113,15 @@
                         record_uuid.append(tmp)
         files = ["dir1"]
         self.job.download(tasks, files)
         cc = 0
         for ii in tasks:
             for jj in ["dir1"]:
                 for kk in ["test6", "test7"]:
-                    with open(os.path.join("loc", ii, jj, kk), "r") as fp:
+                    with open(os.path.join("loc", ii, jj, kk)) as fp:
                         tmp = fp.read()
                         self.assertEqual(tmp, record_uuid[cc])
                         cc += 1
 
     def test_dl_t_t(self):
         # has local, has remote
         work_profile = LocalSession({"work_path": "rmt"})
@@ -152,15 +149,15 @@
                         record_uuid.append(tmp)
         files = ["dir1"]
         self.job.download(tasks, files)
         cc = 0
         for ii in tasks:
             for jj in ["dir1"]:
                 for kk in ["test6", "test7"]:
-                    with open(os.path.join("loc", ii, jj, kk), "r") as fp:
+                    with open(os.path.join("loc", ii, jj, kk)) as fp:
                         tmp = fp.read()
                         self.assertEqual(tmp, record_uuid[cc])
                         cc += 1
 
     def test_download_non_exist(self):
         work_profile = LocalSession({"work_path": "rmt"})
         self.job = LocalContext("loc", work_profile)
@@ -199,22 +196,22 @@
         # donwload
         files = ["test0", "dir0", "test4", "test5", "dir1"]
         self.job.download(tasks, files)
         # check dlded
         cc = 0
         for ii in tasks:
             for jj in ["test4", "test5"]:
-                with open(os.path.join("loc", ii, jj), "r") as fp:
+                with open(os.path.join("loc", ii, jj)) as fp:
                     tmp = fp.read()
                     self.assertEqual(tmp, record_uuid[cc])
                     cc += 1
         for ii in tasks:
             for jj in ["dir1"]:
                 for kk in ["test6"]:
-                    with open(os.path.join("loc", ii, jj, kk), "r") as fp:
+                    with open(os.path.join("loc", ii, jj, kk)) as fp:
                         tmp = fp.read()
                         self.assertEqual(tmp, record_uuid[cc])
                         cc += 1
         # check links preserved
         for ii in tasks:
             for jj in ["test0"]:
                 locf = os.path.join("loc", ii, jj)
@@ -263,15 +260,15 @@
                         os.path.exists(
                             os.path.join("loc", ii, "tag_failure_download_%s" % jj)
                         ),
                         msg="failed to find "
                         + os.path.join("loc", ii, "tag_failure_download_%s" % jj),
                     )
                     continue
-                with open(os.path.join("loc", ii, jj), "r") as fp:
+                with open(os.path.join("loc", ii, jj)) as fp:
                     tmp = fp.read()
                     self.assertEqual(tmp, record_uuid[cc])
                     cc += 1
         for ii in tasks:
             for jj in ["dir1"]:
                 self.assertFalse(os.path.exists(os.path.join("loc", ii, jj)))
                 self.assertTrue(
@@ -316,15 +313,15 @@
                         os.path.exists(
                             os.path.join("loc", ii, "tag_failure_download_%s" % jj)
                         ),
                         msg="found "
                         + os.path.join("loc", ii, "tag_failure_download_%s" % jj),
                     )
                     continue
-                with open(os.path.join("loc", ii, jj), "r") as fp:
+                with open(os.path.join("loc", ii, jj)) as fp:
                     tmp = fp.read()
                     self.assertEqual(tmp, record_uuid[cc])
                     cc += 1
         for ii in tasks:
             for jj in ["dir1"]:
                 self.assertFalse(os.path.exists(os.path.join("loc", ii, jj)))
                 self.assertFalse(
```

### Comparing `dpdispatcher-0.5.5/tests/old/test_ssh_context.py` & `dpdispatcher-0.5.6/tests/old/test_ssh_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import getpass
-import glob
-import json
 import os
 import shutil
 import sys
 import unittest
 import uuid
-from pathlib import Path
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
-from .context import SSHContext, SSHSession, setUpModule
+from .context import SSHContext, SSHSession
 
 
 class TestSSHContext(unittest.TestCase):
     def setUp(self):
         os.makedirs("loc", exist_ok=True)
         os.makedirs("loc/task0", exist_ok=True)
         os.makedirs("loc/task1", exist_ok=True)
@@ -110,22 +107,22 @@
         # donwload
         files = ["test4", "test5", "dir1"]
         self.job.download(tasks, files)
         # check dlded
         cc = 0
         for ii in tasks:
             for jj in ["test4", "test5"]:
-                with open(os.path.join("loc", ii, jj), "r") as fp:
+                with open(os.path.join("loc", ii, jj)) as fp:
                     tmp = fp.read()
                     self.assertEqual(tmp, record_uuid[cc])
                     cc += 1
         for ii in tasks:
             for jj in ["dir1"]:
                 for kk in ["test6"]:
-                    with open(os.path.join("loc", ii, jj, kk), "r") as fp:
+                    with open(os.path.join("loc", ii, jj, kk)) as fp:
                         tmp = fp.read()
                         self.assertEqual(tmp, record_uuid[cc])
                         cc += 1
 
     def test_donwload_check_mark(self):
         tasks = ["task0", "task1"]
         self.job.upload(tasks, ["test0", "dir0"])
@@ -159,15 +156,15 @@
                         os.path.exists(
                             os.path.join("loc", ii, "tag_failure_download_%s" % jj)
                         ),
                         msg="failed to find "
                         + os.path.join("loc", ii, "tag_failure_download_%s" % jj),
                     )
                     continue
-                with open(os.path.join("loc", ii, jj), "r") as fp:
+                with open(os.path.join("loc", ii, jj)) as fp:
                     tmp = fp.read()
                     self.assertEqual(tmp, record_uuid[cc])
                     cc += 1
         for ii in tasks:
             for jj in ["dir1"]:
                 self.assertFalse(os.path.exists(os.path.join("loc", ii, jj)))
                 self.assertTrue(
@@ -220,15 +217,15 @@
                         os.path.exists(
                             os.path.join("loc", ii, "tag_failure_download_%s" % jj)
                         ),
                         msg="found "
                         + os.path.join("loc", ii, "tag_failure_download_%s" % jj),
                     )
                     continue
-                with open(os.path.join("loc", ii, jj), "r") as fp:
+                with open(os.path.join("loc", ii, jj)) as fp:
                     tmp = fp.read()
                     self.assertEqual(tmp, record_uuid[cc])
                     cc += 1
         for ii in tasks:
             for jj in ["dir1"]:
                 self.assertFalse(os.path.exists(os.path.join("loc", ii, jj)))
                 self.assertFalse(
```

### Comparing `dpdispatcher-0.5.5/tests/pbs/test_dispatcher.py` & `dpdispatcher-0.5.6/tests/pbs/test_dispatcher.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,18 @@
-import glob
-import json
 import os
 import shutil
 import sys
-import time
 import unittest
-import uuid
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "pbs"
 from .context import (
-    PBS,
     Dispatcher,
-    JobStatus,
-    LocalContext,
-    LocalSession,
     my_file_cmp,
-    setUpModule,
+    setUpModule,  # noqa: F401
 )
 
 
 @unittest.skipIf(not shutil.which("qsub"), "requires PBS")
 class TestDispatcher(unittest.TestCase):
     def setUp(self):
         os.makedirs("loc", exist_ok=True)
```

### Comparing `dpdispatcher-0.5.5/tests/pbs/test_pbs_local.py` & `dpdispatcher-0.5.6/tests/pbs/test_pbs_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-import glob
-import json
 import os
 import shutil
 import sys
-import time
 import unittest
 import uuid
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "pbs"
-from .context import PBS, JobStatus, LocalContext, LocalSession, setUpModule
+from .context import PBS, LocalContext, LocalSession, setUpModule  # noqa: F401
 
 
 @unittest.skipIf(not shutil.which("qsub"), "requires PBS")
 class TestPBS(unittest.TestCase):
     def setUp(self):
         os.makedirs("loc", exist_ok=True)
         os.makedirs("rmt", exist_ok=True)
```

### Comparing `dpdispatcher-0.5.5/tests/sample_class.py` & `dpdispatcher-0.5.6/tests/sample_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,26 @@
-import glob
-import json
 import os
-import shutil
 import sys
-import time
-import unittest
-import uuid
-from unittest.mock import MagicMock, PropertyMock, patch
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
 # from .context import LocalSession
 # from .context import LocalContext
 # from dpdispatcher.local_context import LocalContext
 from .context import (
     PBS,
-    Job,
-    JobStatus,
     LocalContext,
     Resources,
     Slurm,
     Submission,
     Task,
 )
 
 
-class SampleClass(object):
+class SampleClass:
     @classmethod
     def get_sample_resources(cls):
         resources = Resources(
             number_node=1,
             cpu_per_node=4,
             gpu_per_node=1,
             queue_name="T4_4_15",
```

### Comparing `dpdispatcher-0.5.5/tests/shell/test_dispatcher.py` & `dpdispatcher-0.5.6/tests/slurm/test_dispatcher_lazy_local.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-import glob
-import json
 import os
 import shutil
 import sys
-import time
 import unittest
-import uuid
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
-__package__ = "shell"
+__package__ = "slurm"
 from .context import (
     Dispatcher,
-    JobStatus,
-    LocalContext,
-    LocalSession,
-    Shell,
     my_file_cmp,
-    setUpModule,
+    setUpModule,  # noqa: F401
 )
 
 
+@unittest.skipIf(not shutil.which("sbatch"), "requires Slurm")
 class TestDispatcher(unittest.TestCase):
     def setUp(self):
         os.makedirs("loc", exist_ok=True)
         os.makedirs("rmt", exist_ok=True)
         os.makedirs("loc/task0", exist_ok=True)
         os.makedirs("loc/task1", exist_ok=True)
         os.makedirs("loc/task2", exist_ok=True)
         for ii in ["loc/task0", "loc/task1", "loc/task2"]:
             with open(os.path.join(ii, "test0"), "w") as fp:
                 fp.write("this is test0 from " + ii + "\n")
-        work_profile = {"work_path": "rmt"}
-        self.disp = Dispatcher(work_profile, context_type="local", batch_type="shell")
+        work_profile = {}
+        self.disp = Dispatcher(work_profile, "lazy-local", "slurm")
+
+    def tearDown(self):
+        shutil.rmtree("loc")
+        shutil.rmtree("rmt")
+        if os.path.exists("dpgen.log"):
+            os.remove("dpgen.log")
 
     def test_sub_success(self):
         tasks = ["task0", "task1", "task2"]
         self.disp.run_jobs(
             None,
             "cp test0 test1",
             "loc",
```

### Comparing `dpdispatcher-0.5.5/tests/shell/test_shell_local.py` & `dpdispatcher-0.5.6/tests/shell/test_shell_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import glob
-import json
 import os
 import shutil
 import sys
 import time
 import unittest
 import uuid
 
@@ -11,15 +9,15 @@
 __package__ = "shell"
 from .context import (
     JobStatus,
     LocalContext,
     LocalSession,
     Shell,
     my_file_cmp,
-    setUpModule,
+    setUpModule,  # noqa: F401
 )
 
 
 class TestShell(unittest.TestCase):
     def setUp(self):
         os.makedirs("loc", exist_ok=True)
         os.makedirs("rmt", exist_ok=True)
```

### Comparing `dpdispatcher-0.5.5/tests/shell/test_shell_ssh.py` & `dpdispatcher-0.5.6/tests/shell/test_shell_ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import getpass
-import glob
-import json
 import os
 import shutil
 import sys
 import time
 import unittest
 import uuid
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "shell"
-from .context import JobStatus, Shell, SSHContext, SSHSession, setUpModule
+from .context import JobStatus, Shell, SSHContext, SSHSession, setUpModule  # noqa: F401
 
 
 class TestShell(unittest.TestCase):
     def setUp(self):
         os.makedirs("loc", exist_ok=True)
         os.makedirs("rmt", exist_ok=True)
         os.makedirs("loc/task0", exist_ok=True)
```

### Comparing `dpdispatcher-0.5.5/tests/slurm/context.py` & `dpdispatcher-0.5.6/tests/pbs/context.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import os
 import sys
 
 sys.path.insert(
     0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..", "..", ".."))
 )
 
-from dpgen.dispatcher.Dispatcher import Dispatcher
-from dpgen.dispatcher.JobStatus import JobStatus
-from dpgen.dispatcher.LazyLocalContext import LazyLocalContext
-from dpgen.dispatcher.LocalContext import LocalContext, LocalSession
-from dpgen.dispatcher.Slurm import Slurm
-from dpgen.dispatcher.SSHContext import SSHContext, SSHSession
+from dpgen.dispatcher.Dispatcher import Dispatcher  # noqa: F401
+from dpgen.dispatcher.JobStatus import JobStatus  # noqa: F401
+from dpgen.dispatcher.LocalContext import LocalContext, LocalSession  # noqa: F401
+from dpgen.dispatcher.PBS import PBS  # noqa: F401
+from dpgen.dispatcher.SSHContext import SSHContext, SSHSession  # noqa: F401
 
 
 def my_file_cmp(test, f0, f1):
     with open(f0) as fp0:
         with open(f1) as fp1:
             test.assertTrue(fp0.read() == fp1.read())
```

### Comparing `dpdispatcher-0.5.5/tests/slurm/test_dispatcher.py` & `dpdispatcher-0.5.6/tests/slurm/test_dispatcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,18 @@
-import glob
-import json
 import os
 import shutil
 import sys
-import time
 import unittest
-import uuid
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "slurm"
 from .context import (
     Dispatcher,
-    JobStatus,
-    LocalContext,
-    LocalSession,
-    Slurm,
     my_file_cmp,
-    setUpModule,
+    setUpModule,  # noqa: F401
 )
 
 
 @unittest.skipIf(not shutil.which("sbatch"), "requires Slurm")
 class TestDispatcher(unittest.TestCase):
     def setUp(self):
         os.makedirs("loc", exist_ok=True)
```

### Comparing `dpdispatcher-0.5.5/tests/slurm/test_slurm_lazy_local.py` & `dpdispatcher-0.5.6/tests/slurm/test_slurm_lazy_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import glob
-import json
 import os
 import shutil
 import sys
 import time
 import unittest
 import uuid
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "slurm"
-from .context import JobStatus, LazyLocalContext, Slurm, setUpModule
+from .context import JobStatus, LazyLocalContext, Slurm, setUpModule  # noqa: F401
 
 
 @unittest.skipIf(not shutil.which("sbatch"), "requires Slurm")
 class TestSlurm(unittest.TestCase):
     def setUp(self):
         os.makedirs("loc", exist_ok=True)
         os.makedirs("rmt", exist_ok=True)
```

### Comparing `dpdispatcher-0.5.5/tests/slurm/test_slurm_local.py` & `dpdispatcher-0.5.6/tests/slurm/test_slurm_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-import glob
-import json
 import os
 import shutil
 import sys
 import time
 import unittest
 import uuid
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "slurm"
-from .context import JobStatus, LocalContext, LocalSession, Slurm, setUpModule
+from .context import (
+    JobStatus,
+    LocalContext,
+    LocalSession,
+    Slurm,
+)
 
 
 @unittest.skipIf(not shutil.which("sbatch"), "requires Slurm")
 class TestSlurm(unittest.TestCase):
     def setUp(self):
         os.makedirs("loc", exist_ok=True)
         os.makedirs("rmt", exist_ok=True)
```

### Comparing `dpdispatcher-0.5.5/tests/slurm/test_slurm_ssh.py` & `dpdispatcher-0.5.6/tests/slurm/test_slurm_ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import glob
-import json
 import os
 import shutil
 import sys
 import time
 import unittest
 import uuid
 
@@ -11,15 +9,15 @@
 __package__ = "slurm"
 from .context import (
     JobStatus,
     LocalContext,
     LocalSession,
     Slurm,
     my_file_cmp,
-    setUpModule,
+    setUpModule,  # noqa: F401
 )
 
 
 @unittest.skipIf(not shutil.which("sbatch"), "requires Slurm")
 class TestSlurm(unittest.TestCase):
     def setUp(self):
         os.makedirs("loc", exist_ok=True)
```

### Comparing `dpdispatcher-0.5.5/tests/test_argcheck.py` & `dpdispatcher-0.5.6/tests/test_argcheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 import unittest
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
 
-from .context import Machine, Resources, Task, setUpModule
+from .context import Machine, Resources, Task, setUpModule  # noqa: F401
 
 
 class TestJob(unittest.TestCase):
     def test_machine_argcheck(self):
         norm_dict = Machine.load_from_dict(
             {
                 "batch_type": "slurm",
```

### Comparing `dpdispatcher-0.5.5/tests/test_class_job.py` & `dpdispatcher-0.5.6/tests/test_class_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,19 @@
-import glob
-import json
 import os
-import shutil
 import sys
-import time
 import unittest
-import uuid
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
 # from .context import LocalSession
 # from .context import LocalContext
 from .context import (
-    PBS,
     Job,
-    JobStatus,
-    LocalContext,
-    Resources,
     Submission,
-    Task,
-    setUpModule,
+    setUpModule,  # noqa: F401
 )
 from .sample_class import SampleClass
 
 
 class TestJob(unittest.TestCase):
     def setUp(self):
         self.job = SampleClass.get_sample_job()
```

### Comparing `dpdispatcher-0.5.5/tests/test_class_machine.py` & `dpdispatcher-0.5.6/tests/test_class_machine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,18 @@
-import glob
-import json
 import os
-import shutil
 import sys
-import time
 import unittest
-import uuid
-from socket import gaierror
-from unittest.mock import MagicMock, PropertyMock, patch
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
-from dargs.dargs import ArgumentKeyError
 
 from .context import (
-    LSF,
     PBS,
-    BaseContext,
-    DistributedShell,
-    HDFSContext,
-    JobStatus,
-    LazyLocalContext,
-    LocalContext,
     Machine,
-    Shell,
-    Slurm,
-    SSHContext,
-    dargs,
+    setUpModule,  # noqa: F401
 )
 from .sample_class import SampleClass
 
 
 class TestMachineInit(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
```

### Comparing `dpdispatcher-0.5.5/tests/test_class_machine_dispatch.py` & `dpdispatcher-0.5.6/tests/test_class_machine_dispatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,29 @@
-import glob
-import json
 import os
-import shutil
 import sys
-import time
 import unittest
-import uuid
 from socket import gaierror
-from unittest.mock import MagicMock, PropertyMock, patch
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
 from dargs.dargs import ArgumentValueError
 
 from .context import (
     LSF,
     PBS,
     BaseContext,
     DistributedShell,
-    HDFSContext,
-    JobStatus,
     LazyLocalContext,
     Lebesgue,
     LocalContext,
     Machine,
     Shell,
     Slurm,
-    SSHContext,
-    dargs,
+    setUpModule,  # noqa: F401
 )
-from .sample_class import SampleClass
 
 
 class TestMachineDispatch(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
 
     def test_init_machine_pbs_lazy_local(self):
```

### Comparing `dpdispatcher-0.5.5/tests/test_class_resources.py` & `dpdispatcher-0.5.6/tests/test_class_resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,19 @@
-import glob
 import json
 import os
-import shutil
 import sys
-import time
 import unittest
-import uuid
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
 # from .context import LocalSession
 # from .context import LocalContext
 from .context import (
-    PBS,
-    Job,
-    JobStatus,
-    LocalContext,
     Resources,
-    Submission,
-    Task,
-    setUpModule,
+    setUpModule,  # noqa: F401
 )
 from .sample_class import SampleClass
 
 
 class TestResources(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
@@ -43,15 +33,15 @@
     def test_serialize_deserialize(self):
         self.assertEqual(
             self.resources,
             Resources.deserialize(resources_dict=self.resources.serialize()),
         )
 
     def test_resources_json(self):
-        with open("jsons/resources.json", "r") as f:
+        with open("jsons/resources.json") as f:
             resources_json_dict = json.load(f)
         self.assertTrue(resources_json_dict, self.resources_dict)
         self.assertTrue(resources_json_dict, self.resources.serialize())
 
     def test_load_from_json(self):
         resources = Resources.load_from_json("jsons/resources.json")
         self.assertTrue(resources, self.resources)
```

### Comparing `dpdispatcher-0.5.5/tests/test_class_submission.py` & `dpdispatcher-0.5.6/tests/test_class_submission.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import glob
 import json
 import os
-import shutil
 import sys
-import time
 import unittest
-import uuid
-from unittest.mock import MagicMock, PropertyMock, patch
+from unittest.mock import MagicMock, patch
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
-from .context import PBS, Job, JobStatus, LocalContext, Resources, Submission, Task
+from .context import (
+    JobStatus,
+    Submission,
+    setUpModule,  # noqa: F401
+)
 from .sample_class import SampleClass
 
 
 class TestSubmission(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
         pbs = SampleClass.get_sample_pbs_local_context()
@@ -104,11 +104,7 @@
         submission_repr = repr(self.submission)
         j = json.dumps(self.submission.serialize(), indent=4)
         self.assertEqual(submission_repr, j)
         # self.submission_to_json()
 
     def test_clean(self):
         pass
-
-    def test_try_recover_from_json(self):
-        pass
-        # self.submission.try_recover_from_json
```

### Comparing `dpdispatcher-0.5.5/tests/test_class_submission_init.py` & `dpdispatcher-0.5.6/tests/test_class_submission_init.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-import glob
-import json
 import os
-import shutil
 import sys
-import time
 import unittest
-import uuid
-from unittest.mock import MagicMock, PropertyMock, patch
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
-from .context import PBS, Job, JobStatus, LocalContext, Resources, Submission, Task
+from .context import setUpModule  # noqa: F401
 from .sample_class import SampleClass
 
 # print('in', SampleClass.get_sample_empty_submission())
 
 
 class TestSubmissionInit(unittest.TestCase):
     def setUp(self):
```

### Comparing `dpdispatcher-0.5.5/tests/test_class_task.py` & `dpdispatcher-0.5.6/tests/test_class_task.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-import glob
 import json
 import os
-import shutil
 import sys
-import time
 import unittest
-import uuid
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
 # from .context import LocalContext
-from dpdispatcher.local_context import LocalContext
 
 # from .context import Dispatcher
-from .context import Job, JobStatus, Resources, Submission, Task, setUpModule
+from .context import (
+    Task,
+    setUpModule,  # noqa: F401
+)
 from .sample_class import SampleClass
 
 
 class TestTask(unittest.TestCase):
     def setUp(self):
         self.task = SampleClass.get_sample_task()
         self.task_dict = SampleClass.get_sample_task_dict()
@@ -29,15 +27,15 @@
         task = Task.deserialize(task_dict=self.task_dict)
         self.assertTrue(task, self.task)
 
     def test_serialize_deserialize(self):
         self.assertEqual(Task.deserialize(task_dict=self.task.serialize()), self.task)
 
     def test_task_json(self):
-        with open("jsons/task.json", "r") as f:
+        with open("jsons/task.json") as f:
             task_json_dict = json.load(f)
         self.assertTrue(task_json_dict, self.task_dict)
         self.assertTrue(task_json_dict, self.task.serialize())
 
     def test_repr(self):
         task_repr = repr(self.task)
         print("debug:", task_repr, self.task_dict)
```

### Comparing `dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_context_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.5.6/tests/test_context_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_group_size.py` & `dpdispatcher-0.5.6/tests/test_group_size.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 import os
 import sys
 from pathlib import Path
 from unittest import TestCase
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
-from .context import Machine, Resources, Submission, Task
+from .context import (
+    Machine,
+    Resources,
+    Submission,
+    Task,
+    setUpModule,  # noqa: F401
+)
 
 # 99 tasks in total
 # group_size - expected_ntasks
 group_ntasks_pairs = [
     (1, 99),
     (3, 33),
     (10, 10),
```

### Comparing `dpdispatcher-0.5.5/tests/test_hdfs_context.py` & `dpdispatcher-0.5.6/tests/test_hdfs_context.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-import getpass
-import glob
 import json
 import os
-import pathlib
 import shutil
 import sys
 import tarfile
 import unittest
-import uuid
+from glob import glob
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
-from glob import glob
 
-from .context import HDFS, HDFSContext, Machine
+from .context import (
+    HDFS,
+    HDFSContext,
+    Machine,
+    setUpModule,  # noqa: F401
+)
 from .sample_class import SampleClass
 
 
 @unittest.skipIf(not shutil.which("hadoop"), "requires hadoop")
 class TestHDFSContext(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        with open("jsons/machine_yarn.json", "r") as f:
+        with open("jsons/machine_yarn.json") as f:
             mdata = json.load(f)
         cls.machine = Machine.load_from_dict(mdata["machine"])
         cls.submission = SampleClass.get_sample_submission()
         cls.submission.bind_machine(cls.machine)
         cls.submission_hash = cls.submission.submission_hash
 
     def setUp(self):
```

### Comparing `dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_hdfs_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.5.6/tests/test_hdfs_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_lazy_local_context.py` & `dpdispatcher-0.5.6/tests/test_lazy_local_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-import glob
-import json
 import os
 import shutil
 import sys
-import time
 import unittest
-import uuid
-from pathlib import Path
-from unittest.mock import MagicMock, PropertyMock, patch
+from unittest.mock import MagicMock
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
-from .context import LazyLocalContext, setUpModule
+from .context import (
+    LazyLocalContext,
+    setUpModule,  # noqa: F401
+)
 
 
 class TestLazyLocalContext(unittest.TestCase):
     def setUp(self):
         # os.makedirs('loc', exist_ok = True)
         # os.makedirs('loc/task0', exist_ok = True)
         # os.makedirs('loc/task1', exist_ok = True)
```

### Comparing `dpdispatcher-0.5.5/tests/test_local_context.py` & `dpdispatcher-0.5.6/tests/test_local_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # %%
-import glob
-import json
 import os
 import shutil
 import sys
-import time
 import unittest
 import uuid
-from pathlib import Path
-from unittest.mock import MagicMock, PropertyMock, patch
+from unittest.mock import MagicMock
 
 # %%
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
 # from .context import LocalSession
-from .context import LocalContext, Task, _identical_files, get_file_md5, setUpModule
-from .sample_class import SampleClass
+from .context import (
+    LocalContext,
+    _identical_files,
+    get_file_md5,
+    setUpModule,  # noqa: F401
+)
 
 # from .context import dpd
 
 
 class TestIdFile(unittest.TestCase):
     def test_id(self):
         with open("f0", "w") as fp:
```

### Comparing `dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_lsf_dir/0_md/submission.json` & `dpdispatcher-0.5.6/tests/test_lsf_dir/0_md/submission.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_lsf_script_generation.py` & `dpdispatcher-0.5.6/tests/test_lsf_script_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 # from dpdispatcher.batch_object import BatchObject
 # from dpdispatcher.batch import Batch
 import os
-import shutil
 import sys
 import textwrap
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
 import json
 import unittest
 
 from .context import (
-    Job,
-    LocalContext,
     Machine,
     Resources,
-    Shell,
     Submission,
     Task,
-    get_file_md5,
+    setUpModule,  # noqa: F401
 )
 
 
 class TestLSFScriptGeneration(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
 
     def test_shell_trival(self):
-        with open("jsons/machine_lazy_local_lsf.json", "r") as f:
+        with open("jsons/machine_lazy_local_lsf.json") as f:
             machine_dict = json.load(f)
 
         machine = Machine(**machine_dict["machine"])
         resources = Resources(**machine_dict["resources"])
 
         task1 = Task(
             command="cat example.txt",
```

### Comparing `dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_pbs_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.5.6/tests/test_pbs_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_retry.py` & `dpdispatcher-0.5.6/tests/test_retry.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import os
 import sys
 import unittest
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
-from .context import RetrySignal, retry
+from .context import (
+    RetrySignal,
+    retry,
+    setUpModule,  # noqa: F401
+)
 
 
 class TestRetry(unittest.TestCase):
     def test_retry_fail(self):
-        """Always retry"""
+        """Always retry."""
 
         @retry(max_retry=3, sleep=0.05, catch_exception=RetrySignal)
         def some_method():
             raise RetrySignal("Failed to do something")
 
         with self.assertRaises(RuntimeError):
             some_method()
 
     def test_retry_success(self):
-        """Retry less than 3 times"""
+        """Retry less than 3 times."""
         retry_times = [0]
 
         @retry(max_retry=3, sleep=0.05, catch_exception=RetrySignal)
         def some_method(retry_times):
             if retry_times[0] < 2:
                 retry_times[0] += 1
                 raise RetrySignal("Failed to do something")
```

### Comparing `dpdispatcher-0.5.5/tests/test_run_submission.py` & `dpdispatcher-0.5.6/tests/test_run_submission.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 import shutil
 import sys
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
 import unittest
 
-from .context import Machine, Resources, Submission, Task
+from .context import (
+    Machine,
+    Resources,
+    Submission,
+    Task,
+    setUpModule,  # noqa: F401
+)
 
 
 class RunSubmission:
     def setUp(self):
         self.machine_dict = {
             "batch_type": "Shell",
             "context_type": "LocalContext",
@@ -60,15 +66,15 @@
                 outlog=f"out{ii}.txt",
             )
             task_list.append(task)
 
         # test space in file name
         task_list.append(
             Task(
-                command=f"echo dpdispatcher_unittest_space",
+                command="echo dpdispatcher_unittest_space",
                 task_work_path="test space/",
                 forward_files=["inp space.txt"],
                 backward_files=["out space.txt"],
                 outlog="out space.txt",
             )
         )
         submission = Submission(
```

### Comparing `dpdispatcher-0.5.5/tests/test_shell_cuda_multi_devices.py` & `dpdispatcher-0.5.6/tests/test_shell_cuda_multi_devices.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,32 +4,30 @@
 import sys
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
 import unittest
 
 from .context import (
-    Job,
-    LocalContext,
     Machine,
     Resources,
-    Shell,
     Submission,
     Task,
     get_file_md5,
+    setUpModule,  # noqa: F401
 )
 
 
 @unittest.skipIf(sys.platform == "win32", "Shell is not supported on Windows")
 class TestShellCudaMultiDevices(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
 
     def test_shell_cuda_multi_devices(self):
-        with open("jsons/machine_if_cuda_multi_devices.json", "r") as f:
+        with open("jsons/machine_if_cuda_multi_devices.json") as f:
             machine_dict = json.load(f)
         machine = Machine.load_from_dict(machine_dict["machine"])
         resources = Resources.load_from_dict(machine_dict["resources"])
 
         task_list = []
         for ii in range(16):
             task = Task(
```

### Comparing `dpdispatcher-0.5.5/tests/test_shell_trival.py` & `dpdispatcher-0.5.6/tests/test_shell_trival.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,36 +6,34 @@
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
 import json
 import unittest
 
 from .context import (
-    Job,
-    LocalContext,
     Machine,
     Resources,
-    Shell,
     Submission,
     Task,
     get_file_md5,
+    setUpModule,  # noqa: F401
 )
 
 
 @unittest.skipIf(sys.platform == "win32", "Shell is not supported on Windows")
 class TestShellTrival(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
         # self.local_context_dict = {
         #     'local_root': './test_shell_trival_dir',
         #     'remote_root': './tmp_shell_trival_dir'
         # }
 
     def test_shell_trival(self):
-        with open("jsons/machine_local_shell.json", "r") as f:
+        with open("jsons/machine_local_shell.json") as f:
             machine_dict = json.load(f)
 
         machine = Machine(**machine_dict["machine"])
         resources = Resources(**machine_dict["resources"])
 
         task1 = Task(
             command="cat example.txt",
@@ -81,15 +79,15 @@
             f1 = os.path.join(
                 "test_shell_trival_dir/", "parent_dir/", dir, "example.txt"
             )
             f2 = os.path.join("test_shell_trival_dir/", "parent_dir/", dir, "out.txt")
             self.assertEqual(get_file_md5(f1), get_file_md5(f2))
 
     def test_shell_fail(self):
-        with open("jsons/machine_local_shell.json", "r") as f:
+        with open("jsons/machine_local_shell.json") as f:
             machine_dict = json.load(f)
 
         machine = Machine(**machine_dict["machine"])
         resources = Resources(**machine_dict["resources"])
 
         task = Task(
             command="cat mock_fail_task.txt && exit 1",
@@ -111,25 +109,25 @@
             backward_common_files=[],
             task_list=task_list,
         )
         with self.assertRaises(RuntimeError):
             submission.run_submission()
 
     def test_shell_recover(self):
-        with open("jsons/machine_lazylocal_shell.json", "r") as f:
+        with open("jsons/machine_lazylocal_shell.json") as f:
             machine_dict = json.load(f)
 
         machine = Machine(**machine_dict["machine"])
         resources = Resources(**machine_dict["resources"])
 
         pass
 
     def test_dir_with_space(self):
-        """Test directory with space"""
-        with open("jsons/machine_local_shell.json", "r") as f:
+        """Test directory with space."""
+        with open("jsons/machine_local_shell.json") as f:
             machine_dict = json.load(f)
 
         machine = Machine(**machine_dict["machine"])
         resources = Resources(**machine_dict["resources"])
 
         task1 = Task(
             command="cat example.txt",
```

### Comparing `dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json` & `dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_slurm_dir/0_md/submission.json` & `dpdispatcher-0.5.6/tests/test_slurm_dir/0_md/submission.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.5/tests/test_slurm_script_generation.py` & `dpdispatcher-0.5.6/tests/test_slurm_script_generation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 # from dpdispatcher.batch_object import BatchObject
 # from dpdispatcher.batch import Batch
 import os
-import shutil
 import sys
 import textwrap
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
 import json
 import unittest
 
 from .context import (
-    Job,
-    LocalContext,
     Machine,
     Resources,
-    Shell,
     Submission,
     Task,
-    get_file_md5,
+    setUpModule,  # noqa: F401
 )
 
 
 class TestSlurmScriptGeneration(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
 
     def test_shell_trival(self):
-        with open("jsons/machine_lazy_local_slurm.json", "r") as f:
+        with open("jsons/machine_lazy_local_slurm.json") as f:
             machine_dict = json.load(f)
 
         machine = Machine(**machine_dict["machine"])
         resources = Resources(**machine_dict["resources"])
 
         task1 = Task(
             command="cat example.txt",
```

### Comparing `dpdispatcher-0.5.5/tests/test_ssh_context.py` & `dpdispatcher-0.5.6/tests/test_ssh_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,22 @@
 import sys
 import unittest
 
 from paramiko.ssh_exception import SSHException
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
-from .context import Machine, Resources, SSHSession, Submission, Task
+from .context import (
+    Machine,
+    Resources,
+    SSHSession,
+    Submission,
+    Task,
+    setUpModule,  # noqa: F401
+)
 from .sample_class import SampleClass
 
 
 @unittest.skipIf(
     os.environ.get("DPDISPATCHER_TEST") != "ssh", "outside the ssh testing environment"
 )
 class TestSSHContext(unittest.TestCase):
@@ -85,19 +92,19 @@
                 "cpu_per_node": 1,
                 "gpu_per_node": 0,
                 "queue_name": "?",
                 "group_size": 2,
             }
         )
         task = Task(
-            command=f"echo dpdispatcher_unittest",
+            command="echo dpdispatcher_unittest",
             task_work_path="./",
             forward_files=[],
             backward_files=[],
-            outlog=f"out.txt",
+            outlog="out.txt",
         )
 
         submission = Submission(
             work_base="./",
             machine=machine,
             resources=resources,
             forward_common_files=[],
```

