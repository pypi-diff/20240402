# Comparing `tmp/unstract_adapters-0.7.1.tar.gz` & `tmp/unstract_adapters-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstract_adapters-0.7.1.tar", last modified: Tue Mar 26 08:32:05 2024, max compression
+gzip compressed data, was "unstract_adapters-0.8.0.tar", last modified: Tue Apr  2 04:46:27 2024, max compression
```

## Comparing `unstract_adapters-0.7.1.tar` & `unstract_adapters-0.8.0.tar`

### file list

```diff
@@ -1,152 +1,153 @@
--rw-r--r--   0        0        0     1396 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/README.md
--rw-r--r--   0        0        0     1555 2024-03-26 08:32:05.456656 unstract_adapters-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      297 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/__init__.py
--rw-r--r--   0        0        0     2665 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/adapterkit.py
--rw-r--r--   0        0        0     1745 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/base.py
--rw-r--r--   0        0        0      282 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/constants.py
--rw-r--r--   0        0        0      183 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/__init__.py
--rw-r--r--   0        0        0      154 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/azure_open_ai/README.md
--rw-r--r--   0        0        0      514 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/azure_open_ai/pyproject.toml
--rw-r--r--   0        0        0      216 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/azure_open_ai/src/__init__.py
--rw-r--r--   0        0        0     2511 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py
--rw-r--r--   0        0        0     1548 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0      899 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/embedding_adapter.py
--rw-r--r--   0        0        0     1324 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/helper.py
--rw-r--r--   0        0        0       42 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/hugging_face/README.md
--rw-r--r--   0        0        0      517 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/hugging_face/pyproject.toml
--rw-r--r--   0        0        0      215 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/hugging_face/src/__init__.py
--rw-r--r--   0        0        0     2876 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py
--rw-r--r--   0        0        0      940 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json
--rw-r--r--   0        0        0       30 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/open_ai/README.md
--rw-r--r--   0        0        0      503 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/open_ai/pyproject.toml
--rw-r--r--   0        0        0      190 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/open_ai/src/__init__.py
--rw-r--r--   0        0        0     2091 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/open_ai/src/open_ai.py
--rw-r--r--   0        0        0      719 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0       35 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/palm/README.md
--rw-r--r--   0        0        0      510 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/palm/pyproject.toml
--rw-r--r--   0        0        0      179 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/palm/src/__init__.py
--rw-r--r--   0        0        0     2041 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/palm/src/palm.py
--rw-r--r--   0        0        0      804 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/palm/src/static/json_schema.json
--rw-r--r--   0        0        0       46 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/qdrant_fast_embed/README.md
--rw-r--r--   0        0        0      524 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/qdrant_fast_embed/pyproject.toml
--rw-r--r--   0        0        0      239 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/__init__.py
--rw-r--r--   0        0        0     1827 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py
--rw-r--r--   0        0        0      553 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json
--rw-r--r--   0        0        0     2086 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/embedding/register.py
--rw-r--r--   0        0        0      184 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/enums.py
--rw-r--r--   0        0        0      321 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/exceptions.py
--rw-r--r--   0        0        0      165 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/llm/__init__.py
--rw-r--r--   0        0        0       33 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/llm/anthropic/README.md
--rw-r--r--   0        0        0      498 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/llm/anthropic/pyproject.toml
--rw-r--r--   0        0        0      207 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/llm/anthropic/src/__init__.py
--rw-r--r--   0        0        0     2324 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/llm/anthropic/src/anthropic.py
--rw-r--r--   0        0        0     1017 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/llm/anthropic/src/static/json_schema.json
--rw-r--r--   0        0        0       33 2024-03-26 08:31:44.960684 unstract_adapters-0.7.1/src/unstract/adapters/llm/any_scale/README.md
--rw-r--r--   0        0        0      498 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/any_scale/pyproject.toml
--rw-r--r--   0        0        0      202 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/any_scale/src/__init__.py
--rw-r--r--   0        0        0     2520 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/any_scale/src/anyscale.py
--rw-r--r--   0        0        0     1327 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/any_scale/src/static/json_schema.json
--rw-r--r--   0        0        0       37 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/azure_open_ai/README.md
--rw-r--r--   0        0        0      503 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/azure_open_ai/pyproject.toml
--rw-r--r--   0        0        0      219 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/azure_open_ai/src/__init__.py
--rw-r--r--   0        0        0     2350 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py
--rw-r--r--   0        0        0     1681 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0       41 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/constants.py
--rw-r--r--   0        0        0      844 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/helper.py
--rw-r--r--   0        0        0     1094 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/llm_adapter.py
--rw-r--r--   0        0        0       34 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/mistral/README.md
--rw-r--r--   0        0        0      500 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/mistral/pyproject.toml
--rw-r--r--   0        0        0      197 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/mistral/src/__init__.py
--rw-r--r--   0        0        0     1824 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/mistral/src/mistral.py
--rw-r--r--   0        0        0      852 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/mistral/src/static/json_schema.json
--rw-r--r--   0        0        0       31 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/open_ai/README.md
--rw-r--r--   0        0        0      491 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/open_ai/pyproject.toml
--rw-r--r--   0        0        0      193 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/open_ai/src/__init__.py
--rw-r--r--   0        0        0     2763 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/open_ai/src/open_ai.py
--rw-r--r--   0        0        0     1489 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0       26 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/palm/README.md
--rw-r--r--   0        0        0      496 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/palm/pyproject.toml
--rw-r--r--   0        0        0      182 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/palm/src/__init__.py
--rw-r--r--   0        0        0     2136 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/palm/src/palm.py
--rw-r--r--   0        0        0      989 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/palm/src/static/json_schema.json
--rw-r--r--   0        0        0     1963 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/register.py
--rw-r--r--   0        0        0       33 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/replicate/README.md
--rw-r--r--   0        0        0      499 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/replicate/pyproject.toml
--rw-r--r--   0        0        0      207 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/replicate/src/__init__.py
--rw-r--r--   0        0        0     1766 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/replicate/src/replicate.py
--rw-r--r--   0        0        0      840 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/replicate/src/static/json_schema.json
--rw-r--r--   0        0        0      273 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/vertex_ai/README.md
--rw-r--r--   0        0        0      480 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/vertex_ai/pyproject.toml
--rw-r--r--   0        0        0      203 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/vertex_ai/src/__init__.py
--rw-r--r--   0        0        0      964 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json
--rw-r--r--   0        0        0     2137 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py
--rw-r--r--   0        0        0      165 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/ocr/__init__.py
--rw-r--r--   0        0        0      430 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/ocr/constants.py
--rw-r--r--   0        0        0       42 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/ocr/google_document_ai/README.md
--rw-r--r--   0        0        0      491 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/ocr/google_document_ai/pyproject.toml
--rw-r--r--   0        0        0       42 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/ocr/google_document_ai/src/README.md
--rw-r--r--   0        0        0      237 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/ocr/google_document_ai/src/__init__.py
--rw-r--r--   0        0        0     5994 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py
--rw-r--r--   0        0        0      817 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json
--rw-r--r--   0        0        0      978 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/ocr/ocr_adapter.py
--rw-r--r--   0        0        0     1964 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/ocr/register.py
--rw-r--r--   0        0        0      277 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/registry.py
--rw-r--r--   0        0        0     1106 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/utils.py
--rw-r--r--   0        0        0      181 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/__init__.py
--rw-r--r--   0        0        0      225 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/constants.py
--rw-r--r--   0        0        0     4187 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/helper.py
--rw-r--r--   0        0        0       27 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/milvus/README.md
--rw-r--r--   0        0        0      508 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/milvus/pyproject.toml
--rw-r--r--   0        0        0      188 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/milvus/src/__init__.py
--rw-r--r--   0        0        0     2775 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/milvus/src/milvus.py
--rw-r--r--   0        0        0      805 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json
--rw-r--r--   0        0        0       29 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/pinecone/README.md
--rw-r--r--   0        0        0      519 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/pinecone/pyproject.toml
--rw-r--r--   0        0        0      198 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/pinecone/src/__init__.py
--rw-r--r--   0        0        0     3541 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/pinecone/src/pinecone.py
--rw-r--r--   0        0        0      771 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json
--rw-r--r--   0        0        0       29 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/postgres/README.md
--rw-r--r--   0        0        0      512 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/postgres/pyproject.toml
--rw-r--r--   0        0        0      198 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/postgres/src/__init__.py
--rw-r--r--   0        0        0     3930 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/postgres/src/postgres.py
--rw-r--r--   0        0        0      912 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json
--rw-r--r--   0        0        0       27 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/qdrant/README.md
--rw-r--r--   0        0        0      513 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/qdrant/pyproject.toml
--rw-r--r--   0        0        0      188 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/qdrant/src/__init__.py
--rw-r--r--   0        0        0     3019 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/qdrant/src/qdrant.py
--rw-r--r--   0        0        0      571 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json
--rw-r--r--   0        0        0     2039 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/register.py
--rw-r--r--   0        0        0    75042 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/samples/sample1.txt
--rw-r--r--   0        0        0       29 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/supabase/README.md
--rw-r--r--   0        0        0      512 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/supabase/pyproject.toml
--rw-r--r--   0        0        0      198 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/supabase/src/__init__.py
--rw-r--r--   0        0        0      937 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json
--rw-r--r--   0        0        0     3349 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/supabase/src/supabase.py
--rw-r--r--   0        0        0      947 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/vectordb_adapter.py
--rw-r--r--   0        0        0       29 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/weaviate/README.md
--rw-r--r--   0        0        0      520 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/weaviate/pyproject.toml
--rw-r--r--   0        0        0      198 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/weaviate/src/__init__.py
--rw-r--r--   0        0        0      678 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json
--rw-r--r--   0        0        0     3722 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/vectordb/weaviate/src/weaviate.py
--rw-r--r--   0        0        0      174 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/__init__.py
--rw-r--r--   0        0        0      145 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/constants.py
--rw-r--r--   0        0        0     4339 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/helper.py
--rw-r--r--   0        0        0       40 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/llm_whisperer/README.md
--rw-r--r--   0        0        0      495 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/llm_whisperer/pyproject.toml
--rw-r--r--   0        0        0      217 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/llm_whisperer/src/__init__.py
--rw-r--r--   0        0        0      981 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/llm_whisperer/src/constants.py
--rw-r--r--   0        0        0     6287 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py
--rw-r--r--   0        0        0     3115 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json
--rw-r--r--   0        0        0     1991 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/register.py
--rw-r--r--   0        0        0       51 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/unstructured_community/README.md
--rw-r--r--   0        0        0      499 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/unstructured_community/pyproject.toml
--rw-r--r--   0        0        0      255 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/unstructured_community/src/__init__.py
--rw-r--r--   0        0        0      583 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json
--rw-r--r--   0        0        0     1972 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py
--rw-r--r--   0        0        0       52 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/unstructured_enterprise/README.md
--rw-r--r--   0        0        0      499 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/unstructured_enterprise/pyproject.toml
--rw-r--r--   0        0        0      259 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/unstructured_enterprise/src/__init__.py
--rw-r--r--   0        0        0      805 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json
--rw-r--r--   0        0        0     1979 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py
--rw-r--r--   0        0        0     1006 2024-03-26 08:31:44.964684 unstract_adapters-0.7.1/src/unstract/adapters/x2text/x2text_adapter.py
--rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 unstract_adapters-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-02 04:46:08.105988 unstract_adapters-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1598 2024-04-02 04:46:08.105988 unstract_adapters-0.8.0/README.md
+-rw-r--r--   0        0        0     2271 2024-04-02 04:46:27.253869 unstract_adapters-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      297 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/__init__.py
+-rw-r--r--   0        0        0     2665 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/adapterkit.py
+-rw-r--r--   0        0        0     1745 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/base.py
+-rw-r--r--   0        0        0      282 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/constants.py
+-rw-r--r--   0        0        0      183 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/README.md
+-rw-r--r--   0        0        0      514 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/pyproject.toml
+-rw-r--r--   0        0        0      216 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2511 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py
+-rw-r--r--   0        0        0     1548 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0      899 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/embedding_adapter.py
+-rw-r--r--   0        0        0     1324 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/helper.py
+-rw-r--r--   0        0        0       42 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/README.md
+-rw-r--r--   0        0        0      517 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/pyproject.toml
+-rw-r--r--   0        0        0      215 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/src/__init__.py
+-rw-r--r--   0        0        0     2876 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py
+-rw-r--r--   0        0        0      940 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json
+-rw-r--r--   0        0        0       30 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/open_ai/README.md
+-rw-r--r--   0        0        0      503 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/open_ai/pyproject.toml
+-rw-r--r--   0        0        0      190 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2091 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/open_ai/src/open_ai.py
+-rw-r--r--   0        0        0      719 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0       35 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/palm/README.md
+-rw-r--r--   0        0        0      510 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/palm/pyproject.toml
+-rw-r--r--   0        0        0      179 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/palm/src/__init__.py
+-rw-r--r--   0        0        0     2041 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/palm/src/palm.py
+-rw-r--r--   0        0        0      804 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/palm/src/static/json_schema.json
+-rw-r--r--   0        0        0       46 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/README.md
+-rw-r--r--   0        0        0      524 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/pyproject.toml
+-rw-r--r--   0        0        0      239 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/__init__.py
+-rw-r--r--   0        0        0     1827 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py
+-rw-r--r--   0        0        0      553 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json
+-rw-r--r--   0        0        0     2086 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/register.py
+-rw-r--r--   0        0        0      184 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/enums.py
+-rw-r--r--   0        0        0      502 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/exceptions.py
+-rw-r--r--   0        0        0      165 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/anthropic/README.md
+-rw-r--r--   0        0        0      498 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/anthropic/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/anthropic/src/__init__.py
+-rw-r--r--   0        0        0     2324 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/anthropic/src/anthropic.py
+-rw-r--r--   0        0        0     1017 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/anthropic/src/static/json_schema.json
+-rw-r--r--   0        0        0       33 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/any_scale/README.md
+-rw-r--r--   0        0        0      498 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/any_scale/pyproject.toml
+-rw-r--r--   0        0        0      202 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/any_scale/src/__init__.py
+-rw-r--r--   0        0        0     2520 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/any_scale/src/anyscale.py
+-rw-r--r--   0        0        0     1327 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/any_scale/src/static/json_schema.json
+-rw-r--r--   0        0        0       37 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/azure_open_ai/README.md
+-rw-r--r--   0        0        0      503 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/azure_open_ai/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/azure_open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2312 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py
+-rw-r--r--   0        0        0     1681 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0       41 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/constants.py
+-rw-r--r--   0        0        0      844 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/helper.py
+-rw-r--r--   0        0        0     1544 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/llm_adapter.py
+-rw-r--r--   0        0        0       34 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/mistral/README.md
+-rw-r--r--   0        0        0      500 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/mistral/pyproject.toml
+-rw-r--r--   0        0        0      197 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/mistral/src/__init__.py
+-rw-r--r--   0        0        0     1824 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/mistral/src/mistral.py
+-rw-r--r--   0        0        0      852 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/mistral/src/static/json_schema.json
+-rw-r--r--   0        0        0       31 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/open_ai/README.md
+-rw-r--r--   0        0        0      491 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/open_ai/pyproject.toml
+-rw-r--r--   0        0        0      193 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2763 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/open_ai/src/open_ai.py
+-rw-r--r--   0        0        0     1489 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0       26 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/palm/README.md
+-rw-r--r--   0        0        0      496 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/palm/pyproject.toml
+-rw-r--r--   0        0        0      182 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/palm/src/__init__.py
+-rw-r--r--   0        0        0     2136 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/palm/src/palm.py
+-rw-r--r--   0        0        0      989 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/palm/src/static/json_schema.json
+-rw-r--r--   0        0        0     1963 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/register.py
+-rw-r--r--   0        0        0       33 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/replicate/README.md
+-rw-r--r--   0        0        0      499 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/replicate/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/replicate/src/__init__.py
+-rw-r--r--   0        0        0     1766 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/replicate/src/replicate.py
+-rw-r--r--   0        0        0      840 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/replicate/src/static/json_schema.json
+-rw-r--r--   0        0        0      273 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/vertex_ai/README.md
+-rw-r--r--   0        0        0      480 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/vertex_ai/pyproject.toml
+-rw-r--r--   0        0        0      203 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/vertex_ai/src/__init__.py
+-rw-r--r--   0        0        0      964 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0     2137 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py
+-rw-r--r--   0        0        0      165 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/__init__.py
+-rw-r--r--   0        0        0      430 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/constants.py
+-rw-r--r--   0        0        0       42 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/README.md
+-rw-r--r--   0        0        0      491 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/src/README.md
+-rw-r--r--   0        0        0      237 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/src/__init__.py
+-rw-r--r--   0        0        0     5994 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py
+-rw-r--r--   0        0        0      817 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0      978 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/ocr_adapter.py
+-rw-r--r--   0        0        0     1964 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/register.py
+-rw-r--r--   0        0        0      277 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/registry.py
+-rw-r--r--   0        0        0     1745 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/utils.py
+-rw-r--r--   0        0        0      181 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/constants.py
+-rw-r--r--   0        0        0     4187 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/helper.py
+-rw-r--r--   0        0        0       27 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/milvus/README.md
+-rw-r--r--   0        0        0      508 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/milvus/pyproject.toml
+-rw-r--r--   0        0        0      188 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/milvus/src/__init__.py
+-rw-r--r--   0        0        0     2775 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/milvus/src/milvus.py
+-rw-r--r--   0        0        0      805 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json
+-rw-r--r--   0        0        0       29 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/README.md
+-rw-r--r--   0        0        0      519 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/src/__init__.py
+-rw-r--r--   0        0        0     3541 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/src/pinecone.py
+-rw-r--r--   0        0        0      771 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json
+-rw-r--r--   0        0        0       29 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/README.md
+-rw-r--r--   0        0        0      512 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/src/__init__.py
+-rw-r--r--   0        0        0     3930 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/src/postgres.py
+-rw-r--r--   0        0        0      912 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json
+-rw-r--r--   0        0        0       27 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/README.md
+-rw-r--r--   0        0        0      513 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/pyproject.toml
+-rw-r--r--   0        0        0      188 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/src/__init__.py
+-rw-r--r--   0        0        0     3019 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/src/qdrant.py
+-rw-r--r--   0        0        0      571 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json
+-rw-r--r--   0        0        0     2039 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/register.py
+-rw-r--r--   0        0        0    75042 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/samples/sample1.txt
+-rw-r--r--   0        0        0       29 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/README.md
+-rw-r--r--   0        0        0      512 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/src/__init__.py
+-rw-r--r--   0        0        0      937 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json
+-rw-r--r--   0        0        0     3349 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/src/supabase.py
+-rw-r--r--   0        0        0      947 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/vectordb_adapter.py
+-rw-r--r--   0        0        0       29 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/README.md
+-rw-r--r--   0        0        0      520 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/src/__init__.py
+-rw-r--r--   0        0        0      678 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json
+-rw-r--r--   0        0        0     3722 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/src/weaviate.py
+-rw-r--r--   0        0        0      174 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/constants.py
+-rw-r--r--   0        0        0     5407 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/helper.py
+-rw-r--r--   0        0        0       40 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/README.md
+-rw-r--r--   0        0        0      495 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/pyproject.toml
+-rw-r--r--   0        0        0      217 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/src/__init__.py
+-rw-r--r--   0        0        0      981 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/src/constants.py
+-rw-r--r--   0        0        0     6562 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py
+-rw-r--r--   0        0        0     3115 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json
+-rw-r--r--   0        0        0     1991 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/register.py
+-rw-r--r--   0        0        0       51 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_community/README.md
+-rw-r--r--   0        0        0      499 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_community/pyproject.toml
+-rw-r--r--   0        0        0      255 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_community/src/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json
+-rw-r--r--   0        0        0     1463 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py
+-rw-r--r--   0        0        0       52 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_enterprise/README.md
+-rw-r--r--   0        0        0      499 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_enterprise/pyproject.toml
+-rw-r--r--   0        0        0      259 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_enterprise/src/__init__.py
+-rw-r--r--   0        0        0      805 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json
+-rw-r--r--   0        0        0     1468 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py
+-rw-r--r--   0        0        0     1006 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/x2text_adapter.py
+-rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 unstract_adapters-0.8.0/PKG-INFO
```

### Comparing `unstract_adapters-0.7.1/README.md` & `unstract_adapters-0.8.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+<div align="center">
+<img src="docs/assets/unstract_u_logo.png" style="height: 120px">
+
+# Unstract
+
+## No-code LLM Platform to launch APIs and ETL Pipelines to structure unstructured documents
+
+</div>
+
 # Unstract Adapters
 
 This is Unstract's python package which helps to configure to a number of different LLMs, Embeddings and VectorDBs.
 
 ## LLMs
 The following LLMs are supported:
```

### Comparing `unstract_adapters-0.7.1/pyproject.toml` & `unstract_adapters-0.8.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -3,20 +3,18 @@
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "unstract-adapters"
 dynamic = []
-description = "Unstract Adapters"
-authors = [
-    { name = "Zipstack Inc.", email = "devsupport@zipstack.com" },
-]
+description = "Unstract interface for LLMs, Embeddings and VectorDBs"
 dependencies = [
     "llama-index==0.9.28",
+    "requests>=2.31.0",
     "openai==1.3.9",
     "google-generativeai==0.3.1",
     "google-cloud-aiplatform==1.40.0",
     "fastembed==0.1.3",
     "huggingface==0.0.1",
     "pymilvus==2.3.4",
     "vecs==0.4.3",
@@ -29,46 +27,66 @@
     "SQLAlchemy==2.0.26",
     "anthropic==0.7.8",
     "replicate==0.22.0",
     "anyscale==0.5.165",
     "mistralai==0.0.8",
     "filetype~=1.2.0",
 ]
-requires-python = ">=3.9,<3.12"
 readme = "README.md"
+authors = [
+    { name = "Zipstack Inc.", email = "devsupport@zipstack.com" },
+]
+requires-python = ">=3.9,<3.12"
 classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: GNU Affero General Public License v3",
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: MacOS :: MacOS X",
     "Programming Language :: Python",
+    "Programming Language :: Python :: 3.9",
+    "Topic :: Scientific/Engineering",
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-version = "0.7.1"
+version = "0.8.0"
+
+[project.urls]
+Homepage = "https://unstract.com"
+"Release notes" = "https://github.com/Zipstack/unstract-adapters/releases"
+Source = "https://github.com/Zipstack/unstract-adapters"
 
 [project.license]
-text = "MIT"
+text = "AGPL v3"
 
 [tool.pdm.version]
 source = "file"
 path = "src/unstract/adapters/__init__.py"
 
 [tool.pdm.dev-dependencies]
 lint = [
+    "absolufy-imports~=0.3.1",
     "autopep8~=2.0.2",
-    "black~=23.3.0",
+    "black~=24.3.0",
     "docutils~=0.20.1",
-    "flake8~=6.0.0",
+    "flake8~=7.0.0",
     "flake8-pyproject~=1.2.2",
-    "isort~=5.12.0",
-    "pre-commit~=3.3.1",
-    "yamllint>=1.35.1",
-    "mypy~=1.2.0",
-    "absolufy-imports~=0.3.1",
-    "types-requests~=2.31.0.6",
-    "types-redis~=4.6.0.3",
-    "types-PyYAML~=6.0.12.12",
-    "types-pyOpenSSL~=23.2.0.2",
+    "isort~=5.13.2",
+    "mypy~=1.9.0",
+    "pre-commit~=3.6.2",
     "types-PyMySQL~=1.1.0.1",
+    "types-pyOpenSSL~=24.0.0.20240311",
+    "types-PyYAML~=6.0.12.12",
+    "types-redis~=4.6.0.3",
+    "types-requests~=2.31.0.6",
     "types-tzlocal~=5.1.0.1",
+    "yamllint>=1.35.1",
 ]
 
 [tool.pdm.build]
 includes = [
     "src",
 ]
 package-dir = "src"
+
+[tool.pdm.resolution.overrides]
+grpcio = ">=1.62.1"
+urllib3 = "<3,>=1.21.1"
```

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/adapterkit.py` & `unstract_adapters-0.8.0/src/unstract/adapters/adapterkit.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/base.py` & `unstract_adapters-0.8.0/src/unstract/adapters/base.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/azure_open_ai/pyproject.toml` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/embedding_adapter.py` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/embedding_adapter.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/helper.py` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/helper.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/hugging_face/pyproject.toml` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/open_ai/src/open_ai.py` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/open_ai/src/open_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/palm/src/palm.py` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/palm/src/palm.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/palm/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/palm/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/qdrant_fast_embed/pyproject.toml` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/embedding/register.py` & `unstract_adapters-0.8.0/src/unstract/adapters/embedding/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/anthropic/src/anthropic.py` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/anthropic/src/anthropic.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/anthropic/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/anthropic/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/any_scale/src/anyscale.py` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/any_scale/src/anyscale.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/any_scale/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/any_scale/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from typing import Any, Optional
 
 from llama_index.llms.azure_openai import AzureOpenAI
 from llama_index.llms.llm import LLM
+
 from unstract.adapters.exceptions import AdapterError
 from unstract.adapters.llm.constants import LLMKeys
 from unstract.adapters.llm.helper import LLMHelper
 from unstract.adapters.llm.llm_adapter import LLMAdapter
 
 
 class Constants:
@@ -35,18 +36,15 @@
 
     @staticmethod
     def get_description() -> str:
         return "AzureOpenAI LLM"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/AzureopenAI.png"
-        )
+        return "/icons/adapter-icons/AzureopenAI.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
```

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/helper.py` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/helper.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/llm_adapter.py` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/vectordb_adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-import logging
 from abc import ABC
-from typing import Any, Optional
+from typing import Any, Union
 
-from llama_index.llms.llm import LLM
+from llama_index.vector_stores.types import BasePydanticVectorStore, VectorStore
 from unstract.adapters.base import Adapter
 from unstract.adapters.enums import AdapterTypes
 
-logger = logging.getLogger(__name__)
 
-
-class LLMAdapter(Adapter, ABC):
+class VectorDBAdapter(Adapter, ABC):
     def __init__(self, name: str):
         super().__init__(name)
         self.name = name
 
     @staticmethod
     def get_id() -> str:
         return ""
@@ -32,19 +29,13 @@
 
     @staticmethod
     def get_json_schema() -> str:
         return ""
 
     @staticmethod
     def get_adapter_type() -> AdapterTypes:
-        return AdapterTypes.LLM
-
-    def get_llm_instance(self) -> Optional[LLM]:
-        """Instantiate the llama index LLM class.
+        return AdapterTypes.VECTOR_DB
 
-        Returns:
-            Optional[LLM]: llama index implementation of the LLM
-        """
+    def get_vector_db_instance(
+        self, vector_db_config: dict[str, Any]
+    ) -> Union[BasePydanticVectorStore, VectorStore, None]:
         return None
-
-    def test_connection(self, llm_metadata: dict[str, Any]) -> bool:
-        return False
```

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/mistral/src/mistral.py` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/mistral/src/mistral.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/mistral/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/mistral/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/open_ai/src/open_ai.py` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/open_ai/src/open_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/open_ai/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/palm/src/palm.py` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/palm/src/palm.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/palm/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/palm/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/register.py` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/replicate/src/replicate.py` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/replicate/src/replicate.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/replicate/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/replicate/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py` & `unstract_adapters-0.8.0/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py` & `unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/ocr/ocr_adapter.py` & `unstract_adapters-0.8.0/src/unstract/adapters/ocr/ocr_adapter.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/ocr/register.py` & `unstract_adapters-0.8.0/src/unstract/adapters/ocr/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/helper.py` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/helper.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/milvus/src/milvus.py` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/milvus/src/milvus.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/pinecone/pyproject.toml` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/pinecone/src/pinecone.py` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/src/pinecone.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/postgres/pyproject.toml` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/postgres/src/postgres.py` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/src/postgres.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/qdrant/pyproject.toml` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/qdrant/src/qdrant.py` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/src/qdrant.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/register.py` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/samples/sample1.txt` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/samples/sample1.txt`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/supabase/pyproject.toml` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/supabase/src/supabase.py` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/src/supabase.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/vectordb_adapter.py` & `unstract_adapters-0.8.0/src/unstract/adapters/x2text/x2text_adapter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from abc import ABC
-from typing import Any, Union
+from typing import Any, Optional
 
-from llama_index.vector_stores.types import BasePydanticVectorStore, VectorStore
 from unstract.adapters.base import Adapter
 from unstract.adapters.enums import AdapterTypes
 
 
-class VectorDBAdapter(Adapter, ABC):
+class X2TextAdapter(Adapter, ABC):
     def __init__(self, name: str):
         super().__init__(name)
         self.name = name
 
     @staticmethod
     def get_id() -> str:
         return ""
@@ -29,13 +28,20 @@
 
     @staticmethod
     def get_json_schema() -> str:
         return ""
 
     @staticmethod
     def get_adapter_type() -> AdapterTypes:
-        return AdapterTypes.VECTOR_DB
+        return AdapterTypes.X2TEXT
 
-    def get_vector_db_instance(
-        self, vector_db_config: dict[str, Any]
-    ) -> Union[BasePydanticVectorStore, VectorStore, None]:
-        return None
+    def test_connection(self) -> bool:
+        return False
+
+    def process(
+        self,
+        input_file_path: str,
+        output_file_path: Optional[str] = None,
+        **kwargs: dict[Any, Any],
+    ) -> str:
+        # Overriding methods will have the actual implementation
+        return ""
```

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/weaviate/pyproject.toml` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/vectordb/weaviate/src/weaviate.py` & `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/src/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/x2text/helper.py` & `unstract_adapters-0.8.0/src/unstract/adapters/x2text/helper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,97 @@
 import logging
 from typing import Any, Optional
 
 import requests
 from requests import Response
+from requests.exceptions import ConnectionError, HTTPError, Timeout
 
 from unstract.adapters.exceptions import AdapterError
+from unstract.adapters.utils import AdapterUtils
 from unstract.adapters.x2text.constants import X2TextConstants
 
 logger = logging.getLogger(__name__)
 
 
+class X2TextHelper:
+    """Helpers meant for x2text adapters."""
+
+    @staticmethod
+    def parse_response(
+        response: Response, out_file_path: Optional[str] = None
+    ) -> tuple[str, bool]:
+        """Parses the response from a request.
+
+        Optionally it can write the output to a file
+
+        Args:
+            response (Response): Response to parse
+            out_file_path (Optional[str], optional): Output file path to write
+                 to, skipped if None or emtpy. Defaults to None.
+        Returns:
+            tuple[str, bool]: Response's content and status of parsing
+        """
+        if not response.ok and not response.content:
+            return "", False
+        if isinstance(response.content, bytes):
+            output = response.content.decode("utf-8")
+        if out_file_path:
+            with open(out_file_path, "w", encoding="utf-8") as f:
+                f.write(output)
+        return output, True
+
+
 class UnstructuredHelper:
+    """Helpers meant for unstructured-community and unstructured-enterprise."""
+
     URL = "url"
     API_KEY = "api_key"
     TEST_CONNECTION = "test-connection"
     PROCESS = "process"
 
     @staticmethod
     def test_server_connection(
         unstructured_adapter_config: dict[str, Any]
     ) -> bool:
-        try:
-            response = UnstructuredHelper.make_request(
-                unstructured_adapter_config, UnstructuredHelper.TEST_CONNECTION
-            )
-            if response.status_code != 200:
-                logger.error(
-                    "Error in unstructured IO test-connection: "
-                    f"[{response.status_code}] {response.reason}"
-                )
-
-                raise AdapterError(
-                    f"{response.status_code} - {response.reason}"
-                )
-            else:
-                return True
-        except Exception as e:
-            if not isinstance(e, AdapterError):
-                raise AdapterError(str(e))
-            else:
-                raise e
+        UnstructuredHelper.make_request(
+            unstructured_adapter_config, UnstructuredHelper.TEST_CONNECTION
+        )
+        return True
 
     @staticmethod
     def process_document(
         unstructured_adapter_config: dict[str, Any],
         input_file_path: str,
         output_file_path: Optional[str] = None,
     ) -> str:
         try:
-            input_f = open(input_file_path, "rb")
-            files = {"file": input_f}
-            response = UnstructuredHelper.make_request(
-                unstructured_adapter_config,
-                UnstructuredHelper.PROCESS,
-                files=files,
-            )
-            if response.status_code != 200:
-                logger.error(
-                    "Error in unstructured IO process document: "
-                    f"[{response.status_code}] {response.reason}"
+            response: Response
+            with open(input_file_path, "rb") as input_f:
+                mime_type = AdapterUtils.get_file_mime_type(
+                    input_file=input_file_path
                 )
-                raise AdapterError(
-                    f"{response.status_code} - {response.reason}"
+                files = {"file": (input_file_path, input_f, mime_type)}
+                response = UnstructuredHelper.make_request(
+                    unstructured_adapter_config=unstructured_adapter_config,
+                    request_type=UnstructuredHelper.PROCESS,
+                    files=files,
                 )
-            else:
-                if response.content is not None:
-                    if isinstance(response.content, bytes):
-                        output = response.content.decode("utf-8")
-                    if output_file_path is not None:
-                        with open(output_file_path, "w", encoding="utf-8") as f:
-                            f.write(output)
-                            f.close()
-                    return output
-                else:
-                    raise AdapterError("No extracted content")
-        except Exception as e:
-            if not isinstance(e, AdapterError):
-                raise AdapterError(str(e))
-            else:
-                raise e
-        finally:
-            if input_f is not None:
-                input_f.close()
+            output, is_success = X2TextHelper.parse_response(
+                response=response, out_file_path=output_file_path
+            )
+            if not is_success:
+                raise AdapterError("Couldn't extract text from file")
+            return output
+        except OSError as e:
+            msg = f"OS error while reading {input_file_path} "
+            if output_file_path:
+                msg += f"and writing {output_file_path}"
+            msg += f": {str(e)}"
+            logger.error(msg)
+            raise AdapterError(str(e))
 
     @staticmethod
     def make_request(
         unstructured_adapter_config: dict[str, Any],
         request_type: str,
         **kwargs: dict[Any, Any],
     ) -> Response:
@@ -107,22 +113,41 @@
             "Authorization": f"Bearer {platform_service_api_key}",
         }
         body = {
             "unstructured-url": unstructured_url,
         }
         # Add api key only if present
         api_key = unstructured_adapter_config.get(UnstructuredHelper.API_KEY)
-        if api_key is not None and api_key != "":
+        if api_key:
             body["unstructured-api-key"] = api_key
 
         x2text_url = (
             f"{x2text_service_url}:{x2text_service_port}"
             f"/api/v1/x2text/{request_type}"
         )
         # Add files only if the request is for process
         files = None
         if "files" in kwargs:
             files = kwargs["files"] if kwargs["files"] is not None else None
-        response = requests.post(
-            x2text_url, headers=headers, data=body, files=files
-        )
+        try:
+            response = requests.post(
+                x2text_url, headers=headers, data=body, files=files
+            )
+            response.raise_for_status()
+        except ConnectionError as e:
+            logger.error(f"Adapter error: {e}")
+            raise AdapterError(
+                "Unable to connect to unstructured-io's service, "
+                "please check the URL"
+            )
+        except Timeout as e:
+            msg = "Request to unstructured-io's service has timed out"
+            logger.error(f"{msg}: {e}")
+            raise AdapterError(msg)
+        except HTTPError as e:
+            logger.error(f"Adapter error: {e}")
+            default_err = "Error while calling the unstructured-io service"
+            msg = AdapterUtils.get_msg_from_request_exc(
+                err=e, message_key="detail", default_err=default_err
+            )
+            raise AdapterError("unstructured-io: " + msg)
         return response
```

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/x2text/llm_whisperer/src/constants.py` & `unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/src/constants.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py` & `unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 import os
 from typing import Any, Optional
 
 import requests
 from requests import Response
-from requests.exceptions import ConnectionError, RequestException
+from requests.exceptions import ConnectionError, HTTPError, Timeout
 
 from unstract.adapters.exceptions import AdapterError
 from unstract.adapters.utils import AdapterUtils
 from unstract.adapters.x2text.constants import X2TextConstants
+from unstract.adapters.x2text.helper import X2TextHelper
 from unstract.adapters.x2text.llm_whisperer.src.constants import (
     HTTPMethod,
     OutputModes,
     ProcessingModes,
     WhispererConfig,
     WhispererDefaults,
     WhispererEndpoint,
@@ -80,35 +81,39 @@
             data = f.read()
             headers["Content-Type"] = "application/octet-stream"
 
         try:
             response: Response
             if request_method == HTTPMethod.GET:
                 response = requests.get(
-                    url=llm_whisperer_svc_url, headers=headers  # type: ignore
+                    url=llm_whisperer_svc_url, headers=headers
                 )
             elif request_method == HTTPMethod.POST:
                 response = requests.post(
                     url=llm_whisperer_svc_url,
-                    headers=headers,  # type: ignore
+                    headers=headers,
                     params=params,
                     data=data,
                 )
             else:
                 raise AdapterError(
                     f"Unsupported request method: {request_method}"
                 )
             response.raise_for_status()
         except ConnectionError as e:
             logger.error(f"Adapter error: {e}")
             raise AdapterError(
                 "Unable to connect to LLM Whisperer service, "
                 "please check the URL"
             )
-        except RequestException as e:
+        except Timeout as e:
+            msg = "Request to LLM whisperer has timed out"
+            logger.error(f"{msg}: {e}")
+            raise AdapterError(msg)
+        except HTTPError as e:
             logger.error(f"Adapter error: {e}")
             default_err = "Error while calling the LLM Whisperer service"
             msg = AdapterUtils.get_msg_from_request_exc(
                 err=e, message_key="message", default_err=default_err
             )
             raise AdapterError(msg)
         return response
@@ -151,25 +156,27 @@
 
             response = self._make_request(
                 request_method=HTTPMethod.POST,
                 request_endpoint=WhispererEndpoint.WHISPER,
                 params=params,
                 files=files,
             )
-            if response.ok and response.content is not None:
-                if isinstance(response.content, bytes):
-                    output = response.content.decode("utf-8")
-                if output_file_path is not None:
-                    with open(output_file_path, "w", encoding="utf-8") as f:
-                        f.write(output)
-                        f.close()
-                return output
-            return ""
-        except AdapterError:
-            raise
+            output, is_success = X2TextHelper.parse_response(
+                response=response, out_file_path=output_file_path
+            )
+            if not is_success:
+                raise AdapterError("Couldn't extract text from file")
+            return output  # type: ignore
+        except OSError as e:
+            msg = f"OS error while reading {input_file_path} "
+            if output_file_path:
+                msg += f"and writing {output_file_path}"
+            msg += f": {str(e)}"
+            logger.error(msg)
+            raise AdapterError(str(e))
         # TODO: Review this practice and remove if unnecessary
         except Exception as e:
             logger.error(f"Error occured while processing document: {e}")
             raise AdapterError(str(e))
         finally:
             if input_f is not None:
                 input_f.close()
```

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/x2text/register.py` & `unstract_adapters-0.8.0/src/unstract/adapters/x2text/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py` & `unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,49 +23,30 @@
 
     @staticmethod
     def get_description() -> str:
         return "Unstructured IO Community X2Text"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/UnstructuredIO.png"
-        )
+        return "/icons/" "adapter-icons/UnstructuredIO.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
     def process(
         self,
         input_file_path: str,
         output_file_path: Optional[str] = None,
         **kwargs: dict[Any, Any],
     ) -> str:
-        try:
-            output: str = UnstructuredHelper.process_document(
-                self.config, input_file_path, output_file_path
-            )
-            return output
-        except Exception as e:
-            logger.error(
-                f"Error occured while "
-                f"unstructured IO Community process document {e}"
-            )
-            raise e
+        output: str = UnstructuredHelper.process_document(
+            self.config, input_file_path, output_file_path
+        )
+        return output
 
     def test_connection(self) -> bool:
-        try:
-            result: bool = UnstructuredHelper.test_server_connection(
-                self.config
-            )
-            return result
-        except Exception as e:
-            logger.error(
-                f"Error occured while testing "
-                f"unstructured IO Community adapter {e}"
-            )
-            raise e
+        result: bool = UnstructuredHelper.test_server_connection(self.config)
+        return result
```

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json` & `unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.7.1/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py` & `unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,49 +23,30 @@
 
     @staticmethod
     def get_description() -> str:
         return "Unstructured IO Enterprise X2Text"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/UnstructuredIO.png"
-        )
+        return "/icons/" "adapter-icons/UnstructuredIO.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
     def process(
         self,
         input_file_path: str,
         output_file_path: Optional[str] = None,
         **kwargs: dict[Any, Any],
     ) -> str:
-        try:
-            output: str = UnstructuredHelper.process_document(
-                self.config, input_file_path, output_file_path
-            )
-            return output
-        except Exception as e:
-            logger.error(
-                f"Error occured while "
-                f"unstructured IO Enterprise process document {e}"
-            )
-            raise e
+        output: str = UnstructuredHelper.process_document(
+            self.config, input_file_path, output_file_path
+        )
+        return output
 
     def test_connection(self) -> bool:
-        try:
-            result: bool = UnstructuredHelper.test_server_connection(
-                self.config
-            )
-            return result
-        except Exception as e:
-            logger.error(
-                f"Error occured while testing "
-                f"unstructured IO Enterprise adapter {e}"
-            )
-            raise e
+        result: bool = UnstructuredHelper.test_server_connection(self.config)
+        return result
```

