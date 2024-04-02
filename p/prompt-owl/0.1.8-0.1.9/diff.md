# Comparing `tmp/prompt-owl-0.1.8.tar.gz` & `tmp/prompt-owl-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt-owl-0.1.8.tar", last modified: Sat Mar 23 14:13:57 2024, max compression
+gzip compressed data, was "prompt-owl-0.1.9.tar", last modified: Sat Mar 23 14:52:12 2024, max compression
```

## Comparing `prompt-owl-0.1.8.tar` & `prompt-owl-0.1.9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.032808 prompt-owl-0.1.8/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     1067 2024-03-19 09:56:00.000000 prompt-owl-0.1.8/LICENSE
--rw-rw-r--   0 osiris    (1000) osiris    (1000)      243 2024-03-19 10:00:08.000000 prompt-owl-0.1.8/MANIFEST.in
--rw-rw-r--   0 osiris    (1000) osiris    (1000)    23350 2024-03-23 14:13:57.032808 prompt-owl-0.1.8/PKG-INFO
--rw-rw-r--   0 osiris    (1000) osiris    (1000)    22873 2024-03-19 11:17:24.000000 prompt-owl-0.1.8/README.md
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.024808 prompt-owl-0.1.8/prompt_owl.egg-info/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)    23350 2024-03-23 14:13:57.000000 prompt-owl-0.1.8/prompt_owl.egg-info/PKG-INFO
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     1607 2024-03-23 14:13:57.000000 prompt-owl-0.1.8/prompt_owl.egg-info/SOURCES.txt
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        1 2024-03-23 14:13:57.000000 prompt-owl-0.1.8/prompt_owl.egg-info/dependency_links.txt
--rw-rw-r--   0 osiris    (1000) osiris    (1000)       42 2024-03-23 14:13:57.000000 prompt-owl-0.1.8/prompt_owl.egg-info/entry_points.txt
--rw-rw-r--   0 osiris    (1000) osiris    (1000)       32 2024-03-23 14:13:57.000000 prompt-owl-0.1.8/prompt_owl.egg-info/requires.txt
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        6 2024-03-23 14:13:57.000000 prompt-owl-0.1.8/prompt_owl.egg-info/top_level.txt
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.024808 prompt-owl-0.1.8/prowl/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)       54 2024-03-21 16:56:27.000000 prompt-owl-0.1.8/prowl/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     4336 2024-03-20 09:46:24.000000 prompt-owl-0.1.8/prowl/cli.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/examples/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/examples/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     1879 2024-03-23 12:54:54.000000 prompt-owl-0.1.8/prowl/examples/aggsummary.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     2226 2024-02-18 19:58:52.000000 prompt-owl-0.1.8/prowl/examples/codeit.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     1085 2024-03-23 13:42:27.000000 prompt-owl-0.1.8/prowl/examples/image.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)      546 2024-03-14 20:42:31.000000 prompt-owl-0.1.8/prowl/examples/knowledge.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)      374 2024-02-17 16:58:15.000000 prompt-owl-0.1.8/prowl/examples/monster_gen.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     2531 2024-03-23 13:24:48.000000 prompt-owl-0.1.8/prowl/examples/ragtot.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)      588 2024-01-14 19:26:21.000000 prompt-owl-0.1.8/prowl/examples/self_improve.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     1744 2024-01-14 19:26:06.000000 prompt-owl-0.1.8/prowl/examples/self_write.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     4458 2024-02-12 20:48:13.000000 prompt-owl-0.1.8/prowl/examples/state.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)      393 2024-03-21 17:03:18.000000 prompt-owl-0.1.8/prowl/examples/streaming.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)      385 2024-01-14 19:25:36.000000 prompt-owl-0.1.8/prowl/examples/todo.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/lib/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/lib/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)      333 2024-01-18 23:59:16.000000 prompt-owl-0.1.8/prowl/lib/error.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)    18599 2024-03-21 17:00:39.000000 prompt-owl-0.1.8/prowl/lib/prowl.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)    18579 2024-03-21 16:56:21.000000 prompt-owl-0.1.8/prowl/lib/stack.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     2989 2024-01-30 18:34:09.000000 prompt-owl-0.1.8/prowl/lib/tool.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     5518 2024-03-23 14:12:45.000000 prompt-owl-0.1.8/prowl/lib/vllm.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/tools/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/tools/__init__.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/tools/collect/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/tools/collect/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     1076 2024-03-21 22:52:04.000000 prompt-owl-0.1.8/prowl/tools/collect/tool.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/tools/comfy/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/tools/comfy/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     3398 2024-01-27 10:56:11.000000 prompt-owl-0.1.8/prowl/tools/comfy/comfyutil.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     4147 2024-03-21 22:44:50.000000 prompt-owl-0.1.8/prowl/tools/comfy/tool.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/tools/concat/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/tools/concat/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)      506 2024-03-21 22:52:14.000000 prompt-owl-0.1.8/prowl/tools/concat/tool.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/tools/each/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/tools/each/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     3224 2024-03-21 22:53:37.000000 prompt-owl-0.1.8/prowl/tools/each/tool.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/tools/file/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/tools/file/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)      650 2024-03-21 22:53:46.000000 prompt-owl-0.1.8/prowl/tools/file/tool.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/tools/include/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/tools/include/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)      672 2024-03-21 23:17:08.000000 prompt-owl-0.1.8/prowl/tools/include/tool.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/tools/list/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/tools/list/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     1412 2024-03-21 23:17:15.000000 prompt-owl-0.1.8/prowl/tools/list/tool.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/tools/navigate/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/tools/navigate/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)      736 2024-03-21 23:17:21.000000 prompt-owl-0.1.8/prowl/tools/navigate/tool.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/tools/out/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/tools/out/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     2457 2024-03-21 23:17:26.000000 prompt-owl-0.1.8/prowl/tools/out/tool.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/tools/prowl/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/tools/prowl/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     1640 2024-03-21 23:17:36.000000 prompt-owl-0.1.8/prowl/tools/prowl/tool.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/tools/recall/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/tools/recall/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     1198 2024-03-21 23:17:44.000000 prompt-owl-0.1.8/prowl/tools/recall/tool.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/tools/script/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/tools/script/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)      667 2024-03-21 23:17:52.000000 prompt-owl-0.1.8/prowl/tools/script/tool.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.028808 prompt-owl-0.1.8/prowl/tools/search/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/tools/search/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)      840 2024-03-21 23:18:14.000000 prompt-owl-0.1.8/prowl/tools/search/tool.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.032808 prompt-owl-0.1.8/prowl/tools/time/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/tools/time/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)      987 2024-03-21 23:18:28.000000 prompt-owl-0.1.8/prowl/tools/time/tool.py
-drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:13:57.032808 prompt-owl-0.1.8/prowl/util/
--rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.8/prowl/util/__init__.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)      454 2024-01-17 19:31:27.000000 prompt-owl-0.1.8/prowl/util/vardump.py
--rw-rw-r--   0 osiris    (1000) osiris    (1000)       38 2024-03-23 14:13:57.032808 prompt-owl-0.1.8/setup.cfg
--rw-rw-r--   0 osiris    (1000) osiris    (1000)     1070 2024-03-23 14:13:54.000000 prompt-owl-0.1.8/setup.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.094978 prompt-owl-0.1.9/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     1067 2024-03-19 09:56:00.000000 prompt-owl-0.1.9/LICENSE
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)      243 2024-03-19 10:00:08.000000 prompt-owl-0.1.9/MANIFEST.in
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)    23350 2024-03-23 14:52:12.094978 prompt-owl-0.1.9/PKG-INFO
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)    22873 2024-03-19 11:17:24.000000 prompt-owl-0.1.9/README.md
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.086978 prompt-owl-0.1.9/prompt_owl.egg-info/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)    23350 2024-03-23 14:52:12.000000 prompt-owl-0.1.9/prompt_owl.egg-info/PKG-INFO
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     1607 2024-03-23 14:52:12.000000 prompt-owl-0.1.9/prompt_owl.egg-info/SOURCES.txt
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        1 2024-03-23 14:52:12.000000 prompt-owl-0.1.9/prompt_owl.egg-info/dependency_links.txt
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)       42 2024-03-23 14:52:12.000000 prompt-owl-0.1.9/prompt_owl.egg-info/entry_points.txt
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)       32 2024-03-23 14:52:12.000000 prompt-owl-0.1.9/prompt_owl.egg-info/requires.txt
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        6 2024-03-23 14:52:12.000000 prompt-owl-0.1.9/prompt_owl.egg-info/top_level.txt
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.086978 prompt-owl-0.1.9/prowl/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)       54 2024-03-21 16:56:27.000000 prompt-owl-0.1.9/prowl/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     4336 2024-03-20 09:46:24.000000 prompt-owl-0.1.9/prowl/cli.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.090978 prompt-owl-0.1.9/prowl/examples/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/examples/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     1879 2024-03-23 12:54:54.000000 prompt-owl-0.1.9/prowl/examples/aggsummary.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     2226 2024-02-18 19:58:52.000000 prompt-owl-0.1.9/prowl/examples/codeit.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     1085 2024-03-23 13:42:27.000000 prompt-owl-0.1.9/prowl/examples/image.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)      546 2024-03-14 20:42:31.000000 prompt-owl-0.1.9/prowl/examples/knowledge.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)      374 2024-02-17 16:58:15.000000 prompt-owl-0.1.9/prowl/examples/monster_gen.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     2531 2024-03-23 13:24:48.000000 prompt-owl-0.1.9/prowl/examples/ragtot.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)      588 2024-01-14 19:26:21.000000 prompt-owl-0.1.9/prowl/examples/self_improve.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     1744 2024-01-14 19:26:06.000000 prompt-owl-0.1.9/prowl/examples/self_write.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     4458 2024-02-12 20:48:13.000000 prompt-owl-0.1.9/prowl/examples/state.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)      393 2024-03-21 17:03:18.000000 prompt-owl-0.1.9/prowl/examples/streaming.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)      385 2024-01-14 19:25:36.000000 prompt-owl-0.1.9/prowl/examples/todo.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.090978 prompt-owl-0.1.9/prowl/lib/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/lib/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)      333 2024-01-18 23:59:16.000000 prompt-owl-0.1.9/prowl/lib/error.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)    18807 2024-03-23 14:50:12.000000 prompt-owl-0.1.9/prowl/lib/prowl.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)    18579 2024-03-21 16:56:21.000000 prompt-owl-0.1.9/prowl/lib/stack.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     2989 2024-01-30 18:34:09.000000 prompt-owl-0.1.9/prowl/lib/tool.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     5518 2024-03-23 14:47:20.000000 prompt-owl-0.1.9/prowl/lib/vllm.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.090978 prompt-owl-0.1.9/prowl/tools/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/tools/__init__.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.090978 prompt-owl-0.1.9/prowl/tools/collect/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/tools/collect/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     1076 2024-03-21 22:52:04.000000 prompt-owl-0.1.9/prowl/tools/collect/tool.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.090978 prompt-owl-0.1.9/prowl/tools/comfy/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/tools/comfy/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     3398 2024-01-27 10:56:11.000000 prompt-owl-0.1.9/prowl/tools/comfy/comfyutil.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     4147 2024-03-21 22:44:50.000000 prompt-owl-0.1.9/prowl/tools/comfy/tool.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.090978 prompt-owl-0.1.9/prowl/tools/concat/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/tools/concat/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)      506 2024-03-21 22:52:14.000000 prompt-owl-0.1.9/prowl/tools/concat/tool.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.090978 prompt-owl-0.1.9/prowl/tools/each/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/tools/each/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     3224 2024-03-21 22:53:37.000000 prompt-owl-0.1.9/prowl/tools/each/tool.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.090978 prompt-owl-0.1.9/prowl/tools/file/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/tools/file/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)      650 2024-03-21 22:53:46.000000 prompt-owl-0.1.9/prowl/tools/file/tool.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.090978 prompt-owl-0.1.9/prowl/tools/include/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/tools/include/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)      672 2024-03-21 23:17:08.000000 prompt-owl-0.1.9/prowl/tools/include/tool.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.090978 prompt-owl-0.1.9/prowl/tools/list/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/tools/list/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     1412 2024-03-21 23:17:15.000000 prompt-owl-0.1.9/prowl/tools/list/tool.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.090978 prompt-owl-0.1.9/prowl/tools/navigate/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/tools/navigate/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)      736 2024-03-21 23:17:21.000000 prompt-owl-0.1.9/prowl/tools/navigate/tool.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.090978 prompt-owl-0.1.9/prowl/tools/out/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/tools/out/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     2457 2024-03-21 23:17:26.000000 prompt-owl-0.1.9/prowl/tools/out/tool.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.090978 prompt-owl-0.1.9/prowl/tools/prowl/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/tools/prowl/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     1640 2024-03-21 23:17:36.000000 prompt-owl-0.1.9/prowl/tools/prowl/tool.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.094978 prompt-owl-0.1.9/prowl/tools/recall/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/tools/recall/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     1198 2024-03-21 23:17:44.000000 prompt-owl-0.1.9/prowl/tools/recall/tool.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.094978 prompt-owl-0.1.9/prowl/tools/script/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/tools/script/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)      667 2024-03-21 23:17:52.000000 prompt-owl-0.1.9/prowl/tools/script/tool.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.094978 prompt-owl-0.1.9/prowl/tools/search/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/tools/search/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)      840 2024-03-21 23:18:14.000000 prompt-owl-0.1.9/prowl/tools/search/tool.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.094978 prompt-owl-0.1.9/prowl/tools/time/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/tools/time/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)      987 2024-03-21 23:18:28.000000 prompt-owl-0.1.9/prowl/tools/time/tool.py
+drwxrwxr-x   0 osiris    (1000) osiris    (1000)        0 2024-03-23 14:52:12.094978 prompt-owl-0.1.9/prowl/util/
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)        0 2023-07-17 15:17:53.000000 prompt-owl-0.1.9/prowl/util/__init__.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)      454 2024-01-17 19:31:27.000000 prompt-owl-0.1.9/prowl/util/vardump.py
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)       38 2024-03-23 14:52:12.094978 prompt-owl-0.1.9/setup.cfg
+-rw-rw-r--   0 osiris    (1000) osiris    (1000)     1070 2024-03-23 14:50:40.000000 prompt-owl-0.1.9/setup.py
```

### Comparing `prompt-owl-0.1.8/LICENSE` & `prompt-owl-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/PKG-INFO` & `prompt-owl-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-owl
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Declarative Prompting Language for LLMs
 Home-page: https://github.com/lks-ai/prowl
 Author: LoreKeeper Ltd
 Author-email: nathaniel@lorekeeper.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prompt-owl-0.1.8/README.md` & `prompt-owl-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prompt_owl.egg-info/PKG-INFO` & `prompt-owl-0.1.9/prompt_owl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-owl
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Declarative Prompting Language for LLMs
 Home-page: https://github.com/lks-ai/prowl
 Author: LoreKeeper Ltd
 Author-email: nathaniel@lorekeeper.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prompt-owl-0.1.8/prompt_owl.egg-info/SOURCES.txt` & `prompt-owl-0.1.9/prompt_owl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/cli.py` & `prompt-owl-0.1.9/prowl/cli.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/examples/aggsummary.py` & `prompt-owl-0.1.9/prowl/examples/aggsummary.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/examples/codeit.py` & `prompt-owl-0.1.9/prowl/examples/codeit.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/examples/image.py` & `prompt-owl-0.1.9/prowl/examples/image.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/examples/knowledge.py` & `prompt-owl-0.1.9/prowl/examples/knowledge.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/examples/ragtot.py` & `prompt-owl-0.1.9/prowl/examples/ragtot.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/examples/self_improve.py` & `prompt-owl-0.1.9/prowl/examples/self_improve.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/examples/self_write.py` & `prompt-owl-0.1.9/prowl/examples/self_write.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/examples/state.py` & `prompt-owl-0.1.9/prowl/examples/state.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/lib/prowl.py` & `prompt-owl-0.1.9/prowl/lib/prowl.py`

 * *Files 2% similar despite different names*

```diff
@@ -365,14 +365,18 @@
                         prompt.rstrip(" "),
                         max_tokens = int_arg,
                         temperature = float_arg + fex,
                         stop = stops,
                         streaming = stream_level == prowl.StreamLevel.TOKEN,
                         stream_callback = token_event,
                     )
+                    if r.get('object', '') == 'error':
+                        if not silent:
+                            print(f"VLLM ERROR: {r}")
+                        raise ValueError(f"{r['message']}")
                     usage.add(r['usage'])
                     # get the final completion and perform cleanup from 0th choice
                     completion = await prowl.align_conditioning(prompt, (var_name, int_arg, float_arg), r['choices'][0], usage, llm, multiline, continue_ratio=continue_ratio, stops=stops, token_event=token_event)
                     tries += 1
                     if tries >= max_retries:
                         left_context = None if len(prompt) < 30 else prompt[-30:].replace("\n", "\\n")
                         if not silent:
```

### Comparing `prompt-owl-0.1.8/prowl/lib/stack.py` & `prompt-owl-0.1.9/prowl/lib/stack.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/lib/tool.py` & `prompt-owl-0.1.9/prowl/lib/tool.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/lib/vllm.py` & `prompt-owl-0.1.9/prowl/lib/vllm.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/tools/collect/tool.py` & `prompt-owl-0.1.9/prowl/tools/collect/tool.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/tools/comfy/comfyutil.py` & `prompt-owl-0.1.9/prowl/tools/comfy/comfyutil.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/tools/comfy/tool.py` & `prompt-owl-0.1.9/prowl/tools/comfy/tool.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/tools/each/tool.py` & `prompt-owl-0.1.9/prowl/tools/each/tool.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/tools/file/tool.py` & `prompt-owl-0.1.9/prowl/tools/file/tool.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/tools/include/tool.py` & `prompt-owl-0.1.9/prowl/tools/include/tool.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/tools/list/tool.py` & `prompt-owl-0.1.9/prowl/tools/list/tool.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/tools/navigate/tool.py` & `prompt-owl-0.1.9/prowl/tools/navigate/tool.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/tools/out/tool.py` & `prompt-owl-0.1.9/prowl/tools/out/tool.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/tools/prowl/tool.py` & `prompt-owl-0.1.9/prowl/tools/prowl/tool.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/tools/recall/tool.py` & `prompt-owl-0.1.9/prowl/tools/recall/tool.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/tools/script/tool.py` & `prompt-owl-0.1.9/prowl/tools/script/tool.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/tools/search/tool.py` & `prompt-owl-0.1.9/prowl/tools/search/tool.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/prowl/tools/time/tool.py` & `prompt-owl-0.1.9/prowl/tools/time/tool.py`

 * *Files identical despite different names*

### Comparing `prompt-owl-0.1.8/setup.py` & `prompt-owl-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='prompt-owl',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(where='.'),
     install_requires=[
         'requests>=2.31.0',
         'aiohttp>=3.9.1',
     ],
     python_requires='>=3.9',
     entry_points={
```

