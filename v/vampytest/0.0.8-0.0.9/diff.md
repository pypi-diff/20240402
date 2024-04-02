# Comparing `tmp/vampytest-0.0.8.tar.gz` & `tmp/vampytest-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vampytest-0.0.8.tar", last modified: Thu Jun  8 09:05:27 2023, max compression
+gzip compressed data, was "vampytest-0.0.9.tar", last modified: Thu Jun  8 09:49:05 2023, max compression
```

## Comparing `vampytest-0.0.8.tar` & `vampytest-0.0.9.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.937160 vampytest-0.0.8/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1506 2023-06-08 09:05:27.937160 vampytest-0.0.8/PKG-INFO
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      323 2022-07-05 13:34:12.000000 vampytest-0.0.8/README.md
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       38 2023-06-08 09:05:27.937160 vampytest-0.0.8/setup.cfg
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2360 2023-06-04 20:39:03.000000 vampytest-0.0.8/setup.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.917160 vampytest-0.0.8/vampytest/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       67 2023-06-08 09:02:15.000000 vampytest-0.0.8/vampytest/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      311 2022-12-19 10:57:15.000000 vampytest-0.0.8/vampytest/__main__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.917160 vampytest-0.0.8/vampytest/core/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      674 2023-06-04 13:10:23.000000 vampytest-0.0.8/vampytest/core/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.921160 vampytest-0.0.8/vampytest/core/assertions/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1347 2023-06-03 10:56:18.000000 vampytest-0.0.8/vampytest/core/assertions/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1839 2023-06-03 11:01:35.000000 vampytest-0.0.8/vampytest/core/assertions/aliases.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1705 2023-06-03 08:34:35.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10829 2023-06-03 16:26:49.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_conditional_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      972 2023-06-03 10:54:02.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_contains.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      933 2023-06-03 11:32:10.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_equals.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1215 2023-06-03 10:54:53.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_false.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      964 2023-06-03 12:54:40.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_identical.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4849 2023-06-03 18:52:54.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_instance.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      994 2023-06-03 10:56:54.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_not_contains.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      943 2023-06-03 10:57:21.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_not_equals.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      982 2023-06-03 12:54:58.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_not_identical.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3467 2023-06-03 19:04:59.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_raising.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      717 2023-06-03 08:30:46.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_states.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3960 2023-06-03 16:28:00.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_subtype.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1200 2023-06-03 10:59:18.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_true.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3973 2023-06-03 08:32:34.000000 vampytest-0.0.8/vampytest/core/assertions/exceptions.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.921160 vampytest-0.0.8/vampytest/core/contexts/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      224 2023-06-04 15:53:08.000000 vampytest-0.0.8/vampytest/core/contexts/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1880 2023-06-04 15:35:26.000000 vampytest-0.0.8/vampytest/core/contexts/base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3965 2023-06-04 17:02:08.000000 vampytest-0.0.8/vampytest/core/contexts/calling.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1336 2023-06-04 15:38:42.000000 vampytest-0.0.8/vampytest/core/contexts/garbage_collect.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1614 2023-06-05 07:44:04.000000 vampytest-0.0.8/vampytest/core/contexts/output_capturing.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.925160 vampytest-0.0.8/vampytest/core/environment/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      326 2022-12-19 11:05:35.000000 vampytest-0.0.8/vampytest/core/environment/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6417 2022-12-19 10:51:03.000000 vampytest-0.0.8/vampytest/core/environment/configuration.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      172 2022-07-04 12:58:23.000000 vampytest-0.0.8/vampytest/core/environment/constants.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1899 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/environment/default.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1336 2023-06-03 19:11:36.000000 vampytest-0.0.8/vampytest/core/environment/helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3368 2023-06-04 14:14:50.000000 vampytest-0.0.8/vampytest/core/environment/manager.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4303 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/environment/scarletio_coroutine.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.925160 vampytest-0.0.8/vampytest/core/event_handling/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      342 2023-06-04 18:26:40.000000 vampytest-0.0.8/vampytest/core/event_handling/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4916 2022-12-19 10:54:12.000000 vampytest-0.0.8/vampytest/core/event_handling/base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      459 2023-06-04 18:26:24.000000 vampytest-0.0.8/vampytest/core/event_handling/colors.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8165 2023-06-04 20:14:28.000000 vampytest-0.0.8/vampytest/core/event_handling/default.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4079 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/event_handling/default_output_writer.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.925160 vampytest-0.0.8/vampytest/core/event_handling/rendering_helpers/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      207 2023-06-04 18:27:13.000000 vampytest-0.0.8/vampytest/core/event_handling/rendering_helpers/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1964 2023-06-05 06:48:49.000000 vampytest-0.0.8/vampytest/core/event_handling/rendering_helpers/result_modifier_parameters.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11879 2023-06-04 20:37:50.000000 vampytest-0.0.8/vampytest/core/event_handling/rendering_helpers/result_rendering.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2957 2023-06-04 20:17:32.000000 vampytest-0.0.8/vampytest/core/event_handling/rendering_helpers/writers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1855 2023-06-04 18:36:03.000000 vampytest-0.0.8/vampytest/core/event_handling/text_styling.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.929160 vampytest-0.0.8/vampytest/core/events/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      526 2022-07-01 16:44:50.000000 vampytest-0.0.8/vampytest/core/events/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2545 2023-06-04 07:01:57.000000 vampytest-0.0.8/vampytest/core/events/base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      249 2022-07-01 16:40:47.000000 vampytest-0.0.8/vampytest/core/events/constants.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      751 2022-07-01 19:12:39.000000 vampytest-0.0.8/vampytest/core/events/file_load_done.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      470 2022-07-01 19:12:39.000000 vampytest-0.0.8/vampytest/core/events/file_registration.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      427 2022-07-01 19:12:39.000000 vampytest-0.0.8/vampytest/core/events/file_registration_done.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      470 2022-07-01 19:12:42.000000 vampytest-0.0.8/vampytest/core/events/file_testing_done.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      438 2023-06-04 07:01:41.000000 vampytest-0.0.8/vampytest/core/events/test_done.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      371 2022-07-01 19:12:49.000000 vampytest-0.0.8/vampytest/core/events/testing_end.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      381 2022-07-01 19:12:52.000000 vampytest-0.0.8/vampytest/core/events/testing_start.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.929160 vampytest-0.0.8/vampytest/core/file/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      235 2022-07-24 17:11:51.000000 vampytest-0.0.8/vampytest/core/file/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3234 2022-07-24 20:51:54.000000 vampytest-0.0.8/vampytest/core/file/collection.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9474 2023-02-15 17:01:20.000000 vampytest-0.0.8/vampytest/core/file/file_system_entry.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2106 2022-12-19 10:54:46.000000 vampytest-0.0.8/vampytest/core/file/load_failure.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15847 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/file/test_file.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21860 2023-06-04 15:55:12.000000 vampytest-0.0.8/vampytest/core/handle.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.933160 vampytest-0.0.8/vampytest/core/helpers/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      273 2023-06-03 15:00:30.000000 vampytest-0.0.8/vampytest/core/helpers/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1518 2023-06-03 18:40:58.000000 vampytest-0.0.8/vampytest/core/helpers/exception_matching.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2549 2023-06-03 14:53:17.000000 vampytest-0.0.8/vampytest/core/helpers/hashing.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1633 2023-06-03 14:55:07.000000 vampytest-0.0.8/vampytest/core/helpers/merging.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2366 2023-06-03 14:57:31.000000 vampytest-0.0.8/vampytest/core/helpers/path_repr.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2354 2023-06-03 14:52:20.000000 vampytest-0.0.8/vampytest/core/helpers/un_nesting.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.933160 vampytest-0.0.8/vampytest/core/result/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      110 2023-06-04 12:40:46.000000 vampytest-0.0.8/vampytest/core/result/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.933160 vampytest-0.0.8/vampytest/core/result/reports/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      241 2023-06-04 19:01:59.000000 vampytest-0.0.8/vampytest/core/result/reports/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1115 2023-06-04 18:41:12.000000 vampytest-0.0.8/vampytest/core/result/reports/asserting.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      869 2023-06-04 16:49:37.000000 vampytest-0.0.8/vampytest/core/result/reports/base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      698 2023-06-04 16:52:34.000000 vampytest-0.0.8/vampytest/core/result/reports/output.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2006 2023-06-04 19:05:23.000000 vampytest-0.0.8/vampytest/core/result/reports/raising.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1472 2023-06-04 19:12:11.000000 vampytest-0.0.8/vampytest/core/result/reports/returning.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10268 2023-06-04 20:37:00.000000 vampytest-0.0.8/vampytest/core/result/result.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8411 2023-06-04 07:01:08.000000 vampytest-0.0.8/vampytest/core/run_state.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.933160 vampytest-0.0.8/vampytest/core/runner/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      104 2022-12-19 10:55:58.000000 vampytest-0.0.8/vampytest/core/runner/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10798 2023-06-04 20:30:43.000000 vampytest-0.0.8/vampytest/core/runner/context.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10435 2023-06-04 07:02:40.000000 vampytest-0.0.8/vampytest/core/runner/runner.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7836 2023-06-04 08:01:22.000000 vampytest-0.0.8/vampytest/core/test_case.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.933160 vampytest-0.0.8/vampytest/core/utils/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      207 2023-06-05 06:55:53.000000 vampytest-0.0.8/vampytest/core/utils/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      150 2023-06-05 07:43:47.000000 vampytest-0.0.8/vampytest/core/utils/aliases.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2189 2023-06-05 08:05:15.000000 vampytest-0.0.8/vampytest/core/utils/capture_output_context_manager.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      360 2023-06-03 15:06:42.000000 vampytest-0.0.8/vampytest/core/utils/wrap_nothing.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.937160 vampytest-0.0.8/vampytest/core/wrappers/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      883 2023-06-03 19:28:37.000000 vampytest-0.0.8/vampytest/core/wrappers/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1221 2023-06-05 09:29:38.000000 vampytest-0.0.8/vampytest/core/wrappers/aliases.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7302 2023-06-05 09:14:21.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20677 2023-06-05 09:06:02.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_call.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17716 2023-06-05 09:54:49.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_call_from.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3866 2023-06-03 19:12:42.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_chainer.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3067 2023-06-04 17:39:27.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_conflict.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1771 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_environment.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2572 2023-06-04 14:02:29.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_garbage_collect.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      921 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_reverse.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      743 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_skip.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1612 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_skip_conditional.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.937160 vampytest-0.0.8/vampytest/main/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5617 2022-12-19 11:06:38.000000 vampytest-0.0.8/vampytest/main/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.917160 vampytest-0.0.8/vampytest.egg-info/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1506 2023-06-08 09:05:27.000000 vampytest-0.0.8/vampytest.egg-info/PKG-INFO
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4021 2023-06-08 09:05:27.000000 vampytest-0.0.8/vampytest.egg-info/SOURCES.txt
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)        1 2023-06-08 09:05:27.000000 vampytest-0.0.8/vampytest.egg-info/dependency_links.txt
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       10 2023-06-08 09:05:27.000000 vampytest-0.0.8/vampytest.egg-info/requires.txt
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       10 2023-06-08 09:05:27.000000 vampytest-0.0.8/vampytest.egg-info/top_level.txt
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.332494 vampytest-0.0.9/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1506 2023-06-08 09:49:05.332494 vampytest-0.0.9/PKG-INFO
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      323 2022-07-05 13:34:12.000000 vampytest-0.0.9/README.md
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       38 2023-06-08 09:49:05.332494 vampytest-0.0.9/setup.cfg
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2360 2023-06-04 20:39:03.000000 vampytest-0.0.9/setup.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.324494 vampytest-0.0.9/vampytest/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       67 2023-06-08 09:44:59.000000 vampytest-0.0.9/vampytest/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      311 2022-12-19 10:57:15.000000 vampytest-0.0.9/vampytest/__main__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.324494 vampytest-0.0.9/vampytest/core/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      674 2023-06-04 13:10:23.000000 vampytest-0.0.9/vampytest/core/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.324494 vampytest-0.0.9/vampytest/core/assertions/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1347 2023-06-03 10:56:18.000000 vampytest-0.0.9/vampytest/core/assertions/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1839 2023-06-03 11:01:35.000000 vampytest-0.0.9/vampytest/core/assertions/aliases.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1705 2023-06-03 08:34:35.000000 vampytest-0.0.9/vampytest/core/assertions/assertion_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10829 2023-06-03 16:26:49.000000 vampytest-0.0.9/vampytest/core/assertions/assertion_conditional_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      972 2023-06-03 10:54:02.000000 vampytest-0.0.9/vampytest/core/assertions/assertion_contains.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      933 2023-06-03 11:32:10.000000 vampytest-0.0.9/vampytest/core/assertions/assertion_equals.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1215 2023-06-03 10:54:53.000000 vampytest-0.0.9/vampytest/core/assertions/assertion_false.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      964 2023-06-03 12:54:40.000000 vampytest-0.0.9/vampytest/core/assertions/assertion_identical.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4849 2023-06-03 18:52:54.000000 vampytest-0.0.9/vampytest/core/assertions/assertion_instance.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      994 2023-06-03 10:56:54.000000 vampytest-0.0.9/vampytest/core/assertions/assertion_not_contains.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      943 2023-06-03 10:57:21.000000 vampytest-0.0.9/vampytest/core/assertions/assertion_not_equals.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      982 2023-06-03 12:54:58.000000 vampytest-0.0.9/vampytest/core/assertions/assertion_not_identical.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3467 2023-06-03 19:04:59.000000 vampytest-0.0.9/vampytest/core/assertions/assertion_raising.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      717 2023-06-03 08:30:46.000000 vampytest-0.0.9/vampytest/core/assertions/assertion_states.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3960 2023-06-03 16:28:00.000000 vampytest-0.0.9/vampytest/core/assertions/assertion_subtype.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1200 2023-06-03 10:59:18.000000 vampytest-0.0.9/vampytest/core/assertions/assertion_true.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3973 2023-06-03 08:32:34.000000 vampytest-0.0.9/vampytest/core/assertions/exceptions.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.324494 vampytest-0.0.9/vampytest/core/contexts/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      224 2023-06-04 15:53:08.000000 vampytest-0.0.9/vampytest/core/contexts/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1880 2023-06-04 15:35:26.000000 vampytest-0.0.9/vampytest/core/contexts/base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3965 2023-06-04 17:02:08.000000 vampytest-0.0.9/vampytest/core/contexts/calling.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1336 2023-06-04 15:38:42.000000 vampytest-0.0.9/vampytest/core/contexts/garbage_collect.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1614 2023-06-05 07:44:04.000000 vampytest-0.0.9/vampytest/core/contexts/output_capturing.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.328494 vampytest-0.0.9/vampytest/core/environment/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      326 2022-12-19 11:05:35.000000 vampytest-0.0.9/vampytest/core/environment/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6417 2022-12-19 10:51:03.000000 vampytest-0.0.9/vampytest/core/environment/configuration.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      172 2022-07-04 12:58:23.000000 vampytest-0.0.9/vampytest/core/environment/constants.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1899 2023-06-05 09:55:49.000000 vampytest-0.0.9/vampytest/core/environment/default.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1336 2023-06-03 19:11:36.000000 vampytest-0.0.9/vampytest/core/environment/helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3368 2023-06-04 14:14:50.000000 vampytest-0.0.9/vampytest/core/environment/manager.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4303 2023-06-05 09:55:49.000000 vampytest-0.0.9/vampytest/core/environment/scarletio_coroutine.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.328494 vampytest-0.0.9/vampytest/core/event_handling/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      342 2023-06-04 18:26:40.000000 vampytest-0.0.9/vampytest/core/event_handling/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4916 2022-12-19 10:54:12.000000 vampytest-0.0.9/vampytest/core/event_handling/base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      459 2023-06-04 18:26:24.000000 vampytest-0.0.9/vampytest/core/event_handling/colors.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8165 2023-06-04 20:14:28.000000 vampytest-0.0.9/vampytest/core/event_handling/default.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4079 2023-06-05 09:55:49.000000 vampytest-0.0.9/vampytest/core/event_handling/default_output_writer.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.328494 vampytest-0.0.9/vampytest/core/event_handling/rendering_helpers/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      207 2023-06-04 18:27:13.000000 vampytest-0.0.9/vampytest/core/event_handling/rendering_helpers/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1964 2023-06-05 06:48:49.000000 vampytest-0.0.9/vampytest/core/event_handling/rendering_helpers/result_modifier_parameters.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11896 2023-06-08 09:42:22.000000 vampytest-0.0.9/vampytest/core/event_handling/rendering_helpers/result_rendering.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2957 2023-06-04 20:17:32.000000 vampytest-0.0.9/vampytest/core/event_handling/rendering_helpers/writers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1855 2023-06-04 18:36:03.000000 vampytest-0.0.9/vampytest/core/event_handling/text_styling.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.328494 vampytest-0.0.9/vampytest/core/events/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      526 2022-07-01 16:44:50.000000 vampytest-0.0.9/vampytest/core/events/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2545 2023-06-04 07:01:57.000000 vampytest-0.0.9/vampytest/core/events/base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      249 2022-07-01 16:40:47.000000 vampytest-0.0.9/vampytest/core/events/constants.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      751 2022-07-01 19:12:39.000000 vampytest-0.0.9/vampytest/core/events/file_load_done.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      470 2022-07-01 19:12:39.000000 vampytest-0.0.9/vampytest/core/events/file_registration.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      427 2022-07-01 19:12:39.000000 vampytest-0.0.9/vampytest/core/events/file_registration_done.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      470 2022-07-01 19:12:42.000000 vampytest-0.0.9/vampytest/core/events/file_testing_done.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      438 2023-06-04 07:01:41.000000 vampytest-0.0.9/vampytest/core/events/test_done.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      371 2022-07-01 19:12:49.000000 vampytest-0.0.9/vampytest/core/events/testing_end.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      381 2022-07-01 19:12:52.000000 vampytest-0.0.9/vampytest/core/events/testing_start.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.328494 vampytest-0.0.9/vampytest/core/file/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      235 2022-07-24 17:11:51.000000 vampytest-0.0.9/vampytest/core/file/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3234 2022-07-24 20:51:54.000000 vampytest-0.0.9/vampytest/core/file/collection.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9474 2023-02-15 17:01:20.000000 vampytest-0.0.9/vampytest/core/file/file_system_entry.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2106 2022-12-19 10:54:46.000000 vampytest-0.0.9/vampytest/core/file/load_failure.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15847 2023-06-05 09:55:49.000000 vampytest-0.0.9/vampytest/core/file/test_file.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21860 2023-06-04 15:55:12.000000 vampytest-0.0.9/vampytest/core/handle.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.328494 vampytest-0.0.9/vampytest/core/helpers/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      273 2023-06-03 15:00:30.000000 vampytest-0.0.9/vampytest/core/helpers/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1518 2023-06-03 18:40:58.000000 vampytest-0.0.9/vampytest/core/helpers/exception_matching.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2549 2023-06-03 14:53:17.000000 vampytest-0.0.9/vampytest/core/helpers/hashing.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1633 2023-06-03 14:55:07.000000 vampytest-0.0.9/vampytest/core/helpers/merging.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2366 2023-06-03 14:57:31.000000 vampytest-0.0.9/vampytest/core/helpers/path_repr.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2354 2023-06-03 14:52:20.000000 vampytest-0.0.9/vampytest/core/helpers/un_nesting.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.328494 vampytest-0.0.9/vampytest/core/result/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      110 2023-06-04 12:40:46.000000 vampytest-0.0.9/vampytest/core/result/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.332494 vampytest-0.0.9/vampytest/core/result/reports/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      241 2023-06-04 19:01:59.000000 vampytest-0.0.9/vampytest/core/result/reports/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1115 2023-06-04 18:41:12.000000 vampytest-0.0.9/vampytest/core/result/reports/asserting.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      869 2023-06-04 16:49:37.000000 vampytest-0.0.9/vampytest/core/result/reports/base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      698 2023-06-04 16:52:34.000000 vampytest-0.0.9/vampytest/core/result/reports/output.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2006 2023-06-04 19:05:23.000000 vampytest-0.0.9/vampytest/core/result/reports/raising.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1472 2023-06-04 19:12:11.000000 vampytest-0.0.9/vampytest/core/result/reports/returning.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10268 2023-06-04 20:37:00.000000 vampytest-0.0.9/vampytest/core/result/result.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8411 2023-06-04 07:01:08.000000 vampytest-0.0.9/vampytest/core/run_state.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.332494 vampytest-0.0.9/vampytest/core/runner/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      104 2022-12-19 10:55:58.000000 vampytest-0.0.9/vampytest/core/runner/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10798 2023-06-04 20:30:43.000000 vampytest-0.0.9/vampytest/core/runner/context.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10435 2023-06-04 07:02:40.000000 vampytest-0.0.9/vampytest/core/runner/runner.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7836 2023-06-04 08:01:22.000000 vampytest-0.0.9/vampytest/core/test_case.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.332494 vampytest-0.0.9/vampytest/core/utils/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      207 2023-06-05 06:55:53.000000 vampytest-0.0.9/vampytest/core/utils/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      150 2023-06-05 07:43:47.000000 vampytest-0.0.9/vampytest/core/utils/aliases.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2189 2023-06-05 08:05:15.000000 vampytest-0.0.9/vampytest/core/utils/capture_output_context_manager.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      360 2023-06-03 15:06:42.000000 vampytest-0.0.9/vampytest/core/utils/wrap_nothing.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.332494 vampytest-0.0.9/vampytest/core/wrappers/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      883 2023-06-03 19:28:37.000000 vampytest-0.0.9/vampytest/core/wrappers/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1221 2023-06-05 09:29:38.000000 vampytest-0.0.9/vampytest/core/wrappers/aliases.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7302 2023-06-05 09:14:21.000000 vampytest-0.0.9/vampytest/core/wrappers/wrapper_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20677 2023-06-05 09:06:02.000000 vampytest-0.0.9/vampytest/core/wrappers/wrapper_call.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17716 2023-06-05 09:54:49.000000 vampytest-0.0.9/vampytest/core/wrappers/wrapper_call_from.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3866 2023-06-03 19:12:42.000000 vampytest-0.0.9/vampytest/core/wrappers/wrapper_chainer.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3067 2023-06-04 17:39:27.000000 vampytest-0.0.9/vampytest/core/wrappers/wrapper_conflict.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1771 2023-06-05 09:55:49.000000 vampytest-0.0.9/vampytest/core/wrappers/wrapper_environment.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2572 2023-06-04 14:02:29.000000 vampytest-0.0.9/vampytest/core/wrappers/wrapper_garbage_collect.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      921 2023-06-05 09:55:49.000000 vampytest-0.0.9/vampytest/core/wrappers/wrapper_reverse.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      743 2023-06-05 09:55:49.000000 vampytest-0.0.9/vampytest/core/wrappers/wrapper_skip.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1612 2023-06-05 09:55:49.000000 vampytest-0.0.9/vampytest/core/wrappers/wrapper_skip_conditional.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.332494 vampytest-0.0.9/vampytest/main/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5617 2022-12-19 11:06:38.000000 vampytest-0.0.9/vampytest/main/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:49:05.324494 vampytest-0.0.9/vampytest.egg-info/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1506 2023-06-08 09:49:05.000000 vampytest-0.0.9/vampytest.egg-info/PKG-INFO
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4021 2023-06-08 09:49:05.000000 vampytest-0.0.9/vampytest.egg-info/SOURCES.txt
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)        1 2023-06-08 09:49:05.000000 vampytest-0.0.9/vampytest.egg-info/dependency_links.txt
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       10 2023-06-08 09:49:05.000000 vampytest-0.0.9/vampytest.egg-info/requires.txt
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       10 2023-06-08 09:49:05.000000 vampytest-0.0.9/vampytest.egg-info/top_level.txt
```

### Comparing `vampytest-0.0.8/PKG-INFO` & `vampytest-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vampytest
-Version: 0.0.8
+Version: 0.0.9
 Summary: A vampy test framework
 Home-page: https://github.com/HuyaneMatsu/vampytest
 Author: HuyaneMatsu
 Author-email: re.ism.tm@gmail.com
 License: DBAD
 Description: <h1 align="center">
             Vampytest
```

### Comparing `vampytest-0.0.8/setup.py` & `vampytest-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/__init__.py` & `vampytest-0.0.9/vampytest/core/__init__.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/__init__.py` & `vampytest-0.0.9/vampytest/core/assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/aliases.py` & `vampytest-0.0.9/vampytest/core/assertions/aliases.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/assertion_base.py` & `vampytest-0.0.9/vampytest/core/assertions/assertion_base.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/assertion_conditional_base.py` & `vampytest-0.0.9/vampytest/core/assertions/assertion_conditional_base.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/assertion_contains.py` & `vampytest-0.0.9/vampytest/core/assertions/assertion_contains.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/assertion_equals.py` & `vampytest-0.0.9/vampytest/core/assertions/assertion_equals.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/assertion_false.py` & `vampytest-0.0.9/vampytest/core/assertions/assertion_false.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/assertion_identical.py` & `vampytest-0.0.9/vampytest/core/assertions/assertion_identical.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/assertion_instance.py` & `vampytest-0.0.9/vampytest/core/assertions/assertion_instance.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/assertion_not_contains.py` & `vampytest-0.0.9/vampytest/core/assertions/assertion_not_contains.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/assertion_not_equals.py` & `vampytest-0.0.9/vampytest/core/assertions/assertion_not_equals.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/assertion_not_identical.py` & `vampytest-0.0.9/vampytest/core/assertions/assertion_not_identical.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/assertion_raising.py` & `vampytest-0.0.9/vampytest/core/assertions/assertion_raising.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/assertion_states.py` & `vampytest-0.0.9/vampytest/core/assertions/assertion_states.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/assertion_subtype.py` & `vampytest-0.0.9/vampytest/core/assertions/assertion_subtype.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/assertion_true.py` & `vampytest-0.0.9/vampytest/core/assertions/assertion_true.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/assertions/exceptions.py` & `vampytest-0.0.9/vampytest/core/assertions/exceptions.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/contexts/base.py` & `vampytest-0.0.9/vampytest/core/contexts/base.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/contexts/calling.py` & `vampytest-0.0.9/vampytest/core/contexts/calling.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/contexts/garbage_collect.py` & `vampytest-0.0.9/vampytest/core/contexts/garbage_collect.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/contexts/output_capturing.py` & `vampytest-0.0.9/vampytest/core/contexts/output_capturing.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/environment/configuration.py` & `vampytest-0.0.9/vampytest/core/environment/configuration.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/environment/default.py` & `vampytest-0.0.9/vampytest/core/environment/default.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/environment/helpers.py` & `vampytest-0.0.9/vampytest/core/environment/helpers.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/environment/manager.py` & `vampytest-0.0.9/vampytest/core/environment/manager.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/environment/scarletio_coroutine.py` & `vampytest-0.0.9/vampytest/core/environment/scarletio_coroutine.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/event_handling/base.py` & `vampytest-0.0.9/vampytest/core/event_handling/base.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/event_handling/default.py` & `vampytest-0.0.9/vampytest/core/event_handling/default.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/event_handling/default_output_writer.py` & `vampytest-0.0.9/vampytest/core/event_handling/default_output_writer.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/event_handling/rendering_helpers/result_modifier_parameters.py` & `vampytest-0.0.9/vampytest/core/event_handling/rendering_helpers/result_modifier_parameters.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/event_handling/rendering_helpers/result_rendering.py` & `vampytest-0.0.9/vampytest/core/event_handling/rendering_helpers/result_rendering.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,15 +317,15 @@
     Returns
     -------
     into : `list` of `str`
     """
     into = render_test_position_into(into, 'Assertion failed', COLOR_FAIL, result)
     maybe_render_parameters_section_into(into, result)
     into.append('\n')
-    into = report.assertion_exception.render_into_into(into)
+    into = report.assertion_exception.render_failure_message_parts_into(into)
     into = maybe_render_output_into(into, result)
     return into
 
 
 def render_report_raising_into(into, result, report):
     """
     Renders raising failure report.
```

### Comparing `vampytest-0.0.8/vampytest/core/event_handling/rendering_helpers/writers.py` & `vampytest-0.0.9/vampytest/core/event_handling/rendering_helpers/writers.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/event_handling/text_styling.py` & `vampytest-0.0.9/vampytest/core/event_handling/text_styling.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/events/__init__.py` & `vampytest-0.0.9/vampytest/core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/events/base.py` & `vampytest-0.0.9/vampytest/core/events/base.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/events/file_load_done.py` & `vampytest-0.0.9/vampytest/core/events/file_load_done.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/file/collection.py` & `vampytest-0.0.9/vampytest/core/file/collection.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/file/file_system_entry.py` & `vampytest-0.0.9/vampytest/core/file/file_system_entry.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/file/load_failure.py` & `vampytest-0.0.9/vampytest/core/file/load_failure.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/file/test_file.py` & `vampytest-0.0.9/vampytest/core/file/test_file.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/handle.py` & `vampytest-0.0.9/vampytest/core/handle.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/helpers/exception_matching.py` & `vampytest-0.0.9/vampytest/core/helpers/exception_matching.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/helpers/hashing.py` & `vampytest-0.0.9/vampytest/core/helpers/hashing.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/helpers/merging.py` & `vampytest-0.0.9/vampytest/core/helpers/merging.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/helpers/path_repr.py` & `vampytest-0.0.9/vampytest/core/helpers/path_repr.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/helpers/un_nesting.py` & `vampytest-0.0.9/vampytest/core/helpers/un_nesting.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/result/reports/asserting.py` & `vampytest-0.0.9/vampytest/core/result/reports/asserting.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/result/reports/base.py` & `vampytest-0.0.9/vampytest/core/result/reports/base.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/result/reports/output.py` & `vampytest-0.0.9/vampytest/core/result/reports/output.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/result/reports/raising.py` & `vampytest-0.0.9/vampytest/core/result/reports/raising.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/result/reports/returning.py` & `vampytest-0.0.9/vampytest/core/result/reports/returning.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/result/result.py` & `vampytest-0.0.9/vampytest/core/result/result.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/run_state.py` & `vampytest-0.0.9/vampytest/core/run_state.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/runner/context.py` & `vampytest-0.0.9/vampytest/core/runner/context.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/runner/runner.py` & `vampytest-0.0.9/vampytest/core/runner/runner.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/test_case.py` & `vampytest-0.0.9/vampytest/core/test_case.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/utils/capture_output_context_manager.py` & `vampytest-0.0.9/vampytest/core/utils/capture_output_context_manager.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/wrappers/__init__.py` & `vampytest-0.0.9/vampytest/core/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/wrappers/aliases.py` & `vampytest-0.0.9/vampytest/core/wrappers/aliases.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/wrappers/wrapper_base.py` & `vampytest-0.0.9/vampytest/core/wrappers/wrapper_base.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/wrappers/wrapper_call.py` & `vampytest-0.0.9/vampytest/core/wrappers/wrapper_call.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/wrappers/wrapper_call_from.py` & `vampytest-0.0.9/vampytest/core/wrappers/wrapper_call_from.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/wrappers/wrapper_chainer.py` & `vampytest-0.0.9/vampytest/core/wrappers/wrapper_chainer.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/wrappers/wrapper_conflict.py` & `vampytest-0.0.9/vampytest/core/wrappers/wrapper_conflict.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/wrappers/wrapper_environment.py` & `vampytest-0.0.9/vampytest/core/wrappers/wrapper_environment.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/wrappers/wrapper_garbage_collect.py` & `vampytest-0.0.9/vampytest/core/wrappers/wrapper_garbage_collect.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/wrappers/wrapper_reverse.py` & `vampytest-0.0.9/vampytest/core/wrappers/wrapper_reverse.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/wrappers/wrapper_skip.py` & `vampytest-0.0.9/vampytest/core/wrappers/wrapper_skip.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/core/wrappers/wrapper_skip_conditional.py` & `vampytest-0.0.9/vampytest/core/wrappers/wrapper_skip_conditional.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest/main/__init__.py` & `vampytest-0.0.9/vampytest/main/__init__.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.8/vampytest.egg-info/PKG-INFO` & `vampytest-0.0.9/vampytest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vampytest
-Version: 0.0.8
+Version: 0.0.9
 Summary: A vampy test framework
 Home-page: https://github.com/HuyaneMatsu/vampytest
 Author: HuyaneMatsu
 Author-email: re.ism.tm@gmail.com
 License: DBAD
 Description: <h1 align="center">
             Vampytest
```

### Comparing `vampytest-0.0.8/vampytest.egg-info/SOURCES.txt` & `vampytest-0.0.9/vampytest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

