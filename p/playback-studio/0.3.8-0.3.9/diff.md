# Comparing `tmp/playback-studio-0.3.8.tar.gz` & `tmp/playback-studio-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/playback-studio-0.3.8.tar", last modified: Sun Aug 15 15:36:44 2021, max compression
+gzip compressed data, was "dist/playback-studio-0.3.9.tar", last modified: Thu Dec 16 14:26:01 2021, max compression
```

## Comparing `playback-studio-0.3.8.tar` & `playback-studio-0.3.9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/examples/flask/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/examples/flask/__init__.py
--rw-r--r--   0 root         (0) root         (0)      480 2021-08-15 15:36:41.000000 playback-studio-0.3.8/examples/flask/main.py
--rw-r--r--   0 root         (0) root         (0)     1530 2021-08-15 15:36:41.000000 playback-studio-0.3.8/examples/flask/playback_context.py
--rw-r--r--   0 root         (0) root         (0)     2296 2021-08-15 15:36:41.000000 playback-studio-0.3.8/examples/flask/playback_runner.py
--rw-r--r--   0 root         (0) root         (0)     2502 2021-08-15 15:36:41.000000 playback-studio-0.3.8/examples/flask/web_services.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/examples/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3946 2021-08-15 15:36:41.000000 playback-studio-0.3.8/examples/basic_service_operation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback/interception/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback/interception/files/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/interception/files/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5777 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/interception/files/file_interception.py
--rw-r--r--   0 root         (0) root         (0)     1749 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/interception/files/input_file_interception.py
--rw-r--r--   0 root         (0) root         (0)     2246 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/interception/files/output_file_interception.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/interception/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1396 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/interception/input_interception.py
--rw-r--r--   0 root         (0) root         (0)     1179 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/interception/output_interception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback/recordings/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback/recordings/memory/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/recordings/memory/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1875 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/recordings/memory/memory_recording.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/recordings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback/studio/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/studio/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16695 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/studio/equalizer.py
--rw-r--r--   0 root         (0) root         (0)     1315 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/studio/equalizer_tuning.py
--rw-r--r--   0 root         (0) root         (0)     1909 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/studio/recordings_lookup.py
--rw-r--r--   0 root         (0) root         (0)     4708 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/studio/studio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback/tape_cassettes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback/tape_cassettes/asynchronous/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/tape_cassettes/asynchronous/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7184 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/tape_cassettes/asynchronous/async_record_only_tape_cassette.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback/tape_cassettes/file_based/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/tape_cassettes/file_based/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4114 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/tape_cassettes/file_based/file_based_tape_cassette.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback/tape_cassettes/in_memory/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/tape_cassettes/in_memory/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3247 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/tape_cassettes/in_memory/in_memory_tape_cassette.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback/tape_cassettes/s3/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/tape_cassettes/s3/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3388 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/tape_cassettes/s3/s3_basic_facade.py
--rw-r--r--   0 root         (0) root         (0)    14949 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/tape_cassettes/s3/s3_tape_cassette.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/tape_cassettes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/utils/timing_utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/__init__.py
--rw-r--r--   0 root         (0) root         (0)      889 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2117 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/recording.py
--rw-r--r--   0 root         (0) root         (0)     4553 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/tape_cassette.py
--rw-r--r--   0 root         (0) root         (0)    44261 2021-08-15 15:36:41.000000 playback-studio-0.3.8/playback/tape_recorder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback_studio.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23584 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback_studio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2305 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback_studio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback_studio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      386 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback_studio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2021-08-15 15:36:44.000000 playback-studio-0.3.8/playback_studio.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/tests/interception/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/interception/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6906 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/interception/test_file_interception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/tests/mocks/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/mocks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2040 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/mocks/delayed_in_memory_tape_cassette.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/tests/studio/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/studio/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36187 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/studio/test_equalizer.py
--rw-r--r--   0 root         (0) root         (0)     4117 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/studio/test_studio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/tests/test_cassettes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/tests/test_cassettes/async/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/test_cassettes/async/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2855 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/test_cassettes/async/test_async_tape_cassette_behavior.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/tests/test_cassettes/file_based/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/test_cassettes/file_based/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6515 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/test_cassettes/file_based/test_file_based_tape_cassette.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-15 15:36:44.000000 playback-studio-0.3.8/tests/test_cassettes/s3/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/test_cassettes/s3/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17869 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/test_cassettes/s3/test_s3_tape_cassette.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/test_cassettes/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49481 2021-08-15 15:36:41.000000 playback-studio-0.3.8/tests/test_tape_recorder.py
--rw-r--r--   0 root         (0) root         (0)    20031 2021-08-15 15:36:41.000000 playback-studio-0.3.8/README.md
--rw-r--r--   0 root         (0) root         (0)     2108 2021-08-15 15:36:41.000000 playback-studio-0.3.8/setup.py
--rw-r--r--   0 root         (0) root         (0)    23584 2021-08-15 15:36:44.000000 playback-studio-0.3.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2021-08-15 15:36:44.000000 playback-studio-0.3.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/examples/flask/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/examples/flask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      480 2021-12-16 14:25:58.000000 playback-studio-0.3.9/examples/flask/main.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2021-12-16 14:25:58.000000 playback-studio-0.3.9/examples/flask/playback_context.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2021-12-16 14:25:58.000000 playback-studio-0.3.9/examples/flask/playback_runner.py
+-rw-r--r--   0 root         (0) root         (0)     2502 2021-12-16 14:25:58.000000 playback-studio-0.3.9/examples/flask/web_services.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3946 2021-12-16 14:25:58.000000 playback-studio-0.3.9/examples/basic_service_operation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/playback/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/playback/interception/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/playback/interception/files/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/interception/files/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5777 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/interception/files/file_interception.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/interception/files/input_file_interception.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/interception/files/output_file_interception.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/interception/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/interception/input_interception.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/interception/output_interception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/playback/recordings/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/playback/recordings/memory/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/recordings/memory/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/recordings/memory/memory_recording.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/recordings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/playback/studio/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/studio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16695 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/studio/equalizer.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/studio/equalizer_tuning.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/studio/recordings_lookup.py
+-rw-r--r--   0 root         (0) root         (0)     4708 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/studio/studio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/playback/tape_cassettes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/playback/tape_cassettes/asynchronous/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/tape_cassettes/asynchronous/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7184 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/tape_cassettes/asynchronous/async_record_only_tape_cassette.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/playback/tape_cassettes/file_based/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/tape_cassettes/file_based/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/tape_cassettes/file_based/file_based_tape_cassette.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/playback/tape_cassettes/in_memory/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/tape_cassettes/in_memory/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3247 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/tape_cassettes/in_memory/in_memory_tape_cassette.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/playback/tape_cassettes/s3/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/tape_cassettes/s3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3388 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/tape_cassettes/s3/s3_basic_facade.py
+-rw-r--r--   0 root         (0) root         (0)    15069 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/tape_cassettes/s3/s3_tape_cassette.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/tape_cassettes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/playback/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/utils/timing_utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      889 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/recording.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/tape_cassette.py
+-rw-r--r--   0 root         (0) root         (0)    44261 2021-12-16 14:25:58.000000 playback-studio-0.3.9/playback/tape_recorder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/playback_studio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23823 2021-12-16 14:26:00.000000 playback-studio-0.3.9/playback_studio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2305 2021-12-16 14:26:00.000000 playback-studio-0.3.9/playback_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-16 14:26:00.000000 playback-studio-0.3.9/playback_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      386 2021-12-16 14:26:00.000000 playback-studio-0.3.9/playback_studio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2021-12-16 14:26:00.000000 playback-studio-0.3.9/playback_studio.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/tests/interception/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/interception/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6906 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/interception/test_file_interception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/tests/mocks/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/mocks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/mocks/delayed_in_memory_tape_cassette.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/tests/studio/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/studio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36187 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/studio/test_equalizer.py
+-rw-r--r--   0 root         (0) root         (0)     4117 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/studio/test_studio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/tests/test_cassettes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/tests/test_cassettes/async/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/test_cassettes/async/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/test_cassettes/async/test_async_tape_cassette_behavior.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/tests/test_cassettes/file_based/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/test_cassettes/file_based/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6515 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/test_cassettes/file_based/test_file_based_tape_cassette.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 14:26:01.000000 playback-studio-0.3.9/tests/test_cassettes/s3/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/test_cassettes/s3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19393 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/test_cassettes/s3/test_s3_tape_cassette.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/test_cassettes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49481 2021-12-16 14:25:58.000000 playback-studio-0.3.9/tests/test_tape_recorder.py
+-rw-r--r--   0 root         (0) root         (0)    20270 2021-12-16 14:25:58.000000 playback-studio-0.3.9/README.md
+-rw-r--r--   0 root         (0) root         (0)     2084 2021-12-16 14:25:58.000000 playback-studio-0.3.9/setup.py
+-rw-r--r--   0 root         (0) root         (0)    23823 2021-12-16 14:26:01.000000 playback-studio-0.3.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2021-12-16 14:26:01.000000 playback-studio-0.3.9/setup.cfg
```

### Comparing `playback-studio-0.3.8/examples/flask/playback_context.py` & `playback-studio-0.3.9/examples/flask/playback_context.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/examples/flask/playback_runner.py` & `playback-studio-0.3.9/examples/flask/playback_runner.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/examples/flask/web_services.py` & `playback-studio-0.3.9/examples/flask/web_services.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/examples/basic_service_operation.py` & `playback-studio-0.3.9/examples/basic_service_operation.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/interception/files/file_interception.py` & `playback-studio-0.3.9/playback/interception/files/file_interception.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/interception/files/input_file_interception.py` & `playback-studio-0.3.9/playback/interception/files/input_file_interception.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/interception/files/output_file_interception.py` & `playback-studio-0.3.9/playback/interception/files/output_file_interception.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/interception/input_interception.py` & `playback-studio-0.3.9/playback/interception/input_interception.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/interception/output_interception.py` & `playback-studio-0.3.9/playback/interception/output_interception.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/recordings/memory/memory_recording.py` & `playback-studio-0.3.9/playback/recordings/memory/memory_recording.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/studio/equalizer.py` & `playback-studio-0.3.9/playback/studio/equalizer.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/studio/equalizer_tuning.py` & `playback-studio-0.3.9/playback/studio/equalizer_tuning.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/studio/recordings_lookup.py` & `playback-studio-0.3.9/playback/studio/recordings_lookup.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/studio/studio.py` & `playback-studio-0.3.9/playback/studio/studio.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/tape_cassettes/asynchronous/async_record_only_tape_cassette.py` & `playback-studio-0.3.9/playback/tape_cassettes/asynchronous/async_record_only_tape_cassette.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/tape_cassettes/file_based/file_based_tape_cassette.py` & `playback-studio-0.3.9/playback/tape_cassettes/file_based/file_based_tape_cassette.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/tape_cassettes/in_memory/in_memory_tape_cassette.py` & `playback-studio-0.3.9/playback/tape_cassettes/in_memory/in_memory_tape_cassette.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/tape_cassettes/s3/s3_basic_facade.py` & `playback-studio-0.3.9/playback/tape_cassettes/s3/s3_basic_facade.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/tape_cassettes/s3/s3_tape_cassette.py` & `playback-studio-0.3.9/playback/tape_cassettes/s3/s3_tape_cassette.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,14 +255,16 @@
                 recorded_value = recording_metadata.get(k)
                 if recorded_value is None and v is not None:
                     return False
 
                 if isinstance(v, str):
                     if not fnmatch(recorded_value, v):
                         return False
+                elif isinstance(v, list):
+                    return any(fnmatch(recorded_value, value) for value in v)
                 elif recorded_value != v:
                     return False
 
             return True
         return content_filter_func
 
     def iter_recording_ids(self, category, start_date=None, end_date=None, metadata=None, limit=None):
```

### Comparing `playback-studio-0.3.8/playback/exceptions.py` & `playback-studio-0.3.9/playback/exceptions.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/recording.py` & `playback-studio-0.3.9/playback/recording.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/tape_cassette.py` & `playback-studio-0.3.9/playback/tape_cassette.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback/tape_recorder.py` & `playback-studio-0.3.9/playback/tape_recorder.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/playback_studio.egg-info/PKG-INFO` & `playback-studio-0.3.9/playback_studio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: playback-studio
-Version: 0.3.8
+Version: 0.3.9
 Summary: Record your service operations in production and replay them locally at any time in a sandbox
 Home-page: https://github.com/Optibus/playback
 Author: Optibus
 Author-email: eitan@optibus.com
 License: UNKNOWN
-Description: # playback [![CircleCI](https://circleci.com/gh/Optibus/playback.svg?branch=main&style=shield)](https://circleci.com/gh/Optibus/playback) [![codecov](https://codecov.io/gh/Optibus/playback/branch/main/graph/badge.svg?branch=main&token=CA8OMGPFQT)](https://codecov.io/gh/Optibus/playback)
+Description: # playback [![CircleCI](https://circleci.com/gh/Optibus/playback.svg?branch=main&style=shield)](https://circleci.com/gh/Optibus/playback) [![codecov](https://codecov.io/gh/Optibus/playback/branch/main/graph/badge.svg?branch=main&token=CA8OMGPFQT)](https://codecov.io/gh/Optibus/playback) [![PyPi Version](https://badge.fury.io/py/playback-studio.svg)](https://pypi.python.org/pypi/playback-studio/) [![Python Versions](https://img.shields.io/pypi/pyversions/playback-studio.svg)](https://pypi.python.org/pypi/playback-studio/)
         
         A Python decorator-based framework that lets you "record" and "replay" operations (e.g. API requests, workers consuming jobs from queues).
         
         ## Main uses
         
         * Regression testing - replay recorded production traffic on modified code before pushing it
         * Debug production issues locally
```

### Comparing `playback-studio-0.3.8/playback_studio.egg-info/SOURCES.txt` & `playback-studio-0.3.9/playback_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/tests/interception/test_file_interception.py` & `playback-studio-0.3.9/tests/interception/test_file_interception.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/tests/mocks/delayed_in_memory_tape_cassette.py` & `playback-studio-0.3.9/tests/mocks/delayed_in_memory_tape_cassette.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/tests/studio/test_equalizer.py` & `playback-studio-0.3.9/tests/studio/test_equalizer.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/tests/studio/test_studio.py` & `playback-studio-0.3.9/tests/studio/test_studio.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/tests/test_cassettes/async/test_async_tape_cassette_behavior.py` & `playback-studio-0.3.9/tests/test_cassettes/async/test_async_tape_cassette_behavior.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/tests/test_cassettes/file_based/test_file_based_tape_cassette.py` & `playback-studio-0.3.9/tests/test_cassettes/file_based/test_file_based_tape_cassette.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/tests/test_cassettes/s3/test_s3_tape_cassette.py` & `playback-studio-0.3.9/tests/test_cassettes/s3/test_s3_tape_cassette.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,14 +264,38 @@
                            list(self.cassette.iter_recording_ids(category='test_operation1',
                                                                  metadata={'property': 'val2*'})))
 
         assert_items_equal(self, [recording1.id, recording2.id],
                            list(self.cassette.iter_recording_ids(category='test_operation1',
                                                                  metadata={'property': 'val*'})))
 
+    def test_fetch_recording_ids_with_matching_metadata_value_not_set(self):
+        recording1 = self.cassette.create_new_recording('test_operation1')
+        recording1.add_metadata({'property': 'val11'})
+        self.cassette.save_recording(recording1)
+        recording2 = self.cassette.create_new_recording('test_operation1')
+        recording2.add_metadata({'property': 'val21'})
+        self.cassette.save_recording(recording2)
+        recording3 = self.cassette.create_new_recording('test_operation1')
+        recording3.add_metadata({'property': 'test'})
+        self.cassette.save_recording(recording3)
+        recording4 = self.cassette.create_new_recording('test_operation1')
+        self.cassette.save_recording(recording4)
+
+        assert_items_equal(self, [recording2.id, recording3.id],
+                           list(self.cassette.iter_recording_ids(category='test_operation1',
+                                                                 metadata={'property': ['val2*', 'test']})))
+
+        assert_items_equal(self, [recording1.id, recording2.id, recording3.id],
+                           list(self.cassette.iter_recording_ids(category='test_operation1',
+                                                                 metadata={'property': ['val*', 't*']})))
+        assert_items_equal(self, [],
+                           list(self.cassette.iter_recording_ids(category='test_operation1',
+                                                                 metadata={'property': ['try1', 'try2']})))
+
     def test_fetch_recording_ids_by_category_and_limit(self):
         recording1 = self.cassette.create_new_recording('test_operation1')
         self.cassette.save_recording(recording1)
         recording2 = self.cassette.create_new_recording('test_operation1')
         self.cassette.save_recording(recording2)
         recording3 = self.cassette.create_new_recording('test_operation1')
         self.cassette.save_recording(recording3)
```

### Comparing `playback-studio-0.3.8/tests/test_tape_recorder.py` & `playback-studio-0.3.9/tests/test_tape_recorder.py`

 * *Files identical despite different names*

### Comparing `playback-studio-0.3.8/README.md` & `playback-studio-0.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# playback [![CircleCI](https://circleci.com/gh/Optibus/playback.svg?branch=main&style=shield)](https://circleci.com/gh/Optibus/playback) [![codecov](https://codecov.io/gh/Optibus/playback/branch/main/graph/badge.svg?branch=main&token=CA8OMGPFQT)](https://codecov.io/gh/Optibus/playback)
+# playback [![CircleCI](https://circleci.com/gh/Optibus/playback.svg?branch=main&style=shield)](https://circleci.com/gh/Optibus/playback) [![codecov](https://codecov.io/gh/Optibus/playback/branch/main/graph/badge.svg?branch=main&token=CA8OMGPFQT)](https://codecov.io/gh/Optibus/playback) [![PyPi Version](https://badge.fury.io/py/playback-studio.svg)](https://pypi.python.org/pypi/playback-studio/) [![Python Versions](https://img.shields.io/pypi/pyversions/playback-studio.svg)](https://pypi.python.org/pypi/playback-studio/)
 
 A Python decorator-based framework that lets you "record" and "replay" operations (e.g. API requests, workers consuming jobs from queues).
 
 ## Main uses
 
 * Regression testing - replay recorded production traffic on modified code before pushing it
 * Debug production issues locally
```

### Comparing `playback-studio-0.3.8/setup.py` & `playback-studio-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import setuptools
 from setuptools.command.install import install
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-VERSION = '0.3.8'
+VERSION = '0.3.9'
 
 
 class VerifyVersionCommand(install):
     """Custom command to verify that the git tag matches our version"""
     description = 'verify that the git tag matches our version'
 
     def run(self):
@@ -43,15 +43,15 @@
     extras_require={'dev': [
         'mock==2.0.0',
         'rsa<=4.0; python_version < \'3\'',
         'python-jose<=0.3.2; python_version < \'3\'',
         'moto==1.3.13',
         'pytest==4.6.9',
         'parameterized==0.7.0',
-        'Werkzeug==0.16.1; python_version < \'3\'',
+        'Werkzeug==0.16.1',
         'Flask==1.1.2',
         'flask-restplus==0.13.0',
         'pylint==2.6.0; python_version > "3.0"',
         'pylint-junit==0.3.2; python_version > "3.0"',
         'flake8==3.8.4; python_version > "3.0"',
         'flake8-formatter-junit-xml==0.0.6; python_version > "3.0"',
         'pytest-cov==2.10.1; python_version > "3.0"'
```

### Comparing `playback-studio-0.3.8/PKG-INFO` & `playback-studio-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: playback-studio
-Version: 0.3.8
+Version: 0.3.9
 Summary: Record your service operations in production and replay them locally at any time in a sandbox
 Home-page: https://github.com/Optibus/playback
 Author: Optibus
 Author-email: eitan@optibus.com
 License: UNKNOWN
-Description: # playback [![CircleCI](https://circleci.com/gh/Optibus/playback.svg?branch=main&style=shield)](https://circleci.com/gh/Optibus/playback) [![codecov](https://codecov.io/gh/Optibus/playback/branch/main/graph/badge.svg?branch=main&token=CA8OMGPFQT)](https://codecov.io/gh/Optibus/playback)
+Description: # playback [![CircleCI](https://circleci.com/gh/Optibus/playback.svg?branch=main&style=shield)](https://circleci.com/gh/Optibus/playback) [![codecov](https://codecov.io/gh/Optibus/playback/branch/main/graph/badge.svg?branch=main&token=CA8OMGPFQT)](https://codecov.io/gh/Optibus/playback) [![PyPi Version](https://badge.fury.io/py/playback-studio.svg)](https://pypi.python.org/pypi/playback-studio/) [![Python Versions](https://img.shields.io/pypi/pyversions/playback-studio.svg)](https://pypi.python.org/pypi/playback-studio/)
         
         A Python decorator-based framework that lets you "record" and "replay" operations (e.g. API requests, workers consuming jobs from queues).
         
         ## Main uses
         
         * Regression testing - replay recorded production traffic on modified code before pushing it
         * Debug production issues locally
```

