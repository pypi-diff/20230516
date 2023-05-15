# Comparing `tmp/parsl-2023.5.15.tar.gz` & `tmp/parsl-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsl-2023.5.15.tar", last modified: Mon May 15 22:42:49 2023, max compression
+gzip compressed data, was "parsl-2023.5.8.tar", last modified: Mon May  8 22:42:47 2023, max compression
```

## Comparing `parsl-2023.5.15.tar` & `parsl-2023.5.8.tar`

### file list

```diff
@@ -1,475 +1,475 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.416597 parsl-2023.5.15/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 22:42:44.000000 parsl-2023.5.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-15 22:42:44.000000 parsl-2023.5.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-15 22:42:49.416597 parsl-2023.5.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-15 22:42:44.000000 parsl-2023.5.15/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.376597 parsl-2023.5.15/parsl/
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.376597 parsl-2023.5.15/parsl/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/app/bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/app/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/app/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/app/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.376597 parsl-2023.5.15/parsl/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/benchmark/perf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.376597 parsl-2023.5.15/parsl/channels/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/channels/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/channels/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.376597 parsl-2023.5.15/parsl/channels/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/channels/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/channels/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.376597 parsl-2023.5.15/parsl/channels/oauth_ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/channels/oauth_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/channels/oauth_ssh/oauth_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.376597 parsl-2023.5.15/parsl/channels/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/channels/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/channels/ssh/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.376597 parsl-2023.5.15/parsl/channels/ssh_il/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/channels/ssh_il/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/channels/ssh_il/ssh_il.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.376597 parsl-2023.5.15/parsl/concurrent/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/concurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.380597 parsl-2023.5.15/parsl/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/ASPIRE1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/Azure.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/ad_hoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/cooley.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/cori.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/exex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/illinoiscluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/osg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/polaris.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/stampede2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/toss3_llnl.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/configs/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.380597 parsl-2023.5.15/parsl/data_provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/data_provider/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/data_provider/file_noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/data_provider/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/data_provider/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/data_provider/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/data_provider/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/data_provider/rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/data_provider/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.380597 parsl-2023.5.15/parsl/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62294 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/dataflow/dflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/dataflow/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/dataflow/executor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/dataflow/flow_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/dataflow/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/dataflow/job_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/dataflow/job_status_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/dataflow/memoization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/dataflow/rundirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/dataflow/states.py
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/dataflow/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/dataflow/taskrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.380597 parsl-2023.5.15/parsl/executors/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.384597 parsl-2023.5.15/parsl/executors/extreme_scale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/extreme_scale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/extreme_scale/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18710 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/extreme_scale/mpi_worker_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.384597 parsl-2023.5.15/parsl/executors/flux/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/flux/execute_parsl_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/flux/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/flux/flux_instance_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.384597 parsl-2023.5.15/parsl/executors/high_throughput/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/high_throughput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/high_throughput/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    33199 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/high_throughput/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29929 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/high_throughput/interchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/high_throughput/manager_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/high_throughput/monitoring_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/high_throughput/probe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33011 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/high_throughput/process_worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/status_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/swift_t.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.384597 parsl-2023.5.15/parsl/executors/workqueue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/workqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/workqueue/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/workqueue/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    47999 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/workqueue/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/workqueue/parsl_coprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/executors/workqueue/parsl_coprocess_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.384597 parsl-2023.5.15/parsl/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/launchers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/launchers/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.384597 parsl-2023.5.15/parsl/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/db_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    23301 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.384597 parsl-2023.5.15/parsl/monitoring/queries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/queries/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/radios.py
--rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.384597 parsl-2023.5.15/parsl/monitoring/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.384597 parsl-2023.5.15/parsl/monitoring/visualization/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.388597 parsl-2023.5.15/parsl/monitoring/visualization/plots/default/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/plots/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/plots/default/task_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/plots/default/workflow_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.388597 parsl-2023.5.15/parsl/monitoring/visualization/static/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/static/parsl-logo-white.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/static/parsl-monitor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.388597 parsl-2023.5.15/parsl/monitoring/visualization/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/templates/app.html
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/templates/dag.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/templates/resource_usage.html
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/templates/task.html
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/templates/workflow.html
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/templates/workflows_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/monitoring/visualization/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/process_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.388597 parsl-2023.5.15/parsl/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.388597 parsl-2023.5.15/parsl/providers/ad_hoc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/ad_hoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/ad_hoc/ad_hoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.388597 parsl-2023.5.15/parsl/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29073 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/aws/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/aws/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.388597 parsl-2023.5.15/parsl/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18367 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/azure/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/azure/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/cluster_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.388597 parsl-2023.5.15/parsl/providers/cobalt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/cobalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/cobalt/cobalt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/cobalt/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.388597 parsl-2023.5.15/parsl/providers/condor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/condor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/condor/condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/condor/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.388597 parsl-2023.5.15/parsl/providers/googlecloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/googlecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/googlecloud/googlecloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.388597 parsl-2023.5.15/parsl/providers/grid_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/grid_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/grid_engine/grid_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/grid_engine/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.388597 parsl-2023.5.15/parsl/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/kubernetes/kube.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/kubernetes/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.388597 parsl-2023.5.15/parsl/providers/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.388597 parsl-2023.5.15/parsl/providers/lsf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/lsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/lsf/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/lsf/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.388597 parsl-2023.5.15/parsl/providers/pbspro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/pbspro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/pbspro/pbspro.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/pbspro/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.396597 parsl-2023.5.15/parsl/providers/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/slurm/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/slurm/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.396597 parsl-2023.5.15/parsl/providers/torque/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/torque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/torque/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/providers/torque/torque.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.396597 parsl-2023.5.15/parsl/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/serialize/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/serialize/concretes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/serialize/facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.396597 parsl-2023.5.15/parsl/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/callables_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.400597 parsl-2023.5.15/parsl/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/ad_hoc_cluster_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/azure_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/cooley_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/cori.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/ec2_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/ec2_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/exex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/htex_ad_hoc_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/htex_local_alternate.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/htex_local_intask_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/htex_local_rsync_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/local_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/local_threads_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/local_threads_checkpoint_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/local_threads_checkpoint_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/local_threads_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/local_threads_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/local_threads_http_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/local_threads_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/local_threads_no_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/nscc_singapore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/osg_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/petrelkube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/swan_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/user_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/workqueue_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/configs/workqueue_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.400597 parsl-2023.5.15/parsl/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/integration/latency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.400597 parsl-2023.5.15/parsl/tests/integration/test_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/integration/test_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.400597 parsl-2023.5.15/parsl/tests/integration/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/integration/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/integration/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/integration/test_channels/test_local_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/integration/test_channels/test_scp_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/integration/test_channels/test_ssh_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/integration/test_channels/test_ssh_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/integration/test_channels/test_ssh_file_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/integration/test_channels/test_ssh_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/integration/test_parsl_load_default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.400597 parsl-2023.5.15/parsl/tests/integration/test_stress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/integration/test_stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/integration/test_stress/test_python_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/integration/test_stress/test_python_threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.404597 parsl-2023.5.15/parsl/tests/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/manual_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/manual_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/manual_tests/test_ad_hoc_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/manual_tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/manual_tests/test_log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/manual_tests/test_memory_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/manual_tests/test_oauth_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/manual_tests/test_udp_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/manual_tests/test_worker_count.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.404597 parsl-2023.5.15/parsl/tests/site_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/site_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/site_tests/site_config_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/site_tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/site_tests/test_site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.404597 parsl-2023.5.15/parsl/tests/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/sites/test_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/sites/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/sites/test_dynamic_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/sites/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/sites/test_launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/sites/test_local_adhoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.404597 parsl-2023.5.15/parsl/tests/sites/test_mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/sites/test_mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/sites/test_start_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/sites/test_worker_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_aalst_patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.404597 parsl-2023.5.15/parsl/tests/test_bash_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_bash_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_bash_apps/test_apptimeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_bash_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_bash_apps/test_error_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_bash_apps/test_file_bug_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_bash_apps/test_keyword_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_bash_apps/test_kwarg_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_bash_apps/test_memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_bash_apps/test_multiline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_bash_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_bash_apps/test_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_callables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.404597 parsl-2023.5.15/parsl/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_channels/test_large_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.404597 parsl-2023.5.15/parsl/tests/test_checkpointing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_checkpointing/test_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_checkpointing/test_regression_232.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_checkpointing/test_regression_233.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_checkpointing/test_regression_239.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_checkpointing/test_task_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.408597 parsl-2023.5.15/parsl/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_data/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_data/test_file_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_data/test_file_staging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.408597 parsl-2023.5.15/parsl/tests/test_docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_docs/test_from_slides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_docs/test_tutorial_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_docs/test_workflow1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_docs/test_workflow2.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_docs/test_workflow3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_docs/test_workflow4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.408597 parsl-2023.5.15/parsl/tests/test_error_handling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_error_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_error_handling/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_error_handling/test_htex_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_error_handling/test_htex_missing_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_error_handling/test_htex_worker_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_error_handling/test_python_walltime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_error_handling/test_rand_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_error_handling/test_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_error_handling/test_retries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_error_handling/test_retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_error_handling/test_retry_handler_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_error_handling/test_serialization_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_error_handling/test_wrap_with_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.408597 parsl-2023.5.15/parsl/tests/test_flowcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_flowcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_flowcontrol/test_one_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_flowcontrol/test_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.408597 parsl-2023.5.15/parsl/tests/test_manual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_manual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_manual/test_regression_220.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.408597 parsl-2023.5.15/parsl/tests/test_monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_monitoring/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_monitoring/test_db_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_monitoring/test_fuzz_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_monitoring/test_memoization_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.408597 parsl-2023.5.15/parsl/tests/test_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_providers/test_local_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.412598 parsl-2023.5.15/parsl/tests/test_python_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_arg_input_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_at_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_dep_standard_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_depfail_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_fibonacci_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_fibonacci_recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_garbage_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_import_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_mapred.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_memoize_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_memoize_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_memoize_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_memoize_joinapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_type5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_python_apps/test_worker_fail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.412598 parsl-2023.5.15/parsl/tests/test_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_regression/test_1480.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_regression/test_1653.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_regression/test_221.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_regression/test_226.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_regression/test_2652.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_regression/test_69a.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_regression/test_69b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_regression/test_854.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_regression/test_97.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_regression/test_98.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.412598 parsl-2023.5.15/parsl/tests/test_scaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_scaling/test_scale_down.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.416597 parsl-2023.5.15/parsl/tests/test_staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_staging/staging_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_staging/test_1316.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_staging/test_docs_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_staging/test_docs_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_staging/test_elaborate_noop_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_staging/test_staging_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_staging/test_staging_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_staging/test_staging_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_staging/test_staging_https.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_staging/test_staging_https_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_swift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_thread_parallelism.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.416597 parsl-2023.5.15/parsl/tests/test_threads/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_threads/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/test_threads/test_lazy_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.416597 parsl-2023.5.15/parsl/tests/workqueue_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/workqueue_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/workqueue_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/workqueue_tests/local_threads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3835 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/workqueue_tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/workqueue_tests/wqex_condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/tests/workqueue_tests/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.416597 parsl-2023.5.15/parsl/usage_tracking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/usage_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/usage_tracking/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-05-15 22:42:44.000000 parsl-2023.5.15/parsl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-15 22:42:48.000000 parsl-2023.5.15/parsl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:42:49.376597 parsl-2023.5.15/parsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-15 22:42:49.000000 parsl-2023.5.15/parsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-05-15 22:42:49.000000 parsl-2023.5.15/parsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:42:49.000000 parsl-2023.5.15/parsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-15 22:42:49.000000 parsl-2023.5.15/parsl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-15 22:42:49.000000 parsl-2023.5.15/parsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 22:42:49.000000 parsl-2023.5.15/parsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 22:42:44.000000 parsl-2023.5.15/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:42:49.416597 parsl-2023.5.15/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2624 2023-05-15 22:42:44.000000 parsl-2023.5.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.564188 parsl-2023.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 22:42:42.000000 parsl-2023.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-08 22:42:42.000000 parsl-2023.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-08 22:42:47.564188 parsl-2023.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-08 22:42:42.000000 parsl-2023.5.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/app/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/app/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/app/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/app/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/benchmark/perf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/channels/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/channels/oauth_ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/oauth_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/oauth_ssh/oauth_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/channels/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/channels/ssh_il/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/ssh_il/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/ssh_il/ssh_il.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/concurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.540188 parsl-2023.5.8/parsl/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/ASPIRE1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/Azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/ad_hoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/cooley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/cori.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/exex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/illinoiscluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/osg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/polaris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/stampede2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/toss3_llnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.540188 parsl-2023.5.8/parsl/data_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/file_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.540188 parsl-2023.5.8/parsl/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62334 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/dflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/executor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/flow_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/job_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/job_status_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/rundirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/taskrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.540188 parsl-2023.5.8/parsl/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.540188 parsl-2023.5.8/parsl/executors/extreme_scale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/extreme_scale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/extreme_scale/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18710 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/extreme_scale/mpi_worker_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.540188 parsl-2023.5.8/parsl/executors/flux/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/flux/execute_parsl_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/flux/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/flux/flux_instance_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/executors/high_throughput/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33199 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29929 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/interchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/manager_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/monitoring_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/probe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33007 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/process_worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/status_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/swift_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/executors/workqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/workqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/workqueue/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/workqueue/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47999 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/workqueue/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/workqueue/parsl_coprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/workqueue/parsl_coprocess_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/launchers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/launchers/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23301 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/monitoring/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/queries/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/radios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/monitoring/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/monitoring/visualization/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/monitoring/visualization/plots/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/plots/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/plots/default/task_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/plots/default/workflow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/monitoring/visualization/static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/static/parsl-logo-white.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/static/parsl-monitor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/monitoring/visualization/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/dag.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/resource_usage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/task.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/workflow.html
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/workflows_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/process_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/providers/ad_hoc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/ad_hoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/ad_hoc/ad_hoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29073 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/aws/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/aws/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18367 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/azure/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/azure/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/cluster_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/cobalt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/cobalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/cobalt/cobalt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/cobalt/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/condor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/condor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/condor/condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/condor/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/googlecloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/googlecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/googlecloud/googlecloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/grid_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/grid_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/grid_engine/grid_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/grid_engine/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/kubernetes/kube.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/kubernetes/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/lsf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/lsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/lsf/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/lsf/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/pbspro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/pbspro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/pbspro/pbspro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/pbspro/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/slurm/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/slurm/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/torque/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/torque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/torque/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/torque/torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/serialize/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/serialize/concretes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/serialize/facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/callables_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.552188 parsl-2023.5.8/parsl/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/ad_hoc_cluster_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/azure_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/cooley_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/cori.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/ec2_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/ec2_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/exex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/htex_ad_hoc_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/htex_local_alternate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/htex_local_intask_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/htex_local_rsync_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_checkpoint_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_checkpoint_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_http_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_no_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/nscc_singapore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/osg_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/petrelkube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/swan_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/user_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/workqueue_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/workqueue_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.552188 parsl-2023.5.8/parsl/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/latency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.552188 parsl-2023.5.8/parsl/tests/integration/test_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.552188 parsl-2023.5.8/parsl/tests/integration/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/test_local_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/test_scp_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_file_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_parsl_load_default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.552188 parsl-2023.5.8/parsl/tests/integration/test_stress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_stress/test_python_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_stress/test_python_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.552188 parsl-2023.5.8/parsl/tests/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_ad_hoc_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_memory_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_oauth_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_udp_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_worker_count.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/site_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/site_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/site_tests/site_config_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/site_tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/site_tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_dynamic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_local_adhoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/sites/test_mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_start_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_worker_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_aalst_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/test_bash_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_apptimeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_file_bug_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_keyword_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_kwarg_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_callables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_channels/test_large_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/test_checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_regression_232.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_regression_233.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_regression_239.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_task_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_data/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_data/test_file_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_data/test_file_staging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/test_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_docs/test_from_slides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_docs/test_tutorial_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_docs/test_workflow1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_docs/test_workflow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_docs/test_workflow3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_docs/test_workflow4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.560188 parsl-2023.5.8/parsl/tests/test_error_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_htex_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_htex_missing_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_htex_worker_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_python_walltime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_rand_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_retry_handler_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_serialization_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_wrap_with_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.560188 parsl-2023.5.8/parsl/tests/test_flowcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_flowcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_flowcontrol/test_one_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_flowcontrol/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.560188 parsl-2023.5.8/parsl/tests/test_manual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_manual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_manual/test_regression_220.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.560188 parsl-2023.5.8/parsl/tests/test_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_monitoring/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_monitoring/test_db_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_monitoring/test_fuzz_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_monitoring/test_memoization_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.560188 parsl-2023.5.8/parsl/tests/test_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_providers/test_local_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.560188 parsl-2023.5.8/parsl/tests/test_python_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_arg_input_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_at_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_dep_standard_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_depfail_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_fibonacci_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_fibonacci_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_garbage_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_import_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_mapred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_joinapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_type5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_worker_fail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.564188 parsl-2023.5.8/parsl/tests/test_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_1480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_1653.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_221.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_226.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_2652.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_69a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_69b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_854.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_97.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_98.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.564188 parsl-2023.5.8/parsl/tests/test_scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_scaling/test_scale_down.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.564188 parsl-2023.5.8/parsl/tests/test_staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/staging_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_1316.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_docs_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_docs_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_elaborate_noop_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_staging_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_staging_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_staging_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_staging_https.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_staging_https_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_swift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_thread_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.564188 parsl-2023.5.8/parsl/tests/test_threads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_threads/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_threads/test_lazy_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.564188 parsl-2023.5.8/parsl/tests/workqueue_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/workqueue_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/workqueue_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/workqueue_tests/local_threads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3835 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/workqueue_tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/workqueue_tests/wqex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/workqueue_tests/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.564188 parsl-2023.5.8/parsl/usage_tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/usage_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/usage_tracking/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-08 22:42:46.000000 parsl-2023.5.8/parsl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-08 22:42:47.000000 parsl-2023.5.8/parsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-05-08 22:42:47.000000 parsl-2023.5.8/parsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:42:47.000000 parsl-2023.5.8/parsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-08 22:42:47.000000 parsl-2023.5.8/parsl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-08 22:42:47.000000 parsl-2023.5.8/parsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 22:42:47.000000 parsl-2023.5.8/parsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-08 22:42:42.000000 parsl-2023.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 22:42:47.564188 parsl-2023.5.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2624 2023-05-08 22:42:42.000000 parsl-2023.5.8/setup.py
```

### Comparing `parsl-2023.5.15/LICENSE` & `parsl-2023.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/PKG-INFO` & `parsl-2023.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2023.5.15
+Version: 2023.5.8
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2023.05.15.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2023.05.08.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2023.5.15/README.rst` & `parsl-2023.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/__init__.py` & `parsl-2023.5.8/parsl/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/addresses.py` & `parsl-2023.5.8/parsl/addresses.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/app/app.py` & `parsl-2023.5.8/parsl/app/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/app/bash.py` & `parsl-2023.5.8/parsl/app/bash.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/app/errors.py` & `parsl-2023.5.8/parsl/app/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/app/futures.py` & `parsl-2023.5.8/parsl/app/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/app/python.py` & `parsl-2023.5.8/parsl/app/python.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/benchmark/perf.py` & `parsl-2023.5.8/parsl/benchmark/perf.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/channels/base.py` & `parsl-2023.5.8/parsl/channels/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/channels/errors.py` & `parsl-2023.5.8/parsl/channels/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/channels/local/local.py` & `parsl-2023.5.8/parsl/channels/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/channels/oauth_ssh/oauth_ssh.py` & `parsl-2023.5.8/parsl/channels/oauth_ssh/oauth_ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/channels/ssh/ssh.py` & `parsl-2023.5.8/parsl/channels/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/channels/ssh_il/ssh_il.py` & `parsl-2023.5.8/parsl/channels/ssh_il/ssh_il.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/concurrent/__init__.py` & `parsl-2023.5.8/parsl/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/config.py` & `parsl-2023.5.8/parsl/config.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/ASPIRE1.py` & `parsl-2023.5.8/parsl/configs/ASPIRE1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/Azure.py` & `parsl-2023.5.8/parsl/configs/Azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/ad_hoc.py` & `parsl-2023.5.8/parsl/configs/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/bluewaters.py` & `parsl-2023.5.8/parsl/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/bridges.py` & `parsl-2023.5.8/parsl/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/cc_in2p3.py` & `parsl-2023.5.8/parsl/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/comet.py` & `parsl-2023.5.8/parsl/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/cooley.py` & `parsl-2023.5.8/parsl/configs/cooley.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/cori.py` & `parsl-2023.5.8/parsl/configs/cori.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/ec2.py` & `parsl-2023.5.8/parsl/configs/ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/exex_local.py` & `parsl-2023.5.8/parsl/configs/exex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/frontera.py` & `parsl-2023.5.8/parsl/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/illinoiscluster.py` & `parsl-2023.5.8/parsl/configs/illinoiscluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/kubernetes.py` & `parsl-2023.5.8/parsl/configs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/midway.py` & `parsl-2023.5.8/parsl/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/osg.py` & `parsl-2023.5.8/parsl/configs/osg.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/polaris.py` & `parsl-2023.5.8/parsl/configs/polaris.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/stampede2.py` & `parsl-2023.5.8/parsl/configs/stampede2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/summit.py` & `parsl-2023.5.8/parsl/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/theta.py` & `parsl-2023.5.8/parsl/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/toss3_llnl.py` & `parsl-2023.5.8/parsl/configs/toss3_llnl.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/configs/wqex_local.py` & `parsl-2023.5.8/parsl/configs/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/data_provider/data_manager.py` & `parsl-2023.5.8/parsl/data_provider/data_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/data_provider/files.py` & `parsl-2023.5.8/parsl/data_provider/files.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/data_provider/ftp.py` & `parsl-2023.5.8/parsl/data_provider/ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/data_provider/globus.py` & `parsl-2023.5.8/parsl/data_provider/globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/data_provider/http.py` & `parsl-2023.5.8/parsl/data_provider/http.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/data_provider/rsync.py` & `parsl-2023.5.8/parsl/data_provider/rsync.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/data_provider/staging.py` & `parsl-2023.5.8/parsl/data_provider/staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/dataflow/dflow.py` & `parsl-2023.5.8/parsl/dataflow/dflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1351,34 +1351,36 @@
                 logger.error(reason)
                 raise BadCheckpoint(reason)
 
             logger.info("Completed loading checkpoint: {0} with {1} tasks".format(checkpoint_file,
                                                                                   len(memo_lookup_table.keys())))
         return memo_lookup_table
 
-    @typeguard.typechecked
-    def load_checkpoints(self, checkpointDirs: Optional[Sequence[str]]) -> Dict[str, Future]:
+    def load_checkpoints(self, checkpointDirs):
         """Load checkpoints from the checkpoint files into a dictionary.
 
         The results are used to pre-populate the memoizer's lookup_table
 
         Kwargs:
              - checkpointDirs (list) : List of run folder to use as checkpoints
                Eg. ['runinfo/001', 'runinfo/002']
 
         Returns:
              - dict containing, hashed -> future mappings
         """
         self.memo_lookup_table = None
 
-        if checkpointDirs:
-            return self._load_checkpoints(checkpointDirs)
-        else:
+        if not checkpointDirs:
             return {}
 
+        if type(checkpointDirs) is not list:
+            raise BadCheckpoint("checkpointDirs expects a list of checkpoints")
+
+        return self._load_checkpoints(checkpointDirs)
+
     @staticmethod
     def _log_std_streams(task_record: TaskRecord) -> None:
         if task_record['app_fu'].stdout is not None:
             logger.info("Standard output for task {} available at {}".format(task_record['id'], task_record['app_fu'].stdout))
         if task_record['app_fu'].stderr is not None:
             logger.info("Standard error for task {} available at {}".format(task_record['id'], task_record['app_fu'].stderr))
```

### Comparing `parsl-2023.5.15/parsl/dataflow/errors.py` & `parsl-2023.5.8/parsl/dataflow/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/dataflow/futures.py` & `parsl-2023.5.8/parsl/dataflow/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/dataflow/job_error_handler.py` & `parsl-2023.5.8/parsl/dataflow/job_error_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/dataflow/job_status_poller.py` & `parsl-2023.5.8/parsl/dataflow/job_status_poller.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/dataflow/memoization.py` & `parsl-2023.5.8/parsl/dataflow/memoization.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/dataflow/rundirs.py` & `parsl-2023.5.8/parsl/dataflow/rundirs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/dataflow/states.py` & `parsl-2023.5.8/parsl/dataflow/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/dataflow/strategy.py` & `parsl-2023.5.8/parsl/dataflow/strategy.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/dataflow/taskrecord.py` & `parsl-2023.5.8/parsl/dataflow/taskrecord.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/errors.py` & `parsl-2023.5.8/parsl/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/base.py` & `parsl-2023.5.8/parsl/executors/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import parsl  # noqa F401
 
 
 class ParslExecutor(metaclass=ABCMeta):
     """Executors are abstractions that represent available compute resources
     to which you could submit arbitrary App tasks.
 
-    This is an abstract base class that only enforces concrete implementations
-    of functionality by the child classes.
+    This is a metaclass that only enforces concrete implementations of
+    functionality by the child classes.
 
     Can be used as a context manager. On exit, calls ``self.shutdown()`` with
     no arguments and re-raises any thrown exception.
 
     In addition to the listed methods, a ParslExecutor instance must always
     have a member field:
 
@@ -72,14 +72,18 @@
         """
         pass
 
     @abstractmethod
     def scale_out(self, blocks: int) -> List[str]:
         """Scale out method.
 
+        We should have the scale out method simply take resource object
+        which will have the scaling methods, scale_out itself should be a coroutine, since
+        scaling tasks can be slow.
+
         :return: A list of block ids corresponding to the blocks that were added.
         """
         pass
 
     @abstractmethod
     def scale_in(self, blocks: int) -> List[str]:
         """Scale in method.
```

### Comparing `parsl-2023.5.15/parsl/executors/errors.py` & `parsl-2023.5.8/parsl/executors/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/extreme_scale/executor.py` & `parsl-2023.5.8/parsl/executors/extreme_scale/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/extreme_scale/mpi_worker_pool.py` & `parsl-2023.5.8/parsl/executors/extreme_scale/mpi_worker_pool.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/flux/execute_parsl_task.py` & `parsl-2023.5.8/parsl/executors/flux/execute_parsl_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/flux/executor.py` & `parsl-2023.5.8/parsl/executors/flux/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/flux/flux_instance_manager.py` & `parsl-2023.5.8/parsl/executors/flux/flux_instance_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/high_throughput/executor.py` & `parsl-2023.5.8/parsl/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/high_throughput/interchange.py` & `parsl-2023.5.8/parsl/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/high_throughput/probe.py` & `parsl-2023.5.8/parsl/executors/high_throughput/probe.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/high_throughput/process_worker_pool.py` & `parsl-2023.5.8/parsl/executors/high_throughput/process_worker_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -590,15 +590,15 @@
             worker_queue.get()
         except queue.Empty:
             logger.warning("Worker ID: {} failed to remove itself from ready_worker_queue".format(worker_id))
             pass
 
         try:
             result = execute_task(req['buffer'])
-            serialized_result = serialize(result, buffer_threshold=1000000)
+            serialized_result = serialize(result, buffer_threshold=1e6)
         except Exception as e:
             logger.info('Caught an exception: {}'.format(e))
             result_package = {'type': 'result', 'task_id': tid, 'exception': serialize(RemoteExceptionWrapper(*sys.exc_info()))}
         else:
             result_package = {'type': 'result', 'task_id': tid, 'result': serialized_result}
             # logger.debug("Result: {}".format(result))
```

### Comparing `parsl-2023.5.15/parsl/executors/high_throughput/zmq_pipes.py` & `parsl-2023.5.8/parsl/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/status_handling.py` & `parsl-2023.5.8/parsl/executors/status_handling.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/swift_t.py` & `parsl-2023.5.8/parsl/executors/swift_t.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/threads.py` & `parsl-2023.5.8/parsl/executors/threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/workqueue/exec_parsl_function.py` & `parsl-2023.5.8/parsl/executors/workqueue/exec_parsl_function.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/workqueue/executor.py` & `parsl-2023.5.8/parsl/executors/workqueue/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/workqueue/parsl_coprocess.py` & `parsl-2023.5.8/parsl/executors/workqueue/parsl_coprocess.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/executors/workqueue/parsl_coprocess_stub.py` & `parsl-2023.5.8/parsl/executors/workqueue/parsl_coprocess_stub.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/launchers/__init__.py` & `parsl-2023.5.8/parsl/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/launchers/launchers.py` & `parsl-2023.5.8/parsl/launchers/launchers.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/log_utils.py` & `parsl-2023.5.8/parsl/log_utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/db_manager.py` & `parsl-2023.5.8/parsl/monitoring/db_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/monitoring.py` & `parsl-2023.5.8/parsl/monitoring/monitoring.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/queries/pandas.py` & `parsl-2023.5.8/parsl/monitoring/queries/pandas.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/radios.py` & `parsl-2023.5.8/parsl/monitoring/radios.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/remote.py` & `parsl-2023.5.8/parsl/monitoring/remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/types.py` & `parsl-2023.5.8/parsl/monitoring/types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/visualization/app.py` & `parsl-2023.5.8/parsl/monitoring/visualization/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/visualization/models.py` & `parsl-2023.5.8/parsl/monitoring/visualization/models.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/visualization/plots/default/task_plots.py` & `parsl-2023.5.8/parsl/monitoring/visualization/plots/default/task_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/visualization/plots/default/workflow_plots.py` & `parsl-2023.5.8/parsl/monitoring/visualization/plots/default/workflow_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py` & `parsl-2023.5.8/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/visualization/static/parsl-logo-white.png` & `parsl-2023.5.8/parsl/monitoring/visualization/static/parsl-logo-white.png`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/visualization/templates/app.html` & `parsl-2023.5.8/parsl/monitoring/visualization/templates/app.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/visualization/templates/dag.html` & `parsl-2023.5.8/parsl/monitoring/visualization/templates/dag.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/visualization/templates/layout.html` & `parsl-2023.5.8/parsl/monitoring/visualization/templates/layout.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/visualization/templates/resource_usage.html` & `parsl-2023.5.8/parsl/monitoring/visualization/templates/resource_usage.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/visualization/templates/task.html` & `parsl-2023.5.8/parsl/monitoring/visualization/templates/task.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/visualization/templates/workflow.html` & `parsl-2023.5.8/parsl/monitoring/visualization/templates/workflow.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/visualization/templates/workflows_summary.html` & `parsl-2023.5.8/parsl/monitoring/visualization/templates/workflows_summary.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/monitoring/visualization/views.py` & `parsl-2023.5.8/parsl/monitoring/visualization/views.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/multiprocessing.py` & `parsl-2023.5.8/parsl/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/process_loggers.py` & `parsl-2023.5.8/parsl/process_loggers.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/__init__.py` & `parsl-2023.5.8/parsl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/ad_hoc/ad_hoc.py` & `parsl-2023.5.8/parsl/providers/ad_hoc/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/aws/aws.py` & `parsl-2023.5.8/parsl/providers/aws/aws.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/azure/azure.py` & `parsl-2023.5.8/parsl/providers/azure/azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/base.py` & `parsl-2023.5.8/parsl/providers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/cluster_provider.py` & `parsl-2023.5.8/parsl/providers/cluster_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/cobalt/cobalt.py` & `parsl-2023.5.8/parsl/providers/cobalt/cobalt.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/condor/condor.py` & `parsl-2023.5.8/parsl/providers/condor/condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/condor/template.py` & `parsl-2023.5.8/parsl/providers/condor/template.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/errors.py` & `parsl-2023.5.8/parsl/providers/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/googlecloud/googlecloud.py` & `parsl-2023.5.8/parsl/providers/googlecloud/googlecloud.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/grid_engine/grid_engine.py` & `parsl-2023.5.8/parsl/providers/grid_engine/grid_engine.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/kubernetes/kube.py` & `parsl-2023.5.8/parsl/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/local/local.py` & `parsl-2023.5.8/parsl/providers/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/lsf/lsf.py` & `parsl-2023.5.8/parsl/providers/lsf/lsf.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/pbspro/pbspro.py` & `parsl-2023.5.8/parsl/providers/pbspro/pbspro.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/slurm/slurm.py` & `parsl-2023.5.8/parsl/providers/slurm/slurm.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/providers/torque/torque.py` & `parsl-2023.5.8/parsl/providers/torque/torque.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/serialize/concretes.py` & `parsl-2023.5.8/parsl/serialize/concretes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 import dill
 import pickle
 import logging
 
 logger = logging.getLogger(__name__)
 from parsl.serialize.base import SerializerBase
 
-from typing import Any
-
 
 class PickleSerializer(SerializerBase):
     """ Pickle serialization covers most python objects, with some notable exceptions:
 
     * functions defined in a interpreter/notebook
     * classes defined in local context and not importable using a fully qualified name
     * closures, generators and coroutines
     * [sometimes] issues with wrapped/decorated functions
     """
 
     _identifier = b'01\n'
     _for_code = True
     _for_data = True
 
-    def serialize(self, data: Any) -> bytes:
+    def serialize(self, data):
         x = pickle.dumps(data)
         return self.identifier + x
 
-    def deserialize(self, payload: bytes) -> Any:
+    def deserialize(self, payload):
         chomped = self.chomp(payload)
         data = pickle.loads(chomped)
         return data
 
 
 class DillSerializer(SerializerBase):
     """ Dill serialization works on a superset of object including the ones covered by pickle.
@@ -43,15 +41,15 @@
     * closures
     """
 
     _identifier = b'02\n'
     _for_code = True
     _for_data = True
 
-    def serialize(self, data: Any) -> bytes:
+    def serialize(self, data):
         x = dill.dumps(data)
         return self.identifier + x
 
-    def deserialize(self, payload: bytes) -> Any:
+    def deserialize(self, payload):
         chomped = self.chomp(payload)
         data = dill.loads(chomped)
         return data
```

### Comparing `parsl-2023.5.15/parsl/serialize/facade.py` & `parsl-2023.5.8/parsl/serialize/facade.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from parsl.serialize.concretes import *  # noqa: F403,F401
-from parsl.serialize.base import METHODS_MAP_DATA, METHODS_MAP_CODE, SerializerBase
+from parsl.serialize.base import METHODS_MAP_DATA, METHODS_MAP_CODE
 import logging
 
-from typing import Any, Dict, List, Tuple, Union
-
 logger = logging.getLogger(__name__)
 
 
 """ Instantiate the appropriate classes
 """
 headers = list(METHODS_MAP_CODE.keys()) + list(METHODS_MAP_DATA.keys())
 header_size = len(headers[0])
@@ -19,140 +17,144 @@
     methods_for_code[key] = METHODS_MAP_CODE[key]()
     methods_for_code[key].enable_caching(maxsize=128)
 
     for key in METHODS_MAP_DATA:
         methods_for_data[key] = METHODS_MAP_DATA[key]()
 
 
-def _list_methods() -> Tuple[Dict[bytes, SerializerBase], Dict[bytes, SerializerBase]]:
+def _list_methods():
     return methods_for_code, methods_for_data
 
 
-def pack_apply_message(func: Any, args: Any, kwargs: Any, buffer_threshold: int = int(128 * 1e6)) -> bytes:
+def pack_apply_message(func, args, kwargs, buffer_threshold=128 * 1e6):
     """Serialize and pack function and parameters
 
     Parameters
     ----------
 
     func: Function
         A function to ship
 
     args: Tuple/list of objects
         positional parameters as a list
 
     kwargs: Dict
         Dict containing named parameters
 
-    buffer_threshold: int
+    buffer_threshold: Ignored
         Limits buffer to specified size in bytes. Exceeding this limit would give you
         a warning in the log. Default is 128MB.
     """
     b_func = serialize(func, buffer_threshold=buffer_threshold)
     b_args = serialize(args, buffer_threshold=buffer_threshold)
     b_kwargs = serialize(kwargs, buffer_threshold=buffer_threshold)
     packed_buffer = pack_buffers([b_func, b_args, b_kwargs])
     return packed_buffer
 
 
-def unpack_apply_message(packed_buffer: bytes, user_ns: Any = None, copy: Any = False) -> List[Any]:
+def unpack_apply_message(packed_buffer, user_ns=None, copy=False):
     """ Unpack and deserialize function and parameters
 
     """
     return [deserialize(buf) for buf in unpack_buffers(packed_buffer)]
 
 
-def serialize(obj: Any, buffer_threshold: int = int(1e6)) -> bytes:
+def serialize(obj, buffer_threshold=1e6):
     """ Try available serialization methods one at a time
 
     Individual serialization methods might raise a TypeError (eg. if objects are non serializable)
     This method will raise the exception from the last method that was tried, if all methods fail.
     """
-    result: Union[bytes, Exception]
+    serialized = None
+    serialized_flag = False
+    last_exception = None
     if callable(obj):
         for method in methods_for_code.values():
             try:
-                result = method.serialize(obj)
+                serialized = method.serialize(obj)
             except Exception as e:
-                result = e
+                last_exception = e
                 continue
             else:
+                serialized_flag = True
                 break
     else:
         for method in methods_for_data.values():
             try:
-                result = method.serialize(obj)
+                serialized = method.serialize(obj)
             except Exception as e:
-                result = e
+                last_exception = e
                 continue
             else:
+                serialized_flag = True
                 break
 
-    if isinstance(result, BaseException):
-        raise result
-    else:
-        if len(result) > buffer_threshold:
-            logger.warning(f"Serialized object exceeds buffer threshold of {buffer_threshold} bytes, this could cause overflows")
-        return result
+    if serialized_flag is False:
+        # TODO : Replace with a SerializationError
+        raise last_exception
+
+    if len(serialized) > buffer_threshold:
+        logger.warning(f"Serialized object exceeds buffer threshold of {buffer_threshold} bytes, this could cause overflows")
+    return serialized
 
 
-def deserialize(payload: bytes) -> Any:
+def deserialize(payload):
     """
     Parameters
     ----------
     payload : str
        Payload object to be deserialized
 
     """
     header = payload[0:header_size]
     if header in methods_for_code:
         result = methods_for_code[header].deserialize(payload)
     elif header in methods_for_data:
         result = methods_for_data[header].deserialize(payload)
     else:
-        raise TypeError("Invalid header: {!r} in data payload. Buffer is either corrupt or not created by ParslSerializer".format(header))
+        raise TypeError("Invalid header: {} in data payload. Buffer is either corrupt or not created by ParslSerializer".format(header))
 
     return result
 
 
-def pack_buffers(buffers: List[bytes]) -> bytes:
+def pack_buffers(buffers):
     """
     Parameters
     ----------
-    buffers: list of byte strings
+    buffers : list of \n terminated strings
     """
     packed = b''
     for buf in buffers:
         s_length = bytes(str(len(buf)) + '\n', 'utf-8')
         packed += s_length + buf
 
     return packed
 
 
-def unpack_buffers(packed_buffer: bytes) -> List[bytes]:
+def unpack_buffers(packed_buffer):
     """
     Parameters
     ----------
-    packed_buffers : packed buffer as byte sequence
+    packed_buffers : packed buffer as string
     """
     unpacked = []
     while packed_buffer:
         s_length, buf = packed_buffer.split(b'\n', 1)
         i_length = int(s_length.decode('utf-8'))
         current, packed_buffer = buf[:i_length], buf[i_length:]
         unpacked.extend([current])
 
     return unpacked
 
 
-def unpack_and_deserialize(packed_buffer: bytes) -> Any:
-    """ Unpacks a packed buffer of 3 byte sequences and returns the
-    deserialized contents for use in function application.
+def unpack_and_deserialize(packed_buffer):
+    """ Unpacks a packed buffer and returns the deserialized contents
     Parameters
     ----------
-    packed_buffers : packed buffer of 3 byte sequences
+    packed_buffers : packed buffer as string
     """
     unpacked = []
     while packed_buffer:
         s_length, buf = packed_buffer.split(b'\n', 1)
         i_length = int(s_length.decode('utf-8'))
         current, packed_buffer = buf[:i_length], buf[i_length:]
         deserialized = deserialize(current)
```

### Comparing `parsl-2023.5.15/parsl/tests/configs/ad_hoc_cluster_htex.py` & `parsl-2023.5.8/parsl/tests/configs/ad_hoc_cluster_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/azure_single_node.py` & `parsl-2023.5.8/parsl/tests/configs/azure_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/bluewaters.py` & `parsl-2023.5.8/parsl/tests/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/bridges.py` & `parsl-2023.5.8/parsl/tests/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/cc_in2p3.py` & `parsl-2023.5.8/parsl/tests/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/comet.py` & `parsl-2023.5.8/parsl/tests/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/cooley_htex.py` & `parsl-2023.5.8/parsl/tests/configs/cooley_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/cori.py` & `parsl-2023.5.8/parsl/tests/configs/cori.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/ec2_single_node.py` & `parsl-2023.5.8/parsl/tests/configs/ec2_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/ec2_spot.py` & `parsl-2023.5.8/parsl/tests/configs/ec2_spot.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/exex_local.py` & `parsl-2023.5.8/parsl/tests/configs/exex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/frontera.py` & `parsl-2023.5.8/parsl/tests/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/htex_ad_hoc_cluster.py` & `parsl-2023.5.8/parsl/tests/configs/htex_ad_hoc_cluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/htex_local.py` & `parsl-2023.5.8/parsl/tests/configs/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/htex_local_alternate.py` & `parsl-2023.5.8/parsl/tests/configs/htex_local_alternate.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/htex_local_intask_staging.py` & `parsl-2023.5.8/parsl/tests/configs/htex_local_intask_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/htex_local_rsync_staging.py` & `parsl-2023.5.8/parsl/tests/configs/htex_local_rsync_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/local_threads_globus.py` & `parsl-2023.5.8/parsl/tests/configs/local_threads_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/midway.py` & `parsl-2023.5.8/parsl/tests/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/nscc_singapore.py` & `parsl-2023.5.8/parsl/tests/configs/nscc_singapore.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/osg_htex.py` & `parsl-2023.5.8/parsl/tests/configs/osg_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/petrelkube.py` & `parsl-2023.5.8/parsl/tests/configs/petrelkube.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/summit.py` & `parsl-2023.5.8/parsl/tests/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/swan_htex.py` & `parsl-2023.5.8/parsl/tests/configs/swan_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/theta.py` & `parsl-2023.5.8/parsl/tests/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/user_opts.py` & `parsl-2023.5.8/parsl/tests/configs/user_opts.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/configs/workqueue_blocks.py` & `parsl-2023.5.8/parsl/tests/configs/workqueue_blocks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/conftest.py` & `parsl-2023.5.8/parsl/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/integration/latency.py` & `parsl-2023.5.8/parsl/tests/integration/latency.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/integration/test_channels/test_local_channel.py` & `parsl-2023.5.8/parsl/tests/integration/test_channels/test_local_channel.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/integration/test_channels/test_scp_1.py` & `parsl-2023.5.8/parsl/tests/integration/test_channels/test_scp_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/integration/test_channels/test_ssh_1.py` & `parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/integration/test_channels/test_ssh_errors.py` & `parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/integration/test_channels/test_ssh_file_transport.py` & `parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_file_transport.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/integration/test_channels/test_ssh_interactive.py` & `parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_interactive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/integration/test_stress/test_python_simple.py` & `parsl-2023.5.8/parsl/tests/integration/test_stress/test_python_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/integration/test_stress/test_python_threads.py` & `parsl-2023.5.8/parsl/tests/integration/test_stress/test_python_threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/manual_tests/htex_local.py` & `parsl-2023.5.8/parsl/tests/manual_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/manual_tests/test_ad_hoc_htex.py` & `parsl-2023.5.8/parsl/tests/manual_tests/test_ad_hoc_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/manual_tests/test_basic.py` & `parsl-2023.5.8/parsl/tests/manual_tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py` & `parsl-2023.5.8/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/manual_tests/test_log_filter.py` & `parsl-2023.5.8/parsl/tests/manual_tests/test_log_filter.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/manual_tests/test_memory_limits.py` & `parsl-2023.5.8/parsl/tests/manual_tests/test_memory_limits.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/manual_tests/test_udp_simple.py` & `parsl-2023.5.8/parsl/tests/manual_tests/test_udp_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/manual_tests/test_worker_count.py` & `parsl-2023.5.8/parsl/tests/manual_tests/test_worker_count.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/site_tests/site_config_selector.py` & `parsl-2023.5.8/parsl/tests/site_tests/site_config_selector.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/site_tests/test_provider.py` & `parsl-2023.5.8/parsl/tests/site_tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/site_tests/test_site.py` & `parsl-2023.5.8/parsl/tests/site_tests/test_site.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/sites/test_affinity.py` & `parsl-2023.5.8/parsl/tests/sites/test_affinity.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/sites/test_concurrent.py` & `parsl-2023.5.8/parsl/tests/sites/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/sites/test_dynamic_executor.py` & `parsl-2023.5.8/parsl/tests/sites/test_dynamic_executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/sites/test_ec2.py` & `parsl-2023.5.8/parsl/tests/sites/test_ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/sites/test_local_adhoc.py` & `parsl-2023.5.8/parsl/tests/sites/test_local_adhoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/sites/test_start_method.py` & `parsl-2023.5.8/parsl/tests/sites/test_start_method.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/sites/test_worker_info.py` & `parsl-2023.5.8/parsl/tests/sites/test_worker_info.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_aalst_patterns.py` & `parsl-2023.5.8/parsl/tests/test_aalst_patterns.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_bash_apps/test_apptimeout.py` & `parsl-2023.5.8/parsl/tests/test_bash_apps/test_apptimeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_bash_apps/test_basic.py` & `parsl-2023.5.8/parsl/tests/test_bash_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_bash_apps/test_error_codes.py` & `parsl-2023.5.8/parsl/tests/test_bash_apps/test_error_codes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_bash_apps/test_file_bug_1.py` & `parsl-2023.5.8/parsl/tests/test_bash_apps/test_file_bug_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_bash_apps/test_kwarg_storage.py` & `parsl-2023.5.8/parsl/tests/test_bash_apps/test_kwarg_storage.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_bash_apps/test_memoize.py` & `parsl-2023.5.8/parsl/tests/test_bash_apps/test_memoize.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_bash_apps/test_memoize_ignore_args.py` & `parsl-2023.5.8/parsl/tests/test_bash_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py` & `parsl-2023.5.8/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_bash_apps/test_multiline.py` & `parsl-2023.5.8/parsl/tests/test_bash_apps/test_multiline.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_bash_apps/test_pipeline.py` & `parsl-2023.5.8/parsl/tests/test_bash_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_bash_apps/test_stdout.py` & `parsl-2023.5.8/parsl/tests/test_bash_apps/test_stdout.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_callables.py` & `parsl-2023.5.8/parsl/tests/test_callables.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_channels/test_large_output.py` & `parsl-2023.5.8/parsl/tests/test_channels/test_large_output.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_checkpointing/test_periodic.py` & `parsl-2023.5.8/parsl/tests/test_checkpointing/test_periodic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_checkpointing/test_python_checkpoint_1.py` & `parsl-2023.5.8/parsl/tests/test_checkpointing/test_python_checkpoint_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_checkpointing/test_python_checkpoint_2.py` & `parsl-2023.5.8/parsl/tests/test_checkpointing/test_python_checkpoint_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_checkpointing/test_python_checkpoint_3.py` & `parsl-2023.5.8/parsl/tests/test_checkpointing/test_python_checkpoint_3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_checkpointing/test_regression_232.py` & `parsl-2023.5.8/parsl/tests/test_checkpointing/test_regression_232.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_checkpointing/test_regression_233.py` & `parsl-2023.5.8/parsl/tests/test_checkpointing/test_regression_233.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_checkpointing/test_regression_239.py` & `parsl-2023.5.8/parsl/tests/test_checkpointing/test_regression_239.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_checkpointing/test_task_exit.py` & `parsl-2023.5.8/parsl/tests/test_checkpointing/test_task_exit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_data/test_file.py` & `parsl-2023.5.8/parsl/tests/test_data/test_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_data/test_file_apps.py` & `parsl-2023.5.8/parsl/tests/test_data/test_file_apps.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_data/test_file_staging.py` & `parsl-2023.5.8/parsl/tests/test_data/test_file_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_docs/test_from_slides.py` & `parsl-2023.5.8/parsl/tests/test_docs/test_from_slides.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_docs/test_tutorial_1.py` & `parsl-2023.5.8/parsl/tests/test_docs/test_tutorial_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_docs/test_workflow1.py` & `parsl-2023.5.8/parsl/tests/test_docs/test_workflow1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_docs/test_workflow2.py` & `parsl-2023.5.8/parsl/tests/test_docs/test_workflow2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_docs/test_workflow3.py` & `parsl-2023.5.8/parsl/tests/test_docs/test_workflow3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_docs/test_workflow4.py` & `parsl-2023.5.8/parsl/tests/test_docs/test_workflow4.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_error_handling/test_htex_missing_worker.py` & `parsl-2023.5.8/parsl/tests/test_error_handling/test_htex_missing_worker.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_error_handling/test_htex_worker_failure.py` & `parsl-2023.5.8/parsl/tests/test_error_handling/test_htex_worker_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_error_handling/test_python_walltime.py` & `parsl-2023.5.8/parsl/tests/test_error_handling/test_python_walltime.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_error_handling/test_rand_fail.py` & `parsl-2023.5.8/parsl/tests/test_error_handling/test_rand_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_error_handling/test_resource_spec.py` & `parsl-2023.5.8/parsl/tests/test_error_handling/test_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_error_handling/test_retries.py` & `parsl-2023.5.8/parsl/tests/test_error_handling/test_retries.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_error_handling/test_retry_handler.py` & `parsl-2023.5.8/parsl/tests/test_error_handling/test_retry_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_error_handling/test_retry_handler_failure.py` & `parsl-2023.5.8/parsl/tests/test_error_handling/test_retry_handler_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_error_handling/test_serialization_fail.py` & `parsl-2023.5.8/parsl/tests/test_error_handling/test_serialization_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_error_handling/test_wrap_with_logs.py` & `parsl-2023.5.8/parsl/tests/test_error_handling/test_wrap_with_logs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_flowcontrol/test_one_block.py` & `parsl-2023.5.8/parsl/tests/test_flowcontrol/test_one_block.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_flowcontrol/test_python.py` & `parsl-2023.5.8/parsl/tests/test_flowcontrol/test_python.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_flux.py` & `parsl-2023.5.8/parsl/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_manual/test_regression_220.py` & `parsl-2023.5.8/parsl/tests/test_manual/test_regression_220.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_monitoring/test_basic.py` & `parsl-2023.5.8/parsl/tests/test_monitoring/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_monitoring/test_db_locks.py` & `parsl-2023.5.8/parsl/tests/test_monitoring/test_db_locks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_monitoring/test_fuzz_zmq.py` & `parsl-2023.5.8/parsl/tests/test_monitoring/test_fuzz_zmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_monitoring/test_memoization_representation.py` & `parsl-2023.5.8/parsl/tests/test_monitoring/test_memoization_representation.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_providers/test_local_provider.py` & `parsl-2023.5.8/parsl/tests/test_providers/test_local_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_arg_input_types.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_arg_input_types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_at_scale.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_at_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_basic.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_dep_standard_futures.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_dep_standard_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_depfail_propagation.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_depfail_propagation.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_fail.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_fibonacci_iterative.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_fibonacci_iterative.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_fibonacci_recursive.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_fibonacci_recursive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_futures.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_garbage_collect.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_garbage_collect.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_import_fail.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_import_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_join.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_join.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_mapred.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_mapred.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_memoize_1.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_memoize_2.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_memoize_4.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_4.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_memoize_ignore_args.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_outputs.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_outputs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_overview.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_overview.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_pipeline.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_simple.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_type5.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_type5.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_python_apps/test_worker_fail.py` & `parsl-2023.5.8/parsl/tests/test_python_apps/test_worker_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_regression/test_1480.py` & `parsl-2023.5.8/parsl/tests/test_regression/test_1480.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py` & `parsl-2023.5.8/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_regression/test_1653.py` & `parsl-2023.5.8/parsl/tests/test_regression/test_1653.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_regression/test_221.py` & `parsl-2023.5.8/parsl/tests/test_regression/test_221.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_regression/test_226.py` & `parsl-2023.5.8/parsl/tests/test_regression/test_226.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_regression/test_2652.py` & `parsl-2023.5.8/parsl/tests/test_regression/test_2652.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_regression/test_69a.py` & `parsl-2023.5.8/parsl/tests/test_regression/test_69a.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_regression/test_69b.py` & `parsl-2023.5.8/parsl/tests/test_regression/test_69b.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_regression/test_854.py` & `parsl-2023.5.8/parsl/tests/test_regression/test_854.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_regression/test_97.py` & `parsl-2023.5.8/parsl/tests/test_regression/test_97.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_regression/test_98.py` & `parsl-2023.5.8/parsl/tests/test_regression/test_98.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_scaling/test_scale_down.py` & `parsl-2023.5.8/parsl/tests/test_scaling/test_scale_down.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_staging/staging_provider.py` & `parsl-2023.5.8/parsl/tests/test_staging/staging_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_staging/test_1316.py` & `parsl-2023.5.8/parsl/tests/test_staging/test_1316.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_staging/test_docs_1.py` & `parsl-2023.5.8/parsl/tests/test_staging/test_docs_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_staging/test_elaborate_noop_file.py` & `parsl-2023.5.8/parsl/tests/test_staging/test_elaborate_noop_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_staging/test_staging_ftp.py` & `parsl-2023.5.8/parsl/tests/test_staging/test_staging_ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_staging/test_staging_ftp_in_task.py` & `parsl-2023.5.8/parsl/tests/test_staging/test_staging_ftp_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_staging/test_staging_globus.py` & `parsl-2023.5.8/parsl/tests/test_staging/test_staging_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_staging/test_staging_https.py` & `parsl-2023.5.8/parsl/tests/test_staging/test_staging_https.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_staging/test_staging_https_in_task.py` & `parsl-2023.5.8/parsl/tests/test_staging/test_staging_https_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_summary.py` & `parsl-2023.5.8/parsl/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_swift.py` & `parsl-2023.5.8/parsl/tests/test_swift.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_thread_parallelism.py` & `parsl-2023.5.8/parsl/tests/test_thread_parallelism.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_threads/test_configs.py` & `parsl-2023.5.8/parsl/tests/test_threads/test_configs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/test_threads/test_lazy_errors.py` & `parsl-2023.5.8/parsl/tests/test_threads/test_lazy_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/workqueue_tests/htex_local.py` & `parsl-2023.5.8/parsl/tests/workqueue_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/workqueue_tests/test_scale.py` & `parsl-2023.5.8/parsl/tests/workqueue_tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/workqueue_tests/wqex_condor.py` & `parsl-2023.5.8/parsl/tests/workqueue_tests/wqex_condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/tests/workqueue_tests/wqex_local.py` & `parsl-2023.5.8/parsl/tests/workqueue_tests/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/usage_tracking/usage.py` & `parsl-2023.5.8/parsl/usage_tracking/usage.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl/utils.py` & `parsl-2023.5.8/parsl/utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl.egg-info/PKG-INFO` & `parsl-2023.5.8/parsl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2023.5.15
+Version: 2023.5.8
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2023.05.15.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2023.05.08.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2023.5.15/parsl.egg-info/SOURCES.txt` & `parsl-2023.5.8/parsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/parsl.egg-info/requires.txt` & `parsl-2023.5.8/parsl.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.15/setup.py` & `parsl-2023.5.8/setup.py`

 * *Files identical despite different names*

