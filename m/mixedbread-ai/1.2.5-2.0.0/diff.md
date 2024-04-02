# Comparing `tmp/mixedbread_ai-1.2.5.tar.gz` & `tmp/mixedbread_ai-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixedbread_ai-1.2.5.tar", max compression
+gzip compressed data, was "mixedbread_ai-2.0.0.tar", max compression
```

## Comparing `mixedbread_ai-1.2.5.tar` & `mixedbread_ai-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,51 @@
--rw-r--r--   0        0        0    11348 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/LICENSE.md
--rw-r--r--   0        0        0     1602 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/README.md
--rw-r--r--   0        0        0      155 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/__init__.py
--rw-r--r--   0        0        0     6558 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/client.py
--rw-r--r--   0        0        0      157 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/__init__.py
--rw-r--r--   0        0        0       47 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/api/mixedbread_ai/__init__.py
--rw-r--r--   0        0        0     5920 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/api/mixedbread_ai/embeddings.py
--rw-r--r--   0        0        0    12131 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/client.py
--rw-r--r--   0        0        0      470 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/errors.py
--rw-r--r--   0        0        0      548 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/models/__init__.py
--rw-r--r--   0        0        0     2291 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/models/embedding.py
--rw-r--r--   0        0        0     3096 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/models/embeddings_request.py
--rw-r--r--   0        0        0     3031 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/models/embeddings_response.py
--rw-r--r--   0        0        0     1978 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/models/error_response.py
--rw-r--r--   0        0        0     1243 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/models/error_response_data.py
--rw-r--r--   0        0        0     1824 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/models/model_base_response.py
--rw-r--r--   0        0        0     2238 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/models/model_usage.py
--rw-r--r--   0        0        0       25 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/py.typed
--rw-r--r--   0        0        0      986 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/mixedbread_ai_client/types.py
--rw-r--r--   0        0        0       25 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/mixedbread_ai/py.typed
--rw-r--r--   0        0        0      882 2024-02-01 12:07:11.083497 mixedbread_ai-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 mixedbread_ai-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11348 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0     3841 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/README.md
+-rw-r--r--   0        0        0     1981 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/__init__.py
+-rw-r--r--   0        0        0    17330 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/client.py
+-rw-r--r--   0        0        0      519 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/core/api_error.py
+-rw-r--r--   0        0        0      972 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      163 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/environment.py
+-rw-r--r--   0        0        0      620 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/errors/__init__.py
+-rw-r--r--   0        0        0      305 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/errors/bad_request_error.py
+-rw-r--r--   0        0        0      300 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/errors/forbidden_error.py
+-rw-r--r--   0        0        0      289 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/errors/internal_server_error.py
+-rw-r--r--   0        0        0      297 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/errors/not_found_error.py
+-rw-r--r--   0        0        0      326 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      312 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      300 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     2337 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/types/__init__.py
+-rw-r--r--   0        0        0     1135 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/types/bad_request_error_body.py
+-rw-r--r--   0        0        0      268 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/types/data.py
+-rw-r--r--   0        0        0     1138 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/types/embedding.py
+-rw-r--r--   0        0        0      152 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/types/embedding_item.py
+-rw-r--r--   0        0        0      217 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/types/embeddings_request_encoding_format.py
+-rw-r--r--   0        0        0     1517 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/types/embeddings_response.py
+-rw-r--r--   0        0        0      218 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/types/embeddings_response_encoding_format.py
+-rw-r--r--   0        0        0     1052 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/types/encoding_format.py
+-rw-r--r--   0        0        0     1132 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/types/forbidden_error_body.py
+-rw-r--r--   0        0        0      206 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/types/input.py
+-rw-r--r--   0        0        0     1124 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/types/internal_error.py
+-rw-r--r--   0        0        0     1166 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/types/invalid_matryoshka_dimensions_error.py
+-rw-r--r--   0        0        0     1156 2024-04-02 18:33:28.726333 mixedbread_ai-2.0.0/mixedbread_ai/types/invalid_matryoshka_model_error.py
+-rw-r--r--   0        0        0     1138 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/model_not_found_error.py
+-rw-r--r--   0        0        0     1353 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/multiple_encodings_embedding.py
+-rw-r--r--   0        0        0     1224 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/multiple_encodings_embedding_item.py
+-rw-r--r--   0        0        0     1060 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/mxbai_web_error.py
+-rw-r--r--   0        0        0      171 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/mxbai_web_error_details.py
+-rw-r--r--   0        0        0     1131 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/not_found_error_body.py
+-rw-r--r--   0        0        0      837 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/object_type.py
+-rw-r--r--   0        0        0     1151 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/ranked_document.py
+-rw-r--r--   0        0        0     1462 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/reranking_response.py
+-rw-r--r--   0        0        0      926 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/text_document.py
+-rw-r--r--   0        0        0     1146 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/too_many_requests_error_body.py
+-rw-r--r--   0        0        0      689 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/truncation_strategy.py
+-rw-r--r--   0        0        0     1138 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/unauthorized_error_body.py
+-rw-r--r--   0        0        0     1074 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/usage.py
+-rw-r--r--   0        0        0      141 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/validation_error.py
+-rw-r--r--   0        0        0     1133 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/mixedbread_ai/types/web_truncation_error.py
+-rw-r--r--   0        0        0      543 2024-04-02 18:33:28.730333 mixedbread_ai-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 mixedbread_ai-2.0.0/PKG-INFO
```

### Comparing `mixedbread_ai-1.2.5/LICENSE.md` & `mixedbread_ai-2.0.0/LICENSE.md`

 * *Files identical despite different names*

