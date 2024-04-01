# Comparing `tmp/parsl-2024.3.4.tar.gz` & `tmp/parsl-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsl-2024.3.4.tar", last modified: Mon Mar  4 22:42:53 2024, max compression
+gzip compressed data, was "parsl-2024.4.1.tar", last modified: Mon Apr  1 22:42:41 2024, max compression
```

## Comparing `parsl-2024.3.4.tar` & `parsl-2024.4.1.tar`

### file list

```diff
@@ -1,527 +1,533 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.390261 parsl-2024.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-04 22:42:46.000000 parsl-2024.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-04 22:42:46.000000 parsl-2024.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-04 22:42:53.390261 parsl-2024.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-03-04 22:42:46.000000 parsl-2024.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.326262 parsl-2024.3.4/parsl/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.326262 parsl-2024.3.4/parsl/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/app/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/app/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/app/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/app/futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/app/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.326262 parsl-2024.3.4/parsl/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/benchmark/perf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.330262 parsl-2024.3.4/parsl/channels/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/channels/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/channels/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.330262 parsl-2024.3.4/parsl/channels/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/channels/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/channels/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.330262 parsl-2024.3.4/parsl/channels/oauth_ssh/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/channels/oauth_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/channels/oauth_ssh/oauth_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.330262 parsl-2024.3.4/parsl/channels/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/channels/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/channels/ssh/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.330262 parsl-2024.3.4/parsl/channels/ssh_il/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/channels/ssh_il/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/channels/ssh_il/ssh_il.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.330262 parsl-2024.3.4/parsl/concurrent/
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/concurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.334262 parsl-2024.3.4/parsl/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/ASPIRE1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/Azure.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/ad_hoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/expanse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/illinoiscluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/osg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/polaris.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/stampede2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/toss3_llnl.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/configs/wqex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/curvezmq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.334262 parsl-2024.3.4/parsl/data_provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/data_provider/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/data_provider/file_noop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/data_provider/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/data_provider/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/data_provider/globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/data_provider/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/data_provider/rsync.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/data_provider/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.334262 parsl-2024.3.4/parsl/dataflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63873 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/dataflow/dflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/dataflow/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/dataflow/futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/dataflow/memoization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/dataflow/rundirs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/dataflow/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/dataflow/taskrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.338262 parsl-2024.3.4/parsl/executors/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.338262 parsl-2024.3.4/parsl/executors/flux/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/flux/execute_parsl_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/flux/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/flux/flux_instance_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.338262 parsl-2024.3.4/parsl/executors/high_throughput/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/high_throughput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/high_throughput/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    36464 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/high_throughput/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30200 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/high_throughput/interchange.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/high_throughput/manager_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/high_throughput/monitoring_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/high_throughput/mpi_prefix_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/high_throughput/mpi_resource_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/high_throughput/probe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    39108 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/high_throughput/process_worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/high_throughput/zmq_pipes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.338262 parsl-2024.3.4/parsl/executors/radical/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/radical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21024 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/radical/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/radical/rpex_master.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/radical/rpex_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/radical/rpex_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10940 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/status_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.342262 parsl-2024.3.4/parsl/executors/taskvine/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/taskvine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/taskvine/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/taskvine/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    31404 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/taskvine/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/taskvine/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/taskvine/factory_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25732 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/taskvine/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/taskvine/manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/taskvine/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.342262 parsl-2024.3.4/parsl/executors/workqueue/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/workqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/workqueue/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/workqueue/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    49107 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/workqueue/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5737 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/workqueue/parsl_coprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      735 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/executors/workqueue/parsl_coprocess_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.342262 parsl-2024.3.4/parsl/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/jobs/error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/jobs/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/jobs/job_status_poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/jobs/states.py
--rw-r--r--   0 runner    (1001) docker     (127)    12926 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/jobs/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.342262 parsl-2024.3.4/parsl/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/launchers/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    15358 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/launchers/launchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.346262 parsl-2024.3.4/parsl/monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36308 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/db_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/message_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    24855 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.346262 parsl-2024.3.4/parsl/monitoring/queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/queries/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/radios.py
--rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.346262 parsl-2024.3.4/parsl/monitoring/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.346262 parsl-2024.3.4/parsl/monitoring/visualization/plots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.346262 parsl-2024.3.4/parsl/monitoring/visualization/plots/default/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/plots/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/plots/default/task_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/plots/default/workflow_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.346262 parsl-2024.3.4/parsl/monitoring/visualization/static/
--rwxr-xr-x   0 runner    (1001) docker     (127)    14199 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/static/parsl-logo-white.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      337 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/static/parsl-monitor.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.346262 parsl-2024.3.4/parsl/monitoring/visualization/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/templates/app.html
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/templates/dag.html
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/templates/resource_usage.html
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/templates/task.html
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/templates/workflow.html
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/templates/workflows_summary.html
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/monitoring/visualization/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/process_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.346262 parsl-2024.3.4/parsl/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.350262 parsl-2024.3.4/parsl/providers/ad_hoc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/ad_hoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/ad_hoc/ad_hoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.350262 parsl-2024.3.4/parsl/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29009 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/aws/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/aws/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.350262 parsl-2024.3.4/parsl/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18396 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/azure/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/azure/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/cluster_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.350262 parsl-2024.3.4/parsl/providers/cobalt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/cobalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/cobalt/cobalt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      273 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/cobalt/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.350262 parsl-2024.3.4/parsl/providers/condor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/condor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/condor/condor.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/condor/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.350262 parsl-2024.3.4/parsl/providers/googlecloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/googlecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8006 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/googlecloud/googlecloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.350262 parsl-2024.3.4/parsl/providers/grid_engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/grid_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/grid_engine/grid_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/grid_engine/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.350262 parsl-2024.3.4/parsl/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/kubernetes/kube.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/kubernetes/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.350262 parsl-2024.3.4/parsl/providers/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.350262 parsl-2024.3.4/parsl/providers/lsf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/lsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/lsf/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/lsf/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.354262 parsl-2024.3.4/parsl/providers/pbspro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/pbspro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/pbspro/pbspro.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/pbspro/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.354262 parsl-2024.3.4/parsl/providers/slurm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13720 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/slurm/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/slurm/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.354262 parsl-2024.3.4/parsl/providers/torque/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/torque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/torque/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/providers/torque/torque.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.354262 parsl-2024.3.4/parsl/serialize/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/serialize/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/serialize/concretes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/serialize/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/serialize/facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/serialize/proxystore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.354262 parsl-2024.3.4/parsl/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/callables_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.362262 parsl-2024.3.4/parsl/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/ad_hoc_cluster_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/azure_single_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/cooley_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/ec2_single_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/ec2_spot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/htex_ad_hoc_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/htex_local_alternate.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/htex_local_intask_staging.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/htex_local_rsync_staging.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/local_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/local_radical.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/local_radical_mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/local_threads_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/local_threads_checkpoint_periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/local_threads_checkpoint_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/local_threads_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/local_threads_globus.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/local_threads_http_in_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/local_threads_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/local_threads_no_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/nscc_singapore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/osg_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/petrelkube.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/swan_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/taskvine_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/user_opts.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/configs/workqueue_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.362262 parsl-2024.3.4/parsl/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/integration/latency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.362262 parsl-2024.3.4/parsl/tests/integration/test_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/integration/test_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.362262 parsl-2024.3.4/parsl/tests/integration/test_channels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/integration/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/integration/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/integration/test_channels/test_local_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/integration/test_channels/test_scp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/integration/test_channels/test_ssh_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/integration/test_channels/test_ssh_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/integration/test_channels/test_ssh_file_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/integration/test_channels/test_ssh_interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/integration/test_parsl_load_default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.362262 parsl-2024.3.4/parsl/tests/integration/test_stress/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/integration/test_stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/integration/test_stress/test_python_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/integration/test_stress/test_python_threads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.362262 parsl-2024.3.4/parsl/tests/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/manual_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/manual_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/manual_tests/test_ad_hoc_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/manual_tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/manual_tests/test_log_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/manual_tests/test_memory_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/manual_tests/test_oauth_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/manual_tests/test_regression_220.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/manual_tests/test_udp_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/manual_tests/test_worker_count.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.366262 parsl-2024.3.4/parsl/tests/scaling_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/scaling_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/scaling_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/scaling_tests/local_threads.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3751 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/scaling_tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/scaling_tests/vineex_condor.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/scaling_tests/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/scaling_tests/wqex_condor.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/scaling_tests/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.366262 parsl-2024.3.4/parsl/tests/site_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/site_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/site_tests/site_config_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/site_tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/site_tests/test_site.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.366262 parsl-2024.3.4/parsl/tests/sites/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/sites/test_affinity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/sites/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/sites/test_dynamic_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/sites/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/sites/test_launchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/sites/test_local_adhoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.366262 parsl-2024.3.4/parsl/tests/sites/test_mpi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/sites/test_mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/sites/test_worker_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_aalst_patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.370262 parsl-2024.3.4/parsl/tests/test_bash_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_bash_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_bash_apps/test_apptimeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_bash_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_bash_apps/test_error_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_bash_apps/test_keyword_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_bash_apps/test_kwarg_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_bash_apps/test_memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_bash_apps/test_multiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_bash_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_bash_apps/test_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_callables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.370262 parsl-2024.3.4/parsl/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_channels/test_large_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.370262 parsl-2024.3.4/parsl/tests/test_checkpointing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_checkpointing/test_periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_checkpointing/test_regression_232.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_checkpointing/test_regression_233.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_checkpointing/test_regression_239.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_checkpointing/test_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_curvezmq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.370262 parsl-2024.3.4/parsl/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_data/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_data/test_file_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_data/test_file_staging.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_data/test_output_chain_filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.370262 parsl-2024.3.4/parsl/tests/test_docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_docs/test_from_slides.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_docs/test_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_docs/test_tutorial_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_docs/test_workflow1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_docs/test_workflow2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_docs/test_workflow4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.374261 parsl-2024.3.4/parsl/tests/test_error_handling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_error_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_error_handling/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_error_handling/test_python_walltime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_error_handling/test_rand_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_error_handling/test_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_error_handling/test_retries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_error_handling/test_retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_error_handling/test_retry_handler_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_error_handling/test_serialization_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_error_handling/test_wrap_with_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.374261 parsl-2024.3.4/parsl/tests/test_flowcontrol/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_flowcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.374261 parsl-2024.3.4/parsl/tests/test_htex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_htex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_htex/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_htex/test_connected_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_htex/test_cpu_affinity_explicit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_htex/test_disconnected_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_htex/test_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_htex/test_manager_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_htex/test_missing_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_htex/test_multiple_disconnected_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_htex/test_worker_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_htex/test_zmq_binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.378261 parsl-2024.3.4/parsl/tests/test_monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_monitoring/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_monitoring/test_db_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_monitoring/test_fuzz_zmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_monitoring/test_incomplete_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_monitoring/test_memoization_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_monitoring/test_viz_colouring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.378261 parsl-2024.3.4/parsl/tests/test_mpi_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_mpi_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_mpi_apps/test_bad_mpi_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_mpi_apps/test_mpi_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_mpi_apps/test_mpi_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_mpi_apps/test_resource_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.378261 parsl-2024.3.4/parsl/tests/test_providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_providers/test_cobalt_deprecation_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_providers/test_local_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_providers/test_pbspro_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_providers/test_slurm_instantiate.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_providers/test_slurm_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_providers/test_submiterror_deprecation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.382261 parsl-2024.3.4/parsl/tests/test_python_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_arg_input_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_dep_standard_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_depfail_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_fibonacci_iterative.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_fibonacci_recursive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_garbage_collect.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_import_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_lifted.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_mapred.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_memoize_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_memoize_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_memoize_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_memoize_joinapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_python_apps/test_type5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.382261 parsl-2024.3.4/parsl/tests/test_radical/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_radical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_radical/test_mpi_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.382261 parsl-2024.3.4/parsl/tests/test_regression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_regression/test_1480.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_regression/test_1653.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_regression/test_221.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_regression/test_226.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_regression/test_2652.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_regression/test_69a.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_regression/test_854.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_regression/test_97_parallelism_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_regression/test_98.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.386261 parsl-2024.3.4/parsl/tests/test_scaling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_scaling/test_block_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_scaling/test_regression_1621.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_scaling/test_scale_down.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.386261 parsl-2024.3.4/parsl/tests/test_serialization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_serialization/test_2555_caching_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_serialization/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_serialization/test_htex_code_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_serialization/test_pack_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_serialization/test_proxystore_configured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_serialization/test_proxystore_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.386261 parsl-2024.3.4/parsl/tests/test_staging/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_staging/staging_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_staging/test_1316.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_staging/test_docs_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_staging/test_docs_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_staging/test_elaborate_noop_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_staging/test_staging_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_staging/test_staging_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_staging/test_staging_globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_staging/test_staging_https.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_thread_parallelism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.386261 parsl-2024.3.4/parsl/tests/test_threads/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_threads/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_threads/test_lazy_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.386261 parsl-2024.3.4/parsl/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/test_utils/test_representation_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.386261 parsl-2024.3.4/parsl/usage_tracking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/usage_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/usage_tracking/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10956 2024-03-04 22:42:46.000000 parsl-2024.3.4/parsl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-04 22:42:51.000000 parsl-2024.3.4/parsl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:42:53.326262 parsl-2024.3.4/parsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-04 22:42:53.000000 parsl-2024.3.4/parsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17639 2024-03-04 22:42:53.000000 parsl-2024.3.4/parsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 22:42:53.000000 parsl-2024.3.4/parsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-04 22:42:53.000000 parsl-2024.3.4/parsl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-04 22:42:53.000000 parsl-2024.3.4/parsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 22:42:53.000000 parsl-2024.3.4/parsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-04 22:42:46.000000 parsl-2024.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 22:42:53.390261 parsl-2024.3.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2868 2024-03-04 22:42:46.000000 parsl-2024.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.171953 parsl-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 22:42:37.000000 parsl-2024.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-01 22:42:37.000000 parsl-2024.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-01 22:42:41.167953 parsl-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-01 22:42:37.000000 parsl-2024.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.107952 parsl-2024.4.1/parsl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.107952 parsl-2024.4.1/parsl/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/app/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/app/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/app/futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/app/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.111952 parsl-2024.4.1/parsl/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/benchmark/perf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.111952 parsl-2024.4.1/parsl/channels/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.111952 parsl-2024.4.1/parsl/channels/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.111952 parsl-2024.4.1/parsl/channels/oauth_ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/oauth_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/oauth_ssh/oauth_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.111952 parsl-2024.4.1/parsl/channels/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.111952 parsl-2024.4.1/parsl/channels/ssh_il/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/ssh_il/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/ssh_il/ssh_il.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.111952 parsl-2024.4.1/parsl/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/concurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.115952 parsl-2024.4.1/parsl/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/ASPIRE1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/Azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/ad_hoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/expanse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/illinoiscluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/osg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/polaris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/stampede2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/toss3_llnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/wqex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/curvezmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.115952 parsl-2024.4.1/parsl/data_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/file_noop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.115952 parsl-2024.4.1/parsl/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63593 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/dflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/rundirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/taskrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.115952 parsl-2024.4.1/parsl/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.119952 parsl-2024.4.1/parsl/executors/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/flux/execute_parsl_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/flux/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/flux/flux_instance_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.119952 parsl-2024.4.1/parsl/executors/high_throughput/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37225 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31491 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/interchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/manager_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/monitoring_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/mpi_prefix_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/mpi_resource_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/probe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41221 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/process_worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/zmq_pipes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.119952 parsl-2024.4.1/parsl/executors/radical/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/radical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21024 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/radical/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/radical/rpex_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/radical/rpex_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/radical/rpex_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/status_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.119952 parsl-2024.4.1/parsl/executors/taskvine/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32531 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/factory_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25822 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.123952 parsl-2024.4.1/parsl/executors/workqueue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/workqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/workqueue/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/workqueue/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50038 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/workqueue/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5737 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/workqueue/parsl_coprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      735 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/workqueue/parsl_coprocess_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.123952 parsl-2024.4.1/parsl/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/jobs/error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/jobs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/jobs/job_status_poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/jobs/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/jobs/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.123952 parsl-2024.4.1/parsl/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/launchers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/launchers/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.123952 parsl-2024.4.1/parsl/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37021 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.123952 parsl-2024.4.1/parsl/monitoring/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/queries/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/radios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13900 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/monitoring/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/monitoring/visualization/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/monitoring/visualization/plots/default/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/plots/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/plots/default/task_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/plots/default/workflow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/monitoring/visualization/static/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14199 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/static/parsl-logo-white.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      337 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/static/parsl-monitor.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/monitoring/visualization/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/app.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/dag.html
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/resource_usage.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/task.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/workflow.html
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/workflows_summary.html
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/process_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/providers/ad_hoc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/ad_hoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/ad_hoc/ad_hoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29009 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/aws/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/aws/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18396 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/azure/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/azure/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/cluster_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/cobalt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/cobalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/cobalt/cobalt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      273 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/cobalt/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/condor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/condor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/condor/condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/condor/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/googlecloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/googlecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8006 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/googlecloud/googlecloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/grid_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/grid_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/grid_engine/grid_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/grid_engine/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/kubernetes/kube.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/kubernetes/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/lsf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/lsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/lsf/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/lsf/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/pbspro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/pbspro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/pbspro/pbspro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/pbspro/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/slurm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/slurm/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/slurm/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/torque/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/torque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/torque/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/torque/torque.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.135952 parsl-2024.4.1/parsl/serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/serialize/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/serialize/concretes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/serialize/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/serialize/facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/serialize/proxystore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.135952 parsl-2024.4.1/parsl/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/callables_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.139953 parsl-2024.4.1/parsl/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/ad_hoc_cluster_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/azure_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/cooley_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/ec2_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/ec2_spot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/htex_ad_hoc_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/htex_local_alternate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/htex_local_intask_staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/htex_local_rsync_staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_radical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_radical_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_checkpoint_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_checkpoint_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_http_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_no_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/nscc_singapore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/osg_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/petrelkube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/swan_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/taskvine_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/user_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/workqueue_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.143952 parsl-2024.4.1/parsl/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/latency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.143952 parsl-2024.4.1/parsl/tests/integration/test_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.143952 parsl-2024.4.1/parsl/tests/integration/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/test_local_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/test_scp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_file_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_parsl_load_default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.143952 parsl-2024.4.1/parsl/tests/integration/test_stress/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_stress/test_python_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_stress/test_python_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.143952 parsl-2024.4.1/parsl/tests/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_ad_hoc_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_memory_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_oauth_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_regression_220.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_udp_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_worker_count.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.147952 parsl-2024.4.1/parsl/tests/scaling_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/local_threads.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3751 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/vineex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/wqex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.147952 parsl-2024.4.1/parsl/tests/site_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/site_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/site_tests/site_config_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/site_tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/site_tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.147952 parsl-2024.4.1/parsl/tests/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_dynamic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_local_adhoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.147952 parsl-2024.4.1/parsl/tests/sites/test_mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_worker_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_aalst_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.151953 parsl-2024.4.1/parsl/tests/test_bash_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_apptimeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_keyword_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_kwarg_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_callables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.151953 parsl-2024.4.1/parsl/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_channels/test_large_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.151953 parsl-2024.4.1/parsl/tests/test_checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_regression_232.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_regression_233.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_regression_239.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_curvezmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.151953 parsl-2024.4.1/parsl/tests/test_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_docs/test_from_slides.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_docs/test_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_docs/test_tutorial_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_docs/test_workflow1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_docs/test_workflow2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_docs/test_workflow4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.151953 parsl-2024.4.1/parsl/tests/test_error_handling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_python_walltime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_rand_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_retry_handler_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_serialization_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_wrap_with_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.155953 parsl-2024.4.1/parsl/tests/test_flowcontrol/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_flowcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.155953 parsl-2024.4.1/parsl/tests/test_htex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_connected_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_cpu_affinity_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_disconnected_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_drain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_manager_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_missing_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_multiple_disconnected_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_worker_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_zmq_binding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.155953 parsl-2024.4.1/parsl/tests/test_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_app_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_db_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_fuzz_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_htex_init_blocks_vs_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_incomplete_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_memoization_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_viz_colouring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.159952 parsl-2024.4.1/parsl/tests/test_mpi_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_mpi_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_mpi_apps/test_bad_mpi_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_mpi_apps/test_resource_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.159952 parsl-2024.4.1/parsl/tests/test_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_providers/test_cobalt_deprecation_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_providers/test_local_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_providers/test_pbspro_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_providers/test_slurm_instantiate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_providers/test_slurm_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_providers/test_submiterror_deprecation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.163953 parsl-2024.4.1/parsl/tests/test_python_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_arg_input_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_dep_standard_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_depfail_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_fibonacci_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_fibonacci_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_garbage_collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_import_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_lifted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_mapred.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_joinapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_type5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.163953 parsl-2024.4.1/parsl/tests/test_radical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_radical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_radical/test_mpi_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.163953 parsl-2024.4.1/parsl/tests/test_regression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_1480.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_1653.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_221.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_226.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_2652.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_69a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_854.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_97_parallelism_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_98.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.163953 parsl-2024.4.1/parsl/tests/test_scaling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_scaling/test_block_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_scaling/test_regression_1621.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_scaling/test_scale_down.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_scaling/test_shutdown_scalein.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.167953 parsl-2024.4.1/parsl/tests/test_serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_serialization/test_2555_caching_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_serialization/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_serialization/test_htex_code_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_serialization/test_pack_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_serialization/test_proxystore_configured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_serialization/test_proxystore_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.167953 parsl-2024.4.1/parsl/tests/test_shutdown/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_shutdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_shutdown/test_kill_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.167953 parsl-2024.4.1/parsl/tests/test_staging/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/staging_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_1316.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_docs_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_docs_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_elaborate_noop_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_file_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_file_staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_output_chain_filenames.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_staging_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_staging_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_staging_globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_staging_https.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_thread_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.167953 parsl-2024.4.1/parsl/tests/test_threads/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_threads/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_threads/test_lazy_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.167953 parsl-2024.4.1/parsl/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_utils/test_representation_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.167953 parsl-2024.4.1/parsl/usage_tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/usage_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/usage_tracking/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 22:42:39.000000 parsl-2024.4.1/parsl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.107952 parsl-2024.4.1/parsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-01 22:42:40.000000 parsl-2024.4.1/parsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17956 2024-04-01 22:42:41.000000 parsl-2024.4.1/parsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:42:40.000000 parsl-2024.4.1/parsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-01 22:42:40.000000 parsl-2024.4.1/parsl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-01 22:42:40.000000 parsl-2024.4.1/parsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 22:42:40.000000 parsl-2024.4.1/parsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-01 22:42:37.000000 parsl-2024.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:42:41.171953 parsl-2024.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2874 2024-04-01 22:42:37.000000 parsl-2024.4.1/setup.py
```

### Comparing `parsl-2024.3.4/LICENSE` & `parsl-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/PKG-INFO` & `parsl-2024.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2024.3.4
+Version: 2024.4.1
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2024.03.04.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2024.04.01.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2024.3.4/README.rst` & `parsl-2024.4.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,18 @@
    :alt: NSF award info
 .. |NSF-1550562| image:: https://img.shields.io/badge/NSF-1550562-blue.svg
    :target: https://nsf.gov/awardsearch/showAward?AWD_ID=1550562
    :alt: NSF award info
 .. |NSF-1550528| image:: https://img.shields.io/badge/NSF-1550528-blue.svg
    :target: https://nsf.gov/awardsearch/showAward?AWD_ID=1550528
    :alt: NSF award info
+.. |NSF-1550475| image:: https://img.shields.io/badge/NSF-1550475-blue.svg
+   :target: https://nsf.gov/awardsearch/showAward?AWD_ID=1550475
+   :alt: NSF award info
+
    
 Quickstart
 ==========
 
 Install Parsl using pip::
 
     $ pip3 install parsl
@@ -89,14 +93,15 @@
 1. Download Parsl::
 
     $ git clone https://github.com/Parsl/parsl
 
 
 2. Build and Test::
 
+    $ cd parsl # navigate to the root directory of the project
     $ make   # show all available makefile targets
     $ make virtualenv # create a virtual environment
     $ source .venv/bin/activate # activate the virtual environment
     $ make deps # install python dependencies from test-requirements.txt
     $ make test # make (all) tests. Run "make config_local_test" for a faster, smaller test set.
     $ make clean # remove virtualenv and all test and build artifacts
 
@@ -111,13 +116,13 @@
 ============
 
 Parsl is supported in Python 3.8+. Requirements can be found `here <requirements.txt>`_. Requirements for running tests can be found `here <test-requirements.txt>`_.
 
 Code of Conduct
 ===============
 
-Parsl seeks to foster an open and welcoming environment - Please see the `Parsl Code of Conduct <https://github.com/Parsl/parsl/blob/master/CoC.md>`_ for more details.
+Parsl seeks to foster an open and welcoming environment - Please see the `Parsl Code of Conduct <https://github.com/Parsl/parsl/blob/master/CODE_OF_CONDUCT.md>`_ for more details.
 
 Contributing
 ============
 
 We welcome contributions from the community. Please see our `contributing guide <https://github.com/Parsl/parsl/blob/master/CONTRIBUTING.rst>`_.
```

### Comparing `parsl-2024.3.4/parsl/__init__.py` & `parsl-2024.4.1/parsl/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/addresses.py` & `parsl-2024.4.1/parsl/addresses.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,17 @@
     return ip_addr
 
 
 @typeguard.typechecked
 def address_by_interface(ifname: str) -> str:
     """Returns the IP address of the given interface name, e.g. 'eth0'
 
-    This is taken from a Stack Overflow answer: https://stackoverflow.com/questions/24196932/how-can-i-get-the-ip-address-of-eth0-in-python#24196955
+    This is taken from a Stack Overflow answer:
+    https://stackoverflow.com/questions/24196932/how-can-i-get-the-ip-address-of-eth0-in-python#24196955
+
 
     Parameters
     ----------
     ifname : str
         Name of the interface whose address is to be returned. Required.
 
     """
```

### Comparing `parsl-2024.3.4/parsl/app/app.py` & `parsl-2024.4.1/parsl/app/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/app/bash.py` & `parsl-2024.4.1/parsl/app/bash.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/app/errors.py` & `parsl-2024.4.1/parsl/app/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/app/futures.py` & `parsl-2024.4.1/parsl/app/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/app/python.py` & `parsl-2024.4.1/parsl/app/python.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/benchmark/perf.py` & `parsl-2024.4.1/parsl/benchmark/perf.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/channels/base.py` & `parsl-2024.4.1/parsl/channels/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/channels/errors.py` & `parsl-2024.4.1/parsl/channels/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/channels/local/local.py` & `parsl-2024.4.1/parsl/channels/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/channels/oauth_ssh/oauth_ssh.py` & `parsl-2024.4.1/parsl/channels/oauth_ssh/oauth_ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/channels/ssh/ssh.py` & `parsl-2024.4.1/parsl/channels/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/channels/ssh_il/ssh_il.py` & `parsl-2024.4.1/parsl/channels/ssh_il/ssh_il.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/concurrent/__init__.py` & `parsl-2024.4.1/parsl/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/config.py` & `parsl-2024.4.1/parsl/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,16 @@
     run_dir : str, optional
         Path to run directory. Default is 'runinfo'.
     strategy : str, optional
         Strategy to use for scaling blocks according to workflow needs. Can be 'simple', 'htex_auto_scale', 'none'
         or `None`.
         If 'none' or `None`, dynamic scaling will be disabled. Default is 'simple'. The literal value `None` is
         deprecated.
+    strategy_period : float or int, optional
+        How often the scaling strategy should be executed. Default is 5 seconds.
     max_idletime : float, optional
         The maximum idle time allowed for an executor before strategy could shut down unused blocks. Default is 120.0 seconds.
     usage_tracking : bool, optional
         Set this field to True to opt-in to Parsl's usage tracking system. Parsl only collects minimal, non personally-identifiable,
         information used for reporting to our funding agencies. Default is False.
     initialize_logging : bool, optional
         Make DFK optionally not initialize any logging. Log messages
@@ -84,14 +86,15 @@
                  checkpoint_period: Optional[str] = None,
                  garbage_collect: bool = True,
                  internal_tasks_max_threads: int = 10,
                  retries: int = 0,
                  retry_handler: Optional[Callable[[Exception, TaskRecord], float]] = None,
                  run_dir: str = 'runinfo',
                  strategy: Optional[str] = 'simple',
+                 strategy_period: Union[float, int] = 5,
                  max_idletime: float = 120.0,
                  monitoring: Optional[MonitoringHub] = None,
                  usage_tracking: bool = False,
                  initialize_logging: bool = True) -> None:
 
         executors = tuple(executors or [])
         if not executors:
@@ -117,14 +120,15 @@
         self.checkpoint_period = checkpoint_period
         self.garbage_collect = garbage_collect
         self.internal_tasks_max_threads = internal_tasks_max_threads
         self.retries = retries
         self.retry_handler = retry_handler
         self.run_dir = run_dir
         self.strategy = strategy
+        self.strategy_period = strategy_period
         self.max_idletime = max_idletime
         self.usage_tracking = usage_tracking
         self.initialize_logging = initialize_logging
         self.monitoring = monitoring
 
     @property
     def executors(self) -> Sequence[ParslExecutor]:
```

### Comparing `parsl-2024.3.4/parsl/configs/ASPIRE1.py` & `parsl-2024.4.1/parsl/configs/ASPIRE1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/Azure.py` & `parsl-2024.4.1/parsl/configs/Azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/ad_hoc.py` & `parsl-2024.4.1/parsl/configs/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/bluewaters.py` & `parsl-2024.4.1/parsl/tests/configs/theta.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 from parsl.config import Config
-from parsl.executors import HighThroughputExecutor
+from parsl.providers import CobaltProvider
 from parsl.launchers import AprunLauncher
-from parsl.providers import TorqueProvider
+from parsl.executors import HighThroughputExecutor
+
+from .user_opts import user_opts
 
 
-config = Config(
-    executors=[
-        HighThroughputExecutor(
-            label="bw_htex",
-            cores_per_worker=1,
-            worker_debug=False,
-            provider=TorqueProvider(
-                queue='normal',
-                launcher=AprunLauncher(overrides="-b -- bwpy-environ --"),
-                scheduler_options='',  # string to prepend to #SBATCH blocks in the submit script to the scheduler
-                worker_init='',  # command to run before starting a worker, such as 'source activate env'
-                init_blocks=1,
-                max_blocks=1,
-                min_blocks=1,
-                nodes_per_block=2,
-                walltime='00:10:00'
-            ),
-        )
+def fresh_config():
+    return Config(
+        executors=[
+            HighThroughputExecutor(
+                label='theta_local_htex_multinode',
+                max_workers_per_node=1,
+                encrypted=True,
+                provider=CobaltProvider(
+                    queue=user_opts['theta']['queue'],
+                    account=user_opts['theta']['account'],
+                    launcher=AprunLauncher(overrides="-d 64"),
+                    walltime='00:10:00',
+                    nodes_per_block=2,
+                    init_blocks=1,
+                    max_blocks=1,
+                    # string to prepend to #COBALT blocks in the submit
+                    # script to the scheduler eg: '#COBALT -t 50'
+                    scheduler_options='',
+                    # Command to be run before starting a worker, such as:
+                    # 'module load Anaconda; source activate parsl_env'.
+                    worker_init=user_opts['theta']['worker_init'],
+                    cmd_timeout=120,
+                ),
+            )
+        ],
+    )
 
-    ],
 
-)
+config = fresh_config()
```

### Comparing `parsl-2024.3.4/parsl/configs/bridges.py` & `parsl-2024.4.1/parsl/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/cc_in2p3.py` & `parsl-2024.4.1/parsl/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/ec2.py` & `parsl-2024.4.1/parsl/configs/ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/expanse.py` & `parsl-2024.4.1/parsl/configs/expanse.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/frontera.py` & `parsl-2024.4.1/parsl/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/illinoiscluster.py` & `parsl-2024.4.1/parsl/configs/illinoiscluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/kubernetes.py` & `parsl-2024.4.1/parsl/configs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/midway.py` & `parsl-2024.4.1/parsl/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/osg.py` & `parsl-2024.4.1/parsl/configs/osg.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/polaris.py` & `parsl-2024.4.1/parsl/configs/polaris.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/stampede2.py` & `parsl-2024.4.1/parsl/configs/stampede2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/summit.py` & `parsl-2024.4.1/parsl/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/toss3_llnl.py` & `parsl-2024.4.1/parsl/configs/toss3_llnl.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/vineex_local.py` & `parsl-2024.4.1/parsl/configs/vineex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/configs/wqex_local.py` & `parsl-2024.4.1/parsl/configs/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/curvezmq.py` & `parsl-2024.4.1/parsl/curvezmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/data_provider/data_manager.py` & `parsl-2024.4.1/parsl/data_provider/data_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/data_provider/files.py` & `parsl-2024.4.1/parsl/data_provider/files.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/data_provider/ftp.py` & `parsl-2024.4.1/parsl/data_provider/ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/data_provider/globus.py` & `parsl-2024.4.1/parsl/data_provider/globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/data_provider/http.py` & `parsl-2024.4.1/parsl/data_provider/http.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/data_provider/rsync.py` & `parsl-2024.4.1/parsl/data_provider/rsync.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/data_provider/staging.py` & `parsl-2024.4.1/parsl/data_provider/staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/dataflow/dflow.py` & `parsl-2024.4.1/parsl/dataflow/dflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,20 +30,20 @@
 from parsl.dataflow.futures import AppFuture
 from parsl.dataflow.memoization import Memoizer
 from parsl.dataflow.rundirs import make_rundir
 from parsl.dataflow.states import States, FINAL_STATES, FINAL_FAILURE_STATES
 from parsl.dataflow.taskrecord import TaskRecord
 from parsl.errors import ConfigurationError, InternalConsistencyError, NoDataFlowKernelError
 from parsl.jobs.job_status_poller import JobStatusPoller
-from parsl.jobs.states import JobStatus, JobState
 from parsl.usage_tracking.usage import UsageTracker
 from parsl.executors.base import ParslExecutor
 from parsl.executors.status_handling import BlockProviderExecutor
 from parsl.executors.threads import ThreadPoolExecutor
 from parsl.monitoring import MonitoringHub
+from parsl.monitoring.remote import monitor_wrapper
 from parsl.process_loggers import wrap_with_logs
 from parsl.providers.base import ExecutionProvider
 from parsl.utils import get_version, get_std_fname_mode, get_all_checkpoints, Timer
 
 from parsl.monitoring.message_type import MessageType
 
 logger = logging.getLogger(__name__)
@@ -91,33 +91,33 @@
         logger.info("Starting DataFlowKernel with config\n{}".format(config))
 
         logger.info("Parsl version: {}".format(get_version()))
 
         self.checkpoint_lock = threading.Lock()
 
         self.usage_tracker = UsageTracker(self)
-        self.usage_tracker.send_message()
+        self.usage_tracker.send_start_message()
 
         self.task_state_counts_lock = threading.Lock()
         self.task_state_counts = {state: 0 for state in States}
 
         # Monitoring
         self.run_id = str(uuid4())
 
         self.monitoring: Optional[MonitoringHub]
         self.monitoring = config.monitoring
 
         # hub address and port for interchange to connect
         self.hub_address = None  # type: Optional[str]
-        self.hub_interchange_port = None  # type: Optional[int]
+        self.hub_zmq_port = None  # type: Optional[int]
         if self.monitoring:
             if self.monitoring.logdir is None:
                 self.monitoring.logdir = self.run_dir
             self.hub_address = self.monitoring.hub_address
-            self.hub_interchange_port = self.monitoring.start(self.run_id, self.run_dir, self.config.run_dir)
+            self.hub_zmq_port = self.monitoring.start(self.run_id, self.run_dir, self.config.run_dir)
 
         self.time_began = datetime.datetime.now()
         self.time_completed: Optional[datetime.datetime] = None
 
         logger.info("Run id is: " + self.run_id)
 
         self.workflow_name = None
@@ -174,14 +174,15 @@
         self._checkpoint_timer = None
         self.checkpoint_mode = config.checkpoint_mode
         self.checkpointable_tasks: List[TaskRecord] = []
 
         # this must be set before executors are added since add_executors calls
         # job_status_poller.add_executors.
         self.job_status_poller = JobStatusPoller(strategy=self.config.strategy,
+                                                 strategy_period=self.config.strategy_period,
                                                  max_idletime=self.config.max_idletime,
                                                  dfk=self)
 
         self.executors: Dict[str, ParslExecutor] = {}
 
         self.data_manager = DataManager(self)
         parsl_internal_executor = ThreadPoolExecutor(max_threads=config.internal_tasks_max_threads, label='_parsl_internal')
@@ -201,14 +202,21 @@
 
         self.task_count = 0
         self.tasks: Dict[int, TaskRecord] = {}
         self.submitter_lock = threading.Lock()
 
         atexit.register(self.atexit_cleanup)
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        logger.debug("Exiting the context manager, calling cleanup for DFK")
+        self.cleanup()
+
     def _send_task_log_info(self, task_record: TaskRecord) -> None:
         if self.monitoring:
             task_log_info = self._create_task_log_info(task_record)
             self.monitoring.send(MessageType.TASK_INFO, task_log_info)
 
     def _create_task_log_info(self, task_record):
         """
@@ -702,39 +710,43 @@
             logger.exception("Task {} requested invalid executor {}: config is\n{}".format(task_id, executor_label, self._config))
             raise ValueError("Task {} requested invalid executor {}".format(task_id, executor_label))
 
         try_id = task_record['fail_count']
 
         if self.monitoring is not None and self.monitoring.resource_monitoring_enabled:
             wrapper_logging_level = logging.DEBUG if self.monitoring.monitoring_debug else logging.INFO
-            (function, args, kwargs) = self.monitoring.monitor_wrapper(function, args, kwargs, try_id, task_id,
-                                                                       self.monitoring.monitoring_hub_url,
-                                                                       self.run_id,
-                                                                       wrapper_logging_level,
-                                                                       self.monitoring.resource_monitoring_interval,
-                                                                       executor.radio_mode,
-                                                                       executor.monitor_resources(),
-                                                                       self.run_dir)
+            (function, args, kwargs) = monitor_wrapper(function, args, kwargs, try_id, task_id,
+                                                       self.monitoring.monitoring_hub_url,
+                                                       self.run_id,
+                                                       wrapper_logging_level,
+                                                       self.monitoring.resource_monitoring_interval,
+                                                       executor.radio_mode,
+                                                       executor.monitor_resources(),
+                                                       self.run_dir)
 
         with self.submitter_lock:
             exec_fu = executor.submit(function, task_record['resource_specification'], *args, **kwargs)
         self.update_task_state(task_record, States.launched)
 
         self._send_task_log_info(task_record)
 
         if hasattr(exec_fu, "parsl_executor_task_id"):
-            logger.info(f"Parsl task {task_id} try {try_id} launched on executor {executor.label} with executor id {exec_fu.parsl_executor_task_id}")
+            logger.info(
+                f"Parsl task {task_id} try {try_id} launched on executor {executor.label} "
+                f"with executor id {exec_fu.parsl_executor_task_id}")
+
         else:
             logger.info(f"Parsl task {task_id} try {try_id} launched on executor {executor.label}")
 
         self._log_std_streams(task_record)
 
         return exec_fu
 
-    def _add_input_deps(self, executor: str, args: Sequence[Any], kwargs: Dict[str, Any], func: Callable) -> Tuple[Sequence[Any], Dict[str, Any], Callable]:
+    def _add_input_deps(self, executor: str, args: Sequence[Any], kwargs: Dict[str, Any], func: Callable) -> Tuple[Sequence[Any], Dict[str, Any],
+                                                                                                                   Callable]:
         """Look for inputs of the app that are files. Give the data manager
         the opportunity to replace a file with a data future for that file,
         for example wrapping the result of a staging action.
 
         Args:
             - executor (str) : executor where the app is going to be launched
             - args (List) : Positional args to app function
@@ -1106,48 +1118,42 @@
                 parent, child = pathlib.Path(run_dir).parts[-2:]
                 remote_run_dir = os.path.join(parent, child)
                 channel.script_dir = os.path.join(remote_run_dir, 'remote_submit_scripts')
                 provider.script_dir = os.path.join(run_dir, 'local_submit_scripts')
 
         channel.makedirs(channel.script_dir, exist_ok=True)
 
-    def add_executors(self, executors):
+    def add_executors(self, executors: Sequence[ParslExecutor]) -> None:
         for executor in executors:
             executor.run_id = self.run_id
             executor.run_dir = self.run_dir
             executor.hub_address = self.hub_address
-            executor.hub_port = self.hub_interchange_port
+            executor.hub_port = self.hub_zmq_port
             if hasattr(executor, 'provider'):
                 if hasattr(executor.provider, 'script_dir'):
                     executor.provider.script_dir = os.path.join(self.run_dir, 'submit_scripts')
                     os.makedirs(executor.provider.script_dir, exist_ok=True)
 
                     if hasattr(executor.provider, 'channels'):
                         logger.debug("Creating script_dir across multiple channels")
                         for channel in executor.provider.channels:
                             self._create_remote_dirs_over_channel(executor.provider, channel)
                     else:
                         self._create_remote_dirs_over_channel(executor.provider, executor.provider.channel)
 
             self.executors[executor.label] = executor
-            block_ids = executor.start()
-            if self.monitoring and block_ids:
-                new_status = {}
-                for bid in block_ids:
-                    new_status[bid] = JobStatus(JobState.PENDING)
-                msg = executor.create_monitoring_info(new_status)
-                logger.debug("Sending monitoring message {} to hub from DFK".format(msg))
-                self.monitoring.send(MessageType.BLOCK_INFO, msg)
+            executor.start()
         block_executors = [e for e in executors if isinstance(e, BlockProviderExecutor)]
         self.job_status_poller.add_executors(block_executors)
 
     def atexit_cleanup(self) -> None:
         if not self.cleanup_called:
-            logger.info("DFK cleanup because python process is exiting")
-            self.cleanup()
+            logger.warning("Python is exiting with a DFK still running. "
+                           "You should call parsl.dfk().cleanup() before "
+                           "exiting to release any resources")
         else:
             logger.info("python process is exiting, but DFK has already been cleaned up")
 
     def wait_for_current_tasks(self) -> None:
         """Waits for all tasks in the task list to be completed, by waiting for their
         AppFuture to be completed. This method will not necessarily wait for any tasks
         added after cleanup has started (such as data stageout?)
@@ -1161,15 +1167,16 @@
         task_records = list(self.tasks.values())
         for task_record in task_records:
             # .exception() is a less exception throwing way of
             # waiting for completion than .result()
             fut = task_record['app_fu']
             if not fut.done():
                 fut.exception()
-            # now app future is done, poll until DFK state is final: a DFK state being final and the app future being done do not imply each other.
+            # now app future is done, poll until DFK state is final: a
+            # DFK state being final and the app future being done do not imply each other.
             while task_record['status'] not in FINAL_STATES:
                 time.sleep(0.1)
 
         logger.info("All remaining tasks completed")
 
     @wrap_with_logs
     def cleanup(self) -> None:
@@ -1196,39 +1203,38 @@
             self.checkpoint()
 
             if self._checkpoint_timer:
                 logger.info("Stopping checkpoint timer")
                 self._checkpoint_timer.close()
 
         # Send final stats
-        self.usage_tracker.send_message()
+        self.usage_tracker.send_end_message()
         self.usage_tracker.close()
 
         logger.info("Closing job status poller")
         self.job_status_poller.close()
         logger.info("Terminated job status poller")
 
         logger.info("Scaling in and shutting down executors")
 
+        for ef in self.job_status_poller._executor_facades:
+            if not ef.executor.bad_state_is_set:
+                logger.info(f"Scaling in executor {ef.executor.label}")
+
+                # this code needs to be at least as many blocks as need
+                # cancelling, but it is safe to be more, as the scaling
+                # code will cope with being asked to cancel more blocks
+                # than exist.
+                block_count = len(ef.status)
+                ef.scale_in(block_count)
+
+            else:  # and bad_state_is_set
+                logger.warning(f"Not scaling in executor {ef.executor.label} because it is in bad state")
+
         for executor in self.executors.values():
-            if isinstance(executor, BlockProviderExecutor):
-                if not executor.bad_state_is_set:
-                    logger.info(f"Scaling in executor {executor.label}")
-                    if executor.provider:
-                        job_ids = executor.provider.resources.keys()
-                        block_ids = executor.scale_in(len(job_ids))
-                        if self.monitoring and block_ids:
-                            new_status = {}
-                            for bid in block_ids:
-                                new_status[bid] = JobStatus(JobState.CANCELLED)
-                            msg = executor.create_monitoring_info(new_status)
-                            logger.debug("Sending message {} to hub from DFK".format(msg))
-                            self.monitoring.send(MessageType.BLOCK_INFO, msg)
-                else:  # and bad_state_is_set
-                    logger.warning(f"Not shutting down executor {executor.label} because it is in bad state")
             logger.info(f"Shutting down executor {executor.label}")
             executor.shutdown()
             logger.info(f"Shut down executor {executor.label}")
 
         logger.info("Terminated executors")
         self.time_completed = datetime.datetime.now()
```

### Comparing `parsl-2024.3.4/parsl/dataflow/errors.py` & `parsl-2024.4.1/parsl/dataflow/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/dataflow/futures.py` & `parsl-2024.4.1/parsl/dataflow/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/dataflow/memoization.py` & `parsl-2024.4.1/parsl/dataflow/memoization.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/dataflow/rundirs.py` & `parsl-2024.4.1/parsl/dataflow/rundirs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/dataflow/states.py` & `parsl-2024.4.1/parsl/dataflow/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/dataflow/taskrecord.py` & `parsl-2024.4.1/parsl/dataflow/taskrecord.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,17 @@
     in multiple threads very close together in time, which this lock
     prevents.
     """
 
     # these three could be more strongly typed perhaps but I'm not thinking about that now
     func: Callable
     fn_hash: str
-    args: Sequence[Any]  # in some places we uses a Tuple[Any, ...] and in some places a List[Any]. This is an attempt to correctly type both of those.
+    args: Sequence[Any]
+    # in some places we uses a Tuple[Any, ...] and in some places a List[Any].
+    # This is an attempt to correctly type both of those.
     kwargs: Dict[str, Any]
 
     time_invoked: Optional[datetime.datetime]
     time_returned: Optional[datetime.datetime]
     try_time_launched: Optional[datetime.datetime]
     try_time_returned: Optional[datetime.datetime]
```

### Comparing `parsl-2024.3.4/parsl/errors.py` & `parsl-2024.4.1/parsl/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/base.py` & `parsl-2024.4.1/parsl/executors/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         return self
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Literal[False]:
         self.shutdown()
         return False
 
     @abstractmethod
-    def start(self) -> Optional[List[str]]:
+    def start(self) -> None:
         """Start the executor.
 
         Any spin-up operations (for example: starting thread pools) should be performed here.
         """
         pass
 
     @abstractmethod
@@ -103,14 +103,24 @@
         return self._run_dir
 
     @run_dir.setter
     def run_dir(self, value: str) -> None:
         self._run_dir = value
 
     @property
+    def run_id(self) -> Optional[str]:
+        """UUID for the enclosing DFK.
+        """
+        return self._run_id
+
+    @run_id.setter
+    def run_id(self, value: Optional[str]) -> None:
+        self._run_id = value
+
+    @property
     def hub_address(self) -> Optional[str]:
         """Address to the Hub for monitoring.
         """
         return self._hub_address
 
     @hub_address.setter
     def hub_address(self, value: Optional[str]) -> None:
```

### Comparing `parsl-2024.3.4/parsl/executors/errors.py` & `parsl-2024.4.1/parsl/executors/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/flux/execute_parsl_task.py` & `parsl-2024.4.1/parsl/executors/flux/execute_parsl_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/flux/executor.py` & `parsl-2024.4.1/parsl/executors/flux/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/flux/flux_instance_manager.py` & `parsl-2024.4.1/parsl/executors/flux/flux_instance_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/high_throughput/executor.py` & `parsl-2024.4.1/parsl/executors/high_throughput/executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import typing
+from collections import defaultdict
 from concurrent.futures import Future
 import typeguard
 import logging
 import threading
 import queue
 import datetime
 import pickle
+from dataclasses import dataclass
 from multiprocessing import Process, Queue
 from typing import Dict, Sequence
 from typing import List, Optional, Tuple, Union, Callable
 import math
 import warnings
 
 import parsl.launchers
@@ -50,14 +52,15 @@
                       "--result_port={result_port} "
                       "--cert_dir {cert_dir} "
                       "--logdir={logdir} "
                       "--block_id={{block_id}} "
                       "--hb_period={heartbeat_period} "
                       "{address_probe_timeout_string} "
                       "--hb_threshold={heartbeat_threshold} "
+                      "--drain_period={drain_period} "
                       "--cpu-affinity {cpu_affinity} "
                       "{enable_mpi_mode} "
                       "--mpi-launcher={mpi_launcher} "
                       "--available-accelerators {accelerators}")
 
 
 class HighThroughputExecutor(BlockProviderExecutor, RepresentationMixin):
@@ -196,14 +199,22 @@
         Number of seconds after which a heartbeat message indicating liveness is sent to the
         counterpart (interchange, manager). Default: 30s
 
     poll_period : int
         Timeout period to be used by the executor components in milliseconds. Increasing poll_periods
         trades performance for cpu efficiency. Default: 10ms
 
+    drain_period : int
+        The number of seconds after start when workers will begin to drain
+        and then exit. Set this to a time that is slightly less than the
+        maximum walltime of batch jobs to avoid killing tasks while they
+        execute. For example, you could set this to the walltime minus a grace
+        period for the batch job to start the workers, minus the expected
+        maximum length of an individual task.
+
     worker_logdir_root : string
         In case of a remote file system, specify the path to where logs will be kept.
 
     enable_mpi_mode: bool
         If enabled, MPI launch prefixes will be composed for the batch scheduler based on
         the nodes available in each batch job and the resource_specification dict passed
         from the app. This is an experimental feature, please refer to the following doc section
@@ -235,14 +246,15 @@
                  max_workers: Optional[Union[int, float]] = None,
                  max_workers_per_node: Optional[Union[int, float]] = None,
                  cpu_affinity: str = 'none',
                  available_accelerators: Union[int, Sequence[str]] = (),
                  prefetch_capacity: int = 0,
                  heartbeat_threshold: int = 120,
                  heartbeat_period: int = 30,
+                 drain_period: Optional[int] = None,
                  poll_period: int = 10,
                  address_probe_timeout: Optional[int] = None,
                  worker_logdir_root: Optional[str] = None,
                  enable_mpi_mode: bool = False,
                  mpi_launcher: str = "mpiexec",
                  block_error_handler: Union[bool, Callable[[BlockProviderExecutor, Dict[str, JobStatus]], None]] = True,
                  encrypted: bool = False):
@@ -298,14 +310,15 @@
         self.hub_port = None  # set to the correct hub port in dfk
         self.worker_ports = worker_ports
         self.worker_port_range = worker_port_range
         self.interchange_proc: Optional[Process] = None
         self.interchange_port_range = interchange_port_range
         self.heartbeat_threshold = heartbeat_threshold
         self.heartbeat_period = heartbeat_period
+        self.drain_period = drain_period
         self.poll_period = poll_period
         self.run_dir = '.'
         self.worker_logdir_root = worker_logdir_root
         self.cpu_affinity = cpu_affinity
         self.encrypted = encrypted
         self.cert_dir = None
 
@@ -323,15 +336,15 @@
         self.launch_cmd = launch_cmd
 
     radio_mode = "htex"
 
     def _warn_deprecated(self, old: str, new: str):
         warnings.warn(
             f"{old} is deprecated and will be removed in a future release. "
-            "Please use {new} instead.",
+            f"Please use {new} instead.",
             DeprecationWarning,
             stacklevel=2
         )
 
     @property
     def max_workers(self):
         self._warn_deprecated("max_workers", "max_workers_per_node")
@@ -371,36 +384,27 @@
                                        result_port=self.worker_result_port,
                                        cores_per_worker=self.cores_per_worker,
                                        mem_per_worker=self.mem_per_worker,
                                        max_workers_per_node=max_workers_per_node,
                                        nodes_per_block=self.provider.nodes_per_block,
                                        heartbeat_period=self.heartbeat_period,
                                        heartbeat_threshold=self.heartbeat_threshold,
+                                       drain_period=self.drain_period,
                                        poll_period=self.poll_period,
                                        cert_dir=self.cert_dir,
                                        logdir=self.worker_logdir,
                                        cpu_affinity=self.cpu_affinity,
                                        enable_mpi_mode=enable_mpi_opts,
                                        mpi_launcher=self.mpi_launcher,
                                        accelerators=" ".join(self.available_accelerators))
         self.launch_cmd = l_cmd
         logger.debug("Launch command: {}".format(self.launch_cmd))
 
         logger.debug("Starting HighThroughputExecutor with provider:\n%s", self.provider)
 
-        # TODO: why is this a provider property?
-        block_ids = []
-        if hasattr(self.provider, 'init_blocks'):
-            try:
-                block_ids = self.scale_out(blocks=self.provider.init_blocks)
-            except Exception as e:
-                logger.error("Scaling out failed: {}".format(e))
-                raise e
-        return block_ids
-
     def start(self):
         """Create the Interchange process and connect to it.
         """
         if self.encrypted and self.cert_dir is None:
             logger.debug("Creating CurveZMQ certificates")
             self.cert_dir = curvezmq.create_certificates(self.logdir)
         elif not self.encrypted and self.cert_dir:
@@ -422,16 +426,15 @@
 
         self._queue_management_thread = None
         self._start_queue_management_thread()
         self._start_local_interchange_process()
 
         logger.debug("Created management thread: {}".format(self._queue_management_thread))
 
-        block_ids = self.initialize_scaling()
-        return block_ids
+        self.initialize_scaling()
 
     @wrap_with_logs
     def _queue_management_worker(self):
         """Listen to the queue for task status messages and handle them.
 
         Depending on the message, tasks will be updated with results, exceptions,
         or updates. It expects the following messages:
@@ -624,16 +627,16 @@
                 logger.debug("Sending hold to manager: {}".format(manager['manager']))
                 self.hold_worker(manager['manager'])
 
     def submit(self, func, resource_specification, *args, **kwargs):
         """Submits work to the outgoing_q.
 
         The outgoing_q is an external process listens on this
-        queue for new work. This method behaves like a
-        submit call as described here `Python docs: <https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor>`_
+        queue for new work. This method behaves like a submit call as described here `Python docs: <https://docs.python.org/3/
+        library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor>`_
 
         Args:
             - func (callable) : Callable function
             - resource_specification (dict): Dictionary containing relevant info about task that is needed by underlying executors.
             - args (list) : List of arbitrary positional arguments.
 
         Kwargs:
@@ -681,24 +684,24 @@
         msg = []
         for bid, s in status.items():
             d = {}
             d['run_id'] = self.run_id
             d['status'] = s.status_name
             d['timestamp'] = datetime.datetime.now()
             d['executor_label'] = self.label
-            d['job_id'] = self.blocks.get(bid, None)
+            d['job_id'] = self.blocks_to_job_id.get(bid, None)
             d['block_id'] = bid
             msg.append(d)
         return msg
 
     @property
     def workers_per_node(self) -> Union[int, float]:
         return self._workers_per_node
 
-    def scale_in(self, blocks, max_idletime=None):
+    def scale_in(self, blocks: int, max_idletime: Optional[float] = None) -> List[str]:
         """Scale in the number of active blocks by specified amount.
 
         The scale in method here is very rude. It doesn't give the workers
         the opportunity to finish current tasks or cleanup. This is tracked
         in issue #530
 
         Parameters
@@ -717,33 +720,42 @@
              the requested number.
 
         Returns
         -------
         List of block IDs scaled in
         """
         logger.debug(f"Scale in called, blocks={blocks}")
+
+        @dataclass
+        class BlockInfo:
+            tasks: int  # sum of tasks in this block
+            idle: float  # shortest idle time of any manager in this block
+
         managers = self.connected_managers()
-        block_info = {}  # block id -> list( tasks, idle duration )
+        block_info: Dict[str, BlockInfo] = defaultdict(lambda: BlockInfo(tasks=0, idle=float('inf')))
         for manager in managers:
             if not manager['active']:
                 continue
             b_id = manager['block_id']
-            if b_id not in block_info:
-                block_info[b_id] = [0, float('inf')]
-            block_info[b_id][0] += manager['tasks']
-            block_info[b_id][1] = min(block_info[b_id][1], manager['idle_duration'])
+            block_info[b_id].tasks += manager['tasks']
+            block_info[b_id].idle = min(block_info[b_id].idle, manager['idle_duration'])
+
+        # The scaling policy is that longest idle blocks should be scaled down
+        # in preference to least idle (most recently used) blocks.
+        # Other policies could be implemented here.
+
+        sorted_blocks = sorted(block_info.items(), key=lambda item: (-item[1].idle, item[1].tasks))
 
-        sorted_blocks = sorted(block_info.items(), key=lambda item: (item[1][1], item[1][0]))
         logger.debug(f"Scale in selecting from {len(sorted_blocks)} blocks")
         if max_idletime is None:
             block_ids_to_kill = [x[0] for x in sorted_blocks[:blocks]]
         else:
             block_ids_to_kill = []
             for x in sorted_blocks:
-                if x[1][1] > max_idletime and x[1][0] == 0:
+                if x[1].idle > max_idletime and x[1].tasks == 0:
                     block_ids_to_kill.append(x[0])
                     if len(block_ids_to_kill) == blocks:
                         break
 
             logger.debug("Selected idle block ids to kill: {}".format(
                 block_ids_to_kill))
             if len(block_ids_to_kill) < blocks:
@@ -751,22 +763,22 @@
 
         # Hold the block
         for block_id in block_ids_to_kill:
             self._hold_block(block_id)
 
         # Now kill via provider
         # Potential issue with multiple threads trying to remove the same blocks
-        to_kill = [self.blocks[bid] for bid in block_ids_to_kill if bid in self.blocks]
+        to_kill = [self.blocks_to_job_id[bid] for bid in block_ids_to_kill if bid in self.blocks_to_job_id]
 
         r = self.provider.cancel(to_kill)
         job_ids = self._filter_scale_in_ids(to_kill, r)
 
-        # to_kill block_ids are fetched from self.blocks
-        # If a block_id is in self.block, it must exist in self.block_mapping
-        block_ids_killed = [self.block_mapping[jid] for jid in job_ids]
+        # to_kill block_ids are fetched from self.blocks_to_job_id
+        # If a block_id is in self.blocks_to_job_id, it must exist in self.job_ids_to_block
+        block_ids_killed = [self.job_ids_to_block[jid] for jid in job_ids]
 
         return block_ids_killed
 
     def _get_launch_command(self, block_id: str) -> str:
         if self.launch_cmd is None:
             raise ScalingFailed(self, "No launch command")
         launch_cmd = self.launch_cmd.format(block_id=block_id)
```

### Comparing `parsl-2024.3.4/parsl/executors/high_throughput/interchange.py` & `parsl-2024.4.1/parsl/executors/high_throughput/interchange.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from parsl.app.errors import RemoteExceptionWrapper
 from parsl.executors.high_throughput.manager_record import ManagerRecord
 from parsl.monitoring.message_type import MessageType
 from parsl.process_loggers import wrap_with_logs
 
 
 PKL_HEARTBEAT_CODE = pickle.dumps((2 ** 32) - 1)
+PKL_DRAINED_CODE = pickle.dumps((2 ** 32) - 2)
 
 LOGGER_NAME = "interchange"
 logger = logging.getLogger(LOGGER_NAME)
 
 
 class ManagerLost(Exception):
     ''' Task lost due to manager loss. Manager is considered lost when multiple heartbeats
@@ -97,20 +98,20 @@
              The specific two ports at which workers will connect to the Interchange. Default: None
 
         worker_port_range : tuple(int, int)
              The interchange picks ports at random from the range which will be used by workers.
              This is overridden when the worker_ports option is set. Default: (54000, 55000)
 
         hub_address : str
-             The ip address at which the interchange can send info about managers to when monitoring is enabled.
-             This is passed via dfk and executor automatically. Default: None (meaning monitoring disabled)
+             The IP address at which the interchange can send info about managers to when monitoring is enabled.
+             Default: None (meaning monitoring disabled)
 
         hub_port : str
              The port at which the interchange can send info about managers to when monitoring is enabled.
-             This is passed via dfk and executor automatically. Default: None (meaning monitoring disabled)
+             Default: None (meaning monitoring disabled)
 
         heartbeat_threshold : int
              Number of seconds since the last heartbeat after which worker is considered lost.
 
         logdir : str
              Parsl log directory paths. Logs and temp files go here. Default: '.'
 
@@ -240,27 +241,27 @@
             logger.debug("putting message onto pending_task_queue")
             self.pending_task_queue.put(msg)
             task_counter += 1
             logger.debug(f"Fetched {task_counter} tasks so far")
 
     def _create_monitoring_channel(self) -> Optional[zmq.Socket]:
         if self.hub_address and self.hub_port:
-            logger.info("Connecting to monitoring")
+            logger.info("Connecting to MonitoringHub")
             # This is a one-off because monitoring is unencrypted
             hub_channel = zmq.Context().socket(zmq.DEALER)
             hub_channel.set_hwm(0)
             hub_channel.connect("tcp://{}:{}".format(self.hub_address, self.hub_port))
-            logger.info("Monitoring enabled and connected to hub")
+            logger.info("Connected to MonitoringHub")
             return hub_channel
         else:
             return None
 
     def _send_monitoring_info(self, hub_channel: Optional[zmq.Socket], manager: ManagerRecord) -> None:
         if hub_channel:
-            logger.info("Sending message {} to hub".format(manager))
+            logger.info("Sending message {} to MonitoringHub".format(manager))
 
             d: Dict = cast(Dict, manager.copy())
             d['timestamp'] = datetime.datetime.now()
             d['last_heartbeat'] = datetime.datetime.fromtimestamp(d['last_heartbeat'])
 
             hub_channel.send_pyobj((MessageType.NODE_INFO, d))
 
@@ -304,15 +305,16 @@
                         else:
                             idle_duration = 0.0
                         resp = {'manager': manager_id.decode('utf-8'),
                                 'block_id': m['block_id'],
                                 'worker_count': m['worker_count'],
                                 'tasks': len(m['tasks']),
                                 'idle_duration': idle_duration,
-                                'active': m['active']}
+                                'active': m['active'],
+                                'draining': m['draining']}
                         reply.append(resp)
 
                 elif command_req.startswith("HOLD_WORKER"):
                     cmd, s_manager = command_req.split(';')
                     manager_id = s_manager.encode('utf-8')
                     logger.info("Received HOLD_WORKER for {!r}".format(manager_id))
                     if manager_id in self._ready_managers:
@@ -381,22 +383,28 @@
 
         while not kill_event.is_set():
             self.socks = dict(poller.poll(timeout=poll_period))
 
             self.process_task_outgoing_incoming(interesting_managers, hub_channel, kill_event)
             self.process_results_incoming(interesting_managers, hub_channel)
             self.expire_bad_managers(interesting_managers, hub_channel)
+            self.expire_drained_managers(interesting_managers, hub_channel)
             self.process_tasks_to_send(interesting_managers)
 
         self.zmq_context.destroy()
         delta = time.time() - start
         logger.info("Processed {} tasks in {} seconds".format(self.count, delta))
         logger.warning("Exiting")
 
-    def process_task_outgoing_incoming(self, interesting_managers: Set[bytes], hub_channel: Optional[zmq.Socket], kill_event: threading.Event) -> None:
+    def process_task_outgoing_incoming(
+            self,
+            interesting_managers: Set[bytes],
+            hub_channel: Optional[zmq.Socket],
+            kill_event: threading.Event
+    ) -> None:
         """Process one message from manager on the task_outgoing channel.
         Note that this message flow is in contradiction to the name of the
         channel - it is not an outgoing message and it is not a task.
         """
         if self.task_outgoing in self.socks and self.socks[self.task_outgoing] == zmq.POLLIN:
             logger.debug("starting task_outgoing section")
             message = self.task_outgoing.recv_multipart()
@@ -422,14 +430,15 @@
                 # We set up an entry only if registration works correctly
                 self._ready_managers[manager_id] = {'last_heartbeat': time.time(),
                                                     'idle_since': time.time(),
                                                     'block_id': None,
                                                     'max_capacity': 0,
                                                     'worker_count': 0,
                                                     'active': True,
+                                                    'draining': False,
                                                     'tasks': []}
                 self.connected_block_history.append(msg['block_id'])
 
                 interesting_managers.add(manager_id)
                 logger.info("Adding manager: {!r} to ready queue".format(manager_id))
                 m = self._ready_managers[manager_id]
 
@@ -460,18 +469,36 @@
                     logger.info("Manager {!r} has compatible Parsl version {}".format(manager_id, msg['parsl_v']))
                     logger.info("Manager {!r} has compatible Python version {}".format(manager_id,
                                                                                        msg['python_v'].rsplit(".", 1)[0]))
             elif msg['type'] == 'heartbeat':
                 self._ready_managers[manager_id]['last_heartbeat'] = time.time()
                 logger.debug("Manager {!r} sent heartbeat via tasks connection".format(manager_id))
                 self.task_outgoing.send_multipart([manager_id, b'', PKL_HEARTBEAT_CODE])
+            elif msg['type'] == 'drain':
+                self._ready_managers[manager_id]['draining'] = True
+                logger.debug(f"Manager {manager_id!r} requested drain")
             else:
                 logger.error(f"Unexpected message type received from manager: {msg['type']}")
             logger.debug("leaving task_outgoing section")
 
+    def expire_drained_managers(self, interesting_managers: Set[bytes], hub_channel: Optional[zmq.Socket]) -> None:
+
+        for manager_id in list(interesting_managers):
+            # is it always true that a draining manager will be in interesting managers?
+            # i think so because it will have outstanding capacity?
+            m = self._ready_managers[manager_id]
+            if m['draining'] and len(m['tasks']) == 0:
+                logger.info(f"Manager {manager_id!r} is drained - sending drained message to manager")
+                self.task_outgoing.send_multipart([manager_id, b'', PKL_DRAINED_CODE])
+                interesting_managers.remove(manager_id)
+                self._ready_managers.pop(manager_id)
+
+                m['active'] = False
+                self._send_monitoring_info(hub_channel, m)
+
     def process_tasks_to_send(self, interesting_managers: Set[bytes]) -> None:
         # Check if there are tasks that could be sent to managers
 
         logger.debug("Managers count (interesting/total): {interesting}/{total}".format(
             total=len(self._ready_managers),
             interesting=len(interesting_managers)))
 
@@ -481,15 +508,15 @@
 
             while shuffled_managers and not self.pending_task_queue.empty():  # cf. the if statement above...
                 manager_id = shuffled_managers.pop()
                 m = self._ready_managers[manager_id]
                 tasks_inflight = len(m['tasks'])
                 real_capacity = m['max_capacity'] - tasks_inflight
 
-                if (real_capacity and m['active']):
+                if (real_capacity and m['active'] and not m['draining']):
                     tasks = self.get_tasks(real_capacity)
                     if tasks:
                         self.task_outgoing.send_multipart([manager_id, b'', pickle.dumps(tasks)])
                         task_count = len(tasks)
                         self.count += task_count
                         tids = [t['task_id'] for t in tasks]
                         m['tasks'].extend(tids)
@@ -617,15 +644,21 @@
         Format string to use.
 
     Returns
     -------
         None.
     """
     if format_string is None:
-        format_string = "%(asctime)s.%(msecs)03d %(name)s:%(lineno)d %(processName)s(%(process)d) %(threadName)s %(funcName)s [%(levelname)s]  %(message)s"
+        format_string = (
+
+            "%(asctime)s.%(msecs)03d %(name)s:%(lineno)d "
+            "%(processName)s(%(process)d) %(threadName)s "
+            "%(funcName)s [%(levelname)s] %(message)s"
+
+        )
 
     global logger
     logger = logging.getLogger(LOGGER_NAME)
     logger.setLevel(level)
     handler = logging.FileHandler(filename)
     handler.setLevel(level)
     formatter = logging.Formatter(format_string, datefmt='%Y-%m-%d %H:%M:%S')
```

### Comparing `parsl-2024.3.4/parsl/executors/high_throughput/mpi_prefix_composer.py` & `parsl-2024.4.1/parsl/executors/high_throughput/mpi_prefix_composer.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/high_throughput/mpi_resource_management.py` & `parsl-2024.4.1/parsl/executors/high_throughput/mpi_resource_management.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/high_throughput/probe.py` & `parsl-2024.4.1/parsl/executors/high_throughput/probe.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/high_throughput/process_worker_pool.py` & `parsl-2024.4.1/parsl/executors/high_throughput/process_worker_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     TaskScheduler,
     MPITaskScheduler
 )
 
 from parsl.executors.high_throughput.mpi_prefix_composer import compose_all, VALID_LAUNCHERS
 
 HEARTBEAT_CODE = (2 ** 32) - 1
+DRAINED_CODE = (2 ** 32) - 2
 
 
 class Manager:
     """ Manager manages task execution by the workers
 
                 |         zmq              |    Manager         |   Worker Processes
                 |                          |                    |
@@ -69,15 +70,16 @@
                  heartbeat_threshold,
                  heartbeat_period,
                  poll_period,
                  cpu_affinity,
                  enable_mpi_mode: bool = False,
                  mpi_launcher: str = "mpiexec",
                  available_accelerators: Sequence[str],
-                 cert_dir: Optional[str]):
+                 cert_dir: Optional[str],
+                 drain_period: Optional[int]):
         """
         Parameters
         ----------
         addresses : str
              comma separated list of addresses for the interchange
 
         address_probe_timeout : int
@@ -134,14 +136,17 @@
             info is made available to workers via env vars.
 
         mpi_launcher: str
             Set to one of the supported MPI launchers: ("srun", "aprun", "mpiexec")
 
         cert_dir : str | None
             Path to the certificate directory.
+
+        drain_period: int | None
+            Number of seconds to drain after  TODO: could be a nicer timespec involving m,s,h qualifiers for user friendliness?
         """
 
         logger.info("Manager initializing")
 
         self._start_time = time.time()
 
         try:
@@ -223,14 +228,22 @@
         self.max_queue_size = self.prefetch_capacity + self.worker_count
 
         self.tasks_per_round = 1
 
         self.heartbeat_period = heartbeat_period
         self.heartbeat_threshold = heartbeat_threshold
         self.poll_period = poll_period
+
+        self.drain_time: float
+        if drain_period:
+            self.drain_time = self._start_time + drain_period
+            logger.info(f"Will request drain at {self.drain_time}")
+        else:
+            self.drain_time = float('inf')
+
         self.cpu_affinity = cpu_affinity
 
         # Define accelerator available, adjust worker count accordingly
         self.available_accelerators = available_accelerators
         self.accelerators_available = len(available_accelerators) > 0
         if self.accelerators_available:
             self.worker_count = min(len(self.available_accelerators), self.worker_count)
@@ -258,18 +271,27 @@
         b_msg = json.dumps(msg).encode('utf-8')
         return b_msg
 
     def heartbeat_to_incoming(self):
         """ Send heartbeat to the incoming task queue
         """
         msg = {'type': 'heartbeat'}
+        # don't need to dumps and encode this every time - could do as a global on import?
         b_msg = json.dumps(msg).encode('utf-8')
         self.task_incoming.send(b_msg)
         logger.debug("Sent heartbeat")
 
+    def drain_to_incoming(self):
+        """ Send heartbeat to the incoming task queue
+        """
+        msg = {'type': 'drain'}
+        b_msg = json.dumps(msg).encode('utf-8')
+        self.task_incoming.send(b_msg)
+        logger.debug("Sent drain")
+
     @wrap_with_logs
     def pull_tasks(self, kill_event):
         """ Pull tasks from the incoming tasks zmq pipe onto the internal
         pending task queue
 
         Parameters:
         -----------
@@ -294,39 +316,53 @@
             # arrives or one of these event times is reached. This code
             # assumes that the event times won't change except on iteration
             # of this loop - so will break if a different thread does
             # anything to bring one of the event times earlier - and that the
             # time here are correctly copy-pasted from the relevant if
             # statements.
             next_interesting_event_time = min(last_beat + self.heartbeat_period,
+                                              self.drain_time,
                                               last_interchange_contact + self.heartbeat_threshold)
             try:
                 pending_task_count = self.pending_task_queue.qsize()
             except NotImplementedError:
                 # Ref: https://github.com/python/cpython/blob/6d5e0dc0e330f4009e8dc3d1642e46b129788877/Lib/multiprocessing/queues.py#L125
                 pending_task_count = f"pending task count is not available on {platform.system()}"
 
             logger.debug("ready workers: {}, pending tasks: {}".format(self.ready_worker_count.value,
                                                                        pending_task_count))
 
             if time.time() >= last_beat + self.heartbeat_period:
                 self.heartbeat_to_incoming()
                 last_beat = time.time()
 
+            if time.time() > self.drain_time:
+                logger.info("Requesting drain")
+                self.drain_to_incoming()
+                # This will start the pool draining...
+                # Drained exit behaviour does not happen here. It will be
+                # driven by the interchange sending a DRAINED_CODE message.
+
+                # now set drain time to the far future so we don't send a drain
+                # message every iteration.
+                self.drain_time = float('inf')
+
             poll_duration_s = max(0, next_interesting_event_time - time.time())
             socks = dict(poller.poll(timeout=poll_duration_s * 1000))
 
             if self.task_incoming in socks and socks[self.task_incoming] == zmq.POLLIN:
                 _, pkl_msg = self.task_incoming.recv_multipart()
                 tasks = pickle.loads(pkl_msg)
                 last_interchange_contact = time.time()
 
                 if tasks == HEARTBEAT_CODE:
                     logger.debug("Got heartbeat from interchange")
-
+                elif tasks == DRAINED_CODE:
+                    logger.info("Got fulled drained message from interchange - setting kill flag")
+                    kill_event.set()
                 else:
                     task_recv_counter += len(tasks)
                     logger.debug("Got executor tasks: {}, cumulative count of tasks: {}".format([t['task_id'] for t in tasks], task_recv_counter))
 
                     for task in tasks:
                         self.task_scheduler.put_task(task)
 
@@ -409,15 +445,17 @@
                     try:
                         task = self._tasks_in_progress.pop(worker_id)
                         logger.info("Worker {} was busy when it died".format(worker_id))
                         try:
                             raise WorkerLost(worker_id, platform.node())
                         except Exception:
                             logger.info("Putting exception for executor task {} in the pending result queue".format(task['task_id']))
-                            result_package = {'type': 'result', 'task_id': task['task_id'], 'exception': serialize(RemoteExceptionWrapper(*sys.exc_info()))}
+                            result_package = {'type': 'result',
+                                              'task_id': task['task_id'],
+                                              'exception': serialize(RemoteExceptionWrapper(*sys.exc_info()))}
                             pkl_package = pickle.dumps(result_package)
                             self.pending_result_queue.put(pkl_package)
                     except KeyError:
                         logger.info("Worker {} was not busy when it died".format(worker_id))
 
                     p = self._start_worker(worker_id)
                     self.procs[worker_id] = p
@@ -484,17 +522,16 @@
                                                            name="Monitoring-Handler")
 
         self._task_puller_thread.start()
         self._result_pusher_thread.start()
         self._worker_watchdog_thread.start()
         self._monitoring_handler_thread.start()
 
-        logger.info("Loop start")
+        logger.info("Manager threads started")
 
-        # TODO : Add mechanism in this loop to stop the worker pool
         # This might need a multiprocessing event to signal back.
         self._kill_event.wait()
         logger.critical("Received kill event, terminating worker processes")
 
         self._task_puller_thread.join()
         self._result_pusher_thread.join()
         self._worker_watchdog_thread.join()
@@ -798,14 +835,16 @@
                         help="Caps the maximum workers that can be launched, default:infinity")
     parser.add_argument("-p", "--prefetch_capacity", default=0,
                         help="Number of tasks that can be prefetched to the manager. Default is 0.")
     parser.add_argument("--hb_period", default=30,
                         help="Heartbeat period in seconds. Uses manager default unless set")
     parser.add_argument("--hb_threshold", default=120,
                         help="Heartbeat threshold in seconds. Uses manager default unless set")
+    parser.add_argument("--drain_period", default=None,
+                        help="Drain this pool after specified number of seconds. By default, does not drain.")
     parser.add_argument("--address_probe_timeout", default=30,
                         help="Timeout to probe for viable address to interchange. Default: 30s")
     parser.add_argument("--poll", default=10,
                         help="Poll period used in milliseconds")
     parser.add_argument("-r", "--result_port", required=True,
                         help="REQUIRED: Result port for posting results to the interchange")
 
@@ -818,15 +857,15 @@
         else:
             raise argparse.ArgumentTypeError("cpu-affinity must be one of {} or a list format".format(allowed_strategies))
 
     parser.add_argument("--cpu-affinity", type=strategyorlist,
                         required=True,
                         help="Whether/how workers should control CPU affinity.")
     parser.add_argument("--available-accelerators", type=str, nargs="*",
-                        help="Names of available accelerators")
+                        help="Names of available accelerators, if not given assumed to be zero accelerators available", default=[])
     parser.add_argument("--enable_mpi_mode", action='store_true',
                         help="Enable MPI mode")
     parser.add_argument("--mpi-launcher", type=str, choices=VALID_LAUNCHERS,
                         help="MPI launcher to use iff enable_mpi_mode=true")
 
     args = parser.parse_args()
 
@@ -850,31 +889,36 @@
         logger.info("addresses: {}".format(args.addresses))
         logger.info("max_workers_per_node: {}".format(args.max_workers_per_node))
         logger.info("poll_period: {}".format(args.poll))
         logger.info("address_probe_timeout: {}".format(args.address_probe_timeout))
         logger.info("Prefetch capacity: {}".format(args.prefetch_capacity))
         logger.info("Heartbeat threshold: {}".format(args.hb_threshold))
         logger.info("Heartbeat period: {}".format(args.hb_period))
+        logger.info("Drain period: {}".format(args.drain_period))
         logger.info("CPU affinity: {}".format(args.cpu_affinity))
         logger.info("Accelerators: {}".format(" ".join(args.available_accelerators)))
         logger.info("enable_mpi_mode: {}".format(args.enable_mpi_mode))
         logger.info("mpi_launcher: {}".format(args.mpi_launcher))
 
         manager = Manager(task_port=args.task_port,
                           result_port=args.result_port,
                           addresses=args.addresses,
                           address_probe_timeout=int(args.address_probe_timeout),
                           uid=args.uid,
                           block_id=args.block_id,
                           cores_per_worker=float(args.cores_per_worker),
                           mem_per_worker=None if args.mem_per_worker == 'None' else float(args.mem_per_worker),
-                          max_workers_per_node=args.max_workers_per_node if args.max_workers_per_node == float('inf') else int(args.max_workers_per_node),
+                          max_workers_per_node=(
+                              args.max_workers_per_node if args.max_workers_per_node == float('inf')
+                              else int(args.max_workers_per_node)
+                          ),
                           prefetch_capacity=int(args.prefetch_capacity),
                           heartbeat_threshold=int(args.hb_threshold),
                           heartbeat_period=int(args.hb_period),
+                          drain_period=None if args.drain_period == "None" else int(args.drain_period),
                           poll_period=int(args.poll),
                           cpu_affinity=args.cpu_affinity,
                           enable_mpi_mode=args.enable_mpi_mode,
                           mpi_launcher=args.mpi_launcher,
                           available_accelerators=args.available_accelerators,
                           cert_dir=None if args.cert_dir == "None" else args.cert_dir)
         manager.start()
```

### Comparing `parsl-2024.3.4/parsl/executors/high_throughput/zmq_pipes.py` & `parsl-2024.4.1/parsl/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/radical/executor.py` & `parsl-2024.4.1/parsl/executors/radical/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/radical/rpex_master.py` & `parsl-2024.4.1/parsl/executors/radical/rpex_master.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/radical/rpex_resources.py` & `parsl-2024.4.1/parsl/executors/radical/rpex_resources.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/radical/rpex_worker.py` & `parsl-2024.4.1/parsl/executors/radical/rpex_worker.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/status_handling.py` & `parsl-2024.4.1/parsl/executors/status_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,23 +57,23 @@
                 self.block_error_handler = noop_error_handler
         else:
             self.block_error_handler = block_error_handler
 
         # errors can happen during the submit call to the provider; this is used
         # to keep track of such errors so that they can be handled in one place
         # together with errors reported by status()
-        self._simulated_status: Dict[Any, JobStatus] = {}
+        self._simulated_status: Dict[str, JobStatus] = {}
         self._executor_bad_state = threading.Event()
         self._executor_exception: Optional[Exception] = None
 
         self._block_id_counter = AtomicIDCounter()
 
         self._tasks = {}  # type: Dict[object, Future]
-        self.blocks = {}  # type: Dict[str, str]
-        self.block_mapping = {}  # type: Dict[str, str]
+        self.blocks_to_job_id = {}  # type: Dict[str, str]
+        self.job_ids_to_block = {}  # type: Dict[str, str]
 
     def _make_status_dict(self, block_ids: List[str], status_list: List[JobStatus]) -> Dict[str, JobStatus]:
         """Given a list of block ids and a list of corresponding status strings,
         returns a dictionary mapping each block id to the corresponding status
 
         :param block_ids: the list of block ids
         :param status_list: the list of job status strings
@@ -98,21 +98,18 @@
                  should be done
         """
         if self._provider is None:
             return 0
         else:
             return self._provider.status_polling_interval
 
-    def _fail_job_async(self, block_id: Any, message: str):
+    def _fail_job_async(self, block_id: str, message: str):
         """Marks a job that has failed to start but would not otherwise be included in status()
         as failed and report it in status()
         """
-        if block_id is None:
-            block_id = str(self._block_id_counter.get_id())
-            logger.info(f"Allocated block ID {block_id} for simulated failure")
         self._simulated_status[block_id] = JobStatus(JobState.FAILED, message)
 
     @abstractproperty
     def outstanding(self) -> int:
         """This should return the number of tasks that the executor has been given to run (waiting to run, and running now)"""
 
         raise NotImplementedError("Classes inheriting from BlockProviderExecutor must implement "
@@ -193,32 +190,28 @@
         block_ids = []
         logger.info(f"Scaling out by {blocks} blocks")
         for _ in range(blocks):
             block_id = str(self._block_id_counter.get_id())
             logger.info(f"Allocated block ID {block_id}")
             try:
                 job_id = self._launch_block(block_id)
-                self.blocks[block_id] = job_id
-                self.block_mapping[job_id] = block_id
+                self.blocks_to_job_id[block_id] = job_id
+                self.job_ids_to_block[job_id] = block_id
                 block_ids.append(block_id)
             except Exception as ex:
                 self._fail_job_async(block_id,
                                      "Failed to start block {}: {}".format(block_id, ex))
         return block_ids
 
     @abstractmethod
     def scale_in(self, blocks: int) -> List[str]:
         """Scale in method.
 
         Cause the executor to reduce the number of blocks by count.
 
-        We should have the scale in method simply take resource object
-        which will have the scaling methods, scale_in itself should be a coroutine, since
-        scaling tasks can be slow.
-
         :return: A list of block ids corresponding to the blocks that were removed.
         """
         pass
 
     def _launch_block(self, block_id: str) -> Any:
         launch_cmd = self._get_launch_command(block_id)
         job_name = f"parsl.{self.label}.block-{block_id}"
@@ -235,16 +228,16 @@
     def _get_launch_command(self, block_id: str) -> str:
         pass
 
     def _get_block_and_job_ids(self) -> Tuple[List[str], List[Any]]:
         # Not using self.blocks.keys() and self.blocks.values() simultaneously
         # The dictionary may be changed during invoking this function
         # As scale_in and scale_out are invoked in multiple threads
-        block_ids = list(self.blocks.keys())
+        block_ids = list(self.blocks_to_job_id.keys())
         job_ids = []  # types: List[Any]
         for bid in block_ids:
-            job_ids.append(self.blocks[bid])
+            job_ids.append(self.blocks_to_job_id[bid])
         return block_ids, job_ids
 
     @abstractproperty
     def workers_per_node(self) -> Union[int, float]:
         pass
```

### Comparing `parsl-2024.3.4/parsl/executors/taskvine/errors.py` & `parsl-2024.4.1/parsl/executors/taskvine/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/taskvine/exec_parsl_function.py` & `parsl-2024.4.1/parsl/executors/taskvine/exec_parsl_function.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/taskvine/executor.py` & `parsl-2024.4.1/parsl/executors/taskvine/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ TaskVineExecutor utilizes the TaskVine distributed framework developed by the
 Cooperative Computing Lab (CCL) at Notre Dame to provide a fault-tolerant,
 high-throughput system for delegating Parsl tasks to thousands of remote machines
 """
 
 # Import Python built-in libraries
+import atexit
 import threading
 import multiprocessing
 import logging
 import tempfile
 import hashlib
 import subprocess
 import os
@@ -167,22 +168,40 @@
 
         # Worker command to be given to an execution provider (e.g., local or Condor)
         self._worker_command = ""
 
         # Path to directory that holds all tasks' data and results.
         self._function_data_dir = ""
 
-        # helper scripts to prepare package tarballs for Parsl apps
+        # Helper scripts to prepare package tarballs for Parsl apps
         self._package_analyze_script = shutil.which("poncho_package_analyze")
         self._package_create_script = shutil.which("poncho_package_create")
         if self._package_analyze_script is None or self._package_create_script is None:
             self._poncho_available = False
         else:
             self._poncho_available = True
 
+        # Register atexit handler to cleanup when Python shuts down
+        atexit.register(self.atexit_cleanup)
+
+        # Attribute indicating whether this executor was started to shut it down properly.
+        # This safeguards cases where an object of this executor is created but
+        # the executor never starts, so it shouldn't be shutdowned.
+        self._is_started = False
+
+        # Attribute indicating whether this executor was shutdown before.
+        # This safeguards cases where this object is automatically shut down (e.g.,
+        # via atexit) and the user also explicitly calls shut down. While this is
+        # permitted, the effect of an executor shutdown should happen only once.
+        self._is_shutdown = False
+
+    def atexit_cleanup(self):
+        # Calls this executor's shutdown method upon Python exiting the process.
+        self.shutdown()
+
     def _get_launch_command(self, block_id):
         # Implements BlockProviderExecutor's abstract method.
         # This executor uses different terminology for worker/launch
         # commands than in htex.
         return f"PARSL_WORKER_BLOCK_ID={block_id} {self._worker_command}"
 
     def __synchronize_manager_factory_comm_settings(self):
@@ -192,16 +211,17 @@
         # If the manager can choose any available port (port number = 0),
         # then it must have a project name
         # so the factory can look it up. Otherwise the factory process will not know the
         # port number as it's only chosen when the TaskVine manager process is run.
         if self.manager_config.port == 0 and self.manager_config.project_name is None:
             self.manager_config.project_name = "parsl-vine-" + str(uuid.uuid4())
 
-        # guess the host name if the project name is not given
-        if not self.manager_config.project_name:
+        # guess the host name if the project name is not given and none has been supplied
+        # explicitly in the manager config.
+        if not self.manager_config.project_name and self.manager_config.address is None:
             self.manager_config.address = get_any_address()
 
         # Factory communication settings are overridden by manager communication settings.
         self.factory_config._project_port = self.manager_config.port
         self.factory_config._project_address = self.manager_config.address
         self.factory_config._project_name = self.manager_config.project_name
         self.factory_config._project_password_file = self.manager_config.project_password_file
@@ -224,21 +244,26 @@
         vine_log_dir = os.path.join(os.path.dirname(run_dir), self.label)
         if self.manager_config.vine_log_dir is None:
             self.manager_config.vine_log_dir = vine_log_dir
 
         # factory logs go with manager logs regardless
         self.factory_config.scratch_dir = self.manager_config.vine_log_dir
         logger.debug(f"Function data directory: {self._function_data_dir}, log directory: {log_dir}")
-        logger.debug(f"TaskVine manager log directory: {self.manager_config.vine_log_dir}, factory log directory: {self.factory_config.scratch_dir}")
+        logger.debug(
+            f"TaskVine manager log directory: {self.manager_config.vine_log_dir}, "
+            f"factory log directory: {self.factory_config.scratch_dir}")
 
     def start(self):
         """Create submit process and collector thread to create, send, and
         retrieve Parsl tasks within the TaskVine system.
         """
 
+        # Mark this executor object as started
+        self._is_started = True
+
         # Synchronize connection and communication settings between the manager and factory
         self.__synchronize_manager_factory_comm_settings()
 
         # Create data and logging dirs
         self.__create_data_and_logging_dirs()
 
         logger.debug("Starting TaskVineExecutor")
@@ -557,66 +582,68 @@
         Scales the workers to the appropriate nodes with provider
         """
         # Start scaling in/out
         logger.debug("Starting TaskVineExecutor with provider: %s", self.provider)
         self._worker_command = self._construct_worker_command()
         self._patch_providers()
 
-        if hasattr(self.provider, 'init_blocks'):
-            try:
-                self.scale_out(blocks=self.provider.init_blocks)
-            except Exception as e:
-                logger.error("Initial block scaling out failed: {}".format(e))
-                raise e
-
     @property
     def outstanding(self) -> int:
         """Count the number of outstanding tasks."""
         logger.debug(f"Counted {self._outstanding_tasks} outstanding tasks")
         return self._outstanding_tasks
 
     @property
     def workers_per_node(self) -> Union[int, float]:
         return 1
 
     def scale_in(self, count):
         """Scale in method. Cancel a given number of blocks
         """
         # Obtain list of blocks to kill
-        to_kill = list(self.blocks.keys())[:count]
-        kill_ids = [self.blocks[block] for block in to_kill]
+        to_kill = list(self.blocks_to_job_id.keys())[:count]
+        kill_ids = [self.blocks_to_job_id[block] for block in to_kill]
 
         # Cancel the blocks provisioned
         if self.provider:
             self.provider.cancel(kill_ids)
         else:
             logger.error("No execution provider available to scale")
 
     def shutdown(self, *args, **kwargs):
         """Shutdown the executor. Sets flag to cancel the submit process and
         collector thread, which shuts down the TaskVine system submission.
         """
+        if not self._is_started:
+            # Don't shutdown if the executor never starts.
+            return
+
+        if self._is_shutdown:
+            # Don't shutdown this executor again.
+            return
+
         logger.debug("TaskVine shutdown started")
         self._should_stop.set()
 
         # Remove the workers that are still going
-        kill_ids = [self.blocks[block] for block in self.blocks.keys()]
+        kill_ids = [self.blocks_to_job_id[block] for block in self.blocks_to_job_id.keys()]
         if self.provider:
             logger.debug("Cancelling blocks")
             self.provider.cancel(kill_ids)
 
         # Join all processes before exiting
         logger.debug("Joining on submit process")
         self._submit_process.join()
         logger.debug("Joining on collector thread")
         self._collector_thread.join()
         if self.worker_launch_method == 'factory':
             logger.debug("Joining on factory process")
             self._factory_process.join()
 
+        self._is_shutdown = True
         logger.debug("TaskVine shutdown completed")
 
     @wrap_with_logs
     def _collect_taskvine_results(self):
         """Sets the values of tasks' futures completed by taskvine.
         """
         logger.debug("Starting Collector Thread")
```

### Comparing `parsl-2024.3.4/parsl/executors/taskvine/factory.py` & `parsl-2024.4.1/parsl/executors/taskvine/factory.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/taskvine/factory_config.py` & `parsl-2024.4.1/parsl/executors/taskvine/factory_config.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/taskvine/manager.py` & `parsl-2024.4.1/parsl/executors/taskvine/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,14 +372,15 @@
 
                 for spec in task.output_files:
                     if spec.stage:
                         if spec.parsl_name in parsl_file_name_to_vine_file:
                             task_out_file = parsl_file_name_to_vine_file[spec.parsl_name]
                         else:
                             task_out_file = m.declare_file(spec.parsl_name, cache=spec.cache, peer_transfer=True)
+                            parsl_file_name_to_vine_file[spec.parsl_name] = task_out_file
                         t.add_output(task_out_file, spec.parsl_name)
 
             # Submit the task to the TaskVine object
             logger.debug("Submitting executor task {}, {} to TaskVine".format(task.executor_id, t))
             try:
                 vine_id = m.submit(t)
                 logger.debug("Submitted executor task {} to TaskVine".format(task.executor_id))
```

### Comparing `parsl-2024.3.4/parsl/executors/taskvine/manager_config.py` & `parsl-2024.4.1/parsl/executors/taskvine/manager_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import socket
 from dataclasses import dataclass
 from typing import Optional
 
 # This try except clause prevents import errors
 # when TaskVine is not used in Parsl.
 try:
     from ndcctools.taskvine.cvine import VINE_DEFAULT_PORT
@@ -19,17 +18,17 @@
     ----------
 
     port: int
         Network port for the manager to communicate with workers.
         A value of 0 means TaskVine chooses any available port.
         Default is VINE_DEFAULT_PORT.
 
-    address: str
+    address: Optional[str]
         Address of the local machine.
-        Default is socket.gethostname().
+        If None, socket.gethostname() will be used to determine the address.
 
     project_name: Optional[str]
         If given, TaskVine will periodically report its status and performance
         back to the global TaskVine catalog at
         http://ccl.cse.nd.edu/software/taskvine/status.
         Recommended mode of communication between manager and workers.
         Default is None. Overrides address.
@@ -157,15 +156,15 @@
         Directory to store TaskVine logging facilities.
         Default is None, in which all TaskVine logs will be contained
         in the Parsl logging directory.
     """
 
     # Connection and communication settings
     port: int = VINE_DEFAULT_PORT
-    address: str = socket.gethostname()
+    address: Optional[str] = None
     project_name: Optional[str] = None
     project_password_file: Optional[str] = None
 
     # Global task settings
     env_vars: Optional[dict] = None
     init_command: str = ""
     env_pack: Optional[str] = None
```

### Comparing `parsl-2024.3.4/parsl/executors/taskvine/utils.py` & `parsl-2024.4.1/parsl/executors/taskvine/utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/threads.py` & `parsl-2024.4.1/parsl/executors/threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/workqueue/errors.py` & `parsl-2024.4.1/parsl/executors/workqueue/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/workqueue/exec_parsl_function.py` & `parsl-2024.4.1/parsl/executors/workqueue/exec_parsl_function.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/workqueue/executor.py` & `parsl-2024.4.1/parsl/executors/workqueue/executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ WorkQueueExecutor utilizes the Work Queue distributed framework developed by the
 Cooperative Computing Lab (CCL) at Notre Dame to provide a fault-tolerant,
 high-throughput system for delegating Parsl tasks to thousands of remote machines
 """
 
+import atexit
 import threading
 import multiprocessing
 import logging
 from concurrent.futures import Future
 from ctypes import c_bool
 
 import tempfile
@@ -250,15 +251,14 @@
                                        block_error_handler=True)
         if not _work_queue_enabled:
             raise OptionalModuleMissing(['work_queue'], "WorkQueueExecutor requires the work_queue module.")
 
         self.label = label
         self.task_queue = multiprocessing.Queue()  # type: multiprocessing.Queue
         self.collector_queue = multiprocessing.Queue()  # type: multiprocessing.Queue
-        self.blocks = {}  # type: Dict[str, str]
         self.address = address
         self.port = port
         self.executor_task_counter = -1
         self.project_name = project_name
         self.project_password_file = project_password_file
         self.env = env
         self.init_command = init_command
@@ -294,23 +294,43 @@
                 self.project_password_file = None
 
         # Build foundations of the launch command
         self.launch_cmd = ("{package_prefix}python3 exec_parsl_function.py {mapping} {function} {result}")
         if self.init_command != "":
             self.launch_cmd = self.init_command + "; " + self.launch_cmd
 
+        # register atexit handler to cleanup when Python shuts down
+        atexit.register(self.atexit_cleanup)
+
+        # Attribute indicating whether this executor was started to shut it down properly.
+        # This safeguards cases where an object of this executor is created but
+        # the executor never starts, so it shouldn't be shutdowned.
+        self.is_started = False
+
+        # Attribute indicating whether this executor was shutdown before.
+        # This safeguards cases where this object is automatically shut down (e.g.,
+        # via atexit) and the user also explicitly calls shut down. While this is
+        # permitted, the effect of an executor shutdown should happen only once.
+        self.is_shutdown = False
+
+    def atexit_cleanup(self):
+        # Calls this executor's shutdown method upon Python exiting the process.
+        self.shutdown()
+
     def _get_launch_command(self, block_id):
         # this executor uses different terminology for worker/launch
         # commands than in htex
         return f"PARSL_WORKER_BLOCK_ID={block_id} {self.worker_command}"
 
     def start(self):
         """Create submit process and collector thread to create, send, and
         retrieve Parsl tasks within the Work Queue system.
         """
+        # Mark this executor object as started
+        self.is_started = True
         self.tasks_lock = threading.Lock()
 
         # Create directories for data and results
         if not self.function_dir:
             self.function_data_dir = os.path.join(self.run_dir, self.label, "function_data")
         else:
             tp = str(time.time())
@@ -650,21 +670,14 @@
         Scales the workers to the appropriate nodes with provider
         """
         # Start scaling in/out
         logger.debug("Starting WorkQueueExecutor with provider: %s", self.provider)
         self.worker_command = self._construct_worker_command()
         self._patch_providers()
 
-        if hasattr(self.provider, 'init_blocks'):
-            try:
-                self.scale_out(blocks=self.provider.init_blocks)
-            except Exception as e:
-                logger.error("Initial block scaling out failed: {}".format(e))
-                raise e
-
     @property
     def outstanding(self) -> int:
         """Count the number of outstanding tasks. This is inefficiently
         implemented and probably could be replaced with a counter.
         """
         outstanding = 0
         with self.tasks_lock:
@@ -678,41 +691,50 @@
     def workers_per_node(self) -> Union[int, float]:
         return 1
 
     def scale_in(self, count):
         """Scale in method.
         """
         # Obtain list of blocks to kill
-        to_kill = list(self.blocks.keys())[:count]
-        kill_ids = [self.blocks[block] for block in to_kill]
+        to_kill = list(self.blocks_to_job_id.keys())[:count]
+        kill_ids = [self.blocks_to_job_id[block] for block in to_kill]
 
         # Cancel the blocks provisioned
         if self.provider:
             self.provider.cancel(kill_ids)
         else:
             logger.error("No execution provider available to scale")
 
     def shutdown(self, *args, **kwargs):
         """Shutdown the executor. Sets flag to cancel the submit process and
         collector thread, which shuts down the Work Queue system submission.
         """
+        if not self.is_started:
+            # Don't shutdown if the executor never starts.
+            return
+
+        if self.is_shutdown:
+            # Don't shutdown this executor again.
+            return
+
         logger.debug("Work Queue shutdown started")
         self.should_stop.value = True
 
         # Remove the workers that are still going
-        kill_ids = [self.blocks[block] for block in self.blocks.keys()]
+        kill_ids = [self.blocks_to_job_id[block] for block in self.blocks_to_job_id.keys()]
         if self.provider:
             logger.debug("Cancelling blocks")
             self.provider.cancel(kill_ids)
 
         logger.debug("Joining on submit process")
         self.submit_process.join()
         logger.debug("Joining on collector thread")
         self.collector_thread.join()
 
+        self.is_shutdown = True
         logger.debug("Work Queue shutdown completed")
 
     @wrap_with_logs
     def _collect_work_queue_results(self):
         """Sets the values of tasks' futures of tasks completed by work queue.
         """
         logger.debug("Starting Collector Thread")
```

### Comparing `parsl-2024.3.4/parsl/executors/workqueue/parsl_coprocess.py` & `parsl-2024.4.1/parsl/executors/workqueue/parsl_coprocess.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/executors/workqueue/parsl_coprocess_stub.py` & `parsl-2024.4.1/parsl/executors/workqueue/parsl_coprocess_stub.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/jobs/error_handlers.py` & `parsl-2024.4.1/parsl/jobs/error_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     if hasattr(executor.provider, "init_blocks"):
         threshold = max(1, executor.provider.init_blocks)
 
     if total_jobs >= threshold and failed_jobs == total_jobs:
         executor.set_bad_state_and_fail_all(_get_error(status))
 
 
-def windowed_error_handler(executor: status_handling.BlockProviderExecutor, status: Dict[str, JobStatus], threshold: int = 3):
+def windowed_error_handler(executor: status_handling.BlockProviderExecutor, status: Dict[str, JobStatus], threshold: int = 3) -> None:
     sorted_status = [(key, status[key]) for key in sorted(status, key=lambda x: int(x))]
     current_window = dict(sorted_status[-threshold:])
     total, failed = _count_jobs(current_window)
     if failed == threshold:
         executor.set_bad_state_and_fail_all(_get_error(status))
```

### Comparing `parsl-2024.3.4/parsl/jobs/job_status_poller.py` & `parsl-2024.4.1/parsl/jobs/job_status_poller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import logging
 import parsl
 import time
 import zmq
-from typing import Dict, List, Sequence, Optional
+from typing import Dict, List, Sequence, Optional, Union
 
 from parsl.jobs.states import JobStatus, JobState
 from parsl.jobs.strategy import Strategy
 from parsl.executors.status_handling import BlockProviderExecutor
 from parsl.monitoring.message_type import MessageType
 
 
 from parsl.utils import Timer
 
 
 logger = logging.getLogger(__name__)
 
 
-class PollItem:
+class PolledExecutorFacade:
     def __init__(self, executor: BlockProviderExecutor, dfk: Optional["parsl.dataflow.dflow.DataFlowKernel"] = None):
         self._executor = executor
         self._dfk = dfk
         self._interval = executor.status_polling_interval
         self._last_poll_time = 0.0
         self._status = {}  # type: Dict[str, JobStatus]
+        self.first = True
 
         # Create a ZMQ channel to send poll status to monitoring
         self.monitoring_enabled = False
         if self._dfk and self._dfk.monitoring is not None:
             self.monitoring_enabled = True
             hub_address = self._dfk.hub_address
-            hub_port = self._dfk.hub_interchange_port
+            hub_port = self._dfk.hub_zmq_port
             context = zmq.Context()
             self.hub_channel = context.socket(zmq.DEALER)
             self.hub_channel.set_hwm(0)
             self.hub_channel.connect("tcp://{}:{}".format(hub_address, hub_port))
             logger.info("Monitoring enabled on job status poller")
 
     def _should_poll(self, now: float) -> bool:
@@ -68,69 +69,70 @@
         """
         return self._status
 
     @property
     def executor(self) -> BlockProviderExecutor:
         return self._executor
 
-    def scale_in(self, n, max_idletime=None):
+    def scale_in(self, n: int, max_idletime: Optional[float] = None) -> List[str]:
 
         if max_idletime is None:
             block_ids = self._executor.scale_in(n)
         else:
             # This is a HighThroughputExecutor-specific interface violation.
             # This code hopes, through pan-codebase reasoning, that this
             # scale_in method really does come from HighThroughputExecutor,
             # and so does have an extra max_idletime parameter not present
             # in the executor interface.
-            block_ids = self._executor.scale_in(n, max_idletime=max_idletime)
+            block_ids = self._executor.scale_in(n, max_idletime=max_idletime)  # type: ignore[call-arg]
         if block_ids is not None:
             new_status = {}
             for block_id in block_ids:
                 new_status[block_id] = JobStatus(JobState.CANCELLED)
                 del self._status[block_id]
             self.send_monitoring_info(new_status)
         return block_ids
 
-    def scale_out(self, n):
+    def scale_out(self, n: int) -> List[str]:
         block_ids = self._executor.scale_out(n)
         if block_ids is not None:
             new_status = {}
             for block_id in block_ids:
                 new_status[block_id] = JobStatus(JobState.PENDING)
             self.send_monitoring_info(new_status)
             self._status.update(new_status)
         return block_ids
 
     def __repr__(self) -> str:
         return self._status.__repr__()
 
 
 class JobStatusPoller(Timer):
-    def __init__(self, strategy: Optional[str] = None, max_idletime: float = 0.0,
+    def __init__(self, *, strategy: Optional[str], max_idletime: float,
+                 strategy_period: Union[float, int],
                  dfk: Optional["parsl.dataflow.dflow.DataFlowKernel"] = None) -> None:
-        self._poll_items = []  # type: List[PollItem]
+        self._executor_facades = []  # type: List[PolledExecutorFacade]
         self.dfk = dfk
         self._strategy = Strategy(strategy=strategy,
                                   max_idletime=max_idletime)
-        super().__init__(self.poll, interval=5, name="JobStatusPoller")
+        super().__init__(self.poll, interval=strategy_period, name="JobStatusPoller")
 
     def poll(self) -> None:
         self._update_state()
-        self._run_error_handlers(self._poll_items)
-        self._strategy.strategize(self._poll_items)
+        self._run_error_handlers(self._executor_facades)
+        self._strategy.strategize(self._executor_facades)
 
-    def _run_error_handlers(self, status: List[PollItem]) -> None:
+    def _run_error_handlers(self, status: List[PolledExecutorFacade]) -> None:
         for es in status:
             es.executor.handle_errors(es.status)
 
     def _update_state(self) -> None:
         now = time.time()
-        for item in self._poll_items:
+        for item in self._executor_facades:
             item.poll(now)
 
     def add_executors(self, executors: Sequence[BlockProviderExecutor]) -> None:
         for executor in executors:
             if executor.status_polling_interval > 0:
                 logger.debug("Adding executor {}".format(executor.label))
-                self._poll_items.append(PollItem(executor, self.dfk))
+                self._executor_facades.append(PolledExecutorFacade(executor, self.dfk))
         self._strategy.add_executors(executors)
```

### Comparing `parsl-2024.3.4/parsl/jobs/states.py` & `parsl-2024.4.1/parsl/jobs/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/jobs/strategy.py` & `parsl-2024.4.1/parsl/jobs/strategy.py`

 * *Files 13% similar despite different names*

```diff
@@ -125,16 +125,16 @@
 
     def __init__(self, *, strategy: Optional[str], max_idletime: float) -> None:
         """Initialize strategy."""
         self.executors: Dict[str, ExecutorState]
         self.executors = {}
         self.max_idletime = max_idletime
 
-        self.strategies = {None: self._strategy_noop,
-                           'none': self._strategy_noop,
+        self.strategies = {None: self._strategy_init_only,
+                           'none': self._strategy_init_only,
                            'simple': self._strategy_simple,
                            'htex_auto_scale': self._strategy_htex_auto_scale}
 
         if strategy is None:
             warnings.warn("literal None for strategy choice is deprecated. Use string 'none' instead.",
                           DeprecationWarning)
 
@@ -142,55 +142,68 @@
 
         logger.debug("Scaling strategy: {0}".format(strategy))
 
     def add_executors(self, executors: Sequence[ParslExecutor]) -> None:
         for executor in executors:
             self.executors[executor.label] = {'idle_since': None}
 
-    def _strategy_noop(self, status: List[jsp.PollItem]) -> None:
-        """Do nothing.
+    def _strategy_init_only(self, executor_facades: List[jsp.PolledExecutorFacade]) -> None:
+        """Scale up to init_blocks at the start, then nothing more.
         """
-        logger.debug("strategy_noop: doing nothing")
+        for ef in executor_facades:
+            if ef.first:
+                executor = ef.executor
+                logger.debug(f"strategy_init_only: scaling out {executor.provider.init_blocks} initial blocks for {executor.label}")
+                ef.scale_out(executor.provider.init_blocks)
+                ef.first = False
+            else:
+                logger.debug("strategy_init_only: doing nothing")
 
-    def _strategy_simple(self, status_list: List[jsp.PollItem]) -> None:
-        self._general_strategy(status_list, strategy_type='simple')
+    def _strategy_simple(self, executor_facades: List[jsp.PolledExecutorFacade]) -> None:
+        self._general_strategy(executor_facades, strategy_type='simple')
 
-    def _strategy_htex_auto_scale(self, status_list: List[jsp.PollItem]) -> None:
+    def _strategy_htex_auto_scale(self, executor_facades: List[jsp.PolledExecutorFacade]) -> None:
         """HTEX specific auto scaling strategy
 
         This strategy works only for HTEX. This strategy will scale out by
         requesting additional compute resources via the provider when the
         workload requirements exceed the provisioned capacity. The scale out
         behavior is exactly like the 'simple' strategy.
 
         If there are idle blocks during execution, this strategy will terminate
         those idle blocks specifically. When # of tasks >> # of blocks, HTEX places
         tasks evenly across blocks, which makes it rather difficult to ensure that
         some blocks will reach 0% utilization. Consequently, this strategy can be
         expected to scale in effectively only when # of workers, or tasks executing
         per block is close to 1.
         """
-        self._general_strategy(status_list, strategy_type='htex')
+        self._general_strategy(executor_facades, strategy_type='htex')
 
     @wrap_with_logs
-    def _general_strategy(self, status_list, *, strategy_type):
-        logger.debug(f"general strategy starting with strategy_type {strategy_type} for {len(status_list)} executors")
+    def _general_strategy(self, executor_facades, *, strategy_type):
+        logger.debug(f"general strategy starting with strategy_type {strategy_type} for {len(executor_facades)} executors")
 
-        for exec_status in status_list:
-            executor = exec_status.executor
+        for ef in executor_facades:
+            executor = ef.executor
             label = executor.label
             if not isinstance(executor, BlockProviderExecutor):
                 logger.debug(f"Not strategizing for executor {label} because scaling not enabled")
                 continue
             logger.debug(f"Strategizing for executor {label}")
 
+            if ef.first:
+                executor = ef.executor
+                logger.debug(f"Scaling out {executor.provider.init_blocks} initial blocks for {label}")
+                ef.scale_out(executor.provider.init_blocks)
+                ef.first = False
+
             # Tasks that are either pending completion
             active_tasks = executor.outstanding
 
-            status = exec_status.status
+            status = ef.status
 
             # FIXME we need to handle case where provider does not define these
             # FIXME probably more of this logic should be moved to the provider
             min_blocks = executor.provider.min_blocks
             max_blocks = executor.provider.max_blocks
             tasks_per_node = executor.workers_per_node
 
@@ -238,18 +251,19 @@
 
                     idle_since = self.executors[executor.label]['idle_since']
                     idle_duration = time.time() - idle_since
                     if idle_duration > self.max_idletime:
                         # We have resources idle for the max duration,
                         # we have to scale_in now.
                         logger.debug(f"Idle time has reached {self.max_idletime}s for executor {label}; scaling in")
-                        exec_status.scale_in(active_blocks - min_blocks)
+                        ef.scale_in(active_blocks - min_blocks)
 
                     else:
-                        logger.debug(f"Idle time {idle_duration}s is less than max_idletime {self.max_idletime}s for executor {label}; not scaling in")
+                        logger.debug(
+                                f"Idle time {idle_duration}s is less than max_idletime {self.max_idletime}s for executor {label}; not scaling in")
 
             # Case 2
             # More tasks than the available slots.
             elif (float(active_slots) / active_tasks) < parallelism:
                 logger.debug("Strategy case 2: slots are overloaded - (slot_ratio = active_slots/active_tasks) < parallelism")
 
                 # Case 2a
@@ -260,24 +274,24 @@
                 # Case 2b
                 else:
                     logger.debug(f"Strategy case 2b: active_blocks {active_blocks} < max_blocks {max_blocks} so scaling out")
                     excess_slots = math.ceil((active_tasks * parallelism) - active_slots)
                     excess_blocks = math.ceil(float(excess_slots) / (tasks_per_node * nodes_per_block))
                     excess_blocks = min(excess_blocks, max_blocks - active_blocks)
                     logger.debug(f"Requesting {excess_blocks} more blocks")
-                    exec_status.scale_out(excess_blocks)
+                    ef.scale_out(excess_blocks)
 
             elif active_slots == 0 and active_tasks > 0:
                 logger.debug("Strategy case 4a: No active slots but some active tasks - could scale out by a single block")
 
                 # Case 4a
                 if active_blocks < max_blocks:
                     logger.debug("Requesting single block")
 
-                    exec_status.scale_out(1)
+                    ef.scale_out(1)
                 else:
                     logger.debug("Not requesting single block, because at maxblocks already")
 
             # Case 4b
             # More slots than tasks
             elif active_slots > 0 and active_slots > active_tasks:
                 logger.debug("Strategy case 4b: more slots than tasks")
@@ -285,15 +299,15 @@
                     # Scale in for htex
                     if isinstance(executor, HighThroughputExecutor):
                         if active_blocks > min_blocks:
                             excess_slots = math.ceil(active_slots - (active_tasks * parallelism))
                             excess_blocks = math.ceil(float(excess_slots) / (tasks_per_node * nodes_per_block))
                             excess_blocks = min(excess_blocks, active_blocks - min_blocks)
                             logger.debug(f"Requesting scaling in by {excess_blocks} blocks with idle time {self.max_idletime}s")
-                            exec_status.scale_in(excess_blocks, max_idletime=self.max_idletime)
+                            ef.scale_in(excess_blocks, max_idletime=self.max_idletime)
                     else:
                         logger.error("This strategy does not support scaling in except for HighThroughputExecutor - taking no action")
                 else:
                     logger.debug("This strategy does not support scaling in")
 
             # Case 3
             # tasks ~ slots
```

### Comparing `parsl-2024.3.4/parsl/launchers/__init__.py` & `parsl-2024.4.1/parsl/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/launchers/base.py` & `parsl-2024.4.1/parsl/launchers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/launchers/launchers.py` & `parsl-2024.4.1/parsl/launchers/launchers.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 logger = logging.getLogger(__name__)
 
 
 class SimpleLauncher(Launcher):
     """ Does no wrapping. Just returns the command as-is
     """
-    def __init_(self, debug: bool = True) -> None:
+    def __init__(self, debug: bool = True) -> None:
         super().__init__(debug=debug)
 
     def __call__(self, command: str, tasks_per_node: int, nodes_per_block: int) -> str:
-        """
-        Args:
-        - command (string): The command string to be launched
-        - task_block (string) : bash evaluated string.
 
-        """
+        if nodes_per_block > 1:
+            logger.warning('Simple Launcher only supports single node per block. '
+                           f'Requested nodes: {nodes_per_block}. '
+                           'You may be getting fewer workers than expected')
+
         return command
 
 
 class WrappedLauncher(Launcher):
     """Wraps the command by prepending commands before a user's command
 
     As an example, the wrapped launcher can be used to launch a command
```

### Comparing `parsl-2024.3.4/parsl/log_utils.py` & `parsl-2024.4.1/parsl/log_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,26 +24,26 @@
 )
 
 
 @typeguard.typechecked
 def set_stream_logger(name: str = 'parsl',
                       level: int = logging.DEBUG,
                       format_string: Optional[str] = None,
-                      stream: Optional[io.TextIOWrapper] = None) -> None:
+                      stream: Optional[io.TextIOWrapper] = None) -> logging.Logger:
     """Add a stream log handler.
 
     Args:
          - name (string) : Set the logger name.
          - level (logging.LEVEL) : Set to logging.DEBUG by default.
          - format_string (string) : Set to None by default.
          - stream (io.TextIOWrapper) : Specify sys.stdout or sys.stderr for stream.
             If not specified, the default stream for logging.StreamHandler is used.
 
     Returns:
-         - None
+         - logger for specified name
     """
     if format_string is None:
         # format_string = "%(asctime)s %(name)s [%(levelname)s] Thread:%(thread)d %(message)s"
         format_string = "%(asctime)s %(name)s:%(lineno)d [%(levelname)s]  %(message)s"
 
     logger = logging.getLogger(name)
     logger.setLevel(logging.DEBUG)
@@ -55,30 +55,32 @@
 
     # Concurrent.futures errors are also of interest, as exceptions
     # which propagate out of the top of a callback are logged this way
     # and then discarded. (see #240)
     futures_logger = logging.getLogger("concurrent.futures")
     futures_logger.addHandler(handler)
 
+    return logger
+
 
 @typeguard.typechecked
 def set_file_logger(filename: str,
                     name: str = 'parsl',
                     level: int = logging.DEBUG,
-                    format_string: Optional[str] = None) -> None:
+                    format_string: Optional[str] = None) -> logging.Logger:
     """Add a file log handler.
 
     Args:
         - filename (string): Name of the file to write logs to
         - name (string): Logger name
         - level (logging.LEVEL): Set the logging level.
         - format_string (string): Set the format string
 
     Returns:
-       -  None
+       - logger for specified name
     """
     if format_string is None:
         format_string = DEFAULT_FORMAT
 
     logger = logging.getLogger(name)
     logger.setLevel(logging.DEBUG)
     handler = logging.FileHandler(filename)
@@ -87,7 +89,9 @@
     handler.setFormatter(formatter)
     logger.addHandler(handler)
 
     # see note in set_stream_logger for notes about logging
     # concurrent.futures
     futures_logger = logging.getLogger("concurrent.futures")
     futures_logger.addHandler(handler)
+
+    return logger
```

### Comparing `parsl-2024.3.4/parsl/monitoring/db_manager.py` & `parsl-2024.4.1/parsl/monitoring/db_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,21 @@
         mapper = self._get_mapper(table_obj)
         self.session.bulk_insert_mappings(mapper, mappings)
         self.session.commit()
 
     def rollback(self) -> None:
         self.session.rollback()
 
-    def _generate_mappings(self, table: Table, columns: Optional[List[str]] = None, messages: List[MonitoringMessage] = []) -> List[Dict[str, Any]]:
+    def _generate_mappings(
+        self,
+        table: Table,
+        columns: Optional[List[str]] = None,
+        messages: List[MonitoringMessage] = [],
+    ) -> List[Dict[str, Any]]:
+
         mappings = []
         for msg in messages:
             m = {}
             if columns is None:
                 columns = table.c.keys()
             for column in columns:
                 m[column] = msg.get(column, None)
@@ -246,14 +252,20 @@
             'psutil_process_memory_resident', Float, nullable=True)
         psutil_process_disk_read = Column(
             'psutil_process_disk_read', Float, nullable=True)
         psutil_process_disk_write = Column(
             'psutil_process_disk_write', Float, nullable=True)
         psutil_process_status = Column(
             'psutil_process_status', Text, nullable=True)
+        psutil_cpu_num = Column(
+            'psutil_cpu_num', Text, nullable=True)
+        psutil_process_num_ctx_switches_voluntary = Column(
+            'psutil_process_num_ctx_switches_voluntary', Float, nullable=True)
+        psutil_process_num_ctx_switches_involuntary = Column(
+            'psutil_process_num_ctx_switches_involuntary', Float, nullable=True)
         __table_args__ = (
             PrimaryKeyConstraint('try_id', 'task_id', 'run_id', 'timestamp'),
         )
 
 
 class DatabaseManager:
     def __init__(self,
@@ -514,15 +526,18 @@
                             msg['task_status_name'] = States.running.name
                             msg['task_try_time_running'] = msg['timestamp']
 
                             if task_try_id in inserted_tries:  # TODO: needs to become task_id and try_id, and check against inserted_tries
                                 reprocessable_first_resource_messages.append(msg)
                             else:
                                 if task_try_id in deferred_resource_messages:
-                                    logger.error("Task {} already has a deferred resource message. Discarding previous message.".format(msg['task_id']))
+                                    logger.error(
+                                        "Task {} already has a deferred resource message. "
+                                        "Discarding previous message.".format(msg['task_id'])
+                                    )
                                 deferred_resource_messages[task_try_id] = msg
                         elif msg['last_msg']:
                             # This assumes that the primary key has been added
                             # to the try table already, so doesn't use the same
                             # deferral logic as the first_msg case.
                             msg['task_status_name'] = States.running_ended.name
                             reprocessable_last_resource_messages.append(msg)
@@ -540,15 +555,18 @@
                                           'run_id', 'task_id', 'try_id',
                                           'block_id', 'hostname'],
                                  messages=reprocessable_first_resource_messages)
 
                 if reprocessable_last_resource_messages:
                     self._insert(table=STATUS, messages=reprocessable_last_resource_messages)
             except Exception:
-                logger.exception("Exception in db loop: this might have been a malformed message, or some other error. monitoring data may have been lost")
+                logger.exception(
+                    "Exception in db loop: this might have been a malformed message, "
+                    "or some other error. monitoring data may have been lost"
+                )
                 exception_happened = True
         if exception_happened:
             raise RuntimeError("An exception happened sometime during database processing and should have been logged in database_manager.log")
 
     @wrap_with_logs(target="database_manager")
     def _migrate_logs_to_internal(self, logs_queue: queue.Queue, queue_tag: str, kill_event: threading.Event) -> None:
         logger.info("Starting processing for queue {}".format(queue_tag))
@@ -567,16 +585,18 @@
                     assert isinstance(x, tuple)
                     assert len(x) == 2
                     assert x[0] in [MessageType.WORKFLOW_INFO, MessageType.TASK_INFO], \
                         "_migrate_logs_to_internal can only migrate WORKFLOW_,TASK_INFO message from priority queue, got x[0] == {}".format(x[0])
                     self._dispatch_to_internal(x)
                 elif queue_tag == 'resource':
                     assert isinstance(x, tuple), "_migrate_logs_to_internal was expecting a tuple, got {}".format(x)
-                    assert x[0] == MessageType.RESOURCE_INFO, \
-                        "_migrate_logs_to_internal can only migrate RESOURCE_INFO message from resource queue, got tag {}, message {}".format(x[0], x)
+                    assert x[0] == MessageType.RESOURCE_INFO, (
+                        "_migrate_logs_to_internal can only migrate RESOURCE_INFO message from resource queue, "
+                        "got tag {}, message {}".format(x[0], x)
+                    )
                     self._dispatch_to_internal(x)
                 elif queue_tag == 'node':
                     assert len(x) == 2, "expected message tuple to have exactly two elements"
                     assert x[0] == MessageType.NODE_INFO, "_migrate_logs_to_internal can only migrate NODE_INFO messages from node queue"
 
                     self._dispatch_to_internal(x)
                 elif queue_tag == "block":
@@ -609,15 +629,16 @@
                     self.db.update(table=table, columns=columns, messages=messages)
                     done = True
                 except sa.exc.OperationalError as e:
                     # This code assumes that an OperationalError is something that will go away eventually
                     # if retried - for example, the database being locked because someone else is readying
                     # the tables we are trying to write to. If that assumption is wrong, then this loop
                     # may go on forever.
-                    logger.warning("Got a database OperationalError. Ignoring and retrying on the assumption that it is recoverable: {}".format(e))
+                    logger.warning("Got a database OperationalError. "
+                                   "Ignoring and retrying on the assumption that it is recoverable: {}".format(e))
                     self.db.rollback()
                     time.sleep(1)  # hard coded 1s wait - this should be configurable or exponential backoff or something
 
         except KeyboardInterrupt:
             logger.exception("KeyboardInterrupt when trying to update Table {}".format(table))
             try:
                 self.db.rollback()
@@ -636,15 +657,16 @@
             done = False
             while not done:
                 try:
                     self.db.insert(table=table, messages=messages)
                     done = True
                 except sa.exc.OperationalError as e:
                     # hoping that this is a database locked error during _update, not some other problem
-                    logger.warning("Got a database OperationalError. Ignoring and retrying on the assumption that it is recoverable: {}".format(e))
+                    logger.warning("Got a database OperationalError. "
+                                   "Ignoring and retrying on the assumption that it is recoverable: {}".format(e))
                     self.db.rollback()
                     time.sleep(1)  # hard coded 1s wait - this should be configurable or exponential backoff or something
         except KeyboardInterrupt:
             logger.exception("KeyboardInterrupt when trying to update Table {}".format(table))
             try:
                 self.db.rollback()
             except Exception:
```

### Comparing `parsl-2024.3.4/parsl/monitoring/queries/pandas.py` & `parsl-2024.4.1/parsl/monitoring/queries/pandas.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/monitoring/radios.py` & `parsl-2024.4.1/parsl/monitoring/radios.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/monitoring/remote.py` & `parsl-2024.4.1/parsl/monitoring/remote.py`

 * *Files 16% similar despite different names*

```diff
@@ -197,14 +197,16 @@
     # values that can be summed up to see total resources used by task process and its children
     summable_values = ['memory_percent', 'num_threads']
 
     pm = psutil.Process(pid)
 
     children_user_time = {}  # type: Dict[int, float]
     children_system_time = {}  # type: Dict[int, float]
+    children_num_ctx_switches_voluntary = {}  # type: Dict[int, float]
+    children_num_ctx_switches_involuntary = {}  # type: Dict[int, float]
 
     def accumulate_and_prepare() -> Dict[str, Any]:
         d = {"psutil_process_" + str(k): v for k, v in pm.as_dict().items() if k in simple}
         d["run_id"] = run_id
         d["task_id"] = task_id
         d["try_id"] = try_id
         d['resource_monitoring_interval'] = sleep_dur
@@ -214,14 +216,23 @@
         d['timestamp'] = datetime.datetime.now()
 
         logging.debug("getting children")
         children = pm.children(recursive=True)
         logging.debug("got children")
 
         d["psutil_cpu_count"] = psutil.cpu_count()
+
+        # note that this will be the CPU number of the base process, not anything launched by it
+        d["psutil_cpu_num"] = pm.cpu_num()
+
+        pctxsw = pm.num_ctx_switches()
+
+        d["psutil_process_num_ctx_switches_voluntary"] = pctxsw.voluntary
+        d["psutil_process_num_ctx_switches_involuntary"] = pctxsw.involuntary
+
         d['psutil_process_memory_virtual'] = pm.memory_info().vms
         d['psutil_process_memory_resident'] = pm.memory_info().rss
         d['psutil_process_time_user'] = pm.cpu_times().user
         d['psutil_process_time_system'] = pm.cpu_times().system
         d['psutil_process_children_count'] = len(children)
         try:
             d['psutil_process_disk_write'] = pm.io_counters().write_chars
@@ -234,32 +245,50 @@
         for child in children:
             for k, v in child.as_dict(attrs=summable_values).items():
                 d['psutil_process_' + str(k)] += v
             child_user_time = child.cpu_times().user
             child_system_time = child.cpu_times().system
             children_user_time[child.pid] = child_user_time
             children_system_time[child.pid] = child_system_time
+
+            pctxsw = child.num_ctx_switches()
+            children_num_ctx_switches_voluntary[child.pid] = pctxsw.voluntary
+            children_num_ctx_switches_involuntary[child.pid] = pctxsw.involuntary
+
             d['psutil_process_memory_virtual'] += child.memory_info().vms
             d['psutil_process_memory_resident'] += child.memory_info().rss
             try:
                 d['psutil_process_disk_write'] += child.io_counters().write_chars
                 d['psutil_process_disk_read'] += child.io_counters().read_chars
             except Exception:
                 # occassionally pid temp files that hold this information are unvailable to be read so add zero
                 logging.exception("Exception reading IO counters for child {k}. Recorded IO usage may be incomplete".format(k=k), exc_info=True)
                 d['psutil_process_disk_write'] += 0
                 d['psutil_process_disk_read'] += 0
+
         total_children_user_time = 0.0
         for child_pid in children_user_time:
             total_children_user_time += children_user_time[child_pid]
+
         total_children_system_time = 0.0
         for child_pid in children_system_time:
             total_children_system_time += children_system_time[child_pid]
+
+        total_children_num_ctx_switches_voluntary = 0.0
+        for child_pid in children_num_ctx_switches_voluntary:
+            total_children_num_ctx_switches_voluntary += children_num_ctx_switches_voluntary[child_pid]
+
+        total_children_num_ctx_switches_involuntary = 0.0
+        for child_pid in children_num_ctx_switches_involuntary:
+            total_children_num_ctx_switches_involuntary += children_num_ctx_switches_involuntary[child_pid]
+
         d['psutil_process_time_user'] += total_children_user_time
         d['psutil_process_time_system'] += total_children_system_time
+        d['psutil_process_num_ctx_switches_voluntary'] += total_children_num_ctx_switches_voluntary
+        d['psutil_process_num_ctx_switches_involuntary'] += total_children_num_ctx_switches_involuntary
         logging.debug("sending message")
         return d
 
     next_send = time.time()
     accumulate_dur = 5.0  # TODO: make configurable?
 
     while not terminate_event.is_set() and pm.is_running():
```

### Comparing `parsl-2024.3.4/parsl/monitoring/types.py` & `parsl-2024.4.1/parsl/monitoring/types.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/monitoring/visualization/app.py` & `parsl-2024.4.1/parsl/monitoring/visualization/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/monitoring/visualization/models.py` & `parsl-2024.4.1/parsl/monitoring/visualization/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,9 +98,16 @@
         'psutil_process_memory_resident', db.Float, nullable=True)
     psutil_process_disk_read = db.Column(
         'psutil_process_disk_read', db.Float, nullable=True)
     psutil_process_disk_write = db.Column(
         'psutil_process_disk_write', db.Float, nullable=True)
     psutil_process_status = db.Column(
         'psutil_process_status', db.Text, nullable=True)
+    psutil_cpu_num = db.Column(
+        'psutil_cpu_num', db.Text, nullable=True)
+    psutil_process_num_ctx_switches_voluntary = db.Column(
+        'psutil_process_num_ctx_switches_voluntary', db.Float, nullable=True)
+    psutil_process_num_ctx_switches_involuntary = db.Column(
+        'psutil_process_num_ctx_switches_involuntary', db.Float, nullable=True)
+
     __table_args__ = (
         db.PrimaryKeyConstraint('task_id', 'run_id', 'timestamp'),)
```

### Comparing `parsl-2024.3.4/parsl/monitoring/visualization/plots/default/task_plots.py` & `parsl-2024.4.1/parsl/monitoring/visualization/plots/default/task_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/monitoring/visualization/plots/default/workflow_plots.py` & `parsl-2024.4.1/parsl/monitoring/visualization/plots/default/workflow_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,17 @@
                 'memo_done': 'rgb(64, 200, 64)',
                 'fail_retryable': 'rgb(200, 128,128)'
                 }
 
 
 def task_gantt_plot(df_task, df_status, time_completed=None):
 
+    if df_task.empty:
+        return None
+
     # if the workflow is not recorded as completed, then assume
     # that tasks should continue in their last state until now,
     # rather than the workflow end time.
     if not time_completed:
         time_completed = df_status['timestamp'].max()
 
     df_task = df_task.sort_values(by=['task_id'], ascending=False)
```

### Comparing `parsl-2024.3.4/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py` & `parsl-2024.4.1/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/monitoring/visualization/static/parsl-logo-white.png` & `parsl-2024.4.1/parsl/monitoring/visualization/static/parsl-logo-white.png`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/monitoring/visualization/templates/app.html` & `parsl-2024.4.1/parsl/monitoring/visualization/templates/app.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/monitoring/visualization/templates/dag.html` & `parsl-2024.4.1/parsl/monitoring/visualization/templates/dag.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/monitoring/visualization/templates/layout.html` & `parsl-2024.4.1/parsl/monitoring/visualization/templates/layout.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/monitoring/visualization/templates/resource_usage.html` & `parsl-2024.4.1/parsl/monitoring/visualization/templates/resource_usage.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/monitoring/visualization/templates/task.html` & `parsl-2024.4.1/parsl/monitoring/visualization/templates/task.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/monitoring/visualization/templates/workflow.html` & `parsl-2024.4.1/parsl/monitoring/visualization/templates/workflow.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/monitoring/visualization/templates/workflows_summary.html` & `parsl-2024.4.1/parsl/monitoring/visualization/templates/workflows_summary.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/monitoring/visualization/views.py` & `parsl-2024.4.1/parsl/monitoring/visualization/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 import parsl.monitoring.queries.pandas as queries
 
 from parsl.monitoring.visualization.models import Workflow, Task, Status, db
 
 from parsl.monitoring.visualization.plots.default.workflow_plots import task_gantt_plot, task_per_app_plot, workflow_dag_plot
 from parsl.monitoring.visualization.plots.default.task_plots import time_series_memory_per_task_plot
-from parsl.monitoring.visualization.plots.default.workflow_resource_plots import resource_distribution_plot, resource_efficiency, worker_efficiency
+from parsl.monitoring.visualization.plots.default.workflow_resource_plots import (resource_distribution_plot,
+                                                                                  resource_efficiency, worker_efficiency)
 
 dummy = True
 
 import datetime
 
 
 def format_time(value):
```

### Comparing `parsl-2024.3.4/parsl/multiprocessing.py` & `parsl-2024.4.1/parsl/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/process_loggers.py` & `parsl-2024.4.1/parsl/process_loggers.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/__init__.py` & `parsl-2024.4.1/parsl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/ad_hoc/ad_hoc.py` & `parsl-2024.4.1/parsl/providers/ad_hoc/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/aws/aws.py` & `parsl-2024.4.1/parsl/providers/aws/aws.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/azure/azure.py` & `parsl-2024.4.1/parsl/providers/azure/azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/base.py` & `parsl-2024.4.1/parsl/providers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/cluster_provider.py` & `parsl-2024.4.1/parsl/providers/cluster_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         Args:
               - template (string) : The template string to be used for the writing submit script
               - script_filename (string) : Name of the submit script
               - job_name (string) : job name
               - configs (dict) : configs that get pushed into the template
 
         Returns:
-              - True: on success
+              - None
 
         Raises:
               SchedulerMissingArgs : If template is missing args
               ScriptPathError : Unable to write submit script out
         """
 
         try:
@@ -113,16 +113,14 @@
         except Exception as e:
             print("Template : ", template)
             print("Args : ", job_name)
             print("Kwargs : ", configs)
             logger.error("Uncategorized error: %s", e)
             raise e
 
-        return True
-
     @abstractmethod
     def _status(self):
         pass
 
     def status(self, job_ids):
         """ Get the status of a list of jobs identified by the job identifiers
         returned from the submit request.
```

### Comparing `parsl-2024.3.4/parsl/providers/cobalt/cobalt.py` & `parsl-2024.4.1/parsl/providers/cobalt/cobalt.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/condor/condor.py` & `parsl-2024.4.1/parsl/providers/condor/condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/condor/template.py` & `parsl-2024.4.1/parsl/providers/condor/template.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/errors.py` & `parsl-2024.4.1/parsl/providers/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/googlecloud/googlecloud.py` & `parsl-2024.4.1/parsl/providers/googlecloud/googlecloud.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/grid_engine/grid_engine.py` & `parsl-2024.4.1/parsl/providers/grid_engine/grid_engine.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/kubernetes/kube.py` & `parsl-2024.4.1/parsl/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/local/local.py` & `parsl-2024.4.1/parsl/providers/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/lsf/lsf.py` & `parsl-2024.4.1/parsl/providers/lsf/lsf.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/pbspro/pbspro.py` & `parsl-2024.4.1/parsl/providers/pbspro/pbspro.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/providers/slurm/slurm.py` & `parsl-2024.4.1/parsl/providers/slurm/slurm.py`

 * *Files 4% similar despite different names*

```diff
@@ -276,19 +276,30 @@
                                               'job_stdout_path': job_stdout_path,
                                               'job_stderr_path': job_stderr_path,
                                               }
                     return job_id
             else:
                 logger.error("Could not read job ID from submit command standard output.")
                 logger.error("Retcode:%s STDOUT:%s STDERR:%s", retcode, stdout.strip(), stderr.strip())
-                raise SubmitException(job_name, "Could not read job ID from submit command standard output", stdout=stdout, stderr=stderr, retcode=retcode)
+                raise SubmitException(
+                    job_name,
+                    "Could not read job ID from submit command standard output",
+                    stdout=stdout,
+                    stderr=stderr,
+                    retcode=retcode
+                )
         else:
             logger.error("Submit command failed")
             logger.error("Retcode:%s STDOUT:%s STDERR:%s", retcode, stdout.strip(), stderr.strip())
-            raise SubmitException(job_name, "Could not read job ID from submit command standard output", stdout=stdout, stderr=stderr, retcode=retcode)
+            raise SubmitException(
+                job_name, "Could not read job ID from submit command standard output",
+                stdout=stdout,
+                stderr=stderr,
+                retcode=retcode
+            )
 
     def cancel(self, job_ids):
         ''' Cancels the jobs specified by a list of job ids
 
         Args:
         job_ids : [<job_id> ...]
```

### Comparing `parsl-2024.3.4/parsl/providers/torque/torque.py` & `parsl-2024.4.1/parsl/providers/torque/torque.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/serialize/base.py` & `parsl-2024.4.1/parsl/serialize/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/serialize/concretes.py` & `parsl-2024.4.1/parsl/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/serialize/errors.py` & `parsl-2024.4.1/parsl/serialize/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/serialize/facade.py` & `parsl-2024.4.1/parsl/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/serialize/proxystore.py` & `parsl-2024.4.1/parsl/serialize/proxystore.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/ad_hoc_cluster_htex.py` & `parsl-2024.4.1/parsl/tests/configs/ad_hoc_cluster_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/azure_single_node.py` & `parsl-2024.4.1/parsl/tests/configs/azure_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/bluewaters.py` & `parsl-2024.4.1/parsl/tests/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/bridges.py` & `parsl-2024.4.1/parsl/tests/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/cc_in2p3.py` & `parsl-2024.4.1/parsl/tests/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/comet.py` & `parsl-2024.4.1/parsl/tests/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/cooley_htex.py` & `parsl-2024.4.1/parsl/tests/configs/cooley_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/ec2_single_node.py` & `parsl-2024.4.1/parsl/tests/configs/ec2_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/ec2_spot.py` & `parsl-2024.4.1/parsl/tests/configs/ec2_spot.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/frontera.py` & `parsl-2024.4.1/parsl/tests/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/htex_ad_hoc_cluster.py` & `parsl-2024.4.1/parsl/tests/configs/htex_ad_hoc_cluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/htex_local.py` & `parsl-2024.4.1/parsl/tests/configs/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/htex_local_alternate.py` & `parsl-2024.4.1/parsl/tests/configs/htex_local_alternate.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/htex_local_intask_staging.py` & `parsl-2024.4.1/parsl/tests/configs/htex_local_intask_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/htex_local_rsync_staging.py` & `parsl-2024.4.1/parsl/tests/configs/htex_local_rsync_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/local_radical_mpi.py` & `parsl-2024.4.1/parsl/tests/configs/local_radical_mpi.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/local_threads_globus.py` & `parsl-2024.4.1/parsl/tests/configs/local_threads_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/midway.py` & `parsl-2024.4.1/parsl/tests/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/nscc_singapore.py` & `parsl-2024.4.1/parsl/tests/configs/nscc_singapore.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/osg_htex.py` & `parsl-2024.4.1/parsl/tests/configs/osg_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/petrelkube.py` & `parsl-2024.4.1/parsl/tests/configs/petrelkube.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/summit.py` & `parsl-2024.4.1/parsl/tests/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/swan_htex.py` & `parsl-2024.4.1/parsl/tests/configs/swan_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/taskvine_ex.py` & `parsl-2024.4.1/parsl/tests/configs/taskvine_ex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/configs/user_opts.py` & `parsl-2024.4.1/parsl/tests/configs/user_opts.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,21 +48,24 @@
     #     'scheduler_options': "",
     #     'worker_init': 'export PATH:/home/{}/anaconda3/bin/:$PATH; source activate parsl_0.5.0_py3.6;'.format(COMET_USERNAME),
     # },
     # 'midway': {
     #     'username': MIDWAY_USERNAME,
     #     'script_dir': '/scratch/midway2/{}/parsl_scripts'.format(MIDWAY_USERNAME),
     #     'scheduler_options': "",
-    #     'worker_init': 'cd /scratch/midway2/{}/parsl_scripts; module load Anaconda3/5.1.0; source activate parsl_testing;'.format(MIDWAY_USERNAME),
+    #     'worker_init': 'cd /scratch/midway2/{}/parsl_scripts; '
+    #                    'module load Anaconda3/5.1.0; source activate parsl_testing;'
+    #                    .format(MIDWAY_USERNAME),
     # },
     # 'osg': {
     #     'username': OSG_USERNAME,
     #     'script_dir': '/home/{}/parsl_scripts'.format(OSG_USERNAME),
     #     'scheduler_options': "",
-    #     'worker_init' : 'module load python/3.5.2; python3 -m venv parsl_env; source parsl_env/bin/activate; python3 -m pip install parsl==0.5.2'
+    #     'worker_init' : 'module load python/3.5.2; python3 -m venv parsl_env;
+    #                      source parsl_env/bin/activate; python3 -m pip install parsl==0.5.2'
     # },
     # 'swan': {
     #     'username': SWAN_USERNAME,
     #     'script_dir' : "/home/users/{}/parsl_scripts".format(SWAN_USERNAME),
     #     'scheduler_options': "",
     #     'worker_init': "module load cray-python/3.6.1.1; source parsl_env/bin/activate"
     # },
```

### Comparing `parsl-2024.3.4/parsl/tests/configs/workqueue_ex.py` & `parsl-2024.4.1/parsl/tests/configs/workqueue_ex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/conftest.py` & `parsl-2024.4.1/parsl/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/integration/latency.py` & `parsl-2024.4.1/parsl/tests/integration/latency.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/integration/test_channels/test_local_channel.py` & `parsl-2024.4.1/parsl/tests/integration/test_channels/test_local_channel.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/integration/test_channels/test_scp_1.py` & `parsl-2024.4.1/parsl/tests/integration/test_channels/test_scp_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/integration/test_channels/test_ssh_1.py` & `parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/integration/test_channels/test_ssh_errors.py` & `parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/integration/test_channels/test_ssh_file_transport.py` & `parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_file_transport.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/integration/test_channels/test_ssh_interactive.py` & `parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_interactive.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/integration/test_stress/test_python_simple.py` & `parsl-2024.4.1/parsl/tests/integration/test_stress/test_python_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/integration/test_stress/test_python_threads.py` & `parsl-2024.4.1/parsl/tests/integration/test_stress/test_python_threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/manual_tests/htex_local.py` & `parsl-2024.4.1/parsl/tests/manual_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/manual_tests/test_ad_hoc_htex.py` & `parsl-2024.4.1/parsl/tests/manual_tests/test_ad_hoc_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/manual_tests/test_basic.py` & `parsl-2024.4.1/parsl/tests/manual_tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py` & `parsl-2024.4.1/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/manual_tests/test_log_filter.py` & `parsl-2024.4.1/parsl/tests/manual_tests/test_log_filter.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/manual_tests/test_memory_limits.py` & `parsl-2024.4.1/parsl/tests/manual_tests/test_memory_limits.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/manual_tests/test_regression_220.py` & `parsl-2024.4.1/parsl/tests/manual_tests/test_regression_220.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/manual_tests/test_udp_simple.py` & `parsl-2024.4.1/parsl/tests/manual_tests/test_udp_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/manual_tests/test_worker_count.py` & `parsl-2024.4.1/parsl/tests/manual_tests/test_worker_count.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/scaling_tests/htex_local.py` & `parsl-2024.4.1/parsl/tests/scaling_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/scaling_tests/test_scale.py` & `parsl-2024.4.1/parsl/tests/scaling_tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/scaling_tests/wqex_condor.py` & `parsl-2024.4.1/parsl/tests/scaling_tests/wqex_condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/scaling_tests/wqex_local.py` & `parsl-2024.4.1/parsl/tests/scaling_tests/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/site_tests/site_config_selector.py` & `parsl-2024.4.1/parsl/tests/site_tests/site_config_selector.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/site_tests/test_provider.py` & `parsl-2024.4.1/parsl/tests/site_tests/test_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     status = executor.status()
     logger.info("Got executor status")
     logger.info("Block status: {}".format(status))
     assert status[scale_in_blocks[0]].terminal is True, "Terminal state"
     logger.info("Job in terminal state")
 
     _, current_jobs = executor._get_block_and_job_ids()
-    # PR 1952 stoped removing scale_in blocks from self.blocks
+    # PR 1952 stoped removing scale_in blocks from self.blocks_to_job_id
     # A new PR will handle removing blocks from self.block
     # this includes failed/completed/canceled blocks
     assert len(current_jobs) == 1, "Expected current_jobs == 1"
     dfk.cleanup()
     parsl.clear()
     logger.info("Ended test_provider")
     return True
```

### Comparing `parsl-2024.3.4/parsl/tests/site_tests/test_site.py` & `parsl-2024.4.1/parsl/tests/site_tests/test_site.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/sites/test_affinity.py` & `parsl-2024.4.1/parsl/tests/sites/test_affinity.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/sites/test_concurrent.py` & `parsl-2024.4.1/parsl/tests/sites/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/sites/test_dynamic_executor.py` & `parsl-2024.4.1/parsl/tests/sites/test_dynamic_executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/sites/test_ec2.py` & `parsl-2024.4.1/parsl/tests/sites/test_ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/sites/test_local_adhoc.py` & `parsl-2024.4.1/parsl/tests/sites/test_local_adhoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/sites/test_worker_info.py` & `parsl-2024.4.1/parsl/tests/sites/test_worker_info.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_aalst_patterns.py` & `parsl-2024.4.1/parsl/tests/test_aalst_patterns.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_bash_apps/test_apptimeout.py` & `parsl-2024.4.1/parsl/tests/test_bash_apps/test_apptimeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_bash_apps/test_basic.py` & `parsl-2024.4.1/parsl/tests/test_bash_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_bash_apps/test_error_codes.py` & `parsl-2024.4.1/parsl/tests/test_bash_apps/test_error_codes.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_bash_apps/test_kwarg_storage.py` & `parsl-2024.4.1/parsl/tests/test_bash_apps/test_kwarg_storage.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_bash_apps/test_memoize.py` & `parsl-2024.4.1/parsl/tests/test_bash_apps/test_memoize.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_bash_apps/test_memoize_ignore_args.py` & `parsl-2024.4.1/parsl/tests/test_bash_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py` & `parsl-2024.4.1/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_bash_apps/test_multiline.py` & `parsl-2024.4.1/parsl/tests/test_bash_apps/test_multiline.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_bash_apps/test_pipeline.py` & `parsl-2024.4.1/parsl/tests/test_bash_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_bash_apps/test_stdout.py` & `parsl-2024.4.1/parsl/tests/test_bash_apps/test_stdout.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_callables.py` & `parsl-2024.4.1/parsl/tests/test_callables.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_channels/test_large_output.py` & `parsl-2024.4.1/parsl/tests/test_channels/test_large_output.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_checkpointing/test_periodic.py` & `parsl-2024.4.1/parsl/tests/test_checkpointing/test_periodic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_checkpointing/test_python_checkpoint_1.py` & `parsl-2024.4.1/parsl/tests/test_checkpointing/test_python_checkpoint_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_checkpointing/test_python_checkpoint_2.py` & `parsl-2024.4.1/parsl/tests/test_checkpointing/test_python_checkpoint_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_checkpointing/test_python_checkpoint_3.py` & `parsl-2024.4.1/parsl/tests/test_checkpointing/test_python_checkpoint_3.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_checkpointing/test_regression_232.py` & `parsl-2024.4.1/parsl/tests/test_checkpointing/test_regression_232.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_checkpointing/test_regression_233.py` & `parsl-2024.4.1/parsl/tests/test_checkpointing/test_regression_233.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_checkpointing/test_regression_239.py` & `parsl-2024.4.1/parsl/tests/test_checkpointing/test_regression_239.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_checkpointing/test_task_exit.py` & `parsl-2024.4.1/parsl/tests/test_checkpointing/test_task_exit.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_curvezmq.py` & `parsl-2024.4.1/parsl/tests/test_curvezmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_data/test_file.py` & `parsl-2024.4.1/parsl/tests/test_staging/test_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_data/test_file_apps.py` & `parsl-2024.4.1/parsl/tests/test_staging/test_file_apps.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_data/test_file_staging.py` & `parsl-2024.4.1/parsl/tests/test_staging/test_file_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_data/test_output_chain_filenames.py` & `parsl-2024.4.1/parsl/tests/test_staging/test_output_chain_filenames.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_docs/test_from_slides.py` & `parsl-2024.4.1/parsl/tests/test_docs/test_from_slides.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_docs/test_kwargs.py` & `parsl-2024.4.1/parsl/tests/test_docs/test_kwargs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_docs/test_tutorial_1.py` & `parsl-2024.4.1/parsl/tests/test_docs/test_tutorial_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_docs/test_workflow1.py` & `parsl-2024.4.1/parsl/tests/test_docs/test_workflow1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_docs/test_workflow2.py` & `parsl-2024.4.1/parsl/tests/test_docs/test_workflow2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_docs/test_workflow4.py` & `parsl-2024.4.1/parsl/tests/test_docs/test_workflow4.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_error_handling/test_python_walltime.py` & `parsl-2024.4.1/parsl/tests/test_error_handling/test_python_walltime.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_error_handling/test_rand_fail.py` & `parsl-2024.4.1/parsl/tests/test_error_handling/test_rand_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_error_handling/test_resource_spec.py` & `parsl-2024.4.1/parsl/tests/test_error_handling/test_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_error_handling/test_retries.py` & `parsl-2024.4.1/parsl/tests/test_error_handling/test_retries.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_error_handling/test_retry_handler.py` & `parsl-2024.4.1/parsl/tests/test_error_handling/test_retry_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_error_handling/test_retry_handler_failure.py` & `parsl-2024.4.1/parsl/tests/test_error_handling/test_retry_handler_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_error_handling/test_serialization_fail.py` & `parsl-2024.4.1/parsl/tests/test_error_handling/test_serialization_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_error_handling/test_wrap_with_logs.py` & `parsl-2024.4.1/parsl/tests/test_error_handling/test_wrap_with_logs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_flux.py` & `parsl-2024.4.1/parsl/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_htex/test_connected_blocks.py` & `parsl-2024.4.1/parsl/tests/test_htex/test_connected_blocks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_htex/test_cpu_affinity_explicit.py` & `parsl-2024.4.1/parsl/tests/test_htex/test_cpu_affinity_explicit.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_htex/test_disconnected_blocks.py` & `parsl-2024.4.1/parsl/tests/test_htex/test_disconnected_blocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
                     worker_init="conda deactivate; export PATH=''; which python; exit 0",
                     init_blocks=0,
                     max_blocks=2,
                     min_blocks=0,
                 ),
             )
         ],
-        run_dir="/tmp/test_htex",
         max_idletime=0.5,
         strategy='htex_auto_scale',
     )
 
 
 @parsl.python_app
 def double(x):
```

### Comparing `parsl-2024.3.4/parsl/tests/test_htex/test_htex.py` & `parsl-2024.4.1/parsl/tests/test_htex/test_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_htex/test_manager_failure.py` & `parsl-2024.4.1/parsl/tests/test_htex/test_manager_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_htex/test_missing_worker.py` & `parsl-2024.4.1/parsl/tests/test_htex/test_missing_worker.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_htex/test_multiple_disconnected_blocks.py` & `parsl-2024.4.1/parsl/tests/test_htex/test_multiple_disconnected_blocks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_htex/test_worker_failure.py` & `parsl-2024.4.1/parsl/tests/test_htex/test_worker_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_htex/test_zmq_binding.py` & `parsl-2024.4.1/parsl/tests/test_htex/test_zmq_binding.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_monitoring/test_basic.py` & `parsl-2024.4.1/parsl/tests/test_monitoring/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_monitoring/test_db_locks.py` & `parsl-2024.4.1/parsl/tests/test_monitoring/test_db_locks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_monitoring/test_fuzz_zmq.py` & `parsl-2024.4.1/parsl/tests/test_monitoring/test_fuzz_zmq.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,19 +37,19 @@
     # there are different kinds of fuzz:
     # could send ZMQ messages that are weird
     # could send random bytes to the TCP socket
     #   the latter is what i'm most suspicious of in my present investigation
 
     # dig out the interchange port...
     hub_address = parsl.dfk().hub_address
-    hub_interchange_port = parsl.dfk().hub_interchange_port
+    hub_zmq_port = parsl.dfk().hub_zmq_port
 
     # this will send a string to a new socket connection
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-        s.connect((hub_address, hub_interchange_port))
+        s.connect((hub_address, hub_zmq_port))
         s.sendall(b'fuzzing\r')
 
     # this will send a non-object down the DFK's existing ZMQ connection
     parsl.dfk().monitoring._dfk_channel.send(b'FuzzyByte\rSTREAM')
 
     # This following attack is commented out, because monitoring is not resilient
     # to this.
```

### Comparing `parsl-2024.3.4/parsl/tests/test_monitoring/test_incomplete_futures.py` & `parsl-2024.4.1/parsl/tests/test_monitoring/test_incomplete_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_monitoring/test_memoization_representation.py` & `parsl-2024.4.1/parsl/tests/test_monitoring/test_memoization_representation.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_monitoring/test_viz_colouring.py` & `parsl-2024.4.1/parsl/tests/test_monitoring/test_viz_colouring.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_mpi_apps/test_bad_mpi_config.py` & `parsl-2024.4.1/parsl/tests/test_mpi_apps/test_bad_mpi_config.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py` & `parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py` & `parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_mpi_apps/test_mpi_prefix.py` & `parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_prefix.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_mpi_apps/test_mpi_scheduler.py` & `parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_scheduler.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_mpi_apps/test_resource_spec.py` & `parsl-2024.4.1/parsl/tests/test_mpi_apps/test_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_providers/test_local_provider.py` & `parsl-2024.4.1/parsl/tests/test_providers/test_local_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_providers/test_pbspro_template.py` & `parsl-2024.4.1/parsl/tests/test_providers/test_pbspro_template.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_providers/test_slurm_template.py` & `parsl-2024.4.1/parsl/tests/test_providers/test_slurm_template.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_arg_input_types.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_arg_input_types.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_basic.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_dep_standard_futures.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_dep_standard_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_depfail_propagation.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_depfail_propagation.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_fail.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_fibonacci_iterative.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_fibonacci_iterative.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_fibonacci_recursive.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_fibonacci_recursive.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_futures.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_garbage_collect.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_garbage_collect.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_import_fail.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_import_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_join.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_join.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_lifted.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_lifted.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_mapred.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_mapred.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_memoize_1.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_memoize_2.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_memoize_4.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_4.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_memoize_ignore_args.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_outputs.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_outputs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_pipeline.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_simple.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_timeout.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_timeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_python_apps/test_type5.py` & `parsl-2024.4.1/parsl/tests/test_python_apps/test_type5.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_radical/test_mpi_funcs.py` & `parsl-2024.4.1/parsl/tests/test_radical/test_mpi_funcs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_regression/test_1480.py` & `parsl-2024.4.1/parsl/tests/test_regression/test_1480.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py` & `parsl-2024.4.1/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_regression/test_1653.py` & `parsl-2024.4.1/parsl/tests/test_regression/test_1653.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_regression/test_221.py` & `parsl-2024.4.1/parsl/tests/test_regression/test_221.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_regression/test_226.py` & `parsl-2024.4.1/parsl/tests/test_regression/test_226.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_regression/test_2652.py` & `parsl-2024.4.1/parsl/tests/test_regression/test_2652.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_regression/test_69a.py` & `parsl-2024.4.1/parsl/tests/test_regression/test_69a.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_regression/test_854.py` & `parsl-2024.4.1/parsl/tests/test_regression/test_854.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_regression/test_97_parallelism_0.py` & `parsl-2024.4.1/parsl/tests/test_regression/test_97_parallelism_0.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_scaling/test_block_error_handler.py` & `parsl-2024.4.1/parsl/tests/test_scaling/test_block_error_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_scaling/test_regression_1621.py` & `parsl-2024.4.1/parsl/tests/test_scaling/test_regression_1621.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_scaling/test_scale_down.py` & `parsl-2024.4.1/parsl/tests/test_scaling/test_scale_down.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py` & `parsl-2024.4.1/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,14 +33,15 @@
                     min_blocks=_min_blocks,
                     launcher=SingleNodeLauncher(),
                 ),
             )
         ],
         max_idletime=0.5,
         strategy='htex_auto_scale',
+        strategy_period=0.1
     )
 
 
 @python_app
 def waiting_app(ident: int, outputs=(), inputs=()):
     import pathlib
     import time
@@ -58,24 +59,14 @@
 # see issue #1885 for details of failures of this test.
 # at the time of issue #1885 this test was failing frequently
 # in CI.
 @pytest.mark.local
 def test_scale_out(tmpd_cwd, try_assert):
     dfk = parsl.dfk()
 
-    # reconfigure scaling strategy to run faster than usual. This allows
-    # this test to complete faster - at time of writing 27s with default
-    # 5s strategy, vs XXXX with 0.5s strategy.
-
-    # check this attribute still exists, in the presence of ongoing
-    # development, so we have some belief that setting it will not be
-    # setting a now-ignored parameter.
-    assert hasattr(dfk.job_status_poller, 'interval')
-    dfk.job_status_poller.interval = 0.1
-
     num_managers = len(dfk.executors['htex_local'].connected_managers())
 
     assert num_managers == 0, "Expected 0 managers at start"
     assert dfk.executors['htex_local'].outstanding == 0, "Expected 0 tasks at start"
 
     ntasks = _max_blocks * 2
     ready_path = tmpd_cwd / "workers_ready"
@@ -94,15 +85,16 @@
     assert len(dfk.executors['htex_local'].connected_managers()) == _max_blocks
 
     finish_path.touch()  # Approximation of Event, via files
     [x.result() for x in futs]
 
     assert dfk.executors['htex_local'].outstanding == 0
 
-    # now we can launch one "long" task - and what should happen is that the connected_managers count "eventually" (?) converges to 1 and stays there.
+    # now we can launch one "long" task -
+    # and what should happen is that the connected_managers count "eventually" (?) converges to 1 and stays there.
 
     finish_path = tmpd_cwd / "stage2_workers_may_continue"
 
     fut = waiting_app(0, outputs=outputs, inputs=[File(finish_path)])
 
     def check_one_block():
         return len(dfk.executors['htex_local'].connected_managers()) == 1
```

### Comparing `parsl-2024.3.4/parsl/tests/test_serialization/test_2555_caching_deserializer.py` & `parsl-2024.4.1/parsl/tests/test_serialization/test_2555_caching_deserializer.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_serialization/test_basic.py` & `parsl-2024.4.1/parsl/tests/test_serialization/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_serialization/test_htex_code_cache.py` & `parsl-2024.4.1/parsl/tests/test_serialization/test_htex_code_cache.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_serialization/test_pack_resource_spec.py` & `parsl-2024.4.1/parsl/tests/test_serialization/test_pack_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_serialization/test_proxystore_configured.py` & `parsl-2024.4.1/parsl/tests/test_serialization/test_proxystore_configured.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_serialization/test_proxystore_impl.py` & `parsl-2024.4.1/parsl/tests/test_serialization/test_proxystore_impl.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_staging/staging_provider.py` & `parsl-2024.4.1/parsl/tests/test_staging/staging_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_staging/test_1316.py` & `parsl-2024.4.1/parsl/tests/test_staging/test_1316.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_staging/test_docs_1.py` & `parsl-2024.4.1/parsl/tests/test_staging/test_docs_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_staging/test_elaborate_noop_file.py` & `parsl-2024.4.1/parsl/tests/test_staging/test_elaborate_noop_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_staging/test_staging_ftp.py` & `parsl-2024.4.1/parsl/tests/test_staging/test_staging_ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_staging/test_staging_ftp_in_task.py` & `parsl-2024.4.1/parsl/tests/test_staging/test_staging_ftp_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_staging/test_staging_globus.py` & `parsl-2024.4.1/parsl/tests/test_staging/test_staging_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_staging/test_staging_https.py` & `parsl-2024.4.1/parsl/tests/test_staging/test_staging_https.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_summary.py` & `parsl-2024.4.1/parsl/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_thread_parallelism.py` & `parsl-2024.4.1/parsl/tests/test_thread_parallelism.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_threads/test_configs.py` & `parsl-2024.4.1/parsl/tests/test_threads/test_configs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_threads/test_lazy_errors.py` & `parsl-2024.4.1/parsl/tests/test_threads/test_lazy_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/tests/test_utils/test_representation_mixin.py` & `parsl-2024.4.1/parsl/tests/test_utils/test_representation_mixin.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.3.4/parsl/usage_tracking/usage.py` & `parsl-2024.4.1/parsl/usage_tracking/usage.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,15 +105,14 @@
         self.uuid = str(uuid.uuid4())
         self.parsl_version = PARSL_VERSION
         self.python_version = "{}.{}.{}".format(sys.version_info.major,
                                                 sys.version_info.minor,
                                                 sys.version_info.micro)
         self.tracking_enabled = self.check_tracking_enabled()
         logger.debug("Tracking status: {}".format(self.tracking_enabled))
-        self.initialized = False  # Once first message is sent this will be True
 
     def check_tracking_enabled(self):
         """Check if tracking is enabled.
 
         Tracking will be enabled unless either of these is true:
 
             1. dfk.config.usage_tracking is set to False
@@ -172,23 +171,20 @@
         if self.tracking_enabled:
             try:
                 proc = udp_messenger(self.domain_name, self.UDP_PORT, self.sock_timeout, message)
                 self.procs.append(proc)
             except Exception as e:
                 logger.debug("Usage tracking failed: {}".format(e))
 
-    def send_message(self) -> None:
-        """Send message over UDP.
-        """
-        if not self.initialized:
-            message = self.construct_start_message()
-            self.initialized = True
-        else:
-            message = self.construct_end_message()
+    def send_start_message(self) -> None:
+        message = self.construct_start_message()
+        self.send_UDP_message(message)
 
+    def send_end_message(self) -> None:
+        message = self.construct_end_message()
         self.send_UDP_message(message)
 
     def close(self, timeout: float = 10.0) -> None:
         """First give each process one timeout period to finish what it is
         doing, then kill it (SIGKILL). There's no softer SIGTERM step,
         because that adds one join period of delay for what is almost
         definitely either: going to behave broadly the same as to SIGKILL,
```

### Comparing `parsl-2024.3.4/parsl/utils.py` & `parsl-2024.4.1/parsl/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,20 +292,20 @@
                  wait()
                  break
 
             callback()
 
     """
 
-    def __init__(self, callback: Callable, *args: Any, interval: int = 5, name: Optional[str] = None) -> None:
+    def __init__(self, callback: Callable, *args: Any, interval: Union[float, int] = 5, name: Optional[str] = None) -> None:
         """Initialize the Timer object.
         We start the timer thread here
 
         KWargs:
-             - interval (int) : number of seconds between callback events
+             - interval (int or float) : number of seconds between callback events
              - name (str) : a base name to use when naming the started thread
         """
 
         self.interval = max(0, interval)
         self.cb_args = args
         self.callback = callback
```

### Comparing `parsl-2024.3.4/parsl.egg-info/PKG-INFO` & `parsl-2024.4.1/parsl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2024.3.4
+Version: 2024.4.1
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2024.03.04.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2024.04.01.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2024.3.4/parsl.egg-info/SOURCES.txt` & `parsl-2024.4.1/parsl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 parsl/channels/ssh_il/__init__.py
 parsl/channels/ssh_il/ssh_il.py
 parsl/concurrent/__init__.py
 parsl/configs/ASPIRE1.py
 parsl/configs/Azure.py
 parsl/configs/__init__.py
 parsl/configs/ad_hoc.py
-parsl/configs/bluewaters.py
 parsl/configs/bridges.py
 parsl/configs/cc_in2p3.py
 parsl/configs/ec2.py
 parsl/configs/expanse.py
 parsl/configs/frontera.py
 parsl/configs/htex_local.py
 parsl/configs/illinoiscluster.py
@@ -131,14 +130,15 @@
 parsl/launchers/launchers.py
 parsl/monitoring/__init__.py
 parsl/monitoring/db_manager.py
 parsl/monitoring/message_type.py
 parsl/monitoring/monitoring.py
 parsl/monitoring/radios.py
 parsl/monitoring/remote.py
+parsl/monitoring/router.py
 parsl/monitoring/types.py
 parsl/monitoring/queries/__init__.py
 parsl/monitoring/queries/pandas.py
 parsl/monitoring/visualization/__init__.py
 parsl/monitoring/visualization/app.py
 parsl/monitoring/visualization/models.py
 parsl/monitoring/visualization/utils.py
@@ -320,19 +320,14 @@
 parsl/tests/test_checkpointing/test_python_checkpoint_1.py
 parsl/tests/test_checkpointing/test_python_checkpoint_2.py
 parsl/tests/test_checkpointing/test_python_checkpoint_3.py
 parsl/tests/test_checkpointing/test_regression_232.py
 parsl/tests/test_checkpointing/test_regression_233.py
 parsl/tests/test_checkpointing/test_regression_239.py
 parsl/tests/test_checkpointing/test_task_exit.py
-parsl/tests/test_data/__init__.py
-parsl/tests/test_data/test_file.py
-parsl/tests/test_data/test_file_apps.py
-parsl/tests/test_data/test_file_staging.py
-parsl/tests/test_data/test_output_chain_filenames.py
 parsl/tests/test_docs/__init__.py
 parsl/tests/test_docs/test_from_slides.py
 parsl/tests/test_docs/test_kwargs.py
 parsl/tests/test_docs/test_tutorial_1.py
 parsl/tests/test_docs/test_workflow1.py
 parsl/tests/test_docs/test_workflow2.py
 parsl/tests/test_docs/test_workflow4.py
@@ -348,24 +343,27 @@
 parsl/tests/test_error_handling/test_wrap_with_logs.py
 parsl/tests/test_flowcontrol/__init__.py
 parsl/tests/test_htex/__init__.py
 parsl/tests/test_htex/test_basic.py
 parsl/tests/test_htex/test_connected_blocks.py
 parsl/tests/test_htex/test_cpu_affinity_explicit.py
 parsl/tests/test_htex/test_disconnected_blocks.py
+parsl/tests/test_htex/test_drain.py
 parsl/tests/test_htex/test_htex.py
 parsl/tests/test_htex/test_manager_failure.py
 parsl/tests/test_htex/test_missing_worker.py
 parsl/tests/test_htex/test_multiple_disconnected_blocks.py
 parsl/tests/test_htex/test_worker_failure.py
 parsl/tests/test_htex/test_zmq_binding.py
 parsl/tests/test_monitoring/__init__.py
+parsl/tests/test_monitoring/test_app_names.py
 parsl/tests/test_monitoring/test_basic.py
 parsl/tests/test_monitoring/test_db_locks.py
 parsl/tests/test_monitoring/test_fuzz_zmq.py
+parsl/tests/test_monitoring/test_htex_init_blocks_vs_monitoring.py
 parsl/tests/test_monitoring/test_incomplete_futures.py
 parsl/tests/test_monitoring/test_memoization_representation.py
 parsl/tests/test_monitoring/test_viz_colouring.py
 parsl/tests/test_mpi_apps/__init__.py
 parsl/tests/test_mpi_apps/test_bad_mpi_config.py
 parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py
 parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py
@@ -378,14 +376,15 @@
 parsl/tests/test_providers/test_pbspro_template.py
 parsl/tests/test_providers/test_slurm_instantiate.py
 parsl/tests/test_providers/test_slurm_template.py
 parsl/tests/test_providers/test_submiterror_deprecation.py
 parsl/tests/test_python_apps/__init__.py
 parsl/tests/test_python_apps/test_arg_input_types.py
 parsl/tests/test_python_apps/test_basic.py
+parsl/tests/test_python_apps/test_context_manager.py
 parsl/tests/test_python_apps/test_dep_standard_futures.py
 parsl/tests/test_python_apps/test_dependencies.py
 parsl/tests/test_python_apps/test_depfail_propagation.py
 parsl/tests/test_python_apps/test_fail.py
 parsl/tests/test_python_apps/test_fibonacci_iterative.py
 parsl/tests/test_python_apps/test_fibonacci_recursive.py
 parsl/tests/test_python_apps/test_futures.py
@@ -420,27 +419,34 @@
 parsl/tests/test_regression/test_97_parallelism_0.py
 parsl/tests/test_regression/test_98.py
 parsl/tests/test_scaling/__init__.py
 parsl/tests/test_scaling/test_block_error_handler.py
 parsl/tests/test_scaling/test_regression_1621.py
 parsl/tests/test_scaling/test_scale_down.py
 parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py
+parsl/tests/test_scaling/test_shutdown_scalein.py
 parsl/tests/test_serialization/__init__.py
 parsl/tests/test_serialization/test_2555_caching_deserializer.py
 parsl/tests/test_serialization/test_basic.py
 parsl/tests/test_serialization/test_htex_code_cache.py
 parsl/tests/test_serialization/test_pack_resource_spec.py
 parsl/tests/test_serialization/test_proxystore_configured.py
 parsl/tests/test_serialization/test_proxystore_impl.py
+parsl/tests/test_shutdown/__init__.py
+parsl/tests/test_shutdown/test_kill_monitoring.py
 parsl/tests/test_staging/__init__.py
 parsl/tests/test_staging/staging_provider.py
 parsl/tests/test_staging/test_1316.py
 parsl/tests/test_staging/test_docs_1.py
 parsl/tests/test_staging/test_docs_2.py
 parsl/tests/test_staging/test_elaborate_noop_file.py
+parsl/tests/test_staging/test_file.py
+parsl/tests/test_staging/test_file_apps.py
+parsl/tests/test_staging/test_file_staging.py
+parsl/tests/test_staging/test_output_chain_filenames.py
 parsl/tests/test_staging/test_staging_ftp.py
 parsl/tests/test_staging/test_staging_ftp_in_task.py
 parsl/tests/test_staging/test_staging_globus.py
 parsl/tests/test_staging/test_staging_https.py
 parsl/tests/test_threads/__init__.py
 parsl/tests/test_threads/test_configs.py
 parsl/tests/test_threads/test_lazy_errors.py
```

### Comparing `parsl-2024.3.4/parsl.egg-info/requires.txt` & `parsl-2024.4.1/parsl.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 azure<=4
 msrestazure
 work_queue
 pyyaml
 cffi
 jsonschema
 proxystore
-radical.pilot
+radical.pilot==1.47
 
 [aws]
 boto3
 
 [azure]
 azure<=4
 msrestazure
@@ -71,15 +71,15 @@
 [oauth_ssh]
 oauth-ssh>=0.9
 
 [proxystore]
 proxystore
 
 [radical-pilot]
-radical.pilot
+radical.pilot==1.47
 
 [visualization]
 pydot
 networkx<2.6,>=2.5
 Flask>=1.0.2
 flask_sqlalchemy
 pandas<2.2
```

### Comparing `parsl-2024.3.4/setup.py` & `parsl-2024.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     ],
     'google_cloud' : ['google-auth', 'google-api-python-client'],
     'gssapi' : ['python-gssapi'],
     'azure' : ['azure<=4', 'msrestazure'],
     'workqueue': ['work_queue'],
     'flux': ['pyyaml', 'cffi', 'jsonschema'],
     'proxystore': ['proxystore'],
-    'radical-pilot': ['radical.pilot'],
+    'radical-pilot': ['radical.pilot==1.47'],
     # Disabling psi-j since github direct links are not allowed by pypi
     # 'psij': ['psi-j-parsl@git+https://github.com/ExaWorks/psi-j-parsl']
 }
 extras_require['all'] = sum(extras_require.values(), [])
 
 setup(
     name='parsl',
```

