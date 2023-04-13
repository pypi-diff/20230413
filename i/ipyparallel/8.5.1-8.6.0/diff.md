# Comparing `tmp/ipyparallel-8.5.1.tar.gz` & `tmp/ipyparallel-8.6.0.tar.gz`

## Comparing `ipyparallel-8.5.1.tar` & `ipyparallel-8.6.0.tar`

### file list

```diff
@@ -1,296 +1,295 @@
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/.coveragerc
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/.eslintignore
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/.eslintrc.js
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/.flake8
--rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/.mailmap
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/.prettierignore
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/asv.conf.json
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/install.json
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/package.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/readthedocs.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/tsconfig.eslint.json
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/tsconfig.json
--rw-r--r--   0        0        0   201572 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/yarn.lock
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/.binder/jupyter_config.json
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/.binder/postBuild
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/.binder/requirements.txt
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/.github/workflows/test.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/.gitignore
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/asv.conf.json
--rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/asv_normal.sh
--rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/asv_quick.sh
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/asv_runner.py
--rw-r--r--   0        0        0   182323 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/async_benchmark.ipynb
--rw-r--r--   0        0        0    13159 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/benchmark_result.py
--rw-r--r--   0        0        0   669564 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/benchmark_results.ipynb
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/cluster_start.py
--rw-r--r--   0        0        0    79070 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/depth_benchmark.ipynb
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/engines_test.py
--rwxr-xr-x   0        0        0     5486 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/gcloud_setup.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/instance_setup.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/logger.py
--rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/profiling_initial_results.ipynb
--rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/profiling_latest_results.ipynb
--rw-r--r--   0        0        0   160310 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/push_benchmarks.ipynb
--rw-r--r--   0        0        0   862420 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/scheduler_benchmarks.ipynb
--rw-r--r--   0        0        0   147522 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/throughtput_benchmarks.ipynb
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/benchmarks/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/benchmarks/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/benchmarks/testing.py
--rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/benchmarks/throughput.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/benchmarks/utils.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/explore/control_flow.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/explore/scheduler.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/machine_configs/asv-testing-16.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/machine_configs/asv-testing-32.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/machine_configs/asv-testing-64.json
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/machine_configs/asv-testing-96.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/profiling/__init__.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/profiling/profiling_code.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/profiling/profiling_code_runner.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/profiling/view_profiling_results.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/results/benchmarks.json
--rw-r--r--   0        0        0    16442 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/results/asv-testing-64-2020-04-28/CoalescingBroadcast.json
--rw-r--r--   0        0        0    32378 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/results/asv-testing-64-2020-04-28/CoalescingPush.json
--rw-r--r--   0        0        0    36602 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/results/asv-testing-64-2020-05-12-19-52-58/results.json
--rw-r--r--   0        0        0    49624 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/results/asv-testing-64-2020-05-19-00-04-55/results.json
--rw-r--r--   0        0        0    70610 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/results/asv_testing-16-2020-04-29-20-02-25/results.json
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/benchmarks/results/asv_testing-16-2020-05-04-17-43/results.json
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ci/slurm/Dockerfile
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ci/slurm/docker-compose.yaml
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ci/slurm/entrypoint.sh
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ci/slurm/slurm.conf
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ci/ssh/Dockerfile
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ci/ssh/docker-compose.yaml
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ci/ssh/ipcluster_config.py
--rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/Makefile
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/environment.yml
--rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/make.bat
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/requirements.txt
--rw-r--r--   0        0        0    16334 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/changelog.md
--rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/conf.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/index.md
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/links.txt
--rw-r--r--   0        0        0   234426 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/_static/IPyParallel-MPI-Example.png
--rw-r--r--   0        0        0    69226 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/_static/basic.mp4
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/api/ipyparallel.rst
--rw-r--r--   0        0        0    26434 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/Cluster API.ipynb
--rw-r--r--   0        0        0   279116 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/Data Publication API.ipynb
--rw-r--r--   0        0        0    19257 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/Futures.ipynb
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/Index.ipynb
--rw-r--r--   0        0        0    67353 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/Monitoring an MPI Simulation - 1.ipynb
--rw-r--r--   0        0        0    62592 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/Monitoring an MPI Simulation - 2.ipynb
--rw-r--r--   0        0        0   165516 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/Monte Carlo Options.ipynb
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/Parallel Decorator and map.ipynb
--rw-r--r--   0        0        0  3554371 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/Parallel Magics.ipynb
--rw-r--r--   0        0        0    27919 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/Using Dill.ipynb
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/Using MPI with IPython Parallel.ipynb
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/customresults.py
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/dagdeps.py
--rw-r--r--   0        0        0    42291 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/dask.ipynb
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/dependencies.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/fetchparse.py
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/iopubwatcher.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/itermapresult.py
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/joblib.ipynb
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/nwmerge.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/phistogram.py
--rw-r--r--   0        0        0    48362 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/progress.ipynb
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/task_mod.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/task_profiler.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/throughput.py
--rw-r--r--   0        0        0   329806 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/visualizing-tasks.ipynb
--rw-r--r--   0        0        0   439979 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/broadcast/Broadcast view.ipynb
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/broadcast/Dockerfile
--rw-r--r--   0        0        0    69566 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/broadcast/MPI Broadcast.ipynb
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/broadcast/docker-compose.yaml
--rw-r--r--   0        0        0    84423 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/broadcast/memmap Broadcast.ipynb
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/daVinci Word Count/pwordfreq.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/daVinci Word Count/wordfreq.py
--rw-r--r--   0        0        0     6923 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/interengine/bintree.py
--rwxr-xr-x   0        0        0     2823 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/interengine/bintree_script.py
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/interengine/communicator.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/interengine/interengine.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/pi/parallelpi.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/pi/pidigits.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/rmt/rmt.ipy
--rw-r--r--   0        0        0    45443 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/rmt/rmt.ipynb
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/rmt/rmtkernel.py
--rwxr-xr-x   0        0        0    19532 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/wave2D/RectPartitioner.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/wave2D/communicator.py
--rwxr-xr-x   0        0        0     7226 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/wave2D/parallelwave-mpi.py
--rwxr-xr-x   0        0        0     7405 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/wave2D/parallelwave.py
--rwxr-xr-x   0        0        0    11642 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/examples/wave2D/wavesolver.py
--rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/connections.md
--rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/dag_dependencies.md
--rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/db.md
--rw-r--r--   0        0        0    21297 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/details.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/index.md
--rw-r--r--   0        0        0     6196 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/launchers.md
--rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/messages.md
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/mpi.md
--rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/security.md
--rw-r--r--   0        0        0    32144 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/allconnections.png
--rw-r--r--   0        0        0   303213 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/allconnections.svg
--rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/dagdeps.pdf
--rw-r--r--   0        0        0   202436 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/dagdeps.png
--rw-r--r--   0        0        0   153577 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/frontend-kernel.png
--rw-r--r--   0        0        0   283962 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/frontend-kernel.svg
--rw-r--r--   0        0        0    38554 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/hbfade.png
--rw-r--r--   0        0        0    39136 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/iopubfade.png
--rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/ipy_kernel_and_terminal.png
--rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/ipy_kernel_and_terminal.svg
--rw-r--r--   0        0        0    23877 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/nbconvert.png
--rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/nbconvert.svg
--rw-r--r--   0        0        0    30974 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/notebook_components.png
--rw-r--r--   0        0        0    24792 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/notebook_components.svg
--rw-r--r--   0        0        0    37583 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/notiffade.png
--rw-r--r--   0        0        0    41180 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/other_kernels.png
--rw-r--r--   0        0        0    14281 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/other_kernels.svg
--rw-r--r--   0        0        0    38260 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/queryfade.png
--rw-r--r--   0        0        0    40459 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/queuefade.png
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/simpledag.pdf
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/reference/figs/simpledag.png
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/asyncresult.md
--rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/demos.md
--rw-r--r--   0        0        0    23931 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/direct.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/index.md
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/intro.md
--rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/magics.md
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/process.md
--rw-r--r--   0        0        0    16512 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/task.md
--rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/figs/asian_call.pdf
--rw-r--r--   0        0        0    23681 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/figs/asian_call.png
--rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/figs/asian_put.pdf
--rw-r--r--   0        0        0    23108 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/figs/asian_put.png
--rw-r--r--   0        0        0    48750 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/figs/mec_simple.pdf
--rw-r--r--   0        0        0    50744 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/figs/mec_simple.png
--rw-r--r--   0        0        0   128061 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/figs/parallel_pi.pdf
--rw-r--r--   0        0        0   115825 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/figs/parallel_pi.png
--rw-r--r--   0        0        0    41799 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/figs/single_digits.pdf
--rw-r--r--   0        0        0    36727 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/figs/single_digits.png
--rw-r--r--   0        0        0    74773 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/figs/two_digit_counts.pdf
--rw-r--r--   0        0        0    73675 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/figs/two_digit_counts.png
--rw-r--r--   0        0        0    18561 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/docs/source/tutorial/figs/wideView.png
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/__init__.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/_async.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/_version.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/datapub.py
--rw-r--r--   0        0        0     8108 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/error.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/joblib.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/logger.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/traitlets.py
--rw-r--r--   0        0        0    23239 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/apps/__init__.py
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/apps/baseapp.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/apps/ipclusterapp.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/apps/ipcontrollerapp.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/apps/ipengineapp.py
--rwxr-xr-x   0        0        0     2253 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/apps/iploggerapp.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/apps/launcher.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/apps/logwatcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/client/__init__.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/client/_joblib.py
--rw-r--r--   0        0        0    42086 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/client/asyncresult.py
--rw-r--r--   0        0        0    91782 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/client/client.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/client/futures.py
--rw-r--r--   0        0        0    18633 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/client/magics.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/client/map.py
--rw-r--r--   0        0        0     9867 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/client/remotefunction.py
--rw-r--r--   0        0        0    54129 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/client/view.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/cluster/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/cluster/__main__.py
--rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/cluster/_winhpcjob.py
--rwxr-xr-x   0        0        0    23629 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/cluster/app.py
--rw-r--r--   0        0        0    36537 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/cluster/cluster.py
--rw-r--r--   0        0        0    84108 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/cluster/launcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/controller/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/controller/__main__.py
--rwxr-xr-x   0        0        0    44147 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/controller/app.py
--rw-r--r--   0        0        0     8820 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/controller/broadcast_scheduler.py
--rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/controller/dependency.py
--rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/controller/dictdb.py
--rwxr-xr-x   0        0        0    10768 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/controller/heartmonitor.py
--rw-r--r--   0        0        0    55731 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/controller/hub.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/controller/mongodb.py
--rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/controller/scheduler.py
--rw-r--r--   0        0        0    14842 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/controller/sqlitedb.py
--rw-r--r--   0        0        0    27127 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/controller/task_scheduler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/engine/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/engine/__main__.py
--rwxr-xr-x   0        0        0    33960 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/engine/app.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/engine/datapub.py
--rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/engine/kernel.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/engine/log.py
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/engine/nanny.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/labextension/package.json
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/labextension/schemas/ipyparallel-labextension/package.json.orig
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/labextension/schemas/ipyparallel-labextension/plugin.json
--rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/labextension/static/114.b63b1cb1deb6ab07694a.js
--rw-r--r--   0        0        0    25408 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/labextension/static/592.459a013fb5cd633ee1f8.js
--rw-r--r--   0        0        0     7760 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/labextension/static/remoteEntry.624aa72a8010f7bdad27.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/labextension/static/style.js
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/nbextension/__init__.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/nbextension/base.py
--rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/nbextension/handlers.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/nbextension/install.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/nbextension/static/clusterlist.css
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/nbextension/static/clusterlist.js
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/nbextension/static/main.js
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/serialize/__init__.py
--rw-r--r--   0        0        0    14863 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/serialize/canning.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/serialize/codeutil.py
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/serialize/serialize.py
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/_test_startup_crash.py
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/clienttest.py
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/conftest.py
--rw-r--r--   0        0        0     8255 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_apps.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_async.py
--rw-r--r--   0        0        0    18324 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_asyncresult.py
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_canning.py
--rw-r--r--   0        0        0    24230 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_client.py
--rw-r--r--   0        0        0    12282 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_cluster.py
--rw-r--r--   0        0        0    10702 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_db.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_dependency.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_executor.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_joblib.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_launcher.py
--rw-r--r--   0        0        0     8908 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_lbview.py
--rw-r--r--   0        0        0    18314 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_magics.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_mongodb.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_mpi.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_remotefunction.py
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_serialize.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_slurm.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_ssh.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_util.py
--rw-r--r--   0        0        0    29722 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_view.py
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/ipyparallel/tests/test_view_broadcast.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/jupyter-config/jupyter_notebook_config.d/ipyparallel.json
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/jupyter-config/jupyter_server_config.d/ipyparallel.json
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/jupyter-config/nbconfig/tree.d/ipyparallel.json
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/lab/webpack.config.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/lab/schema/plugin.json
--rw-r--r--   0        0        0    23367 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/lab/src/clusters.tsx
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/lab/src/commands.ts
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/lab/src/dialog.tsx
--rw-r--r--   0        0        0    15382 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/lab/src/index.ts
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/lab/src/sidebar.ts
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/lab/src/svg.d.ts
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/lab/style/code-dark.svg
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/lab/style/code-light.svg
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/lab/style/index.css
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/lab/style/logo.svg
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/.gitignore
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/COPYING.md
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/README.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/hatch_build.py
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/pyproject.toml
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 ipyparallel-8.5.1/PKG-INFO
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.coveragerc
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.eslintignore
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.eslintrc.js
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.flake8
+-rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.mailmap
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.prettierignore
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/asv.conf.json
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/install.json
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/package.json
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/readthedocs.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/tsconfig.eslint.json
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/tsconfig.json
+-rw-r--r--   0        0        0   202459 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/yarn.lock
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.binder/jupyter_config.json
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.binder/postBuild
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.binder/requirements.txt
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/.gitignore
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/asv.conf.json
+-rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/asv_normal.sh
+-rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/asv_quick.sh
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/asv_runner.py
+-rw-r--r--   0        0        0   182323 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/async_benchmark.ipynb
+-rw-r--r--   0        0        0    13159 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/benchmark_result.py
+-rw-r--r--   0        0        0   669564 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/benchmark_results.ipynb
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/cluster_start.py
+-rw-r--r--   0        0        0    79070 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/depth_benchmark.ipynb
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/engines_test.py
+-rwxr-xr-x   0        0        0     5486 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/gcloud_setup.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/instance_setup.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/logger.py
+-rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/profiling_initial_results.ipynb
+-rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/profiling_latest_results.ipynb
+-rw-r--r--   0        0        0   160310 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/push_benchmarks.ipynb
+-rw-r--r--   0        0        0   862420 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/scheduler_benchmarks.ipynb
+-rw-r--r--   0        0        0   147522 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/throughtput_benchmarks.ipynb
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/benchmarks/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/benchmarks/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/benchmarks/testing.py
+-rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/benchmarks/throughput.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/benchmarks/utils.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/explore/control_flow.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/explore/scheduler.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/machine_configs/asv-testing-16.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/machine_configs/asv-testing-32.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/machine_configs/asv-testing-64.json
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/machine_configs/asv-testing-96.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/profiling/__init__.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/profiling/profiling_code.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/profiling/profiling_code_runner.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/profiling/view_profiling_results.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/results/benchmarks.json
+-rw-r--r--   0        0        0    16442 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-04-28/CoalescingBroadcast.json
+-rw-r--r--   0        0        0    32378 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-04-28/CoalescingPush.json
+-rw-r--r--   0        0        0    36602 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-05-12-19-52-58/results.json
+-rw-r--r--   0        0        0    49624 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-05-19-00-04-55/results.json
+-rw-r--r--   0        0        0    70610 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/results/asv_testing-16-2020-04-29-20-02-25/results.json
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/benchmarks/results/asv_testing-16-2020-05-04-17-43/results.json
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ci/slurm/Dockerfile
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ci/slurm/docker-compose.yaml
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ci/slurm/entrypoint.sh
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ci/slurm/slurm.conf
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ci/ssh/Dockerfile
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ci/ssh/docker-compose.yaml
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ci/ssh/ipcluster_config.py
+-rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/Makefile
+-rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/make.bat
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/requirements.txt
+-rw-r--r--   0        0        0    16714 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/changelog.md
+-rw-r--r--   0        0        0    11972 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/conf.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/index.md
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/links.txt
+-rw-r--r--   0        0        0   234426 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/_static/IPyParallel-MPI-Example.png
+-rw-r--r--   0        0        0    69226 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/_static/basic.mp4
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/api/ipyparallel.rst
+-rw-r--r--   0        0        0    26434 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Cluster API.ipynb
+-rw-r--r--   0        0        0   279116 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Data Publication API.ipynb
+-rw-r--r--   0        0        0    19257 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Futures.ipynb
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Index.ipynb
+-rw-r--r--   0        0        0    67353 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Monitoring an MPI Simulation - 1.ipynb
+-rw-r--r--   0        0        0    62592 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Monitoring an MPI Simulation - 2.ipynb
+-rw-r--r--   0        0        0   165516 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Monte Carlo Options.ipynb
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Parallel Decorator and map.ipynb
+-rw-r--r--   0        0        0  3554371 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Parallel Magics.ipynb
+-rw-r--r--   0        0        0    27919 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Using Dill.ipynb
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/Using MPI with IPython Parallel.ipynb
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/customresults.py
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/dagdeps.py
+-rw-r--r--   0        0        0    42291 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/dask.ipynb
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/dependencies.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/fetchparse.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/iopubwatcher.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/itermapresult.py
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/joblib.ipynb
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/nwmerge.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/phistogram.py
+-rw-r--r--   0        0        0    48362 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/progress.ipynb
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/task_mod.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/task_profiler.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/throughput.py
+-rw-r--r--   0        0        0   329806 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/visualizing-tasks.ipynb
+-rw-r--r--   0        0        0   439979 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/broadcast/Broadcast view.ipynb
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/broadcast/Dockerfile
+-rw-r--r--   0        0        0    69566 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/broadcast/MPI Broadcast.ipynb
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/broadcast/docker-compose.yaml
+-rw-r--r--   0        0        0    84423 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/broadcast/memmap Broadcast.ipynb
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/daVinci Word Count/pwordfreq.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/daVinci Word Count/wordfreq.py
+-rw-r--r--   0        0        0     6923 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/interengine/bintree.py
+-rwxr-xr-x   0        0        0     2823 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/interengine/bintree_script.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/interengine/communicator.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/interengine/interengine.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/pi/parallelpi.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/pi/pidigits.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/rmt/rmt.ipy
+-rw-r--r--   0        0        0    45443 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/rmt/rmt.ipynb
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/rmt/rmtkernel.py
+-rwxr-xr-x   0        0        0    19532 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/wave2D/RectPartitioner.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/wave2D/communicator.py
+-rwxr-xr-x   0        0        0     7226 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/wave2D/parallelwave-mpi.py
+-rwxr-xr-x   0        0        0     7405 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/wave2D/parallelwave.py
+-rwxr-xr-x   0        0        0    11642 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/examples/wave2D/wavesolver.py
+-rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/connections.md
+-rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/dag_dependencies.md
+-rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/db.md
+-rw-r--r--   0        0        0    21297 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/details.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/index.md
+-rw-r--r--   0        0        0     6196 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/launchers.md
+-rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/messages.md
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/mpi.md
+-rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/security.md
+-rw-r--r--   0        0        0    32144 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/allconnections.png
+-rw-r--r--   0        0        0   303213 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/allconnections.svg
+-rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/dagdeps.pdf
+-rw-r--r--   0        0        0   202436 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/dagdeps.png
+-rw-r--r--   0        0        0   153577 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/frontend-kernel.png
+-rw-r--r--   0        0        0   283962 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/frontend-kernel.svg
+-rw-r--r--   0        0        0    38554 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/hbfade.png
+-rw-r--r--   0        0        0    39136 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/iopubfade.png
+-rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/ipy_kernel_and_terminal.png
+-rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/ipy_kernel_and_terminal.svg
+-rw-r--r--   0        0        0    23877 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/nbconvert.png
+-rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/nbconvert.svg
+-rw-r--r--   0        0        0    30974 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/notebook_components.png
+-rw-r--r--   0        0        0    24792 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/notebook_components.svg
+-rw-r--r--   0        0        0    37583 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/notiffade.png
+-rw-r--r--   0        0        0    41180 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/other_kernels.png
+-rw-r--r--   0        0        0    14281 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/other_kernels.svg
+-rw-r--r--   0        0        0    38260 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/queryfade.png
+-rw-r--r--   0        0        0    40459 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/queuefade.png
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/simpledag.pdf
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/reference/figs/simpledag.png
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/asyncresult.md
+-rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/demos.md
+-rw-r--r--   0        0        0    23931 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/direct.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/index.md
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/intro.md
+-rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/magics.md
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/process.md
+-rw-r--r--   0        0        0    16512 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/task.md
+-rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/asian_call.pdf
+-rw-r--r--   0        0        0    23681 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/asian_call.png
+-rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/asian_put.pdf
+-rw-r--r--   0        0        0    23108 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/asian_put.png
+-rw-r--r--   0        0        0    48750 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/mec_simple.pdf
+-rw-r--r--   0        0        0    50744 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/mec_simple.png
+-rw-r--r--   0        0        0   128061 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/parallel_pi.pdf
+-rw-r--r--   0        0        0   115825 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/parallel_pi.png
+-rw-r--r--   0        0        0    41799 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/single_digits.pdf
+-rw-r--r--   0        0        0    36727 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/single_digits.png
+-rw-r--r--   0        0        0    74773 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/two_digit_counts.pdf
+-rw-r--r--   0        0        0    73675 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/two_digit_counts.png
+-rw-r--r--   0        0        0    18561 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/docs/source/tutorial/figs/wideView.png
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/__init__.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/_async.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/_version.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/datapub.py
+-rw-r--r--   0        0        0     8108 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/error.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/joblib.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/logger.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/traitlets.py
+-rw-r--r--   0        0        0    23239 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/__init__.py
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/baseapp.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/ipclusterapp.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/ipcontrollerapp.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/ipengineapp.py
+-rwxr-xr-x   0        0        0     2253 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/iploggerapp.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/launcher.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/apps/logwatcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/__init__.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/_joblib.py
+-rw-r--r--   0        0        0    42102 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/asyncresult.py
+-rw-r--r--   0        0        0    91902 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/client.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/futures.py
+-rw-r--r--   0        0        0    18682 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/magics.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/map.py
+-rw-r--r--   0        0        0     9867 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/remotefunction.py
+-rw-r--r--   0        0        0    54129 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/client/view.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/cluster/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/cluster/__main__.py
+-rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/cluster/_winhpcjob.py
+-rwxr-xr-x   0        0        0    23629 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/cluster/app.py
+-rw-r--r--   0        0        0    36537 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/cluster/cluster.py
+-rw-r--r--   0        0        0    84108 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/cluster/launcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/__main__.py
+-rwxr-xr-x   0        0        0    44147 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/app.py
+-rw-r--r--   0        0        0     8820 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/broadcast_scheduler.py
+-rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/dependency.py
+-rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/dictdb.py
+-rwxr-xr-x   0        0        0    10768 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/heartmonitor.py
+-rw-r--r--   0        0        0    55731 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/hub.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/mongodb.py
+-rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/scheduler.py
+-rw-r--r--   0        0        0    14842 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/sqlitedb.py
+-rw-r--r--   0        0        0    27127 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/controller/task_scheduler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/engine/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/engine/__main__.py
+-rwxr-xr-x   0        0        0    33960 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/engine/app.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/engine/datapub.py
+-rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/engine/kernel.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/engine/log.py
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/engine/nanny.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/package.json
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/schemas/ipyparallel-labextension/package.json.orig
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/schemas/ipyparallel-labextension/plugin.json
+-rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/static/114.b63b1cb1deb6ab07694a.js
+-rw-r--r--   0        0        0    25407 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/static/592.2265e4df71d8ba0dbbf6.js
+-rw-r--r--   0        0        0     7758 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/static/remoteEntry.1bb490d7217e637c4abe.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/static/style.js
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/nbextension/__init__.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/nbextension/base.py
+-rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/nbextension/handlers.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/nbextension/install.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/nbextension/static/clusterlist.css
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/nbextension/static/clusterlist.js
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/nbextension/static/main.js
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/serialize/__init__.py
+-rw-r--r--   0        0        0    14863 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/serialize/canning.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/serialize/codeutil.py
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/serialize/serialize.py
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/_test_startup_crash.py
+-rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/clienttest.py
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/conftest.py
+-rw-r--r--   0        0        0     8255 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_apps.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_async.py
+-rw-r--r--   0        0        0    18324 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_asyncresult.py
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_canning.py
+-rw-r--r--   0        0        0    24230 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_client.py
+-rw-r--r--   0        0        0    12282 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_cluster.py
+-rw-r--r--   0        0        0    10702 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_db.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_dependency.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_executor.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_joblib.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_launcher.py
+-rw-r--r--   0        0        0     8908 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_lbview.py
+-rw-r--r--   0        0        0    18314 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_magics.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_mongodb.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_mpi.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_remotefunction.py
+-rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_serialize.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_slurm.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_ssh.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_util.py
+-rw-r--r--   0        0        0    29722 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_view.py
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/ipyparallel/tests/test_view_broadcast.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/jupyter-config/jupyter_notebook_config.d/ipyparallel.json
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/jupyter-config/jupyter_server_config.d/ipyparallel.json
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/jupyter-config/nbconfig/tree.d/ipyparallel.json
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/webpack.config.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/schema/plugin.json
+-rw-r--r--   0        0        0    23367 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/src/clusters.tsx
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/src/commands.ts
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/src/dialog.tsx
+-rw-r--r--   0        0        0    15382 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/src/index.ts
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/src/sidebar.ts
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/src/svg.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/style/code-dark.svg
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/style/code-light.svg
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/style/index.css
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/lab/style/logo.svg
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/.gitignore
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/COPYING.md
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/README.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/hatch_build.py
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 ipyparallel-8.6.0/PKG-INFO
```

### Comparing `ipyparallel-8.5.1/.eslintrc.js` & `ipyparallel-8.6.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/.flake8` & `ipyparallel-8.6.0/.flake8`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/.mailmap` & `ipyparallel-8.6.0/.mailmap`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/.pre-commit-config.yaml` & `ipyparallel-8.6.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         exclude: setupbase.py
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
         exclude: setupbase.py
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         exclude: setupbase.py
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v3.0.0-alpha.6
     hooks:
       - id: prettier
@@ -31,15 +31,15 @@
     rev: v4.4.0
     hooks:
       - id: end-of-file-fixer
       - id: check-case-conflict
       - id: check-executables-have-shebangs
       - id: requirements-txt-fixer
   - repo: https://github.com/pre-commit/mirrors-eslint
-    rev: v8.35.0
+    rev: v8.37.0
     hooks:
       - id: eslint
         files: \.[jt]sx?$ # *.js, *.jsx, *.ts and *.tsx
         exclude: ipyparallel/nbextension/.*
         types: [file]
         additional_dependencies:
           - "@typescript-eslint/eslint-plugin@2.27.0"
```

### Comparing `ipyparallel-8.5.1/CONTRIBUTING.md` & `ipyparallel-8.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/package.json` & `ipyparallel-8.6.0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9699675324675324%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/notebook': '^3.6.3', '@jupyterlab/settingregistry': '^3.6.3'}",*

 * * "'devDependencies'": "{'eslint': '^8.37.0'}",*

 * * "'version'": "'8.6.0'"}*

```diff
@@ -7,17 +7,17 @@
         "@jupyterlab/application": "^3.0.0",
         "@jupyterlab/apputils": "^3.0.0",
         "@jupyterlab/codeeditor": "^3.0.0",
         "@jupyterlab/console": "^3.0.0",
         "@jupyterlab/coreutils": "^5.0.0",
         "@jupyterlab/mainmenu": "^3.0.0",
         "@jupyterlab/nbformat": "^3.0.0",
-        "@jupyterlab/notebook": "^3.0.0",
+        "@jupyterlab/notebook": "^3.6.3",
         "@jupyterlab/services": "^6.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0",
+        "@jupyterlab/settingregistry": "^3.6.3",
         "@jupyterlab/statedb": "^3.0.0",
         "@jupyterlab/ui-components": "^3.0.0",
         "@lumino/algorithm": "^1.3.3",
         "@lumino/coreutils": "^1.5.3",
         "@lumino/domutils": "^1.2.3",
         "@lumino/dragdrop": "^1.7.1",
         "@lumino/messaging": "^1.4.3",
@@ -30,15 +30,15 @@
     "description": "A JupyterLab extension for IPython Parallel.",
     "devDependencies": {
         "@jupyterlab/builder": "^3.1.10",
         "@types/react": "~17.0.0",
         "@types/react-dom": "~17.0.0",
         "@typescript-eslint/eslint-plugin": "^5.18.0",
         "@typescript-eslint/parser": "^5.18.0",
-        "eslint": "^8.12.0",
+        "eslint": "^8.37.0",
         "eslint-config-prettier": "^8.5.0",
         "eslint-plugin-prettier": "^4.0.0",
         "eslint-plugin-react": "^7.21.5",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "typescript": "~4.3.5",
@@ -91,9 +91,9 @@
         "prettier:check": "prettier --list-different '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lab/lib/index.d.ts",
-    "version": "8.5.1"
+    "version": "8.6.0"
 }
```

### Comparing `ipyparallel-8.5.1/tsconfig.json` & `ipyparallel-8.6.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/yarn.lock` & `ipyparallel-8.6.0/yarn.lock`

 * *Files 3% similar despite different names*

```diff
@@ -62,33 +62,33 @@
     eslint-visitor-keys "^3.3.0"
 
 "@eslint-community/regexpp@^4.4.0":
   version "4.4.0"
   resolved "https://registry.yarnpkg.com/@eslint-community/regexpp/-/regexpp-4.4.0.tgz#3e61c564fcd6b921cb789838631c5ee44df09403"
   integrity sha512-A9983Q0LnDGdLPjxyXQ00sbV+K+O+ko2Dr+CZigbHWtX9pNfxlaBkMR8X1CztI73zuEyEBXTVjx7CE+/VSwDiQ==
 
-"@eslint/eslintrc@^2.0.1":
-  version "2.0.1"
-  resolved "https://registry.yarnpkg.com/@eslint/eslintrc/-/eslintrc-2.0.1.tgz#7888fe7ec8f21bc26d646dbd2c11cd776e21192d"
-  integrity sha512-eFRmABvW2E5Ho6f5fHLqgena46rOj7r7OKHYfLElqcBfGFHHpjBhivyi5+jOEQuSpdc/1phIZJlbC2te+tZNIw==
+"@eslint/eslintrc@^2.0.2":
+  version "2.0.2"
+  resolved "https://registry.yarnpkg.com/@eslint/eslintrc/-/eslintrc-2.0.2.tgz#01575e38707add677cf73ca1589abba8da899a02"
+  integrity sha512-3W4f5tDUra+pA+FzgugqL2pRimUTDJWKr7BINqOpkZrC0uYI0NIc0/JFgBROCU07HR6GieA5m3/rsPIhDmCXTQ==
   dependencies:
     ajv "^6.12.4"
     debug "^4.3.2"
-    espree "^9.5.0"
+    espree "^9.5.1"
     globals "^13.19.0"
     ignore "^5.2.0"
     import-fresh "^3.2.1"
     js-yaml "^4.1.0"
     minimatch "^3.1.2"
     strip-json-comments "^3.1.1"
 
-"@eslint/js@8.36.0":
-  version "8.36.0"
-  resolved "https://registry.yarnpkg.com/@eslint/js/-/js-8.36.0.tgz#9837f768c03a1e4a30bd304a64fb8844f0e72efe"
-  integrity sha512-lxJ9R5ygVm8ZWgYdUweoq5ownDlJ4upvoWmO4eLxBYHdMo+vZ/Rx0EN6MbKWDJOSUGrqJy2Gt+Dyv/VKml0fjg==
+"@eslint/js@8.37.0":
+  version "8.37.0"
+  resolved "https://registry.yarnpkg.com/@eslint/js/-/js-8.37.0.tgz#cf1b5fa24217fe007f6487a26d765274925efa7d"
+  integrity sha512-x5vzdtOOGgFVDCUs81QRB2+liax8rFg3+7hqM+QhBG0/G3F1ZsoYl97UrqgHgQ9KKT7G6c4V+aTUCgu/n22v1A==
 
 "@fortawesome/fontawesome-free@^5.12.0":
   version "5.15.4"
   resolved "https://registry.yarnpkg.com/@fortawesome/fontawesome-free/-/fontawesome-free-5.15.4.tgz#ecda5712b61ac852c760d8b3c79c96adca5554e5"
   integrity sha512-eYm8vijH/hpzr/6/1CJ/V/Eb1xQFW2nnUKArb3z+yUWv7HTwj6M7SP957oMjfZjAHU6qpoNc2wQvIxBLWYa/Jg==
 
 "@gar/promisify@^1.0.1":
@@ -164,15 +164,15 @@
     "@jridgewell/sourcemap-codec" "1.4.14"
 
 "@juggle/resize-observer@^3.3.1":
   version "3.4.0"
   resolved "https://registry.yarnpkg.com/@juggle/resize-observer/-/resize-observer-3.4.0.tgz#08d6c5e20cf7e4cc02fd181c4b0c225cd31dbb60"
   integrity sha512-dfLbk+PwWvFzSxwk3n5ySL0hfBog779o8h68wK/7/APo/7cgyWp5jcXockbxdk5kFRkbeXWm4Fbi9FrdN381sA==
 
-"@jupyter/ydoc@~0.2.0":
+"@jupyter/ydoc@~0.2.3":
   version "0.2.3"
   resolved "https://registry.yarnpkg.com/@jupyter/ydoc/-/ydoc-0.2.3.tgz#468a88d0250c5d59800a5cc15a33df211b4b2141"
   integrity sha512-mwmlzOYXr4StXL1ijrSkt6+Bu4cF5nZQAep2zULa5IDe/PVDBqDtMrLqZyKQOgB3IT/sLJidU1P3wTdb8bwmww==
   dependencies:
     "@jupyterlab/nbformat" "^3.0.0 || ^4.0.0-alpha.15"
     "@lumino/coreutils" "^1.11.0 || ^2.0.0-alpha.6"
     "@lumino/disposable" "^1.10.0 || ^2.0.0-alpha.6"
@@ -202,52 +202,52 @@
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.37.1"
 
-"@jupyterlab/apputils@^3.0.0", "@jupyterlab/apputils@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/apputils/-/apputils-3.6.1.tgz#c547886300e67c5eea0b9ee349e6e1acb0576e64"
-  integrity sha512-/kvncjPLuBnq8unPEVxI/iwUVCVPFw9bmpnYenOdoAlbdrDD8nJwsiFi4xpk1d4VittPZ6vJaAMvXA0X2QGYlQ==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/settingregistry" "^3.6.1"
-    "@jupyterlab/statedb" "^3.6.1"
-    "@jupyterlab/translation" "^3.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+"@jupyterlab/apputils@^3.0.0", "@jupyterlab/apputils@^3.6.1", "@jupyterlab/apputils@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/apputils/-/apputils-3.6.3.tgz#bc37683142b281e21d22a2f4698634563658298e"
+  integrity sha512-um2Aaa5fOUwHFpAqKTDA+MFpnAldzOILIi5QsKOWRxiJA2W8x+hlg5HvHbq+eSWuWEU3ah15M7htzBcL3g9d4Q==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/settingregistry" "^3.6.3"
+    "@jupyterlab/statedb" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     "@types/react" "^17.0.0"
     react "^17.0.1"
     react-dom "^17.0.1"
     sanitize-html "~2.7.3"
     url "^0.11.0"
 
-"@jupyterlab/attachments@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/attachments/-/attachments-3.6.1.tgz#af3b3baa0f4150d412a874121b15029e9761c3a8"
-  integrity sha512-0RA8H0pR3apvqHmkzuFJcJrNXXVDa5GG2Y2Nb5QDtOj+IFRMxEa/8Q4rXtiC7p+fDIgKC/B8xa4CTQlfDCEjaw==
-  dependencies:
-    "@jupyterlab/nbformat" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/rendermime" "^3.6.1"
-    "@jupyterlab/rendermime-interfaces" "^3.6.1"
+"@jupyterlab/attachments@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/attachments/-/attachments-3.6.3.tgz#f2e52c3518d3f84cb7a7cc7c8a113f49dfdde4f1"
+  integrity sha512-ZYDJjcoExmojsGkX5f1WVFfW39XJcb7CtfzFcNz3AbytebRK13S1xqCRlef/TFW+XT6BG7hjMSJlpW3GdkCV1Q==
+  dependencies:
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/rendermime-interfaces" "^3.6.3"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
 
 "@jupyterlab/builder@^3.1.10":
   version "3.6.1"
   resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-3.6.1.tgz#a04bf0312e8679d1f452c27fee2554ba4a6af3f5"
   integrity sha512-LvHQe6InEXJisEcvAdvSFbEEl8OhTjxBSNz7MrjRB+Ur+Qs898dg8QhDH9Ad5mgK3uh4nEN1BDq9W7C/NomqoA==
@@ -284,82 +284,82 @@
     to-string-loader "^1.1.6"
     url-loader "~4.1.0"
     webpack "^5.41.1"
     webpack-cli "^4.1.0"
     webpack-merge "^5.1.2"
     worker-loader "^3.0.2"
 
-"@jupyterlab/cells@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/cells/-/cells-3.6.1.tgz#84c4a43cb66e94a934bcf25172b6ded64d87bba6"
-  integrity sha512-Ojep4Sw83c4uzYSDMQcECW7wuan/dkerimKkb/5cm277ryHL51IgjZTEpJKaW8AeEjNxtAwjlo4cl/5KIwKvQw==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.0"
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/attachments" "^3.6.1"
-    "@jupyterlab/codeeditor" "^3.6.1"
-    "@jupyterlab/codemirror" "^3.6.1"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/filebrowser" "^3.6.1"
-    "@jupyterlab/nbformat" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/outputarea" "^3.6.1"
-    "@jupyterlab/rendermime" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+"@jupyterlab/cells@^3.6.1", "@jupyterlab/cells@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/cells/-/cells-3.6.3.tgz#ac8191f99923a004211725435d25280347794cff"
+  integrity sha512-o3Uydof6bZ6HGSRgSm6isuAhaqYVmv+ozsmADYNmIGbwwwC+eb391Cv+rC3kuPZX/+2UhhO6s7fqFxW8aHUDkg==
+  dependencies:
+    "@jupyter/ydoc" "~0.2.3"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/attachments" "^3.6.3"
+    "@jupyterlab/codeeditor" "^3.6.3"
+    "@jupyterlab/codemirror" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/filebrowser" "^3.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/outputarea" "^3.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     marked "^4.0.17"
     react "^17.0.1"
 
-"@jupyterlab/codeeditor@^3.0.0", "@jupyterlab/codeeditor@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/codeeditor/-/codeeditor-3.6.1.tgz#9643e9f4f594f6cc3f02a2d5a192d8e2bc844284"
-  integrity sha512-KIALB/PHY9LheZ0zGYMHnDGVUO5xReiG+u0Gb+658xYET148a/pU4kp47GzTYB2bsQRrmOmtMqda1/Nhn/c0xw==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.0"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/nbformat" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/translation" "^3.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+"@jupyterlab/codeeditor@^3.0.0", "@jupyterlab/codeeditor@^3.6.1", "@jupyterlab/codeeditor@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/codeeditor/-/codeeditor-3.6.3.tgz#a889c1821001888af7b60f66b1ee91e15797c0bb"
+  integrity sha512-SnVo5KDhyRkK/o1SDRX9nehLEAMaOBFf+GUx2jeXBTfr6wTKcwDBnJAUwlOfncwRlMV79aUIqTIcS861FSXDyA==
+  dependencies:
+    "@jupyter/ydoc" "~0.2.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/codemirror@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/codemirror/-/codemirror-3.6.1.tgz#e21134b02d8ae5b6d971549a689b8462987d30c7"
-  integrity sha512-hEjdAm1bSsBNuzjhnCJrphVdl8HZSGh/+q2MioyF7zRK+VbFarx7DKoYdAtaunHu5MkYA9NGf7mjLVyg17dK9g==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.0"
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/codeeditor" "^3.6.1"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/nbformat" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/statusbar" "^3.6.1"
-    "@jupyterlab/translation" "^3.6.1"
+"@jupyterlab/codemirror@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/codemirror/-/codemirror-3.6.3.tgz#7cb19faae58d4fc26bc37064f029c4b17098c20a"
+  integrity sha512-VU5bInzSqsyPGZkEd/w6HtJ9PSw7U5twoyrQSpSM+E2SEYWskaBZOHJf8XNunVoRRKwSvDLyxSs07Ot6zUlA0w==
+  dependencies:
+    "@jupyter/ydoc" "~0.2.3"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/codeeditor" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/statusbar" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     codemirror "~5.61.0"
     react "^17.0.1"
     y-codemirror "^3.0.1"
 
 "@jupyterlab/console@^3.0.0":
   version "3.6.1"
   resolved "https://registry.yarnpkg.com/@jupyterlab/console/-/console-3.6.1.tgz#15f46a43a02813c18182c682827b8a6e4d33d3f3"
@@ -379,111 +379,112 @@
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.37.1"
 
-"@jupyterlab/coreutils@^5.0.0", "@jupyterlab/coreutils@^5.6.1":
-  version "5.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/coreutils/-/coreutils-5.6.1.tgz#da6c2fe28298ffcad09f1ec5ad4202bdaf1c07c8"
-  integrity sha512-nS4ixC9H53lFzdszOfZfDhlM2hlXfOtQAn6TnA/0Ra/gTBQ+LEbFIWdAp588iKuv8eKX39O/Us53T4oq24A31g==
+"@jupyterlab/coreutils@^5.0.0", "@jupyterlab/coreutils@^5.6.1", "@jupyterlab/coreutils@^5.6.3":
+  version "5.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/coreutils/-/coreutils-5.6.3.tgz#3b0b5d481b14596158b560336833c89be509e84e"
+  integrity sha512-jRVTpwGzP9wBNYuaZTip89FS1qbeSYrEO2qdNVdW2rs0mQHcIlu3Fkv5muMFmKYGi0XHhG3UhZiWQ7qiPw2svQ==
   dependencies:
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     minimist "~1.2.0"
     moment "^2.24.0"
     path-browserify "^1.0.0"
     url-parse "~1.5.1"
 
-"@jupyterlab/docmanager@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/docmanager/-/docmanager-3.6.1.tgz#2f62aabb9dc3f8007f5f54b61473274f784b1972"
-  integrity sha512-olDFoXq2H6TsnCk4OMJus4PcmXCtc2uewZy66XcLD7igDxKvQ50h9uF2wnrxohlgvXxZV9HTMyDyLD7layt82g==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/docprovider" "^3.6.1"
-    "@jupyterlab/docregistry" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/statusbar" "^3.6.1"
-    "@jupyterlab/translation" "^3.6.1"
+"@jupyterlab/docmanager@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/docmanager/-/docmanager-3.6.3.tgz#df2c5b45c5e9b38e2a48eb703ff5e3a9b4b7860c"
+  integrity sha512-4d5zGE3SGbg58wsFJtyskUxK7dEvl8d5Wh90hTlmsFNmr+nh5duTWcqTQ/a+d76YxYbGhH5vqOsNm5ORZq4Umw==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/docprovider" "^3.6.3"
+    "@jupyterlab/docregistry" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/statusbar" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     react "^17.0.1"
 
-"@jupyterlab/docprovider@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/docprovider/-/docprovider-3.6.1.tgz#8be66a419d595b490d6ca3f79238fd160d1cd53e"
-  integrity sha512-YeqLMPlC2jEWBvxgIVfhxbeYXWKb5DGEkv+WJp11S6oFgSNqAHZ1zqH1BB/+UgYWwwkafADwAjepaGFhnr2pPw==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.0"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/services" "^6.6.1"
+"@jupyterlab/docprovider@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/docprovider/-/docprovider-3.6.3.tgz#90fbf07214b6c3e98055787fc351a68e9d83470c"
+  integrity sha512-M5IoyykDpWnUFNePHz3+fi/RNvV92UNbQGfAvsaCMSn+fl48rD4rHB9EZGceOisb3m1U+E4SntKYI3pl49yUEg==
+  dependencies:
+    "@jupyter/ydoc" "~0.2.3"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     y-protocols "^1.0.5"
-    y-websocket "^1.3.15"
-    yjs "^13.5.17"
+    y-websocket "^1.4.6"
 
-"@jupyterlab/docregistry@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/docregistry/-/docregistry-3.6.1.tgz#942b76ea7c59ab9ee375dce4a7bb9377d28d7f61"
-  integrity sha512-uQsmw1LpvcRC8CZ/cjmFnQKB+E+kWqJQDGwtzBDjZm4UcADVs1mwvSwPpAZvTBb0gmYBcS09mTZt7WgVv1Nj8A==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.0"
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/codeeditor" "^3.6.1"
-    "@jupyterlab/codemirror" "^3.6.1"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/docprovider" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/rendermime" "^3.6.1"
-    "@jupyterlab/rendermime-interfaces" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/translation" "^3.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+"@jupyterlab/docregistry@^3.6.1", "@jupyterlab/docregistry@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/docregistry/-/docregistry-3.6.3.tgz#4a03fbb704449bda7a94df7a4bd63078c11aef58"
+  integrity sha512-unDMrtCSGKPqX9uvYCkI7zGTvskuC9odAPIHPsYSVMcHL/o5M7lQkHmRZCoSIezfe5OvPGXbYT2boQrBKXqCFw==
+  dependencies:
+    "@jupyter/ydoc" "~0.2.3"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/codeeditor" "^3.6.3"
+    "@jupyterlab/codemirror" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/docprovider" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/rendermime-interfaces" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/filebrowser@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/filebrowser/-/filebrowser-3.6.1.tgz#8fe44d03545fd9318fe8014edd5c4ddbf705bcb5"
-  integrity sha512-brd5PQQ1m9HK+53opahoi6SaEO0oweRloE1GJEA9t9CHKklpiZ18/3QXF+WDgHtV2UU3ZDmND7Fq5YCets2lBg==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/docmanager" "^3.6.1"
-    "@jupyterlab/docregistry" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/statedb" "^3.6.1"
-    "@jupyterlab/statusbar" "^3.6.1"
-    "@jupyterlab/translation" "^3.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+"@jupyterlab/filebrowser@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/filebrowser/-/filebrowser-3.6.3.tgz#169b880e19a8686f9a669a750027c2817b4b6cef"
+  integrity sha512-Qu+Mtx3d0QY7qCMIxg5nQtkQYh+kZ2kGO7tgS+yfKjo0cluPsxo+Zr56KtJU6zyDYjylVCtLYIK2RflwRKhdng==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/docmanager" "^3.6.3"
+    "@jupyterlab/docregistry" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/statedb" "^3.6.3"
+    "@jupyterlab/statusbar" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     react "^17.0.1"
 
 "@jupyterlab/mainmenu@^3.0.0":
   version "3.6.1"
   resolved "https://registry.yarnpkg.com/@jupyterlab/mainmenu/-/mainmenu-3.6.1.tgz#aa7ea5364566adef08453bfa645d62e347d09455"
   integrity sha512-wZqFNHC8DKRNl6rKMIZZWE//ZG9YbYyQ+sX4UOPqA4mg8fmQX90V57+vqV76d0dgivSQffO06CktKhnhD6J94Q==
   dependencies:
@@ -492,200 +493,209 @@
     "@jupyterlab/translation" "^3.6.1"
     "@jupyterlab/ui-components" "^3.6.1"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/widgets" "^1.37.1"
 
-"@jupyterlab/nbformat@^3.0.0", "@jupyterlab/nbformat@^3.0.0 || ^4.0.0-alpha.15", "@jupyterlab/nbformat@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.1.tgz#84f1239ff0a54d693beed21534aef1baeaa93518"
-  integrity sha512-fLJTAwnQZ/5H9dBV/noqlkbGmGBbcsgd0FHWyMVIq+efKFX6CW1MOk61uM76rfahkke3XgYgvlXsw7i7lEIhcA==
+"@jupyterlab/nbformat@^3.0.0", "@jupyterlab/nbformat@^3.0.0 || ^4.0.0-alpha.15", "@jupyterlab/nbformat@^3.6.1", "@jupyterlab/nbformat@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.3.tgz#8520338e3679cbe8ce2ea8eb5a9b816f8b774ad3"
+  integrity sha512-0qJLa4dtOmu9EmHFeM7gaZi4qheovIPc9ZrgGGRuG0obajs4YYlvh4MQvCSgpVhme4AuBfGlcfzhlx+Gbzr5Xw==
   dependencies:
     "@lumino/coreutils" "^1.11.0"
 
-"@jupyterlab/notebook@^3.0.0":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/notebook/-/notebook-3.6.1.tgz#9bb7d78c694f403b1b5d59889737e56c787348d2"
-  integrity sha512-wkc0/HcnLhYSMtF1y5pf2ngvuhU0UE6tmIjCWl4rP0aC4aAjZZzkRNXV4EwNfY73fLT4EGB149l8Jv4vKUVGdQ==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.0"
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/cells" "^3.6.1"
-    "@jupyterlab/codeeditor" "^3.6.1"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/docregistry" "^3.6.1"
-    "@jupyterlab/nbformat" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/rendermime" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/settingregistry" "^3.6.1"
-    "@jupyterlab/statusbar" "^3.6.1"
-    "@jupyterlab/translation" "^3.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+"@jupyterlab/notebook@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/notebook/-/notebook-3.6.3.tgz#1584be72184d67d59291e2b22f55bc257afde436"
+  integrity sha512-id1KD5/9IDPr/IZFCl/YX4Vc+Q198LZshhFNEcVJZcRdjD7Vh+LGvWcLOh80OAv86J4XSTTAsp3gHPr4iSwPDg==
+  dependencies:
+    "@jupyter/ydoc" "~0.2.3"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/cells" "^3.6.3"
+    "@jupyterlab/codeeditor" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/docregistry" "^3.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/settingregistry" "^3.6.3"
+    "@jupyterlab/statusbar" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     react "^17.0.1"
 
-"@jupyterlab/observables@^4.6.1":
-  version "4.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/observables/-/observables-4.6.1.tgz#7d05b60192e85732db29de5f9e8525798a08aee6"
-  integrity sha512-ez+fxyE3qwQ9grZ0nj2fpgcPIGySs/cNfojfcQatziV2rbFZzrBJJsWFSBhPO55vJd1Mue21aPw1eEK3ok4Wfw==
+"@jupyterlab/observables@^4.6.1", "@jupyterlab/observables@^4.6.3":
+  version "4.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/observables/-/observables-4.6.3.tgz#49a9ca49fbda7428abbd1bfb8a4006ecd406c18d"
+  integrity sha512-CvQoL+9WHXOy/CXp/PQLi4c5iZVJ4psz11+GrycDDinX1AdVQ8a43OLTC0gxWl3Tk2C8ZvAi1sgn4FS68E1ACQ==
   dependencies:
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
 
-"@jupyterlab/outputarea@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/outputarea/-/outputarea-3.6.1.tgz#904d0933d4e8c4bedb6e4179da8d4b6cfd32630d"
-  integrity sha512-/OWU9LvKeRUk5mzQskhPQtWY6/NIiRy3bzhbFesSJ1+3f+L1pk7mXCHmRxiG6FSw2ujeCV3vO4uFTXGLxoqiAw==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/nbformat" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/rendermime" "^3.6.1"
-    "@jupyterlab/rendermime-interfaces" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
+"@jupyterlab/outputarea@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/outputarea/-/outputarea-3.6.3.tgz#acf7a604eb352109d096d2a9fdd1fbbddbf80af1"
+  integrity sha512-SSmkDWS8MhdXl7+rQoLu/5wJBKTq1YEkxlQcKh1Z0VN4VjYDCA/bKFGjOmKN7wMmoVP/zRmWvUwl/DLJCHx/Tw==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/rendermime-interfaces" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     resize-observer-polyfill "^1.5.1"
 
 "@jupyterlab/rendermime-interfaces@^3.6.1":
   version "3.6.1"
   resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.6.1.tgz#d531a6ba228df83b581aee0df5041f7f9a1b4495"
   integrity sha512-IB0rFBTRpguGbAF/WmNPa//UfXcZLRur5DuSwP5tRz2iUZIu/dAFeLDq3j8NL2POz1+yeXyQSQyp2Xu9w8CrFw==
   dependencies:
     "@jupyterlab/translation" "^3.6.1"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/widgets" "^1.37.1"
 
-"@jupyterlab/rendermime@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime/-/rendermime-3.6.1.tgz#ebeef56293cf83f6aa8eb8f12edcd16c4eaafae7"
-  integrity sha512-v4YHIxSd+0foqyzTaloBPevdYUBgZ4Tk1uuXzTdCVIdceS9MG76UfjBu8EPl86AZI8R2ihlHh01pxpgLX0Smdw==
+"@jupyterlab/rendermime-interfaces@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.6.3.tgz#80009705d5ded65a4b27c4b826b295f40f126902"
+  integrity sha512-VHZVnqB0K1nmoQMOhFGHwvSYMQmxqcOC3wWDRFeUOv8S+tejTYfbrKXPOZJvhdGB52Jn8XNIesXOuNpLhl4HmQ==
   dependencies:
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/codemirror" "^3.6.1"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/nbformat" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/rendermime-interfaces" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/translation" "^3.6.1"
+    "@jupyterlab/translation" "^3.6.3"
+    "@lumino/coreutils" "^1.11.0"
+    "@lumino/widgets" "^1.37.2"
+
+"@jupyterlab/rendermime@^3.6.1", "@jupyterlab/rendermime@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime/-/rendermime-3.6.3.tgz#48d83c70493b0356d4dac6d89a863d8a5a84f68e"
+  integrity sha512-w3e38OddJin9fbfe7EWsKiiup/0ayvHPrAsacde8PqGLvi/sLeAXT98PqihsKt8EAlOgXSkSO0Ivjbd0JzgGgA==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/codemirror" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/rendermime-interfaces" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     lodash.escape "^4.0.1"
     marked "^4.0.17"
 
-"@jupyterlab/services@^6.0.0", "@jupyterlab/services@^6.6.1":
-  version "6.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/services/-/services-6.6.1.tgz#5fd96574bb1eee2e4217a6d039b4dcdeb51bb66f"
-  integrity sha512-4YIwTsfx7+JO7Lz9YFTpUvniA3aHdR5dDQJfdo9TsCMxs+NDVfjNAvp9VHa1xNJWYll4Ay31lYWbvuN/SI+KEA==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/nbformat" "^3.6.1"
-    "@jupyterlab/observables" "^4.6.1"
-    "@jupyterlab/settingregistry" "^3.6.1"
-    "@jupyterlab/statedb" "^3.6.1"
+"@jupyterlab/services@^6.0.0", "@jupyterlab/services@^6.6.1", "@jupyterlab/services@^6.6.3":
+  version "6.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/services/-/services-6.6.3.tgz#303938e5dc5aebce7a86324a64ed89c25c61c9e7"
+  integrity sha512-BxEOMRl9X18T5wY7iV6ZJhARnibFghpD3OruqeSbnGdbRv6XJi8prsRbCQQ6Mf9agvf81B20KmDvYKikPHC0xQ==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/settingregistry" "^3.6.3"
+    "@jupyterlab/statedb" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     node-fetch "^2.6.0"
     ws "^7.4.6"
 
-"@jupyterlab/settingregistry@^3.0.0", "@jupyterlab/settingregistry@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/settingregistry/-/settingregistry-3.6.1.tgz#cd04e64d598598950c64aa99e1fc8a2c962d8c31"
-  integrity sha512-zNCYIK6/oWG6JnhmwRGE/Zvn5Xhj0kovcJgTlOSHGyIiHqLfJA9TzHZDNUDANqqxAg4+H9fYdh1+agi4XWGL8A==
+"@jupyterlab/settingregistry@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/settingregistry/-/settingregistry-3.6.3.tgz#642f8b6449d626821ef13a7e778ae716fa8331c9"
+  integrity sha512-pnzIge0ZC8V63R97HiNroJ0eaPM0DN6x65SStyLuv/K8Qez4XqpOdc0Wfell5ri5mxMvm1qKekuFeTikqSXQKQ==
   dependencies:
-    "@jupyterlab/statedb" "^3.6.1"
+    "@jupyterlab/statedb" "^3.6.3"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     ajv "^6.12.3"
     json5 "^2.1.1"
 
-"@jupyterlab/statedb@^3.0.0", "@jupyterlab/statedb@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/statedb/-/statedb-3.6.1.tgz#3f64bfee22ff7779404835fa87b08c67e66716c3"
-  integrity sha512-6+fGzKUCaWBKX/fZDdXR++WgfvYE+Dv5ma8gkgcHaS2vEup2snkmgZ8fBUJXm5xVpU4KhXjTUb7dafLfG7BL3Q==
+"@jupyterlab/statedb@^3.0.0", "@jupyterlab/statedb@^3.6.1", "@jupyterlab/statedb@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/statedb/-/statedb-3.6.3.tgz#6ba2166af9232c9a185cf0077cf1272f24cc9a69"
+  integrity sha512-A36L+0NN8f0WOES2GdtZjp9uFuC7IBjhKiO/RlKRX5AFjNxoJ9oO3PZtoxJQYPnGBljMqVdRa+m9aYEfvKhYyQ==
   dependencies:
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
 
-"@jupyterlab/statusbar@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/statusbar/-/statusbar-3.6.1.tgz#382c32eb6599973176d5ac0497e4a0c9dfa8df37"
-  integrity sha512-rpQa6G6agR+lu3Djt/YTroQ4W3ZasfGmtmO24IXsm3C5418nPIl2oQeEJTc7OsXRvsdoCoAK7c/Rh9TeyhBhug==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.1"
-    "@jupyterlab/codeeditor" "^3.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/translation" "^3.6.1"
-    "@jupyterlab/ui-components" "^3.6.1"
+"@jupyterlab/statusbar@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/statusbar/-/statusbar-3.6.3.tgz#29c24427a2d6b205349b94583de0ccb8b9435d88"
+  integrity sha512-m59NLR0Zghm53PU6hDzRF4XVORnJx/YRx0svcjj/TGLk8LSffpQbUDBy24dl3tOuChk4D5cCdgeDH1X30TzCaA==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/codeeditor" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     csstype "~3.0.3"
     react "^17.0.1"
     typestyle "^2.0.4"
 
-"@jupyterlab/translation@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/translation/-/translation-3.6.1.tgz#db1380c349f2e8645b58a9eac4986f3f1c6b320b"
-  integrity sha512-+I1zzQnYNVnU9rrr7ceHPexiyMFavfK0t6I3qdgAHQ1TTLsLVQMp5m/T7S2SaJjPK7/GtRml5DgmErRyy5becA==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/services" "^6.6.1"
-    "@jupyterlab/statedb" "^3.6.1"
+"@jupyterlab/translation@^3.6.1", "@jupyterlab/translation@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/translation/-/translation-3.6.3.tgz#3fd95f726316762bc1799a7b7be0243d5465932a"
+  integrity sha512-m+wwBv/hiN5Y6Sb7Ij150ZhPXZdhN5wI8CT3afnzARwKr2Aww5AIURO3upmMwnKaPVQTrWqsS3+7bZS/21JuJA==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/statedb" "^3.6.3"
     "@lumino/coreutils" "^1.11.0"
 
-"@jupyterlab/ui-components@^3.0.0", "@jupyterlab/ui-components@^3.6.1":
-  version "3.6.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/ui-components/-/ui-components-3.6.1.tgz#1e12b23614288a1c45fda50c2d141483b879bebf"
-  integrity sha512-p9wH9iidGuuKSm2yXFGhHs6gzpoBpsHRCiOJw9bmj2PBsDKEGjh65Rh0YBv0d7TD6VVgAwMmokaT01KqjUmY+g==
+"@jupyterlab/ui-components@^3.0.0", "@jupyterlab/ui-components@^3.6.1", "@jupyterlab/ui-components@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/ui-components/-/ui-components-3.6.3.tgz#36555036b383c5d80346f409a7a168d13c9d8c85"
+  integrity sha512-XzseUo2IXclPlYcGxCIz8evjWF+dCBMmbJlvoE5OF29BYBvI5N/DUaTem8bHN5kmQwHIXX6BImHu7rbC9Xjl6w==
   dependencies:
     "@blueprintjs/core" "^3.36.0"
     "@blueprintjs/select" "^3.15.0"
-    "@jupyterlab/coreutils" "^5.6.1"
-    "@jupyterlab/translation" "^3.6.1"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     "@rjsf/core" "^3.1.0"
     react "^17.0.1"
     react-dom "^17.0.1"
     typestyle "^2.0.4"
 
 "@lumino/algorithm@^1.3.3", "@lumino/algorithm@^1.9.0", "@lumino/algorithm@^1.9.2":
   version "1.9.2"
@@ -752,18 +762,18 @@
     "@lumino/signaling" "^2.0.0"
 
 "@lumino/domutils@^1.2.3", "@lumino/domutils@^1.8.0", "@lumino/domutils@^1.8.2":
   version "1.8.2"
   resolved "https://registry.yarnpkg.com/@lumino/domutils/-/domutils-1.8.2.tgz#d15cdbae12bea52852bbc13c4629360f9f05b7f5"
   integrity sha512-QIpMfkPJrs4GrWBuJf2Sn1fpyVPmvqUUAeD8xAQo8+4V5JAT0vUDLxZ9HijefMgNCi3+Bs8Z3lQwRCrz+cFP1A==
 
-"@lumino/dragdrop@^1.13.0", "@lumino/dragdrop@^1.14.4", "@lumino/dragdrop@^1.7.1":
-  version "1.14.4"
-  resolved "https://registry.yarnpkg.com/@lumino/dragdrop/-/dragdrop-1.14.4.tgz#b6ec4cf4f470c17a849e31f299d5a24acdc8c7d3"
-  integrity sha512-IHX2M8Yqs2YsFHHXKSKiYLgv9DEuhyyKoDS85Chg34J9OaPC5ocT0AmNVnpeq9T4A50sg3vdL9mSRCZ0f302Gw==
+"@lumino/dragdrop@^1.13.0", "@lumino/dragdrop@^1.14.5", "@lumino/dragdrop@^1.7.1":
+  version "1.14.5"
+  resolved "https://registry.yarnpkg.com/@lumino/dragdrop/-/dragdrop-1.14.5.tgz#1db76c8a01f74cb1b0428db6234e820bb58b93ba"
+  integrity sha512-LC5xB82+xGF8hFyl716TMpV32OIMIMl+s3RU1PaqDkD6B7PkgiVk6NkJ4X9/GcEvl2igkvlGQt/3L7qxDAJNxw==
   dependencies:
     "@lumino/coreutils" "^1.12.1"
     "@lumino/disposable" "^1.10.4"
 
 "@lumino/keyboard@^1.8.2":
   version "1.8.2"
   resolved "https://registry.yarnpkg.com/@lumino/keyboard/-/keyboard-1.8.2.tgz#714dbe671f0718f516d1ec23188b31a9ccd82fb2"
@@ -810,25 +820,25 @@
 "@lumino/virtualdom@^1.14.0", "@lumino/virtualdom@^1.14.3":
   version "1.14.3"
   resolved "https://registry.yarnpkg.com/@lumino/virtualdom/-/virtualdom-1.14.3.tgz#e490c36ff506d877cf45771d6968e3e26a8919fd"
   integrity sha512-5joUC1yuxeXbpfbSBm/OR8Mu9HoTo6PDX0RKqzlJ9o97iml7zayFN/ynzcxScKGQAo9iaXOY8uVIvGUT8FnsGw==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
 
-"@lumino/widgets@^1.17.0", "@lumino/widgets@^1.37.1":
-  version "1.37.1"
-  resolved "https://registry.yarnpkg.com/@lumino/widgets/-/widgets-1.37.1.tgz#d7a2398b276e15e60aff4fec58c035d46549a75b"
-  integrity sha512-/whz5B/hL0fjv0bR8JYZ+Emx+CH7HBwXc4TqI9PrrHGm3g6+jRJAyIFGZcQubqkPxxHrRE/VxQgoDKGhINw/Gw==
+"@lumino/widgets@^1.17.0", "@lumino/widgets@^1.37.1", "@lumino/widgets@^1.37.2":
+  version "1.37.2"
+  resolved "https://registry.yarnpkg.com/@lumino/widgets/-/widgets-1.37.2.tgz#b408fae221ecec2f1b028607782fbe1e82588bce"
+  integrity sha512-NHKu1NBDo6ETBDoNrqSkornfUCwc8EFFzw6+LWBfYVxn2PIwciq2SdiJGEyNqL+0h/A9eVKb5ui5z4cwpRekmQ==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/commands" "^1.21.1"
     "@lumino/coreutils" "^1.12.1"
     "@lumino/disposable" "^1.10.4"
     "@lumino/domutils" "^1.8.2"
-    "@lumino/dragdrop" "^1.14.4"
+    "@lumino/dragdrop" "^1.14.5"
     "@lumino/keyboard" "^1.8.2"
     "@lumino/messaging" "^1.10.3"
     "@lumino/properties" "^1.8.2"
     "@lumino/signaling" "^1.11.1"
     "@lumino/virtualdom" "^1.14.3"
 
 "@nodelib/fs.scandir@2.1.5":
@@ -1939,40 +1949,40 @@
   version "7.1.1"
   resolved "https://registry.yarnpkg.com/eslint-scope/-/eslint-scope-7.1.1.tgz#fff34894c2f65e5226d3041ac480b4513a163642"
   integrity sha512-QKQM/UXpIiHcLqJ5AOyIW7XZmzjkzQXYE54n1++wb0u9V/abW3l9uQnxX8Z5Xd18xyKIMTUAyQ0k1e8pz6LUrw==
   dependencies:
     esrecurse "^4.3.0"
     estraverse "^5.2.0"
 
-eslint-visitor-keys@^3.3.0:
-  version "3.3.0"
-  resolved "https://registry.yarnpkg.com/eslint-visitor-keys/-/eslint-visitor-keys-3.3.0.tgz#f6480fa6b1f30efe2d1968aa8ac745b862469826"
-  integrity sha512-mQ+suqKJVyeuwGYHAdjMFqjCyfl8+Ldnxuyp3ldiMBFKkvytrXUZWaiPCEav8qDHKty44bD+qV1IP4T+w+xXRA==
+eslint-visitor-keys@^3.3.0, eslint-visitor-keys@^3.4.0:
+  version "3.4.0"
+  resolved "https://registry.yarnpkg.com/eslint-visitor-keys/-/eslint-visitor-keys-3.4.0.tgz#c7f0f956124ce677047ddbc192a68f999454dedc"
+  integrity sha512-HPpKPUBQcAsZOsHAFwTtIKcYlCje62XB7SEAcxjtmW6TD1WVpkS6i6/hOVtTZIl4zGj/mBqpFVGvaDneik+VoQ==
 
-eslint@^8.12.0:
-  version "8.36.0"
-  resolved "https://registry.yarnpkg.com/eslint/-/eslint-8.36.0.tgz#1bd72202200a5492f91803b113fb8a83b11285cf"
-  integrity sha512-Y956lmS7vDqomxlaaQAHVmeb4tNMp2FWIvU/RnU5BD3IKMD/MJPr76xdyr68P8tV1iNMvN2mRK0yy3c+UjL+bw==
+eslint@^8.37.0:
+  version "8.37.0"
+  resolved "https://registry.yarnpkg.com/eslint/-/eslint-8.37.0.tgz#1f660ef2ce49a0bfdec0b0d698e0b8b627287412"
+  integrity sha512-NU3Ps9nI05GUoVMxcZx1J8CNR6xOvUT4jAUMH5+z8lpp3aEdPVCImKw6PWG4PY+Vfkpr+jvMpxs/qoE7wq0sPw==
   dependencies:
     "@eslint-community/eslint-utils" "^4.2.0"
     "@eslint-community/regexpp" "^4.4.0"
-    "@eslint/eslintrc" "^2.0.1"
-    "@eslint/js" "8.36.0"
+    "@eslint/eslintrc" "^2.0.2"
+    "@eslint/js" "8.37.0"
     "@humanwhocodes/config-array" "^0.11.8"
     "@humanwhocodes/module-importer" "^1.0.1"
     "@nodelib/fs.walk" "^1.2.8"
     ajv "^6.10.0"
     chalk "^4.0.0"
     cross-spawn "^7.0.2"
     debug "^4.3.2"
     doctrine "^3.0.0"
     escape-string-regexp "^4.0.0"
     eslint-scope "^7.1.1"
-    eslint-visitor-keys "^3.3.0"
-    espree "^9.5.0"
+    eslint-visitor-keys "^3.4.0"
+    espree "^9.5.1"
     esquery "^1.4.2"
     esutils "^2.0.2"
     fast-deep-equal "^3.1.3"
     file-entry-cache "^6.0.1"
     find-up "^5.0.0"
     glob-parent "^6.0.2"
     globals "^13.19.0"
@@ -1990,22 +2000,22 @@
     minimatch "^3.1.2"
     natural-compare "^1.4.0"
     optionator "^0.9.1"
     strip-ansi "^6.0.1"
     strip-json-comments "^3.1.0"
     text-table "^0.2.0"
 
-espree@^9.5.0:
-  version "9.5.0"
-  resolved "https://registry.yarnpkg.com/espree/-/espree-9.5.0.tgz#3646d4e3f58907464edba852fa047e6a27bdf113"
-  integrity sha512-JPbJGhKc47++oo4JkEoTe2wjy4fmMwvFpgJT9cQzmfXKp22Dr6Hf1tdCteLz1h0P3t+mGvWZ+4Uankvh8+c6zw==
+espree@^9.5.1:
+  version "9.5.1"
+  resolved "https://registry.yarnpkg.com/espree/-/espree-9.5.1.tgz#4f26a4d5f18905bf4f2e0bd99002aab807e96dd4"
+  integrity sha512-5yxtHSZXRSW5pvv3hAlXM5+/Oswi1AUFqBmbibKb5s6bp3rGIDkyXU6xCoyuuLhijr4SFwPrXRoZjz0AZDN9tg==
   dependencies:
     acorn "^8.8.0"
     acorn-jsx "^5.3.2"
-    eslint-visitor-keys "^3.3.0"
+    eslint-visitor-keys "^3.4.0"
 
 esquery@^1.4.2:
   version "1.5.0"
   resolved "https://registry.yarnpkg.com/esquery/-/esquery-1.5.0.tgz#6ce17738de8577694edd7361c57182ac8cb0db0b"
   integrity sha512-YQLXUplAwJgCydQ78IMJywZCceoqk1oH01OERdSAJc/7U2AylwjhSCLDEtqwg811idIS/9fIU5GjG73IgjKMVg==
   dependencies:
     estraverse "^5.1.0"
@@ -4408,15 +4418,15 @@
 y-protocols@^1.0.5:
   version "1.0.5"
   resolved "https://registry.yarnpkg.com/y-protocols/-/y-protocols-1.0.5.tgz#91d574250060b29fcac8f8eb5e276fbad594245e"
   integrity sha512-Wil92b7cGk712lRHDqS4T90IczF6RkcvCwAD0A2OPg+adKmOe+nOiT/N2hvpQIWS3zfjmtL4CPaH5sIW1Hkm/A==
   dependencies:
     lib0 "^0.2.42"
 
-y-websocket@^1.3.15:
+y-websocket@^1.4.6:
   version "1.5.0"
   resolved "https://registry.yarnpkg.com/y-websocket/-/y-websocket-1.5.0.tgz#3c13ed205f1553185e1d144eac94150b5b5d55d6"
   integrity sha512-A8AO6XtnQlYwWFytWdkDCeXg4l8ghRTIw5h2YUgUYDmEC9ugWGIwYNW80yadhSFAF7CvuWTEkQNEpevnH6EiZw==
   dependencies:
     lib0 "^0.2.52"
     lodash.debounce "^4.0.8"
     y-protocols "^1.0.5"
@@ -4430,15 +4440,15 @@
   integrity sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==
 
 yarn@^1.22.0:
   version "1.22.19"
   resolved "https://registry.yarnpkg.com/yarn/-/yarn-1.22.19.tgz#4ba7fc5c6e704fce2066ecbfb0b0d8976fe62447"
   integrity sha512-/0V5q0WbslqnwP91tirOvldvYISzaqhClxzyUKXYxs07yUILIs5jx/k6CFe8bvKSkds5w+eiOqta39Wk3WxdcQ==
 
-yjs@^13.5.17, yjs@^13.5.40:
+yjs@^13.5.40:
   version "13.5.50"
   resolved "https://registry.yarnpkg.com/yjs/-/yjs-13.5.50.tgz#ab0605c677922163c9fe49295d3fd47c04c8e0e9"
   integrity sha512-Q2KVNfovwjtJV4Yxz+HaFYT6vTYBaFagOSpTL3jbPc7Sbv/My68fLTfPlYy9FmNO87pV8dMBd5XuVar+9WsAWg==
   dependencies:
     lib0 "^0.2.49"
 
 yocto-queue@^0.1.0:
```

### Comparing `ipyparallel-8.5.1/.binder/postBuild` & `ipyparallel-8.6.0/.binder/postBuild`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/.github/workflows/release.yml` & `ipyparallel-8.6.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/.github/workflows/test.yml` & `ipyparallel-8.6.0/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
       - name: Install ipyparallel itself
         run: |
           pip install --upgrade pip
           pip install --no-deps .
 
       - name: Install Python dependencies
         run: |
-          pip install --pre --upgrade ipyparallel[test] codecov
+          pip install --pre --upgrade ipyparallel[test]
 
       - name: Install extra Python packages
         if: ${{ ! startsWith(matrix.python, '3.11') }}
         run: |
           pip install distributed joblib
           pip install --only-binary :all: matplotlib || echo "no matplotlib"
 
@@ -150,16 +150,15 @@
       - name: Fixup coverage permissions ${{ matrix.container }}
         if: ${{ matrix.container }}
         run: |
           ls -l .coverage*
           ${EXEC} chmod -R a+rw .coverage*
 
       - name: Submit codecov report
-        run: |
-          codecov
+        uses: codecov/codecov-action@v3
 
       - name: Report on slurm
         if: ${{ matrix.cluster_type == 'slurm' && failure() }}
         run: |
           set -x
           docker ps -a
           docker logs slurmctld
```

### Comparing `ipyparallel-8.5.1/benchmarks/asv_runner.py` & `ipyparallel-8.6.0/benchmarks/asv_runner.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/async_benchmark.ipynb` & `ipyparallel-8.6.0/benchmarks/async_benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/benchmark_result.py` & `ipyparallel-8.6.0/benchmarks/benchmark_result.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/benchmark_results.ipynb` & `ipyparallel-8.6.0/benchmarks/benchmark_results.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/cluster_start.py` & `ipyparallel-8.6.0/benchmarks/cluster_start.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/depth_benchmark.ipynb` & `ipyparallel-8.6.0/benchmarks/depth_benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/gcloud_setup.py` & `ipyparallel-8.6.0/benchmarks/gcloud_setup.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/instance_setup.py` & `ipyparallel-8.6.0/benchmarks/instance_setup.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/logger.py` & `ipyparallel-8.6.0/benchmarks/logger.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/profiling_initial_results.ipynb` & `ipyparallel-8.6.0/benchmarks/profiling_initial_results.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/profiling_latest_results.ipynb` & `ipyparallel-8.6.0/benchmarks/profiling_latest_results.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/push_benchmarks.ipynb` & `ipyparallel-8.6.0/benchmarks/push_benchmarks.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/scheduler_benchmarks.ipynb` & `ipyparallel-8.6.0/benchmarks/scheduler_benchmarks.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/throughtput_benchmarks.ipynb` & `ipyparallel-8.6.0/benchmarks/throughtput_benchmarks.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/benchmarks/throughput.py` & `ipyparallel-8.6.0/benchmarks/benchmarks/throughput.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/benchmarks/utils.py` & `ipyparallel-8.6.0/benchmarks/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/explore/control_flow.py` & `ipyparallel-8.6.0/benchmarks/explore/control_flow.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/profiling/profiling_code.py` & `ipyparallel-8.6.0/benchmarks/profiling/profiling_code.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/profiling/profiling_code_runner.py` & `ipyparallel-8.6.0/benchmarks/profiling/profiling_code_runner.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/profiling/view_profiling_results.py` & `ipyparallel-8.6.0/benchmarks/profiling/view_profiling_results.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/results/benchmarks.json` & `ipyparallel-8.6.0/benchmarks/results/benchmarks.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/results/asv-testing-64-2020-04-28/CoalescingBroadcast.json` & `ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-04-28/CoalescingBroadcast.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/results/asv-testing-64-2020-04-28/CoalescingPush.json` & `ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-04-28/CoalescingPush.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/results/asv-testing-64-2020-05-12-19-52-58/results.json` & `ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-05-12-19-52-58/results.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/results/asv-testing-64-2020-05-19-00-04-55/results.json` & `ipyparallel-8.6.0/benchmarks/results/asv-testing-64-2020-05-19-00-04-55/results.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/results/asv_testing-16-2020-04-29-20-02-25/results.json` & `ipyparallel-8.6.0/benchmarks/results/asv_testing-16-2020-04-29-20-02-25/results.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/benchmarks/results/asv_testing-16-2020-05-04-17-43/results.json` & `ipyparallel-8.6.0/benchmarks/results/asv_testing-16-2020-05-04-17-43/results.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ci/slurm/Dockerfile` & `ipyparallel-8.6.0/ci/slurm/Dockerfile`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ci/slurm/docker-compose.yaml` & `ipyparallel-8.6.0/ci/slurm/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ci/slurm/slurm.conf` & `ipyparallel-8.6.0/ci/slurm/slurm.conf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ci/ssh/Dockerfile` & `ipyparallel-8.6.0/ci/ssh/Dockerfile`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ci/ssh/ipcluster_config.py` & `ipyparallel-8.6.0/ci/ssh/ipcluster_config.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/Makefile` & `ipyparallel-8.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/make.bat` & `ipyparallel-8.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/changelog.md` & `ipyparallel-8.6.0/docs/source/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 (changelog)=
 
 # Changelog
 
 Changes in IPython Parallel
 
+## 8.6
+
+### 8.6.0
+
+A tiny release fixing issues seen building notebooks with jupyter-book.
+
+([full changelog](https://github.com/ipython/ipyparallel/compare/8.5.1...8.6.0))
+
+- Fix KeyError on parent_header when streaming output with %%px
+- Allow disabling streaming/progress defaults with IPP_NONINTERACTIVE=1 environment variable (e.g. when building notebooks in documentation)
+
 ## 8.5
 
 ### 8.5.1
 
 A tiny bugfix release
 
 ([full changelog](https://github.com/ipython/ipyparallel/compare/8.5.0...8.5.1))
```

### Comparing `ipyparallel-8.5.1/docs/source/conf.py` & `ipyparallel-8.6.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     'sphinx.ext.doctest',
     'sphinx.ext.inheritance_diagram',
     'sphinx.ext.intersphinx',
     'sphinx.ext.napoleon',
     'myst_parser',
     'nbsphinx',
     'IPython.sphinxext.ipython_console_highlighting',
+    'autodoc_traits',
 ]
 
 myst_enable_extensions = [
     'colon_fence',
     'deflist',
 ]
 
@@ -102,15 +103,15 @@
 release = iprelease['__version__']
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
```

### Comparing `ipyparallel-8.5.1/docs/source/index.md` & `ipyparallel-8.6.0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/links.txt` & `ipyparallel-8.6.0/docs/source/links.txt`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/_static/IPyParallel-MPI-Example.png` & `ipyparallel-8.6.0/docs/source/_static/IPyParallel-MPI-Example.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/_static/basic.mp4` & `ipyparallel-8.6.0/docs/source/_static/basic.mp4`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/api/ipyparallel.rst` & `ipyparallel-8.6.0/docs/source/api/ipyparallel.rst`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The IPython parallel version as a tuple of integers.
     There will always be 3 integers. Development releases will have 'dev' as a fourth element.
 
 Classes
 -------
 
-.. autoclass:: Cluster
+.. autoconfigurable:: Cluster
     :inherited-members:
 
 .. autoclass:: Client
     :inherited-members:
 
 .. autoclass:: DirectView
     :inherited-members:
```

### Comparing `ipyparallel-8.5.1/docs/source/examples/Cluster API.ipynb` & `ipyparallel-8.6.0/docs/source/examples/Cluster API.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/Data Publication API.ipynb` & `ipyparallel-8.6.0/docs/source/examples/Data Publication API.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/Futures.ipynb` & `ipyparallel-8.6.0/docs/source/examples/Futures.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/Index.ipynb` & `ipyparallel-8.6.0/docs/source/examples/Index.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/Monitoring an MPI Simulation - 1.ipynb` & `ipyparallel-8.6.0/docs/source/examples/Monitoring an MPI Simulation - 1.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/Monitoring an MPI Simulation - 2.ipynb` & `ipyparallel-8.6.0/docs/source/examples/Monitoring an MPI Simulation - 2.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/Monte Carlo Options.ipynb` & `ipyparallel-8.6.0/docs/source/examples/Monte Carlo Options.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/Parallel Decorator and map.ipynb` & `ipyparallel-8.6.0/docs/source/examples/Parallel Decorator and map.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/Parallel Magics.ipynb` & `ipyparallel-8.6.0/docs/source/examples/Parallel Magics.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/Using Dill.ipynb` & `ipyparallel-8.6.0/docs/source/examples/Using Dill.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/Using MPI with IPython Parallel.ipynb` & `ipyparallel-8.6.0/docs/source/examples/Using MPI with IPython Parallel.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/customresults.py` & `ipyparallel-8.6.0/docs/source/examples/customresults.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/dagdeps.py` & `ipyparallel-8.6.0/docs/source/examples/dagdeps.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/dask.ipynb` & `ipyparallel-8.6.0/docs/source/examples/dask.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/dependencies.py` & `ipyparallel-8.6.0/docs/source/examples/dependencies.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/fetchparse.py` & `ipyparallel-8.6.0/docs/source/examples/fetchparse.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/iopubwatcher.py` & `ipyparallel-8.6.0/docs/source/examples/iopubwatcher.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/itermapresult.py` & `ipyparallel-8.6.0/docs/source/examples/itermapresult.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/joblib.ipynb` & `ipyparallel-8.6.0/docs/source/examples/joblib.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/nwmerge.py` & `ipyparallel-8.6.0/docs/source/examples/nwmerge.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/phistogram.py` & `ipyparallel-8.6.0/docs/source/examples/phistogram.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/progress.ipynb` & `ipyparallel-8.6.0/docs/source/examples/progress.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/task_profiler.py` & `ipyparallel-8.6.0/docs/source/examples/task_profiler.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/throughput.py` & `ipyparallel-8.6.0/docs/source/examples/throughput.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/visualizing-tasks.ipynb` & `ipyparallel-8.6.0/docs/source/examples/visualizing-tasks.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/broadcast/Broadcast view.ipynb` & `ipyparallel-8.6.0/docs/source/examples/broadcast/Broadcast view.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/broadcast/MPI Broadcast.ipynb` & `ipyparallel-8.6.0/docs/source/examples/broadcast/MPI Broadcast.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/broadcast/docker-compose.yaml` & `ipyparallel-8.6.0/docs/source/examples/broadcast/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/broadcast/memmap Broadcast.ipynb` & `ipyparallel-8.6.0/docs/source/examples/broadcast/memmap Broadcast.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/daVinci Word Count/pwordfreq.py` & `ipyparallel-8.6.0/docs/source/examples/daVinci Word Count/pwordfreq.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/daVinci Word Count/wordfreq.py` & `ipyparallel-8.6.0/docs/source/examples/daVinci Word Count/wordfreq.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/interengine/bintree.py` & `ipyparallel-8.6.0/docs/source/examples/interengine/bintree.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/interengine/bintree_script.py` & `ipyparallel-8.6.0/docs/source/examples/interengine/bintree_script.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/interengine/communicator.py` & `ipyparallel-8.6.0/docs/source/examples/interengine/communicator.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/interengine/interengine.py` & `ipyparallel-8.6.0/docs/source/examples/interengine/interengine.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/pi/parallelpi.py` & `ipyparallel-8.6.0/docs/source/examples/pi/parallelpi.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/pi/pidigits.py` & `ipyparallel-8.6.0/docs/source/examples/pi/pidigits.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/rmt/rmt.ipy` & `ipyparallel-8.6.0/docs/source/examples/rmt/rmt.ipy`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/rmt/rmt.ipynb` & `ipyparallel-8.6.0/docs/source/examples/rmt/rmt.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/rmt/rmtkernel.py` & `ipyparallel-8.6.0/docs/source/examples/rmt/rmtkernel.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/wave2D/RectPartitioner.py` & `ipyparallel-8.6.0/docs/source/examples/wave2D/RectPartitioner.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/wave2D/communicator.py` & `ipyparallel-8.6.0/docs/source/examples/wave2D/communicator.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/wave2D/parallelwave-mpi.py` & `ipyparallel-8.6.0/docs/source/examples/wave2D/parallelwave-mpi.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/wave2D/parallelwave.py` & `ipyparallel-8.6.0/docs/source/examples/wave2D/parallelwave.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/examples/wave2D/wavesolver.py` & `ipyparallel-8.6.0/docs/source/examples/wave2D/wavesolver.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/connections.md` & `ipyparallel-8.6.0/docs/source/reference/connections.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/dag_dependencies.md` & `ipyparallel-8.6.0/docs/source/reference/dag_dependencies.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/db.md` & `ipyparallel-8.6.0/docs/source/reference/db.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/details.md` & `ipyparallel-8.6.0/docs/source/reference/details.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/launchers.md` & `ipyparallel-8.6.0/docs/source/reference/launchers.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/messages.md` & `ipyparallel-8.6.0/docs/source/reference/messages.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/mpi.md` & `ipyparallel-8.6.0/docs/source/reference/mpi.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/security.md` & `ipyparallel-8.6.0/docs/source/reference/security.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/allconnections.png` & `ipyparallel-8.6.0/docs/source/reference/figs/allconnections.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/allconnections.svg` & `ipyparallel-8.6.0/docs/source/reference/figs/allconnections.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/dagdeps.pdf` & `ipyparallel-8.6.0/docs/source/reference/figs/dagdeps.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/dagdeps.png` & `ipyparallel-8.6.0/docs/source/reference/figs/dagdeps.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/frontend-kernel.png` & `ipyparallel-8.6.0/docs/source/reference/figs/frontend-kernel.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/frontend-kernel.svg` & `ipyparallel-8.6.0/docs/source/reference/figs/frontend-kernel.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/hbfade.png` & `ipyparallel-8.6.0/docs/source/reference/figs/hbfade.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/iopubfade.png` & `ipyparallel-8.6.0/docs/source/reference/figs/iopubfade.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/ipy_kernel_and_terminal.png` & `ipyparallel-8.6.0/docs/source/reference/figs/ipy_kernel_and_terminal.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/ipy_kernel_and_terminal.svg` & `ipyparallel-8.6.0/docs/source/reference/figs/ipy_kernel_and_terminal.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/nbconvert.png` & `ipyparallel-8.6.0/docs/source/reference/figs/nbconvert.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/nbconvert.svg` & `ipyparallel-8.6.0/docs/source/reference/figs/nbconvert.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/notebook_components.png` & `ipyparallel-8.6.0/docs/source/reference/figs/notebook_components.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/notebook_components.svg` & `ipyparallel-8.6.0/docs/source/reference/figs/notebook_components.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/notiffade.png` & `ipyparallel-8.6.0/docs/source/reference/figs/notiffade.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/other_kernels.png` & `ipyparallel-8.6.0/docs/source/reference/figs/other_kernels.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/other_kernels.svg` & `ipyparallel-8.6.0/docs/source/reference/figs/other_kernels.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/queryfade.png` & `ipyparallel-8.6.0/docs/source/reference/figs/queryfade.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/queuefade.png` & `ipyparallel-8.6.0/docs/source/reference/figs/queuefade.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/simpledag.pdf` & `ipyparallel-8.6.0/docs/source/reference/figs/simpledag.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/reference/figs/simpledag.png` & `ipyparallel-8.6.0/docs/source/reference/figs/simpledag.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/asyncresult.md` & `ipyparallel-8.6.0/docs/source/tutorial/asyncresult.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/demos.md` & `ipyparallel-8.6.0/docs/source/tutorial/demos.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/direct.md` & `ipyparallel-8.6.0/docs/source/tutorial/direct.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/intro.md` & `ipyparallel-8.6.0/docs/source/tutorial/intro.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/magics.md` & `ipyparallel-8.6.0/docs/source/tutorial/magics.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/process.md` & `ipyparallel-8.6.0/docs/source/tutorial/process.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/task.md` & `ipyparallel-8.6.0/docs/source/tutorial/task.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/figs/asian_call.pdf` & `ipyparallel-8.6.0/docs/source/tutorial/figs/asian_call.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/figs/asian_call.png` & `ipyparallel-8.6.0/docs/source/tutorial/figs/asian_call.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/figs/asian_put.pdf` & `ipyparallel-8.6.0/docs/source/tutorial/figs/asian_put.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/figs/asian_put.png` & `ipyparallel-8.6.0/docs/source/tutorial/figs/asian_put.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/figs/mec_simple.pdf` & `ipyparallel-8.6.0/docs/source/tutorial/figs/mec_simple.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/figs/mec_simple.png` & `ipyparallel-8.6.0/docs/source/tutorial/figs/mec_simple.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/figs/parallel_pi.pdf` & `ipyparallel-8.6.0/docs/source/tutorial/figs/parallel_pi.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/figs/parallel_pi.png` & `ipyparallel-8.6.0/docs/source/tutorial/figs/parallel_pi.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/figs/single_digits.pdf` & `ipyparallel-8.6.0/docs/source/tutorial/figs/single_digits.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/figs/single_digits.png` & `ipyparallel-8.6.0/docs/source/tutorial/figs/single_digits.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/figs/two_digit_counts.pdf` & `ipyparallel-8.6.0/docs/source/tutorial/figs/two_digit_counts.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/figs/two_digit_counts.png` & `ipyparallel-8.6.0/docs/source/tutorial/figs/two_digit_counts.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/docs/source/tutorial/figs/wideView.png` & `ipyparallel-8.6.0/docs/source/tutorial/figs/wideView.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/__init__.py` & `ipyparallel-8.6.0/ipyparallel/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The IPython ZMQ-based parallel computing interface."""
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 # export return_when constants
+import os
 from concurrent.futures import ALL_COMPLETED  # noqa
 from concurrent.futures import FIRST_COMPLETED  # noqa
 from concurrent.futures import FIRST_EXCEPTION  # noqa
 
 from traitlets.config.configurable import MultipleInstanceError
 
 from ._version import __version__  # noqa
@@ -96,7 +97,9 @@
     from .nbextension.handlers import load_jupyter_server_extension
 
     return load_jupyter_server_extension(app)
 
 
 # backward-compat
 load_jupyter_server_extension = _load_jupyter_server_extension
+
+_NONINTERACTIVE = os.getenv("IPP_NONINTERACTIVE", "") not in {"", "0"}
```

### Comparing `ipyparallel-8.5.1/ipyparallel/_async.py` & `ipyparallel-8.6.0/ipyparallel/_async.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/_version.py` & `ipyparallel-8.6.0/ipyparallel/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-__version__ = "8.5.1"
+__version__ = "8.6.0"
 
 # matches tbump regex in pyproject.toml
 _version_regex = re.compile(
     r'''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
```

### Comparing `ipyparallel-8.5.1/ipyparallel/error.py` & `ipyparallel-8.6.0/ipyparallel/error.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/joblib.py` & `ipyparallel-8.6.0/ipyparallel/joblib.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/traitlets.py` & `ipyparallel-8.6.0/ipyparallel/traitlets.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/util.py` & `ipyparallel-8.6.0/ipyparallel/util.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/apps/baseapp.py` & `ipyparallel-8.6.0/ipyparallel/apps/baseapp.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/apps/iploggerapp.py` & `ipyparallel-8.6.0/ipyparallel/apps/iploggerapp.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/apps/logwatcher.py` & `ipyparallel-8.6.0/ipyparallel/apps/logwatcher.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/client/_joblib.py` & `ipyparallel-8.6.0/ipyparallel/client/_joblib.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/client/asyncresult.py` & `ipyparallel-8.6.0/ipyparallel/client/asyncresult.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
             in_kernel = False
 
         if msg_type == 'stream':
             msg_content = msg['content']
             stream_name = msg_content['name']
 
             if in_kernel:
-                parent_msg_id = msg['parent_header']['msg_id']
+                parent_msg_id = msg.get('parent_header', {}).get('msg_id', '')
                 display_id = f"{parent_msg_id}-{stream_name}"
                 md = msg_future.output.metadata
                 full_stream = md[stream_name]
                 if display_id in self._already_streamed:
                     update = True
                 else:
                     self._already_streamed[display_id] = True
```

### Comparing `ipyparallel-8.5.1/ipyparallel/client/client.py` & `ipyparallel-8.6.0/ipyparallel/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     Set,
     Unicode,
     default,
 )
 from traitlets.config.configurable import MultipleInstanceError
 from zmq.eventloop.zmqstream import ZMQStream
 
+import ipyparallel as ipp
 from ipyparallel import error, serialize, util
 from ipyparallel.serialize import PrePickled, Reference
 
 from .asyncresult import AsyncHubResult, AsyncResult
 from .futures import MessageFuture, multi_future
 from .view import BroadcastView, DirectView, LoadBalancedView
 
@@ -1498,15 +1499,18 @@
         if timeout >= 0:
             deadline = tic + timeout
         else:
             deadline = None
             seconds_remaining = 1000
 
         if interactive is None:
-            interactive = get_ipython() is not None
+            if ipp._NONINTERACTIVE:
+                interactive = False
+            else:
+                interactive = get_ipython() is not None
 
         if interactive:
             progress_bar = util.progress(
                 widget=widget,
                 initial=len(self.ids),
                 total=n,
                 unit='engine',
```

### Comparing `ipyparallel-8.5.1/ipyparallel/client/futures.py` & `ipyparallel-8.6.0/ipyparallel/client/futures.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/client/magics.py` & `ipyparallel-8.6.0/ipyparallel/client/magics.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 import sys
 from textwrap import dedent
 
 from IPython.core import magic_arguments
 from IPython.core.error import UsageError
 from IPython.core.magic import Magics
 
+import ipyparallel as ipp
+
 from .. import error
 
 # -----------------------------------------------------------------------------
 # Definitions of magic functions for use with IPython
 # -----------------------------------------------------------------------------
 
 
@@ -241,15 +243,15 @@
     # the current view used by the magics:
     view = None
     # last result cache for %pxresult
     last_result = None
     # verbose flag
     verbose = False
     # streaming output flag
-    stream_ouput = True
+    stream_output = not ipp._NONINTERACTIVE
     # seconds to wait before showing progress bar for blocking execution
     progress_after_seconds = 2
     # signal to send to engines on keyboard-interrupt
     signal_on_interrupt = "SIGINT"
 
     def __init__(self, shell, view, suffix=''):
         self.view = view
@@ -295,15 +297,15 @@
         if args.targets:
             self.view.targets = self._eval_target_str(args.targets)
         if args.block is not None:
             self.view.block = args.block
         if args.set_verbose is not None:
             self.verbose = args.set_verbose
         if args.stream is not None:
-            self.stream_ouput = args.stream
+            self.stream_output = args.stream
         if args.signal_on_interrupt is not None:
             self.signal_on_interrupt = self._eval_signal_str(args.signal_on_interrupt)
 
         if args.progress_after_seconds is not None:
             self.progress_after_seconds = args.progress_after_seconds
 
     @magic_arguments.magic_arguments()
@@ -367,15 +369,15 @@
         progress_after=None,
         signal_on_interrupt=None,
     ):
         """implementation used by %px and %%parallel"""
 
         # defaults:
         block = self.view.block if block is None else block
-        stream_output = self.stream_ouput if stream_output is None else stream_output
+        stream_output = self.stream_output if stream_output is None else stream_output
         signal_on_interrupt = (
             self.signal_on_interrupt
             if signal_on_interrupt is None
             else signal_on_interrupt
         )
 
         base = "Parallel" if block else "Async parallel"
```

### Comparing `ipyparallel-8.5.1/ipyparallel/client/map.py` & `ipyparallel-8.6.0/ipyparallel/client/map.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/client/remotefunction.py` & `ipyparallel-8.6.0/ipyparallel/client/remotefunction.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/client/view.py` & `ipyparallel-8.6.0/ipyparallel/client/view.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/cluster/_winhpcjob.py` & `ipyparallel-8.6.0/ipyparallel/cluster/_winhpcjob.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/cluster/app.py` & `ipyparallel-8.6.0/ipyparallel/cluster/app.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/cluster/cluster.py` & `ipyparallel-8.6.0/ipyparallel/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/cluster/launcher.py` & `ipyparallel-8.6.0/ipyparallel/cluster/launcher.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/controller/app.py` & `ipyparallel-8.6.0/ipyparallel/controller/app.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/controller/broadcast_scheduler.py` & `ipyparallel-8.6.0/ipyparallel/controller/broadcast_scheduler.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/controller/dependency.py` & `ipyparallel-8.6.0/ipyparallel/controller/dependency.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/controller/dictdb.py` & `ipyparallel-8.6.0/ipyparallel/controller/dictdb.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/controller/heartmonitor.py` & `ipyparallel-8.6.0/ipyparallel/controller/heartmonitor.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/controller/hub.py` & `ipyparallel-8.6.0/ipyparallel/controller/hub.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/controller/mongodb.py` & `ipyparallel-8.6.0/ipyparallel/controller/mongodb.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/controller/scheduler.py` & `ipyparallel-8.6.0/ipyparallel/controller/scheduler.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/controller/sqlitedb.py` & `ipyparallel-8.6.0/ipyparallel/controller/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/controller/task_scheduler.py` & `ipyparallel-8.6.0/ipyparallel/controller/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/engine/app.py` & `ipyparallel-8.6.0/ipyparallel/engine/app.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/engine/datapub.py` & `ipyparallel-8.6.0/ipyparallel/engine/datapub.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/engine/kernel.py` & `ipyparallel-8.6.0/ipyparallel/engine/kernel.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/engine/log.py` & `ipyparallel-8.6.0/ipyparallel/engine/log.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/engine/nanny.py` & `ipyparallel-8.6.0/ipyparallel/engine/nanny.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/labextension/package.json` & `ipyparallel-8.6.0/ipyparallel/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9692730880230881%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/notebook': '^3.6.3', '@jupyterlab/settingregistry': '^3.6.3'}",*

 * * "'devDependencies'": "{'eslint': '^8.37.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.1bb490d7217e637c4abe.js'}}",*

 * * "'version'": "'8.6.0'"}*

```diff
@@ -7,17 +7,17 @@
         "@jupyterlab/application": "^3.0.0",
         "@jupyterlab/apputils": "^3.0.0",
         "@jupyterlab/codeeditor": "^3.0.0",
         "@jupyterlab/console": "^3.0.0",
         "@jupyterlab/coreutils": "^5.0.0",
         "@jupyterlab/mainmenu": "^3.0.0",
         "@jupyterlab/nbformat": "^3.0.0",
-        "@jupyterlab/notebook": "^3.0.0",
+        "@jupyterlab/notebook": "^3.6.3",
         "@jupyterlab/services": "^6.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0",
+        "@jupyterlab/settingregistry": "^3.6.3",
         "@jupyterlab/statedb": "^3.0.0",
         "@jupyterlab/ui-components": "^3.0.0",
         "@lumino/algorithm": "^1.3.3",
         "@lumino/coreutils": "^1.5.3",
         "@lumino/domutils": "^1.2.3",
         "@lumino/dragdrop": "^1.7.1",
         "@lumino/messaging": "^1.4.3",
@@ -30,15 +30,15 @@
     "description": "A JupyterLab extension for IPython Parallel.",
     "devDependencies": {
         "@jupyterlab/builder": "^3.1.10",
         "@types/react": "~17.0.0",
         "@types/react-dom": "~17.0.0",
         "@typescript-eslint/eslint-plugin": "^5.18.0",
         "@typescript-eslint/parser": "^5.18.0",
-        "eslint": "^8.12.0",
+        "eslint": "^8.37.0",
         "eslint-config-prettier": "^8.5.0",
         "eslint-plugin-prettier": "^4.0.0",
         "eslint-plugin-react": "^7.21.5",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "typescript": "~4.3.5",
@@ -49,15 +49,15 @@
         "lab/schema/*.json",
         "lab/style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/ipython/ipyparallel",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.624aa72a8010f7bdad27.js"
+            "load": "static/remoteEntry.1bb490d7217e637c4abe.js"
         },
         "extension": true,
         "outputDir": "ipyparallel/labextension",
         "schemaDir": "lab/schema",
         "webpackConfig": "lab/webpack.config.js"
     },
     "keywords": [
@@ -95,9 +95,9 @@
         "prettier:check": "prettier --list-different '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lab/lib/index.d.ts",
-    "version": "8.5.1"
+    "version": "8.6.0"
 }
```

### Comparing `ipyparallel-8.5.1/ipyparallel/labextension/schemas/ipyparallel-labextension/package.json.orig` & `ipyparallel-8.6.0/ipyparallel/labextension/schemas/ipyparallel-labextension/package.json.orig`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9699675324675324%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/notebook': '^3.6.3', '@jupyterlab/settingregistry': '^3.6.3'}",*

 * * "'devDependencies'": "{'eslint': '^8.37.0'}",*

 * * "'version'": "'8.6.0'"}*

```diff
@@ -7,17 +7,17 @@
         "@jupyterlab/application": "^3.0.0",
         "@jupyterlab/apputils": "^3.0.0",
         "@jupyterlab/codeeditor": "^3.0.0",
         "@jupyterlab/console": "^3.0.0",
         "@jupyterlab/coreutils": "^5.0.0",
         "@jupyterlab/mainmenu": "^3.0.0",
         "@jupyterlab/nbformat": "^3.0.0",
-        "@jupyterlab/notebook": "^3.0.0",
+        "@jupyterlab/notebook": "^3.6.3",
         "@jupyterlab/services": "^6.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0",
+        "@jupyterlab/settingregistry": "^3.6.3",
         "@jupyterlab/statedb": "^3.0.0",
         "@jupyterlab/ui-components": "^3.0.0",
         "@lumino/algorithm": "^1.3.3",
         "@lumino/coreutils": "^1.5.3",
         "@lumino/domutils": "^1.2.3",
         "@lumino/dragdrop": "^1.7.1",
         "@lumino/messaging": "^1.4.3",
@@ -30,15 +30,15 @@
     "description": "A JupyterLab extension for IPython Parallel.",
     "devDependencies": {
         "@jupyterlab/builder": "^3.1.10",
         "@types/react": "~17.0.0",
         "@types/react-dom": "~17.0.0",
         "@typescript-eslint/eslint-plugin": "^5.18.0",
         "@typescript-eslint/parser": "^5.18.0",
-        "eslint": "^8.12.0",
+        "eslint": "^8.37.0",
         "eslint-config-prettier": "^8.5.0",
         "eslint-plugin-prettier": "^4.0.0",
         "eslint-plugin-react": "^7.21.5",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "typescript": "~4.3.5",
@@ -91,9 +91,9 @@
         "prettier:check": "prettier --list-different '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lab/lib/index.d.ts",
-    "version": "8.5.1"
+    "version": "8.6.0"
 }
```

### Comparing `ipyparallel-8.5.1/ipyparallel/labextension/static/114.b63b1cb1deb6ab07694a.js` & `ipyparallel-8.6.0/ipyparallel/labextension/static/114.b63b1cb1deb6ab07694a.js`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/labextension/static/592.459a013fb5cd633ee1f8.js` & `ipyparallel-8.6.0/ipyparallel/labextension/static/592.2265e4df71d8ba0dbbf6.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,25 +1,25 @@
 (self.webpackChunkipyparallel_labextension = self.webpackChunkipyparallel_labextension || []).push([
     [592], {
         592: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
                 default: () => B
             });
-            var s = n(848),
-                i = n(239),
-                r = n(649),
-                a = n(194),
-                o = n(68),
-                l = n(679),
-                c = n(215),
+            var s = n(142),
+                i = n(687),
+                r = n(282),
+                a = n(38),
+                o = n(933),
+                l = n(123),
+                c = n(502),
                 u = n(840),
-                d = n(431),
-                p = n(884),
-                h = n(613),
+                d = n(832),
+                p = n(33),
+                h = n(820),
                 g = n(918),
                 m = n(526),
                 C = n(520),
                 v = n(694),
                 f = n(358),
                 y = n(271);
             class w extends y.Component {
```

### Comparing `ipyparallel-8.5.1/ipyparallel/labextension/static/remoteEntry.624aa72a8010f7bdad27.js` & `ipyparallel-8.6.0/ipyparallel/labextension/static/remoteEntry.1bb490d7217e637c4abe.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -44,19 +44,19 @@
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
         60: "549e6d23fd01f935aa18",
         114: "b63b1cb1deb6ab07694a",
-        592: "459a013fb5cd633ee1f8"
+        592: "2265e4df71d8ba0dbbf6"
     } [e] + ".js?v=" + {
         60: "549e6d23fd01f935aa18",
         114: "b63b1cb1deb6ab07694a",
-        592: "459a013fb5cd633ee1f8"
+        592: "2265e4df71d8ba0dbbf6"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -108,15 +108,15 @@
                         (!i || !i.loaded && (!n != !i.eager ? n : l > i.from)) && (a[r] = {
                             get: t,
                             from: l,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (i("@lumino/polling", "1.11.4", (() => Promise.all([w.e(114), w.e(60)]).then((() => () => w(114))))), i("ipyparallel-labextension", "8.5.1", (() => Promise.all([w.e(60), w.e(592)]).then((() => () => w(592)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@lumino/polling", "1.11.4", (() => Promise.all([w.e(114), w.e(60)]).then((() => () => w(114))))), i("ipyparallel-labextension", "8.6.0", (() => Promise.all([w.e(60), w.e(592)]).then((() => () => w(592)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -215,33 +215,33 @@
         return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
     })(((e, r, t, n) => (l(e, t), f(r, 0, t, n)))), h = p(((e, r, t, n, a) => {
         var o = r && w.o(r, t) && s(r, t, n);
         return o ? d(o) : a()
     })), v = {}, b = {
         526: () => c("default", "@lumino/coreutils", [1, 1, 11, 0]),
         840: () => c("default", "@lumino/signaling", [1, 1, 10, 0]),
-        68: () => c("default", "@jupyterlab/statedb", [1, 3, 6, 2]),
-        194: () => c("default", "@jupyterlab/settingregistry", [1, 3, 6, 2]),
-        215: () => c("default", "@jupyterlab/ui-components", [1, 3, 6, 2]),
-        239: () => c("default", "@jupyterlab/application", [1, 3, 6, 2]),
+        33: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
+        38: () => c("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
+        123: () => c("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
+        142: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
         271: () => c("default", "react", [1, 17, 0, 1]),
+        282: () => c("default", "@jupyterlab/console", [1, 3, 6, 3]),
         358: () => h("default", "@lumino/polling", [1, 1, 0, 4], (() => w.e(114).then((() => () => w(114))))),
-        431: () => c("default", "@lumino/widgets", [1, 1, 37, 1]),
         456: () => c("default", "react-dom", [1, 17, 0, 1]),
+        502: () => c("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
         520: () => c("default", "@lumino/domutils", [1, 1, 8, 0]),
-        613: () => c("default", "@jupyterlab/services", [1, 6, 6, 2]),
-        649: () => c("default", "@jupyterlab/console", [1, 3, 6, 2]),
-        679: () => c("default", "@jupyterlab/notebook", [1, 3, 6, 2]),
+        687: () => c("default", "@jupyterlab/application", [1, 3, 6, 3]),
         694: () => c("default", "@lumino/dragdrop", [1, 1, 13, 0]),
-        848: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 2]),
-        884: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 2]),
-        918: () => c("default", "@lumino/algorithm", [1, 1, 9, 0])
+        820: () => c("default", "@jupyterlab/services", [1, 6, 6, 3]),
+        832: () => c("default", "@lumino/widgets", [1, 1, 37, 2]),
+        918: () => c("default", "@lumino/algorithm", [1, 1, 9, 0]),
+        933: () => c("default", "@jupyterlab/statedb", [1, 3, 6, 3])
     }, m = {
         60: [526, 840],
-        592: [68, 194, 215, 239, 271, 358, 431, 456, 520, 613, 649, 679, 694, 848, 884, 918]
+        592: [33, 38, 123, 142, 271, 282, 358, 456, 502, 520, 687, 694, 820, 832, 918, 933]
     }, w.f.consumes = (e, r) => {
         w.o(m, e) && m[e].forEach((e => {
             if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
```

### Comparing `ipyparallel-8.5.1/ipyparallel/labextension/static/third-party-licenses.json` & `ipyparallel-8.6.0/ipyparallel/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/nbextension/base.py` & `ipyparallel-8.6.0/ipyparallel/nbextension/base.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/nbextension/handlers.py` & `ipyparallel-8.6.0/ipyparallel/nbextension/handlers.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/nbextension/install.py` & `ipyparallel-8.6.0/ipyparallel/nbextension/install.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/nbextension/static/clusterlist.js` & `ipyparallel-8.6.0/ipyparallel/nbextension/static/clusterlist.js`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/nbextension/static/main.js` & `ipyparallel-8.6.0/ipyparallel/nbextension/static/main.js`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/serialize/__init__.py` & `ipyparallel-8.6.0/ipyparallel/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/serialize/canning.py` & `ipyparallel-8.6.0/ipyparallel/serialize/canning.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/serialize/codeutil.py` & `ipyparallel-8.6.0/ipyparallel/serialize/codeutil.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/serialize/serialize.py` & `ipyparallel-8.6.0/ipyparallel/serialize/serialize.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/__init__.py` & `ipyparallel-8.6.0/ipyparallel/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/clienttest.py` & `ipyparallel-8.6.0/ipyparallel/tests/clienttest.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/conftest.py` & `ipyparallel-8.6.0/ipyparallel/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_apps.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_async.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_asyncresult.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_asyncresult.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_canning.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_canning.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_client.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_cluster.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_db.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_dependency.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_dependency.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_executor.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_joblib.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_joblib.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_launcher.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_lbview.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_lbview.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_magics.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_magics.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_mongodb.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_mpi.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_mpi.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_remotefunction.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_remotefunction.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_serialize.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_slurm.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_slurm.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_ssh.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_ssh.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_util.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_view.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/ipyparallel/tests/test_view_broadcast.py` & `ipyparallel-8.6.0/ipyparallel/tests/test_view_broadcast.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/lab/src/clusters.tsx` & `ipyparallel-8.6.0/lab/src/clusters.tsx`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/lab/src/commands.ts` & `ipyparallel-8.6.0/lab/src/commands.ts`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/lab/src/dialog.tsx` & `ipyparallel-8.6.0/lab/src/dialog.tsx`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/lab/src/index.ts` & `ipyparallel-8.6.0/lab/src/index.ts`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/lab/src/sidebar.ts` & `ipyparallel-8.6.0/lab/src/sidebar.ts`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/lab/style/index.css` & `ipyparallel-8.6.0/lab/style/index.css`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/lab/style/logo.svg` & `ipyparallel-8.6.0/lab/style/logo.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/COPYING.md` & `ipyparallel-8.6.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/README.md` & `ipyparallel-8.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/hatch_build.py` & `ipyparallel-8.6.0/hatch_build.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.5.1/pyproject.toml` & `ipyparallel-8.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "jupyterlab>=3.0.0,==3.*",
   "hatchling>=0.25"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "ipyparallel"
-version = "8.5.1"
+version = "8.6.0"
 authors = [{name = "IPython Development Team", email = "ipython-dev@scipy.org"}]
 license = {file = "COPYING.md"}
 readme = "README.md"
 description = "Interactive Parallel Computing with IPython"
 keywords = [
     "Interactive",
     "Interpreter",
@@ -141,15 +141,15 @@
 ]
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/jupyterhub/jupyterhub"
 
 [tool.tbump.version]
-current = "8.5.1"
+current = "8.6.0"
 
 # pep440 regex
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
```

### Comparing `ipyparallel-8.5.1/PKG-INFO` & `ipyparallel-8.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyparallel
-Version: 8.5.1
+Version: 8.6.0
 Summary: Interactive Parallel Computing with IPython
 Project-URL: Homepage, https://ipython.org
 Author-email: IPython Development Team <ipython-dev@scipy.org>
 License: # Licensing terms
         
         Traitlets is adapted from enthought.traits, Copyright (c) Enthought, Inc.,
         under the terms of the Modified BSD License.
```

