# Comparing `tmp/dailalib-2.3.1.tar.gz` & `tmp/dailalib-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dailalib-2.3.1.tar", last modified: Mon Feb 26 20:39:51 2024, max compression
+gzip compressed data, was "dailalib-2.3.2.tar", last modified: Tue Apr  2 03:55:05 2024, max compression
```

## Comparing `dailalib-2.3.1.tar` & `dailalib-2.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:39:51.919560 dailalib-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-02-26 20:39:51.919560 dailalib-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-02-26 20:39:44.000000 dailalib-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:39:51.915560 dailalib-2.3.1/dailalib/
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-02-26 20:39:44.000000 dailalib-2.3.1/dailalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-02-26 20:39:44.000000 dailalib-2.3.1/dailalib/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:39:51.919560 dailalib-2.3.1/dailalib/api/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-26 20:39:44.000000 dailalib-2.3.1/dailalib/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-02-26 20:39:44.000000 dailalib-2.3.1/dailalib/api/ai_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:39:51.919560 dailalib-2.3.1/dailalib/api/openai/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-26 20:39:44.000000 dailalib-2.3.1/dailalib/api/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-02-26 20:39:44.000000 dailalib-2.3.1/dailalib/api/openai/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-02-26 20:39:44.000000 dailalib-2.3.1/dailalib/api/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-02-26 20:39:44.000000 dailalib-2.3.1/dailalib/api/openai/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:39:51.919560 dailalib-2.3.1/dailalib/binsync_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-02-26 20:39:44.000000 dailalib-2.3.1/dailalib/binsync_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-02-26 20:39:44.000000 dailalib-2.3.1/dailalib/binsync_plugin/ai_bs_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-02-26 20:39:44.000000 dailalib-2.3.1/dailalib/binsync_plugin/ai_user_config_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-02-26 20:39:44.000000 dailalib-2.3.1/dailalib/binsync_plugin/openai_bs_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-02-26 20:39:44.000000 dailalib-2.3.1/dailalib/binsync_plugin/varmodel_bs_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-26 20:39:44.000000 dailalib-2.3.1/dailalib/daila_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-02-26 20:39:44.000000 dailalib-2.3.1/dailalib/installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:39:51.919560 dailalib-2.3.1/dailalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-02-26 20:39:51.000000 dailalib-2.3.1/dailalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-02-26 20:39:51.000000 dailalib-2.3.1/dailalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 20:39:51.000000 dailalib-2.3.1/dailalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-26 20:39:51.000000 dailalib-2.3.1/dailalib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-26 20:39:51.000000 dailalib-2.3.1/dailalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-26 20:39:51.000000 dailalib-2.3.1/dailalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-26 20:39:51.919560 dailalib-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 20:39:44.000000 dailalib-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:55:05.045104 dailalib-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-04-02 03:55:05.045104 dailalib-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-02 03:55:01.000000 dailalib-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:55:05.045104 dailalib-2.3.2/dailalib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:55:05.045104 dailalib-2.3.2/dailalib/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/api/ai_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:55:05.045104 dailalib-2.3.2/dailalib/api/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/api/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/api/openai/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/api/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/api/openai/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:55:05.045104 dailalib-2.3.2/dailalib/binsync_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/binsync_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/binsync_plugin/ai_bs_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/binsync_plugin/ai_user_config_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/binsync_plugin/openai_bs_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/binsync_plugin/varmodel_bs_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/daila_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:55:05.045104 dailalib-2.3.2/dailalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-04-02 03:55:05.000000 dailalib-2.3.2/dailalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-02 03:55:05.000000 dailalib-2.3.2/dailalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 03:55:05.000000 dailalib-2.3.2/dailalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 03:55:05.000000 dailalib-2.3.2/dailalib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 03:55:05.000000 dailalib-2.3.2/dailalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 03:55:05.000000 dailalib-2.3.2/dailalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-02 03:55:05.049104 dailalib-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 03:55:01.000000 dailalib-2.3.2/setup.py
```

### Comparing `dailalib-2.3.1/PKG-INFO` & `dailalib-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dailalib
-Version: 2.3.1
+Version: 2.3.2
 Summary: The Decompiler Artificial Intelligence Language Assistant (DAILA) is a tool for adding AI to decompilers.
 Home-page: https://github.com/mahaloz/DAILA
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
```

### Comparing `dailalib-2.3.1/README.md` & `dailalib-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.1/dailalib/__init__.py` & `dailalib-2.3.2/dailalib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.3.1"
+__version__ = "2.3.2"
 
 from .api import AIAPI, OpenAIAPI
 from libbs.api import DecompilerInterface
 
 
 def create_plugin(*args, **kwargs):
 
@@ -24,15 +24,15 @@
     #
 
     from varbert.api import VariableRenamingAPI
     var_api = VariableRenamingAPI(delay_init=True)
 
     # add single interface, which is to rename variables
     def make_callback(predict_for_all_variables):
-        return lambda *args, **kwargs: var_api.query_model(*args, **kwargs, remove_bad_names=not predict_for_all_variables)
+        return lambda *args, **kwargs: var_api.query_model(**kwargs, remove_bad_names=not predict_for_all_variables)
 
     gui_ctx_menu_actions["DAILA/VarBERT/varbert_rename_vars"] = ("Suggest new variable names (source-like only)", make_callback(predict_for_all_variables=False))
     gui_ctx_menu_actions["DAILA/VarBERT/varbert_rename_vars_all"] = ("Suggest new variable names (for all variables)", make_callback(predict_for_all_variables=True))
 
     #
     # Decompiler Plugin Registration
     #
```

### Comparing `dailalib-2.3.1/dailalib/__main__.py` & `dailalib-2.3.2/dailalib/__main__.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.1/dailalib/api/ai_api.py` & `dailalib-2.3.2/dailalib/api/ai_api.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.1/dailalib/api/openai/openai_api.py` & `dailalib-2.3.2/dailalib/api/openai/openai_api.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.1/dailalib/api/openai/prompt.py` & `dailalib-2.3.2/dailalib/api/openai/prompt.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.1/dailalib/api/openai/prompts.py` & `dailalib-2.3.2/dailalib/api/openai/prompts.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.1/dailalib/binsync_plugin/__init__.py` & `dailalib-2.3.2/dailalib/binsync_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.1/dailalib/binsync_plugin/ai_bs_user.py` & `dailalib-2.3.2/dailalib/binsync_plugin/ai_bs_user.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.1/dailalib/binsync_plugin/ai_user_config_ui.py` & `dailalib-2.3.2/dailalib/binsync_plugin/ai_user_config_ui.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.1/dailalib/binsync_plugin/openai_bs_user.py` & `dailalib-2.3.2/dailalib/binsync_plugin/openai_bs_user.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.1/dailalib/binsync_plugin/varmodel_bs_user.py` & `dailalib-2.3.2/dailalib/binsync_plugin/varmodel_bs_user.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.1/dailalib/daila_plugin.py` & `dailalib-2.3.2/dailalib/daila_plugin.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.1/dailalib/installer.py` & `dailalib-2.3.2/dailalib/installer.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.1/dailalib.egg-info/PKG-INFO` & `dailalib-2.3.2/dailalib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dailalib
-Version: 2.3.1
+Version: 2.3.2
 Summary: The Decompiler Artificial Intelligence Language Assistant (DAILA) is a tool for adding AI to decompilers.
 Home-page: https://github.com/mahaloz/DAILA
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
```

### Comparing `dailalib-2.3.1/dailalib.egg-info/SOURCES.txt` & `dailalib-2.3.2/dailalib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.1/setup.cfg` & `dailalib-2.3.2/setup.cfg`

 * *Files identical despite different names*

