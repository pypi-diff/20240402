# Comparing `tmp/uagents_ai_engine-0.1.2.tar.gz` & `tmp/uagents_ai_engine-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents_ai_engine-0.1.2.tar", max compression
+gzip compressed data, was "uagents_ai_engine-0.1.3.tar", max compression
```

## Comparing `uagents_ai_engine-0.1.2.tar` & `uagents_ai_engine-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0      209 2023-09-14 14:01:16.264573 uagents_ai_engine-0.1.2/README.md
--rw-r--r--   0        0        0      388 2023-10-11 08:52:27.670226 uagents_ai_engine-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       89 2023-10-11 08:51:46.547970 uagents_ai_engine-0.1.2/src/ai_engine/__init__.py
--rw-r--r--   0        0        0      765 2023-10-11 08:50:50.576710 uagents_ai_engine-0.1.2/src/ai_engine/types.py
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 uagents_ai_engine-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      209 2024-03-15 19:58:48.912304 uagents_ai_engine-0.1.3/README.md
+-rw-r--r--   0        0        0      394 2024-03-22 11:42:47.916667 uagents_ai_engine-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       89 2024-03-15 19:58:57.112803 uagents_ai_engine-0.1.3/src/ai_engine/__init__.py
+-rw-r--r--   0        0        0     4487 2024-03-28 09:54:43.757710 uagents_ai_engine-0.1.3/src/ai_engine/chitchat.py
+-rw-r--r--   0        0        0     2284 2024-03-25 05:19:14.446118 uagents_ai_engine-0.1.3/src/ai_engine/dialogue.py
+-rw-r--r--   0        0        0     2964 2024-03-28 14:22:24.183225 uagents_ai_engine-0.1.3/src/ai_engine/messages.py
+-rw-r--r--   0        0        0      765 2024-03-15 19:58:48.914653 uagents_ai_engine-0.1.3/src/ai_engine/types.py
+-rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 uagents_ai_engine-0.1.3/PKG-INFO
```

### Comparing `uagents_ai_engine-0.1.2/src/ai_engine/types.py` & `uagents_ai_engine-0.1.3/src/ai_engine/types.py`

 * *Files identical despite different names*

