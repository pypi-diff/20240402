# Comparing `tmp/aibridge_test-0.2.0.tar.gz` & `tmp/aibridge_test-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibridge_test-0.2.0.tar", last modified: Mon Apr  1 04:21:37 2024, max compression
+gzip compressed data, was "aibridge_test-0.2.1.tar", last modified: Tue Apr  2 04:08:26 2024, max compression
```

## Comparing `aibridge_test-0.2.0.tar` & `aibridge_test-0.2.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:37.500572 aibridge_test-0.2.0/
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:37.019935 aibridge_test-0.2.0/AIBridge/
--rw-rw-rw-   0        0        0     1486 2024-03-22 06:03:11.000000 aibridge_test-0.2.0/AIBridge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:37.274565 aibridge_test-0.2.0/AIBridge/ai_services/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/ai_services/__init__.py
--rw-rw-rw-   0        0        0     8119 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/ai_services/ai21labs_text.py
--rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/ai_services/ai_abstraction.py
--rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/ai_services/ai_services_response.py
--rw-rw-rw-   0        0        0     8024 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/ai_services/cohere_llm.py
--rw-rw-rw-   0        0        0    12961 2024-04-01 04:14:15.000000 aibridge_test-0.2.0/AIBridge/ai_services/geminin_services.py
--rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/ai_services/image_optimisaton.py
--rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.2.0/AIBridge/ai_services/openai_images.py
--rw-rw-rw-   0        0        0    10959 2024-01-22 04:47:33.000000 aibridge_test-0.2.0/AIBridge/ai_services/openai_services.py
--rw-rw-rw-   0        0        0     2947 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/ai_services/palm_chat.py
--rw-rw-rw-   0        0        0     8367 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/ai_services/palm_text.py
--rw-rw-rw-   0        0        0     1849 2024-03-22 05:14:23.000000 aibridge_test-0.2.0/AIBridge/ai_services/process_mq.py
--rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/ai_services/stable_diffusion_image.py
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:37.288569 aibridge_test-0.2.0/AIBridge/constant/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/constant/__init__.py
--rw-rw-rw-   0        0        0     3644 2024-03-22 05:49:31.000000 aibridge_test-0.2.0/AIBridge/constant/common.py
--rw-rw-rw-   0        0        0      711 2024-03-22 08:02:44.000000 aibridge_test-0.2.0/AIBridge/constant/constant.py
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:37.321562 aibridge_test-0.2.0/AIBridge/database/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/database/__init__.py
--rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/database/db_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:37.341562 aibridge_test-0.2.0/AIBridge/database/models/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/database/models/__init__.py
--rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/database/models/ai_response.py
--rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/database/models/prompts.py
--rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/database/models/variables.py
--rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/database/no_sql_service.py
--rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/database/session.py
--rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/database/sql_service.py
--rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/database/table_oprations.py
--rw-rw-rw-   0        0        0     1100 2024-03-22 04:53:56.000000 aibridge_test-0.2.0/AIBridge/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:37.361560 aibridge_test-0.2.0/AIBridge/output_validation/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/output_validation/__init__.py
--rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/output_validation/active_validator.py
--rw-rw-rw-   0        0        0     1505 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/output_validation/convertors.py
--rw-rw-rw-   0        0        0     5468 2024-03-22 07:59:34.000000 aibridge_test-0.2.0/AIBridge/output_validation/validations.py
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:37.384625 aibridge_test-0.2.0/AIBridge/prompts/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/prompts/__init__.py
--rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/prompts/prompt_completion.py
--rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/prompts/prompts_save.py
--rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/prompts/prompts_varibales.py
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:37.404562 aibridge_test-0.2.0/AIBridge/queue_integration/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/queue_integration/__init__.py
--rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/queue_integration/assign_queue.py
--rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/queue_integration/message_queue.py
--rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/queue_integration/queue_model.py
--rw-rw-rw-   0        0        0     5964 2024-03-22 05:13:14.000000 aibridge_test-0.2.0/AIBridge/queue_integration/response_class.py
--rw-rw-rw-   0        0        0     2945 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/AIBridge/setconfig.py
--rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/LICENSE
--rw-rw-rw-   0        0        0    21499 2024-04-01 04:21:37.492566 aibridge_test-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:37.486648 aibridge_test-0.2.0/aibridge_test.egg-info/
--rw-rw-rw-   0        0        0    21499 2024-04-01 04:21:36.000000 aibridge_test-0.2.0/aibridge_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1731 2024-04-01 04:21:36.000000 aibridge_test-0.2.0/aibridge_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 04:21:36.000000 aibridge_test-0.2.0/aibridge_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      209 2024-04-01 04:21:36.000000 aibridge_test-0.2.0/aibridge_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-01 04:21:36.000000 aibridge_test-0.2.0/aibridge_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 04:21:37.502563 aibridge_test-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2836 2024-04-01 04:20:59.000000 aibridge_test-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:08:26.344186 aibridge_test-0.2.1/
+drwxrwxrwx   0        0        0        0 2024-04-02 04:08:25.796443 aibridge_test-0.2.1/AIBridge/
+-rw-rw-rw-   0        0        0     1486 2024-03-22 06:03:11.000000 aibridge_test-0.2.1/AIBridge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:08:25.937438 aibridge_test-0.2.1/AIBridge/ai_services/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/ai_services/__init__.py
+-rw-rw-rw-   0        0        0     8946 2024-04-02 04:04:20.000000 aibridge_test-0.2.1/AIBridge/ai_services/ai21labs_text.py
+-rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/ai_services/ai_abstraction.py
+-rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/ai_services/ai_services_response.py
+-rw-rw-rw-   0        0        0     8853 2024-04-02 04:01:40.000000 aibridge_test-0.2.1/AIBridge/ai_services/cohere_llm.py
+-rw-rw-rw-   0        0        0    13559 2024-04-02 04:03:13.000000 aibridge_test-0.2.1/AIBridge/ai_services/geminin_services.py
+-rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/ai_services/image_optimisaton.py
+-rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.2.1/AIBridge/ai_services/openai_images.py
+-rw-rw-rw-   0        0        0    11426 2024-04-02 04:03:13.000000 aibridge_test-0.2.1/AIBridge/ai_services/openai_services.py
+-rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.2.1/AIBridge/ai_services/palm_chat.py
+-rw-rw-rw-   0        0        0     9198 2024-04-02 03:59:08.000000 aibridge_test-0.2.1/AIBridge/ai_services/palm_text.py
+-rw-rw-rw-   0        0        0     1849 2024-03-22 05:14:23.000000 aibridge_test-0.2.1/AIBridge/ai_services/process_mq.py
+-rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/ai_services/stable_diffusion_image.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:08:25.970443 aibridge_test-0.2.1/AIBridge/constant/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/constant/__init__.py
+-rw-rw-rw-   0        0        0     3644 2024-03-22 05:49:31.000000 aibridge_test-0.2.1/AIBridge/constant/common.py
+-rw-rw-rw-   0        0        0      711 2024-03-22 08:02:44.000000 aibridge_test-0.2.1/AIBridge/constant/constant.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:08:26.058442 aibridge_test-0.2.1/AIBridge/database/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/database/__init__.py
+-rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/database/db_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:08:26.094445 aibridge_test-0.2.1/AIBridge/database/models/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/database/models/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/database/models/ai_response.py
+-rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/database/models/prompts.py
+-rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/database/models/variables.py
+-rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/database/no_sql_service.py
+-rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/database/session.py
+-rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/database/sql_service.py
+-rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/database/table_oprations.py
+-rw-rw-rw-   0        0        0     1100 2024-03-22 04:53:56.000000 aibridge_test-0.2.1/AIBridge/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:08:26.123439 aibridge_test-0.2.1/AIBridge/output_validation/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/output_validation/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/output_validation/active_validator.py
+-rw-rw-rw-   0        0        0     1505 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/output_validation/convertors.py
+-rw-rw-rw-   0        0        0     5468 2024-03-22 07:59:34.000000 aibridge_test-0.2.1/AIBridge/output_validation/validations.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:08:26.141437 aibridge_test-0.2.1/AIBridge/prompts/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/prompts/__init__.py
+-rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/prompts/prompt_completion.py
+-rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/prompts/prompts_save.py
+-rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/prompts/prompts_varibales.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:08:26.189185 aibridge_test-0.2.1/AIBridge/queue_integration/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/queue_integration/__init__.py
+-rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/queue_integration/assign_queue.py
+-rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/queue_integration/message_queue.py
+-rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/queue_integration/queue_model.py
+-rw-rw-rw-   0        0        0     6194 2024-04-01 09:25:14.000000 aibridge_test-0.2.1/AIBridge/queue_integration/response_class.py
+-rw-rw-rw-   0        0        0     2945 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/AIBridge/setconfig.py
+-rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0    21499 2024-04-02 04:08:26.339185 aibridge_test-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 04:08:26.311186 aibridge_test-0.2.1/aibridge_test.egg-info/
+-rw-rw-rw-   0        0        0    21499 2024-04-02 04:08:25.000000 aibridge_test-0.2.1/aibridge_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1731 2024-04-02 04:08:25.000000 aibridge_test-0.2.1/aibridge_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 04:08:25.000000 aibridge_test-0.2.1/aibridge_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      209 2024-04-02 04:08:25.000000 aibridge_test-0.2.1/aibridge_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 04:08:25.000000 aibridge_test-0.2.1/aibridge_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 04:08:26.345192 aibridge_test-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2836 2024-04-02 04:07:51.000000 aibridge_test-0.2.1/setup.py
```

### Comparing `aibridge_test-0.2.0/AIBridge/__init__.py` & `aibridge_test-0.2.1/AIBridge/__init__.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/ai_services/ai21labs_text.py` & `aibridge_test-0.2.1/AIBridge/ai_services/cohere_llm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,50 @@
+import cohere
 import time
 import uuid
-from AIBridge.exceptions import Ai21Exception, AIBridgeException
+from AIBridge.exceptions import CohereException, AIBridgeException
 from AIBridge.prompts.prompt_completion import Completion
 from AIBridge.ai_services.ai_abstraction import AIInterface
 from AIBridge.output_validation.active_validator import ActiveValidator
 import json
 from AIBridge.constant.common import parse_fromat, parse_api_key
-import ai21
 from AIBridge.output_validation.convertors import FromJson, IntoJson
 
 
-class JurasicText(AIInterface):
+class CohereApi(AIInterface):
     """
-    Base class for PalmText's Services
+    Base class for OpenAI Services
     """
 
     @classmethod
     def generate(
         self,
         prompts: list[str] = [],
         prompt_ids: list[str] = [],
         prompt_data: list[dict] = [],
         variables: list[dict] = [],
         output_format: list[str] = [],
         format_strcture: list[str] = [],
-        model="j2-ultra",
+        model="command-nightly",
         variation_count: int = 1,
-        max_tokens: int = 8000,
+        max_tokens: int = 3500,  # max 4096
         temperature: float = 0.5,
         message_queue=False,
         api_key=None,
         output_format_parse=True,
+        context=[],
     ):
         try:
             if prompts and prompt_ids:
-                raise Ai21Exception(
-                    "please provide either prompts or prompts ids at a time"
+                raise CohereException(
+                    "please provide either prompts or prompts ids at time"
                 )
             if not prompts and not prompt_ids:
-                raise Ai21Exception(
-                    "Either provide prompts or prompts ids to generate the data"
+                raise CohereException(
+                    "Either provide prompts or prompts ids to genrate the data"
                 )
             if prompt_ids:
                 prompts_list = Completion.create_prompt_from_id(
                     prompt_ids=prompt_ids,
                     prompt_data_list=prompt_data,
                     variables_list=variables,
                 )
@@ -86,18 +87,19 @@
                 message_data = {
                     "id": str(id),
                     "prompts": json.dumps(updated_prompts),
                     "model": model,
                     "variation_count": variation_count,
                     "max_tokens": max_tokens,
                     "temperature": temperature,
-                    "ai_service": "ai21_api",
+                    "ai_service": "cohere_api",
                     "output_format": json.dumps(output_format),
                     "format_structure": json.dumps(format_strcture),
                     "api_key": api_key,
+                    "context": context,
                 }
                 message = {"data": json.dumps(message_data)}
                 from AIBridge.queue_integration.message_queue import MessageQ
 
                 MessageQ.mq_enque(message=message)
                 return {"response_id": str(id)}
             return self.get_response(
@@ -105,76 +107,93 @@
                 model,
                 variation_count,
                 max_tokens,
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
+                context=context,
             )
         except AIBridgeException as e:
-            raise Ai21Exception(f"Error in generating AI data {e}")
+            raise CohereException(f"Error in generating AI data {e}")
+
+    @classmethod
+    def get_prompt_context(self, context):
+        context_string = ""
+        for _context in context:
+            if _context["role"] not in ["user", "system", "assistance"]:
+                raise CohereException(
+                    "Invalid role provided. Please provide either user or system, assistance"
+                )
+            context_string = (
+                context_string + f"{_context['role']}:{_context['context']}" + "\n"
+            )
+        return context_string
 
     @classmethod
     def get_response(
         self,
         prompts,
-        model="j2-ultra",
+        model="command-nightly",
         variation_count=1,
-        max_tokens=8000,
+        max_tokens=3500,  # max 4096
         temperature=0.5,
         output_format=[],
         format_structure=[],
         api_key=None,
+        context=[],
     ):
         try:
             if output_format:
                 if isinstance(output_format, str):
                     output_format = json.loads(output_format)
             if format_structure:
                 if isinstance(format_structure, str):
                     format_structure = json.loads(format_structure)
             if not prompts:
-                raise Ai21Exception("No prompts provided")
-            api_key = api_key if api_key else parse_api_key("ai21_api")
-            ai21.api_key = api_key
+                raise CohereException("No prompts provided")
+            API_KEY = api_key if api_key else parse_api_key("cohere_api")
+            co = cohere.Client(API_KEY)
             model_output = []
-            token_used = 0
-            for index, prompt in enumerate(prompts):
-                response = ai21.Completion.execute(
+            context_string = self.get_prompt_context(context)
+            token_used = max_tokens
+            for ind, prompt in enumerate(prompts):
+                prompt = context_string + "\n" + prompt
+                response = co.generate(
                     model=model,
                     prompt=prompt,
-                    numResults=variation_count,
-                    maxTokens=max_tokens,
+                    max_tokens=max_tokens,
                     temperature=temperature,
+                    num_generations=variation_count,
                 )
-                token_used = token_used + len(response["prompt"]["tokens"])
-                for res in response["completions"]:
-                    content = res["data"]["text"]
-                    token_used = token_used + len(res["data"]["tokens"])
+                for index, res in enumerate(response.generations):
+                    content = res.text
                     if output_format:
-                        _formatter = output_format[index]
+                        _formatter = output_format[ind]
                         try:
                             if _formatter == "csv":
                                 content = FromJson.json_to_csv(json.loads(content))
                             elif _formatter == "xml":
                                 content = FromJson.json_to_xml(json.loads(content))
                         except AIBridgeException as e:
-                            raise Ai21Exception(
+                            raise CohereException(
                                 f"Ai response is not in valid {_formatter}"
                             )
                         if _formatter == "json":
                             _validate_obj = ActiveValidator.get_active_validator(
                                 _formatter
                             )
                             try:
                                 content = _validate_obj.validate(
                                     content,
-                                    schema=format_structure[prompts.index(prompt)]
-                                    if format_structure
-                                    else None,
+                                    schema=(
+                                        format_structure[index]
+                                        if format_structure
+                                        else None
+                                    ),
                                 )
                             except AIBridgeException as e:
                                 content_error = {
                                     "error": f"{e}",
                                     "ai_response": content,
                                 }
                                 content = json.dumps(content_error)
@@ -183,13 +202,13 @@
                     else:
                         model_output[index]["data"].append(content)
             message_value = {
                 "items": {
                     "response": model_output,
                     "token_used": token_used,
                     "created_at": time.time(),
-                    "ai_service": "ai21_api",
+                    "ai_service": "open_ai",
                 }
             }
             return message_value
         except AIBridgeException as e:
-            raise Ai21Exception(f"{e}")
+            raise CohereException(f"{e}")
```

### Comparing `aibridge_test-0.2.0/AIBridge/ai_services/ai_services_response.py` & `aibridge_test-0.2.1/AIBridge/ai_services/ai_services_response.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/ai_services/cohere_llm.py` & `aibridge_test-0.2.1/AIBridge/ai_services/ai21labs_text.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-import cohere
 import time
 import uuid
-from AIBridge.exceptions import CohereException, AIBridgeException
+from AIBridge.exceptions import Ai21Exception, AIBridgeException
 from AIBridge.prompts.prompt_completion import Completion
 from AIBridge.ai_services.ai_abstraction import AIInterface
 from AIBridge.output_validation.active_validator import ActiveValidator
 import json
 from AIBridge.constant.common import parse_fromat, parse_api_key
+import ai21
 from AIBridge.output_validation.convertors import FromJson, IntoJson
 
 
-class CohereApi(AIInterface):
+class JurasicText(AIInterface):
     """
-    Base class for OpenAI Services
+    Base class for PalmText's Services
     """
 
     @classmethod
     def generate(
         self,
         prompts: list[str] = [],
         prompt_ids: list[str] = [],
         prompt_data: list[dict] = [],
         variables: list[dict] = [],
         output_format: list[str] = [],
         format_strcture: list[str] = [],
-        model="command-nightly",
+        model="j2-ultra",
         variation_count: int = 1,
-        max_tokens: int = 3500,  # max 4096
+        max_tokens: int = 8000,
         temperature: float = 0.5,
         message_queue=False,
         api_key=None,
         output_format_parse=True,
+        context=[],
     ):
         try:
             if prompts and prompt_ids:
-                raise CohereException(
-                    "please provide either prompts or prompts ids at time"
+                raise Ai21Exception(
+                    "please provide either prompts or prompts ids at a time"
                 )
             if not prompts and not prompt_ids:
-                raise CohereException(
-                    "Either provide prompts or prompts ids to genrate the data"
+                raise Ai21Exception(
+                    "Either provide prompts or prompts ids to generate the data"
                 )
             if prompt_ids:
                 prompts_list = Completion.create_prompt_from_id(
                     prompt_ids=prompt_ids,
                     prompt_data_list=prompt_data,
                     variables_list=variables,
                 )
@@ -86,18 +87,19 @@
                 message_data = {
                     "id": str(id),
                     "prompts": json.dumps(updated_prompts),
                     "model": model,
                     "variation_count": variation_count,
                     "max_tokens": max_tokens,
                     "temperature": temperature,
-                    "ai_service": "cohere_api",
+                    "ai_service": "ai21_api",
                     "output_format": json.dumps(output_format),
                     "format_structure": json.dumps(format_strcture),
                     "api_key": api_key,
+                    "context": context,
                 }
                 message = {"data": json.dumps(message_data)}
                 from AIBridge.queue_integration.message_queue import MessageQ
 
                 MessageQ.mq_enque(message=message)
                 return {"response_id": str(id)}
             return self.get_response(
@@ -105,74 +107,95 @@
                 model,
                 variation_count,
                 max_tokens,
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
+                context=context,
             )
         except AIBridgeException as e:
-            raise CohereException(f"Error in generating AI data {e}")
+            raise Ai21Exception(f"Error in generating AI data {e}")
+
+    @classmethod
+    def get_prompt_context(self, context):
+        context_string = ""
+        for _context in context:
+            if _context["role"] not in ["user", "system", "assistance"]:
+                raise Ai21Exception(
+                    "Invalid role provided. Please provide either user or system, assistance"
+                )
+            context_string = (
+                context_string + f"{_context['role']}:{_context['context']}" + "\n"
+            )
+        return context_string
 
     @classmethod
     def get_response(
         self,
         prompts,
-        model="command-nightly",
+        model="j2-ultra",
         variation_count=1,
-        max_tokens=3500,  # max 4096
+        max_tokens=8000,
         temperature=0.5,
         output_format=[],
         format_structure=[],
         api_key=None,
+        context=[],
     ):
         try:
             if output_format:
                 if isinstance(output_format, str):
                     output_format = json.loads(output_format)
             if format_structure:
                 if isinstance(format_structure, str):
                     format_structure = json.loads(format_structure)
             if not prompts:
-                raise CohereException("No prompts provided")
-            API_KEY = api_key if api_key else parse_api_key("cohere_api")
-            co = cohere.Client(API_KEY)
+                raise Ai21Exception("No prompts provided")
+            api_key = api_key if api_key else parse_api_key("ai21_api")
+            ai21.api_key = api_key
             model_output = []
-            token_used = max_tokens
-            for ind, prompt in enumerate(prompts):
-                response = co.generate(
+            token_used = 0
+            context_string = self.get_prompt_context(context)
+            for index, prompt in enumerate(prompts):
+                prompt = context_string + "\n" + prompt
+                response = ai21.Completion.execute(
                     model=model,
                     prompt=prompt,
-                    max_tokens=max_tokens,
+                    numResults=variation_count,
+                    maxTokens=max_tokens,
                     temperature=temperature,
-                    num_generations=variation_count,
                 )
-                for index, res in enumerate(response.generations):
-                    content = res.text
+                token_used = token_used + len(response["prompt"]["tokens"])
+                for res in response["completions"]:
+                    content = res["data"]["text"]
+                    token_used = token_used + len(res["data"]["tokens"])
                     if output_format:
-                        _formatter = output_format[ind]
+                        _formatter = output_format[index]
                         try:
                             if _formatter == "csv":
                                 content = FromJson.json_to_csv(json.loads(content))
                             elif _formatter == "xml":
                                 content = FromJson.json_to_xml(json.loads(content))
                         except AIBridgeException as e:
-                            raise CohereException(
+                            raise Ai21Exception(
                                 f"Ai response is not in valid {_formatter}"
                             )
                         if _formatter == "json":
                             _validate_obj = ActiveValidator.get_active_validator(
                                 _formatter
                             )
                             try:
                                 content = _validate_obj.validate(
                                     content,
-                                    schema=format_structure[prompts.index(prompt)]
-                                    if format_structure
-                                    else None,
+                                    schema=(
+                                        format_structure[index]
+                                        if format_structure
+                                        else None
+                                    ),
                                 )
                             except AIBridgeException as e:
                                 content_error = {
                                     "error": f"{e}",
                                     "ai_response": content,
                                 }
                                 content = json.dumps(content_error)
@@ -181,13 +204,13 @@
                     else:
                         model_output[index]["data"].append(content)
             message_value = {
                 "items": {
                     "response": model_output,
                     "token_used": token_used,
                     "created_at": time.time(),
-                    "ai_service": "open_ai",
+                    "ai_service": "ai21_api",
                 }
             }
             return message_value
         except AIBridgeException as e:
-            raise CohereException(f"{e}")
+            raise Ai21Exception(f"{e}")
```

### Comparing `aibridge_test-0.2.0/AIBridge/ai_services/geminin_services.py` & `aibridge_test-0.2.1/AIBridge/ai_services/geminin_services.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         max_tokens: int = 10000,
         temperature: float = 0.5,
         message_queue=False,
         api_key=None,
         output_format_parse=True,
         stop_subsequence: list[str] = None,
         stream=False,
+        context=[],
     ):
         try:
             if prompts and prompt_ids:
                 raise GeminiException(
                     "please provide either prompts or prompts ids at atime"
                 )
             if not prompts and not prompt_ids:
@@ -99,14 +100,15 @@
                     "temperature": temperature,
                     "ai_service": "gemini_ai",
                     "output_format": json.dumps(output_format),
                     "format_structure": json.dumps(format_strcture),
                     "api_key": api_key,
                     "stop_subsequence": stop_subsequence,
                     "stream": stream,
+                    "context": context,
                 }
                 message = {"data": json.dumps(message_data)}
                 from AIBridge.queue_integration.message_queue import MessageQ
 
                 MessageQ.mq_enque(message=message)
                 return {"response_id": str(id)}
             return self.get_response(
@@ -116,14 +118,15 @@
                 max_tokens,
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
                 stop_subsequence=stop_subsequence,
                 stream=stream,
+                context=context,
             )
         except AIBridgeException as e:
             raise GeminiException(f"Error in generating AI data {e}")
 
     @classmethod
     def execute_text_prompt(
         self,
@@ -179,68 +182,80 @@
                 stream=stream,
                 tools=functions_call,
             ),
             model,
         )
 
     @classmethod
+    def get_prompt_context(self, context):
+        context_list = []
+        for _context in context:
+            if _context["role"] not in ["user", "system", "assistance"]:
+                raise GeminiException(
+                    "Invalid role provided. Please provide either user or system, assistance"
+                )
+            key = "user"
+            if _context["role"] == "assistance":
+                key = "model"
+            context_list.append({"role": key, "parts": [_context["context"]]})
+        return context_list
+
+    @classmethod
     def get_response(
         self,
         prompts,
         model="gemini-pro",
         variation_count=1,
         max_tokens=10000,
         temperature=0.5,
         output_format=[],
         format_structure=[],
         api_key=None,
         stop_subsequence=None,
         stream=False,
+        context=[],
     ):
         try:
             if output_format:
                 if isinstance(output_format, str):
                     output_format = json.loads(output_format)
             if format_structure:
                 if isinstance(format_structure, str):
                     format_structure = json.loads(format_structure)
             if not prompts:
                 raise GeminiException("No prompts provided")
             api_key = api_key if api_key else parse_api_key("gemini_ai")
-            message_data = []
+            message_data = self.get_prompt_context(context) if context else []
             model_output = []
             token_used = 0
             _formatter = "string"
-            for prompt in prompts:
+            for index, prompt in enumerate(prompts):
                 if output_format:
-                    _formatter = output_format[prompts.index(prompt)]
-                # message_data.append({"role": "user", "parts": [prompt]})
-                message_data.append(prompt)
+                    _formatter = output_format[index]
+                message_data.append({"role": "user", "parts": [prompt]})
+                print(message_data)
+                # message_data.append(prompt)
                 if _formatter not in ["json", "csv", "xml"]:
                     response, exe_model = self.execute_text_prompt(
                         api_key,
                         model=model,
                         messages=message_data,
                         n=variation_count,
                         max_tokens=max_tokens,
                         temperature=temperature,
                         stop_subsequence=stop_subsequence,
                         stream=stream,
                     )
                 else:
                     if _formatter == "csv":
-                        schema = IntoJson.csv_to_json(
-                            format_structure[prompts.index(prompt)]
-                        )
+                        schema = IntoJson.csv_to_json(format_structure[index])
                     elif _formatter == "xml":
-                        schema = IntoJson.xml_to_json(
-                            format_structure[prompts.index(prompt)]
-                        )
+                        schema = IntoJson.xml_to_json(format_structure[index])
                     elif _formatter == "json":
-                        schema = json.loads(format_structure[prompts.index(prompt)])
+                        schema = json.loads(format_structure[index])
                     functions = [get_function_from_json(schema, call_from="gemini_ai")]
                     functions = {"function_declarations": functions}
                     print(functions)
                     response, exe_model = self.execute_prompt_function_calling(
                         api_key=api_key,
                         model=model,
                         messages=message_data,
@@ -289,15 +304,15 @@
                             _validate_obj = ActiveValidator.get_active_validator(
                                 _formatter
                             )
                             try:
                                 content = _validate_obj.validate(
                                     content,
                                     schema=(
-                                        format_structure[prompts.index(prompt)]
+                                        format_structure[index]
                                         if format_structure
                                         else None
                                     ),
                                 )
                             except AIBridgeException as e:
                                 content_error = {
                                     "error": f"{e}",
```

### Comparing `aibridge_test-0.2.0/AIBridge/ai_services/image_optimisaton.py` & `aibridge_test-0.2.1/AIBridge/ai_services/image_optimisaton.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/ai_services/openai_images.py` & `aibridge_test-0.2.1/AIBridge/ai_services/openai_images.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/ai_services/openai_services.py` & `aibridge_test-0.2.1/AIBridge/ai_services/openai_services.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         model="gpt-3.5-turbo",
         variation_count: int = 1,
         max_tokens: int = 3500,
         temperature: float = 0.5,
         message_queue=False,
         api_key=None,
         output_format_parse=True,
+        context=[],
     ):
         try:
             if prompts and prompt_ids:
                 raise OpenAIException(
                     "please provide either prompts or prompts ids at atime"
                 )
             if not prompts and not prompt_ids:
@@ -90,14 +91,15 @@
                     "variation_count": variation_count,
                     "max_tokens": max_tokens,
                     "temperature": temperature,
                     "ai_service": "open_ai",
                     "output_format": json.dumps(output_format),
                     "format_structure": json.dumps(format_strcture),
                     "api_key": api_key,
+                    "context": context,
                 }
                 message = {"data": json.dumps(message_data)}
                 from AIBridge.queue_integration.message_queue import MessageQ
 
                 MessageQ.mq_enque(message=message)
                 return {"response_id": str(id)}
             return self.get_response(
@@ -105,14 +107,15 @@
                 model,
                 variation_count,
                 max_tokens,
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
+                context=context,
             )
         except AIBridgeException as e:
             raise OpenAIException(f"Error in generating AI data {e}")
 
     @classmethod
     def execute_text_prompt(
         self, api_key, model, messages, n, max_tokens=3500, temperature=0.5
@@ -145,79 +148,87 @@
             functions=functions_call,
             function_call="auto",
             max_tokens=max_tokens,
             temperature=temperature,
         )
 
     @classmethod
+    def get_prompt_context(context):
+        for _context in context:
+            if _context["role"] not in ["user", "system", "assistance"]:
+                raise OpenAIException(
+                    "Invalid role provided. Please provide either user or system, assistance"
+                )
+        return context
+
+    @classmethod
     def get_response(
         self,
         prompts,
         model="gpt-3.5-turbo",
         variation_count=1,
         max_tokens=3500,
         temperature=0.5,
         output_format=[],
         format_structure=[],
         api_key=None,
+        context=[],
     ):
         try:
             if output_format:
                 if isinstance(output_format, str):
                     output_format = json.loads(output_format)
             if format_structure:
                 if isinstance(format_structure, str):
                     format_structure = json.loads(format_structure)
             if not prompts:
                 raise OpenAIException("No prompts provided")
             api_key = api_key if api_key else parse_api_key("open_ai")
-            message_data = []
+            message_data = context if context else []
             model_output = []
             token_used = 0
             _formatter = "string"
-            for prompt in prompts:
+            for index, prompt in enumerate(prompts):
                 if output_format:
-                    _formatter = output_format[prompts.index(prompt)]
+                    _formatter = output_format[index]
                 message_data.append({"role": "user", "content": prompt})
                 if _formatter not in ["json", "csv", "xml"]:
                     response = self.execute_text_prompt(
                         api_key,
                         model=model,
                         messages=message_data,
                         n=variation_count,
                         max_tokens=max_tokens,
                         temperature=temperature,
                     )
                 else:
                     if _formatter == "csv":
-                        schema = IntoJson.csv_to_json(
-                            format_structure[prompts.index(prompt)]
-                        )
+                        schema = IntoJson.csv_to_json(format_structure[index])
                     elif _formatter == "xml":
-                        schema = IntoJson.xml_to_json(
-                            format_structure[prompts.index(prompt)]
-                        )
+                        schema = IntoJson.xml_to_json(format_structure[index])
                     elif _formatter == "json":
-                        schema = json.loads(format_structure[prompts.index(prompt)])
+                        schema = json.loads(format_structure[index])
                     functions = [get_function_from_json(schema)]
                     response = self.execute_prompt_function_calling(
                         api_key=api_key,
                         model=model,
                         messages=message_data,
                         n=variation_count,
                         functions_call=functions,
                         max_tokens=max_tokens,
                         temperature=temperature,
                     )
                 message_data.append(
                     {
                         "role": response.choices[0].message.role,
-                        "content": response.choices[0].message.content
-                        if response.choices[0].message.content
-                        else response.choices[0].message.function_call.arguments,
+                        "content": (
+                            response.choices[0].message.content
+                            if response.choices[0].message.content
+                            else response.choices[0].message.function_call.arguments
+                        ),
                     }
                 )
                 tokens = response.usage.total_tokens
                 token_used = token_used + tokens
                 for res in response.choices:
                     index = response.choices.index(res)
                     content = (
@@ -238,17 +249,19 @@
                         if _formatter == "json":
                             _validate_obj = ActiveValidator.get_active_validator(
                                 _formatter
                             )
                             try:
                                 content = _validate_obj.validate(
                                     content,
-                                    schema=format_structure[prompts.index(prompt)]
-                                    if format_structure
-                                    else None,
+                                    schema=(
+                                        format_structure[index]
+                                        if format_structure
+                                        else None
+                                    ),
                                 )
                             except AIBridgeException as e:
                                 content_error = {
                                     "error": f"{e}",
                                     "ai_response": content,
                                 }
                                 content = json.dumps(content_error)
```

### Comparing `aibridge_test-0.2.0/AIBridge/ai_services/palm_chat.py` & `aibridge_test-0.2.1/AIBridge/ai_services/palm_chat.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/ai_services/palm_text.py` & `aibridge_test-0.2.1/AIBridge/ai_services/palm_text.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         model="models/text-bison-001",
         variation_count: int = 1,
         max_tokens: int = 10000,
         temperature: float = 0.5,
         message_queue=False,
         api_key=None,
         output_format_parse=True,
+        context=[],
     ):
         try:
             if prompts and prompt_ids:
                 raise PalmTextException(
                     "please provide either prompts or prompts ids at atime"
                 )
             if not prompts and not prompt_ids:
@@ -90,14 +91,15 @@
                     "variation_count": variation_count,
                     "max_tokens": max_tokens,
                     "temperature": temperature,
                     "ai_service": "palm_api",
                     "output_format": json.dumps(output_format),
                     "format_structure": json.dumps(format_strcture),
                     "api_key": api_key,
+                    "context": context,
                 }
                 message = {"data": json.dumps(message_data)}
                 from AIBridge.queue_integration.message_queue import MessageQ
 
                 MessageQ.mq_enque(message=message)
                 return {"response_id": str(id)}
             return self.get_response(
@@ -105,49 +107,66 @@
                 model,
                 variation_count,
                 max_tokens,
                 temperature,
                 output_format,
                 format_strcture,
                 api_key=api_key,
+                context=context,
             )
         except AIBridgeException as e:
             raise PalmTextException(f"Error in generating AI data {e}")
 
     @classmethod
     def get_tokens(Self, model, text):
         tokens = palm.count_text_tokens(model=model, prompt=text)
         return tokens["token_count"]
 
     @classmethod
+    def get_prompt_context(self, context):
+        context_string = ""
+        for _context in context:
+            if _context["role"] not in ["user", "system", "assistance"]:
+                raise PalmTextException(
+                    "Invalid role provided. Please provide either user or system, assistance"
+                )
+            context_string = (
+                context_string + f"{_context['role']}:{_context['context']}" + "\n"
+            )
+        return context_string
+
+    @classmethod
     def get_response(
         self,
         prompts,
         model="models/text-bison-001",
         variation_count=1,
         max_tokens=10000,
         temperature=0.5,
         output_format=[],
         format_structure=[],
         api_key=None,
+        context=[],
     ):
         try:
             if output_format:
                 if isinstance(output_format, str):
                     output_format = json.loads(output_format)
             if format_structure:
                 if isinstance(format_structure, str):
                     format_structure = json.loads(format_structure)
             if not prompts:
                 raise PalmTextException("No prompts provided")
             api_key = api_key if api_key else parse_api_key("palm_api")
             palm.configure(api_key=api_key)
             model_output = []
             token_used = 0
+            context_string = self.get_prompt_context(context)
             for index, prompt in enumerate(prompts):
+                prompt = context_string + "\n" + prompt
                 response = palm.generate_text(
                     model=model,
                     prompt=prompt,
                     temperature=temperature,
                     max_output_tokens=max_tokens,
                     candidate_count=variation_count,
                 )
@@ -169,17 +188,19 @@
                         if _formatter == "json":
                             _validate_obj = ActiveValidator.get_active_validator(
                                 _formatter
                             )
                             try:
                                 content = _validate_obj.validate(
                                     content,
-                                    schema=format_structure[prompts.index(prompt)]
-                                    if format_structure
-                                    else None,
+                                    schema=(
+                                        format_structure[index]
+                                        if format_structure
+                                        else None
+                                    ),
                                 )
                             except AIBridgeException as e:
                                 content_error = {
                                     "error": f"{e}",
                                     "ai_response": content,
                                 }
                                 content = json.dumps(content_error)
```

### Comparing `aibridge_test-0.2.0/AIBridge/ai_services/process_mq.py` & `aibridge_test-0.2.1/AIBridge/ai_services/process_mq.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/ai_services/stable_diffusion_image.py` & `aibridge_test-0.2.1/AIBridge/ai_services/stable_diffusion_image.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/constant/common.py` & `aibridge_test-0.2.1/AIBridge/constant/common.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/constant/constant.py` & `aibridge_test-0.2.1/AIBridge/constant/constant.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/database/db_layer.py` & `aibridge_test-0.2.1/AIBridge/database/db_layer.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/database/no_sql_service.py` & `aibridge_test-0.2.1/AIBridge/database/no_sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/database/session.py` & `aibridge_test-0.2.1/AIBridge/database/session.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/database/sql_service.py` & `aibridge_test-0.2.1/AIBridge/database/sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/exceptions.py` & `aibridge_test-0.2.1/AIBridge/exceptions.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/output_validation/convertors.py` & `aibridge_test-0.2.1/AIBridge/output_validation/convertors.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/output_validation/validations.py` & `aibridge_test-0.2.1/AIBridge/output_validation/validations.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/prompts/prompt_completion.py` & `aibridge_test-0.2.1/AIBridge/prompts/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/prompts/prompts_save.py` & `aibridge_test-0.2.1/AIBridge/prompts/prompts_save.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/prompts/prompts_varibales.py` & `aibridge_test-0.2.1/AIBridge/prompts/prompts_varibales.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/queue_integration/message_queue.py` & `aibridge_test-0.2.1/AIBridge/queue_integration/message_queue.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/queue_integration/queue_model.py` & `aibridge_test-0.2.1/AIBridge/queue_integration/queue_model.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/AIBridge/queue_integration/response_class.py` & `aibridge_test-0.2.1/AIBridge/queue_integration/response_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
             model=message_data["model"],
             variation_count=message_data["variation_count"],
             max_tokens=message_data["max_tokens"],
             temperature=message_data["temperature"],
             output_format=message_data["output_format"],
             format_structure=message_data["format_structure"],
             api_key=message_data["api_key"],
+            context=message_data["context"],
         )
         return data
 
 
 class GeminiAiRes(Caller):
     @classmethod
     def get_response(self, service_obj, message_data):
@@ -34,14 +35,15 @@
             max_tokens=message_data["max_tokens"],
             temperature=message_data["temperature"],
             output_format=message_data["output_format"],
             format_structure=message_data["format_structure"],
             api_key=message_data["api_key"],
             stop_subsequence=message_data["stop_subsequence"],
             stream=message_data["stream"],
+            context=message_data["context"],
         )
         return data
 
 
 class OpenAiImageRes(Caller):
     @classmethod
     def get_response(self, service_obj, message_data):
@@ -67,14 +69,15 @@
             model=message_data["model"],
             variation_count=message_data["variation_count"],
             max_tokens=message_data["max_tokens"],
             temperature=message_data["temperature"],
             output_format=message_data["output_format"],
             format_structure=message_data["format_structure"],
             api_key=message_data["api_key"],
+            context=message_data["context"],
         )
         return data
 
 
 class PalmChatRes(Caller):
     @classmethod
     def get_response(self, service_obj, message_data):
@@ -129,14 +132,15 @@
             model=message_data["model"],
             variation_count=message_data["variation_count"],
             max_tokens=message_data["max_tokens"],
             temperature=message_data["temperature"],
             output_format=message_data["output_format"],
             format_structure=message_data["format_structure"],
             api_key=message_data["api_key"],
+            context=message_data["context"],
         )
         return data
 
 
 class JarasicTextRes(Caller):
     @classmethod
     def get_response(self, service_obj, message_data):
@@ -145,9 +149,10 @@
             model=message_data["model"],
             variation_count=message_data["variation_count"],
             max_tokens=message_data["max_tokens"],
             temperature=message_data["temperature"],
             output_format=message_data["output_format"],
             format_structure=message_data["format_structure"],
             api_key=message_data["api_key"],
+            context=message_data["context"],
         )
         return data
```

### Comparing `aibridge_test-0.2.0/AIBridge/setconfig.py` & `aibridge_test-0.2.1/AIBridge/setconfig.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/LICENSE` & `aibridge_test-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/PKG-INFO` & `aibridge_test-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.2.0
+Version: 0.2.1
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.2.0/README.md` & `aibridge_test-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/aibridge_test.egg-info/PKG-INFO` & `aibridge_test-0.2.1/aibridge_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.2.0
+Version: 0.2.1
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.2.0/aibridge_test.egg-info/SOURCES.txt` & `aibridge_test-0.2.1/aibridge_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.0/setup.py` & `aibridge_test-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = "aibridge_test"
 DESCRIPTION = 'Bridge for LLM"s'
 URL = "https://github.com/me/myproject"
 EMAIL = "ashish.tilekar@opsfuse.com"
 AUTHOR = "Ashish Tilekar"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "0.2.0"
+VERSION = "0.2.1"
 REQUIRED = [
     "openai<=1.7.1",
     "SQLAlchemy>=2.0.19",
     "redis>=4.6.0",
     "PyYAML>=6.0.1",
     "Jinja2>=3.1.2",
     "pymongo>=4.4.1",
```

