# Comparing `tmp/openllm_core-0.5.0a1.tar.gz` & `tmp/openllm_core-0.5.0a2.tar.gz`

## Comparing `openllm_core-0.5.0a1.tar` & `openllm_core-0.5.0a2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/README.md
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/__init__.py
--rw-r--r--   0        0        0    29829 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/_configuration.py
--rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/_schemas.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/_typing_compat.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/_version.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/py.typed
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/__init__.py
--rw-r--r--   0        0        0     8440 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_auto.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_baichuan.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_chatglm.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_dolly_v2.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_falcon.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_flan_t5.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_gemma.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_gpt_neox.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_llama.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_mistral.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_mixtral.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_mpt.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_opt.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_phi.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_qwen.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_stablelm.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_starcoder.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/config/configuration_yi.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/protocol/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/protocol/hf.py
--rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/protocol/openai.py
--rw-r--r--   0        0        0    13798 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/utils/__init__.py
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/utils/__init__.pyi
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/utils/_constants.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/utils/analytics.py
--rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/utils/codegen.py
--rw-r--r--   0        0        0    19677 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/utils/dantic.py
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/utils/import_utils.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/utils/import_utils.pyi
--rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/utils/lazy.py
--rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/utils/peft.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/utils/pkg.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/utils/representation.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/src/openllm_core/utils/serde.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/LICENSE.md
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/pyproject.toml
--rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 openllm_core-0.5.0a1/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/README.md
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/__init__.py
+-rw-r--r--   0        0        0    29829 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/_configuration.py
+-rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/_schemas.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/_typing_compat.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/_version.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/py.typed
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/__init__.py
+-rw-r--r--   0        0        0     8440 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_auto.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_baichuan.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_chatglm.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_dolly_v2.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_falcon.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_flan_t5.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_gemma.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_gpt_neox.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_llama.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_mistral.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_mixtral.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_mpt.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_opt.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_phi.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_qwen.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_stablelm.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_starcoder.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/config/configuration_yi.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/protocol/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/protocol/hf.py
+-rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/protocol/openai.py
+-rw-r--r--   0        0        0    13808 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/utils/__init__.py
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/utils/__init__.pyi
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/utils/_constants.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/utils/analytics.py
+-rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/utils/codegen.py
+-rw-r--r--   0        0        0    19677 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/utils/dantic.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/utils/import_utils.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/utils/import_utils.pyi
+-rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/utils/lazy.py
+-rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/utils/peft.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/utils/pkg.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/utils/representation.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/src/openllm_core/utils/serde.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/LICENSE.md
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/pyproject.toml
+-rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 openllm_core-0.5.0a2/PKG-INFO
```

### Comparing `openllm_core-0.5.0a1/README.md` & `openllm_core-0.5.0a2/README.md`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/__init__.py` & `openllm_core-0.5.0a2/src/openllm_core/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/_configuration.py` & `openllm_core-0.5.0a2/src/openllm_core/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/_schemas.py` & `openllm_core-0.5.0a2/src/openllm_core/_schemas.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/_typing_compat.py` & `openllm_core-0.5.0a2/src/openllm_core/_typing_compat.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/exceptions.py` & `openllm_core-0.5.0a2/src/openllm_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/__init__.py` & `openllm_core-0.5.0a2/src/openllm_core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_auto.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_auto.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_baichuan.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_baichuan.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_chatglm.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_dolly_v2.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_falcon.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_flan_t5.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_gemma.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_gemma.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_gpt_neox.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_llama.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_llama.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_mistral.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_mistral.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_mixtral.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_mixtral.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_mpt.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_mpt.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_opt.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_opt.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_phi.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_phi.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_qwen.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_qwen.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_stablelm.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_starcoder.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/config/configuration_yi.py` & `openllm_core-0.5.0a2/src/openllm_core/config/configuration_yi.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/protocol/openai.py` & `openllm_core-0.5.0a2/src/openllm_core/protocol/openai.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/utils/__init__.py` & `openllm_core-0.5.0a2/src/openllm_core/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,19 +101,19 @@
     raise
 
 
 def io_descriptor(model) -> type[IODescriptor] | None:
   if model is None:
     return model
   try:
-    from _bentoml_sdk.io_models import IOMixin
+    from _bentoml_sdk.io_models import IODescriptor
   except ImportError as err:
     raise RuntimeError('Requires "bentoml>1.2" to use `openllm_core.utils.io_descriptor`') from err
 
-  return pydantic.create_model(f'{model.__class__.__name__}IODescriptor', __base__=(IOMixin, model))
+  return pydantic.create_model(f'{model.__class__.__name__}IODescriptor', __base__=(IODescriptor, model))
 
 
 def api(
   func=None,
   *,
   name=None,
   input=None,
```

### Comparing `openllm_core-0.5.0a1/src/openllm_core/utils/__init__.pyi` & `openllm_core-0.5.0a2/src/openllm_core/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/utils/_constants.py` & `openllm_core-0.5.0a2/src/openllm_core/utils/_constants.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/utils/analytics.py` & `openllm_core-0.5.0a2/src/openllm_core/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/utils/codegen.py` & `openllm_core-0.5.0a2/src/openllm_core/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/utils/dantic.py` & `openllm_core-0.5.0a2/src/openllm_core/utils/dantic.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/utils/import_utils.py` & `openllm_core-0.5.0a2/src/openllm_core/utils/import_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import importlib, importlib.metadata, importlib.util, os, inspect, typing as t
 from .codegen import _make_method
 from ._constants import ENV_VARS_TRUE_VALUES as ENV_VARS_TRUE_VALUES
 
 OPTIONAL_DEPENDENCIES = {'vllm', 'fine-tune', 'ggml', 'agents', 'openai', 'playground', 'gptq', 'grpc', 'awq'}
 ENV_VARS_TRUE_AND_AUTO_VALUES = ENV_VARS_TRUE_VALUES.union({'AUTO'})
 USE_VLLM = os.getenv('USE_VLLM', 'AUTO').upper()
```

### Comparing `openllm_core-0.5.0a1/src/openllm_core/utils/import_utils.pyi` & `openllm_core-0.5.0a2/src/openllm_core/utils/import_utils.pyi`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/utils/lazy.py` & `openllm_core-0.5.0a2/src/openllm_core/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/utils/peft.py` & `openllm_core-0.5.0a2/src/openllm_core/utils/peft.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/utils/pkg.py` & `openllm_core-0.5.0a2/src/openllm_core/utils/pkg.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/utils/representation.py` & `openllm_core-0.5.0a2/src/openllm_core/utils/representation.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/src/openllm_core/utils/serde.py` & `openllm_core-0.5.0a2/src/openllm_core/utils/serde.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/.gitignore` & `openllm_core-0.5.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/LICENSE.md` & `openllm_core-0.5.0a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/pyproject.toml` & `openllm_core-0.5.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a1/PKG-INFO` & `openllm_core-0.5.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm-core
-Version: 0.5.0a1
+Version: 0.5.0a2
 Summary: OpenLLM Core: Core components for OpenLLM.
 Project-URL: Blog, https://modelserving.com
 Project-URL: Chat, https://l.bentoml.com/join-openllm-discord
 Project-URL: Documentation, https://github.com/bentoml/OpenLLM/blob/main/openllm-core/README.md
 Project-URL: GitHub, https://github.com/bentoml/OpenLLM/blob/main/openllm-core
 Project-URL: History, https://github.com/bentoml/OpenLLM/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openllm-core Version: 0.5.0a1 Summary: OpenLLM
+Metadata-Version: 2.1 Name: openllm-core Version: 0.5.0a2 Summary: OpenLLM
 Core: Core components for OpenLLM. Project-URL: Blog, https://modelserving.com
 Project-URL: Chat, https://l.bentoml.com/join-openllm-discord Project-URL:
 Documentation, https://github.com/bentoml/OpenLLM/blob/main/openllm-core/
 README.md Project-URL: GitHub, https://github.com/bentoml/OpenLLM/blob/main/
 openllm-core Project-URL: History, https://github.com/bentoml/OpenLLM/blob/
 main/CHANGELOG.md Project-URL: Homepage, https://bentoml.com Project-URL:
 Tracker, https://github.com/bentoml/OpenLLM/issues Project-URL: Twitter, https:
```

