# Comparing `tmp/hkube_python_wrapper-2.6.0.dev8.tar.gz` & `tmp/hkube_python_wrapper-2.6.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hkube_python_wrapper-2.6.0.dev8.tar", last modified: Sun Feb 25 14:40:20 2024, max compression
+gzip compressed data, was "dist/hkube_python_wrapper-2.6.0.dev9.tar", last modified: Wed Mar  6 13:51:53 2024, max compression
```

## Comparing `hkube_python_wrapper-2.6.0.dev8.tar` & `hkube_python_wrapper-2.6.0.dev9.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/cache/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/codeApi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/codeApi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/codeApi/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/codeApi/hkube_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/codeApi/waitFor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/DataRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/DataServer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/streaming/MessageListener.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/streaming/MessageProducer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/streaming/StreamingManager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/streaming/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/ZMQPingServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/ZMQRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/ZMQServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/ZMQServers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/streaming/ZMQListener.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/streaming/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/streaming/producer/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/streaming/producer/Flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/streaming/producer/MessageQueue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/streaming/producer/ZMQProducer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/streaming/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/streaming/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/storage/base_storage_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/storage/fs_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/storage/s3_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/storage/storage_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/storage/task_output_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/tracing/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/DaemonThread.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/fifo_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/object_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/percentile.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/queueImpl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/stdout_redirector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/timerImpl.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/type_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/uid.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/url_encode_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23909 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/wrapper/algorunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/wrapper/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/wrapper/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/wrapper/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/wrapper/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/wrapper/statelessAlgoWrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/wrapper/wc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-02-25 14:40:18.000000 hkube_python_wrapper-2.6.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/mock_ws_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/mocks/mockdata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:19.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_alg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_alg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_alg/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_hkube_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_storage_manager_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_storage_manager_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_streaming.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_utils_getpath.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/xtest_communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-02-25 14:40:13.000000 hkube_python_wrapper-2.6.0.dev8/tests/xtest_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/cache/caching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/codeApi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/codeApi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/codeApi/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/codeApi/hkube_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/codeApi/waitFor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/DataRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/DataServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/streaming/MessageListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/streaming/MessageProducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/streaming/StreamingManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/streaming/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/ZMQPingServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/ZMQRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/ZMQServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/ZMQServers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/streaming/ZMQListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/streaming/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/streaming/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/streaming/producer/Flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/streaming/producer/MessageQueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/streaming/producer/ZMQProducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/streaming/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/streaming/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/storage/base_storage_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/storage/fs_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/storage/s3_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/storage/storage_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/storage/task_output_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/tracing/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/DaemonThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/fifo_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/object_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/percentile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/queueImpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/stdout_redirector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/timerImpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/type_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/uid.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/url_encode_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23936 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/wrapper/algorunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/wrapper/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/wrapper/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/wrapper/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/wrapper/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/wrapper/statelessAlgoWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/wrapper/wc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-03-06 13:51:51.000000 hkube_python_wrapper-2.6.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/mock_ws_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/mocks/mockdata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:53.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_alg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_alg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_alg/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_hkube_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_storage_manager_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_storage_manager_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_utils_getpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/xtest_communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-06 13:51:48.000000 hkube_python_wrapper-2.6.0.dev9/tests/xtest_encoding.py
```

### Comparing `hkube_python_wrapper-2.6.0.dev8/PKG-INFO` & `hkube_python_wrapper-2.6.0.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkube_python_wrapper
-Version: 2.6.0.dev8
+Version: 2.6.0.dev9
 Summary: Hkube Python Wrapper
 Home-page: https://github.com/kube-HPC/python-wrapper.hkube
 Author: Hkube
 Author-email: hkube.dev@gmail.com
 License: MIT
 Description: # HKube Python Wrapper
         [![Build Status](https://travis-ci.org/kube-HPC/python-wrapper.hkube.svg?branch=master)](https://travis-ci.org/kube-HPC/python-wrapper.hkube)
```

### Comparing `hkube_python_wrapper-2.6.0.dev8/README.md` & `hkube_python_wrapper-2.6.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/cache/caching.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/cache/caching.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/codeApi/hkube_api.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/codeApi/hkube_api.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/codeApi/waitFor.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/codeApi/waitFor.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/DataRequest.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/DataRequest.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/DataServer.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/DataServer.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/streaming/MessageListener.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/streaming/MessageListener.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/streaming/MessageProducer.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/streaming/MessageProducer.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/streaming/StreamingManager.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/streaming/StreamingManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
             if (parent['type'] == 'Add'):
                 options = {}
                 options.update(listenerConfig)
                 options['remoteAddress'] = remoteAddressUrl
                 options['messageOriginNodeName'] = parentName
                 def is_active():
-                    return self._messageListeners[remoteAddressUrl] is not None and self.listeningToMessages # pylint: disable=cell-var-from-loop
+                    return self._messageListeners.get(remoteAddressUrl) is not None and self.listeningToMessages # pylint: disable=cell-var-from-loop
                 listener = MessageListener(options, nodeName,is_active)
                 listener.registerMessageListener(self.onMessage)
                 self._messageListeners[remoteAddressUrl] = listener
                 if(self.listeningToMessages):
                     listener.start()
 
             if (parent['type'] == 'Del'):
```

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/ZMQPingServer.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/ZMQPingServer.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/ZMQRequest.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/ZMQRequest.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/ZMQServer.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/ZMQServer.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/ZMQServers.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/ZMQServers.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/streaming/ZMQListener.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/streaming/ZMQListener.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/streaming/producer/Flow.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/streaming/producer/Flow.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/streaming/producer/MessageQueue.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/streaming/producer/MessageQueue.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/communication/zmq/streaming/producer/ZMQProducer.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/communication/zmq/streaming/producer/ZMQProducer.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/config/config.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/config/config.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/storage/base_storage_manager.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/storage/base_storage_manager.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/storage/fs_adapter.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/storage/fs_adapter.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/storage/s3_adapter.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/storage/s3_adapter.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/storage/storage_manager.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/storage/storage_manager.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/storage/task_output_manager.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/storage/task_output_manager.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/tracing/tracer.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/tracing/tracer.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/decorators.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/decorators.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/encoding.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/encoding.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/logger.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/logger.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/object_path.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/object_path.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/percentile.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/percentile.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/stdout_redirector.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/stdout_redirector.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/util/timerImpl.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/util/timerImpl.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/wrapper/algorunner.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/wrapper/algorunner.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
         producerConfig['messagesMemoryBuff'] = config.discovery['streaming']['messagesMemoryBuff']
         producerConfig['encoding'] = config.discovery['encoding']
         producerConfig['statisticsInterval'] = config.discovery['streaming']['statisticsInterval']
         self.streamingManager.setupStreamingProducer(
             onStatistics, producerConfig, self._job.childs, nodeName)
 
     def _start(self, options):
-        if (self._job.isStreaming):
+        if (self._job and self._job.isStreaming):
             self.streamingManager.setParsedFlows(self._job.parsedFlow, self._job.defaultFlow)
             if (self._job.childs):
                 self._setupStreamingProducer(self._job.nodeName)
                 self.streamingManager.clearMessageListeners()
         # pylint: disable=unused-argument
         span = None
         self._initDataServer(config)
@@ -477,18 +477,17 @@
             try:
                 forceStop = options.get('forceStop', False)
                 if (forceStop is True):
                     log.info('stopping using force flag')
                 else:
                     log.info('stopping gracefully')
 
-                if (self._job.isStreaming):
+                if (self._job and self._job.isStreaming):
                     if (forceStop is False):
                         stoppingState = True
-
                         def stopping():
                             while (stoppingState):
                                 self._sendCommand(messages.outgoing.stopping, None)
                                 time.sleep(1)
 
                         stoppingThread = Thread(target=stopping)
                         stoppingThread.start()
```

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/wrapper/data_adapter.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/wrapper/data_adapter.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/wrapper/job.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/wrapper/job.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/wrapper/messages.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/wrapper/messages.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/wrapper/statelessAlgoWrapper.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/wrapper/statelessAlgoWrapper.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper/wrapper/wc.py` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper/wrapper/wc.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper.egg-info/PKG-INFO` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkube-python-wrapper
-Version: 2.6.0.dev8
+Version: 2.6.0.dev9
 Summary: Hkube Python Wrapper
 Home-page: https://github.com/kube-HPC/python-wrapper.hkube
 Author: Hkube
 Author-email: hkube.dev@gmail.com
 License: MIT
 Description: # HKube Python Wrapper
         [![Build Status](https://travis-ci.org/kube-HPC/python-wrapper.hkube.svg?branch=master)](https://travis-ci.org/kube-HPC/python-wrapper.hkube)
```

### Comparing `hkube_python_wrapper-2.6.0.dev8/hkube_python_wrapper.egg-info/SOURCES.txt` & `hkube_python_wrapper-2.6.0.dev9/hkube_python_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/setup.cfg` & `hkube_python_wrapper-2.6.0.dev9/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.6.0-dev8
+current_version = 2.6.0-dev9
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `hkube_python_wrapper-2.6.0.dev8/setup.py` & `hkube_python_wrapper-2.6.0.dev9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import print_function, division, absolute_import
 
 import setuptools
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '2.6.0-dev8'
+VERSION = '2.6.0-dev9'
 
 
 
 
 
 packages = setuptools.find_packages()
```

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/configs/config.py` & `hkube_python_wrapper-2.6.0.dev9/tests/configs/config.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/conftest.py` & `hkube_python_wrapper-2.6.0.dev9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/mock_ws_server.py` & `hkube_python_wrapper-2.6.0.dev9/tests/mock_ws_server.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/mocks/mockdata.py` & `hkube_python_wrapper-2.6.0.dev9/tests/mocks/mockdata.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/test_cache.py` & `hkube_python_wrapper-2.6.0.dev9/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/test_communication.py` & `hkube_python_wrapper-2.6.0.dev9/tests/test_communication.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/test_data_adapter.py` & `hkube_python_wrapper-2.6.0.dev9/tests/test_data_adapter.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/test_encoding.py` & `hkube_python_wrapper-2.6.0.dev9/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/test_hkube_api.py` & `hkube_python_wrapper-2.6.0.dev9/tests/test_hkube_api.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/test_queue.py` & `hkube_python_wrapper-2.6.0.dev9/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/test_storage_manager_fs.py` & `hkube_python_wrapper-2.6.0.dev9/tests/test_storage_manager_fs.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/test_storage_manager_s3.py` & `hkube_python_wrapper-2.6.0.dev9/tests/test_storage_manager_s3.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/test_streaming.py` & `hkube_python_wrapper-2.6.0.dev9/tests/test_streaming.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/test_tracer.py` & `hkube_python_wrapper-2.6.0.dev9/tests/test_tracer.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/test_utils_getpath.py` & `hkube_python_wrapper-2.6.0.dev9/tests/test_utils_getpath.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/test_wrapper.py` & `hkube_python_wrapper-2.6.0.dev9/tests/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/test_zmq.py` & `hkube_python_wrapper-2.6.0.dev9/tests/test_zmq.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/xtest_communication.py` & `hkube_python_wrapper-2.6.0.dev9/tests/xtest_communication.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.6.0.dev8/tests/xtest_encoding.py` & `hkube_python_wrapper-2.6.0.dev9/tests/xtest_encoding.py`

 * *Files identical despite different names*

