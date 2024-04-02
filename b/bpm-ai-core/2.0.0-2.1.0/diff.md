# Comparing `tmp/bpm_ai_core-2.0.0.tar.gz` & `tmp/bpm_ai_core-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_core-2.0.0.tar", max compression
+gzip compressed data, was "bpm_ai_core-2.1.0.tar", max compression
```

## Comparing `bpm_ai_core-2.0.0.tar` & `bpm_ai_core-2.1.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0       13 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/README.md
--rw-r--r--   0        0        0        0 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/classification/__init__.py
--rw-r--r--   0        0        0     1187 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/classification/zero_shot_classifier.py
--rw-r--r--   0        0        0        0 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/__init__.py
--rw-r--r--   0        0        0      862 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/__init__.py
--rw-r--r--   0        0        0      306 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/_constants.py
--rw-r--r--   0        0        0     6130 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
--rw-r--r--   0        0        0      226 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
--rw-r--r--   0        0        0        0 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/tools/__init__.py
--rw-r--r--   0        0        0     1480 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/tools/base_tool.py
--rw-r--r--   0        0        0     1976 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/tools/messages_api_converters.py
--rw-r--r--   0        0        0     9833 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/tools/prompt_constructors.py
--rw-r--r--   0        0        0     1509 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/tools/tool.py
--rw-r--r--   0        0        0    17771 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/tools/tool_user.py
--rw-r--r--   0        0        0     2629 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/util.py
--rw-r--r--   0        0        0        0 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/common/__init__.py
--rw-r--r--   0        0        0     6036 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/common/blob.py
--rw-r--r--   0        0        0     2445 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/common/llm.py
--rw-r--r--   0        0        0     2710 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/common/message.py
--rw-r--r--   0        0        0     2781 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/common/tool.py
--rw-r--r--   0        0        0     1455 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/openai_chat/__init__.py
--rw-r--r--   0        0        0      438 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/openai_chat/_constants.py
--rw-r--r--   0        0        0     7710 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/openai_chat/openai_chat.py
--rw-r--r--   0        0        0     2626 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/llm/openai_chat/util.py
--rw-r--r--   0        0        0        0 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/ocr/__init__.py
--rw-r--r--   0        0        0     5611 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/ocr/amazon_textract.py
--rw-r--r--   0        0        0     2698 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/ocr/azure_doc_intelligence.py
--rw-r--r--   0        0        0     1220 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/ocr/ocr.py
--rw-r--r--   0        0        0        0 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/pos/__init__.py
--rw-r--r--   0        0        0      590 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/pos/pos_tagger.py
--rw-r--r--   0        0        0        0 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/prompt/__init__.py
--rw-r--r--   0        0        0      372 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/prompt/filters.py
--rw-r--r--   0        0        0     6259 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/prompt/prompt.py
--rw-r--r--   0        0        0        0 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/question_answering/__init__.py
--rw-r--r--   0        0        0     2085 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py
--rw-r--r--   0        0        0     3018 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
--rw-r--r--   0        0        0     1096 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/question_answering/question_answering.py
--rw-r--r--   0        0        0        0 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/speech_recognition/__init__.py
--rw-r--r--   0        0        0      740 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/speech_recognition/asr.py
--rw-r--r--   0        0        0     1395 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/speech_recognition/openai_whisper.py
--rw-r--r--   0        0        0        0 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/testing/__init__.py
--rw-r--r--   0        0        0     2889 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/testing/fake_llm.py
--rw-r--r--   0        0        0        0 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/tracing/__init__.py
--rw-r--r--   0        0        0     2434 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/tracing/decorators.py
--rw-r--r--   0        0        0     1597 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/tracing/delegate.py
--rw-r--r--   0        0        0     4370 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/tracing/langfuse.py
--rw-r--r--   0        0        0     2267 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/tracing/logging.py
--rw-r--r--   0        0        0     1097 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/tracing/tracer.py
--rw-r--r--   0        0        0      876 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/tracing/tracing.py
--rw-r--r--   0        0        0        0 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/translation/__init__.py
--rw-r--r--   0        0        0     1302 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/translation/amazon_translate.py
--rw-r--r--   0        0        0     1572 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/translation/azure_translation.py
--rw-r--r--   0        0        0      475 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/translation/nmt.py
--rw-r--r--   0        0        0        0 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/util/__init__.py
--rw-r--r--   0        0        0     1154 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/util/audio.py
--rw-r--r--   0        0        0     1836 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/util/file.py
--rw-r--r--   0        0        0     5233 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/util/image.py
--rw-r--r--   0        0        0     1670 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/util/json_schema.py
--rw-r--r--   0        0        0    21191 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/util/linguistics.py
--rw-r--r--   0        0        0     1130 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/util/markdown.py
--rw-r--r--   0        0        0     5280 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/util/remote_object.py
--rw-r--r--   0        0        0     2596 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/util/storage.py
--rw-r--r--   0        0        0      675 2024-03-30 23:26:38.745777 bpm_ai_core-2.0.0/bpm_ai_core/util/xml_convert.py
--rw-r--r--   0        0        0     1014 2024-03-30 23:26:38.749777 bpm_ai_core-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 bpm_ai_core-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/classification/__init__.py
+-rw-r--r--   0        0        0     1187 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/classification/zero_shot_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/_constants.py
+-rw-r--r--   0        0        0     6130 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
+-rw-r--r--   0        0        0      226 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
+-rw-r--r--   0        0        0        0 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/tools/__init__.py
+-rw-r--r--   0        0        0     1480 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/tools/base_tool.py
+-rw-r--r--   0        0        0     1976 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/tools/messages_api_converters.py
+-rw-r--r--   0        0        0     9833 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/tools/prompt_constructors.py
+-rw-r--r--   0        0        0     1509 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/tools/tool.py
+-rw-r--r--   0        0        0    17771 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/tools/tool_user.py
+-rw-r--r--   0        0        0     2629 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/common/__init__.py
+-rw-r--r--   0        0        0     6036 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/common/blob.py
+-rw-r--r--   0        0        0     2445 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/common/llm.py
+-rw-r--r--   0        0        0     2710 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/common/message.py
+-rw-r--r--   0        0        0     2781 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/common/tool.py
+-rw-r--r--   0        0        0     1455 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/openai_chat/__init__.py
+-rw-r--r--   0        0        0      438 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/openai_chat/_constants.py
+-rw-r--r--   0        0        0     7710 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/openai_chat/openai_chat.py
+-rw-r--r--   0        0        0     2626 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/llm/openai_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/ocr/__init__.py
+-rw-r--r--   0        0        0     5611 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/ocr/amazon_textract.py
+-rw-r--r--   0        0        0     2698 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/ocr/azure_doc_intelligence.py
+-rw-r--r--   0        0        0     1220 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/ocr/ocr.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/pos/__init__.py
+-rw-r--r--   0        0        0      590 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/pos/pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/prompt/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/prompt/filters.py
+-rw-r--r--   0        0        0     6259 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/prompt/prompt.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/question_answering/__init__.py
+-rw-r--r--   0        0        0     2085 2024-04-02 13:52:03.985600 bpm_ai_core-2.1.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py
+-rw-r--r--   0        0        0     3018 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
+-rw-r--r--   0        0        0     1096 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/question_answering/question_answering.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/speech_recognition/__init__.py
+-rw-r--r--   0        0        0      827 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/speech_recognition/asr.py
+-rw-r--r--   0        0        0     1428 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/speech_recognition/openai_whisper.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/testing/__init__.py
+-rw-r--r--   0        0        0     2889 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/testing/fake_llm.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/tracing/__init__.py
+-rw-r--r--   0        0        0     2434 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/tracing/decorators.py
+-rw-r--r--   0        0        0     1597 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/tracing/delegate.py
+-rw-r--r--   0        0        0     4370 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/tracing/langfuse.py
+-rw-r--r--   0        0        0     2267 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/tracing/logging.py
+-rw-r--r--   0        0        0     1097 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/tracing/tracer.py
+-rw-r--r--   0        0        0      876 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/tracing/tracing.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/translation/__init__.py
+-rw-r--r--   0        0        0     1302 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/translation/amazon_translate.py
+-rw-r--r--   0        0        0     1572 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/translation/azure_translation.py
+-rw-r--r--   0        0        0      475 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/translation/nmt.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/util/__init__.py
+-rw-r--r--   0        0        0     1154 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/util/audio.py
+-rw-r--r--   0        0        0     1836 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/util/file.py
+-rw-r--r--   0        0        0     5233 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/util/image.py
+-rw-r--r--   0        0        0     1670 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/util/json_schema.py
+-rw-r--r--   0        0        0    21191 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/util/linguistics.py
+-rw-r--r--   0        0        0     1130 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/util/markdown.py
+-rw-r--r--   0        0        0     5280 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/util/remote_object.py
+-rw-r--r--   0        0        0     2596 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/util/storage.py
+-rw-r--r--   0        0        0      675 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/bpm_ai_core/util/xml_convert.py
+-rw-r--r--   0        0        0     1014 2024-04-02 13:52:03.989600 bpm_ai_core-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 bpm_ai_core-2.1.0/PKG-INFO
```

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/classification/zero_shot_classifier.py` & `bpm_ai_core-2.1.0/bpm_ai_core/classification/zero_shot_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/__init__.py` & `bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py` & `bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/tools/base_tool.py` & `bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/tools/messages_api_converters.py` & `bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/tools/messages_api_converters.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/tools/prompt_constructors.py` & `bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/tools/prompt_constructors.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/tools/tool.py` & `bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/tools/tool.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/tools/tool_user.py` & `bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/tools/tool_user.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/llm/anthropic_chat/util.py` & `bpm_ai_core-2.1.0/bpm_ai_core/llm/anthropic_chat/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/llm/common/blob.py` & `bpm_ai_core-2.1.0/bpm_ai_core/llm/common/blob.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/llm/common/llm.py` & `bpm_ai_core-2.1.0/bpm_ai_core/llm/common/llm.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/llm/common/message.py` & `bpm_ai_core-2.1.0/bpm_ai_core/llm/common/message.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/llm/common/tool.py` & `bpm_ai_core-2.1.0/bpm_ai_core/llm/common/tool.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/llm/openai_chat/__init__.py` & `bpm_ai_core-2.1.0/bpm_ai_core/llm/openai_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/llm/openai_chat/openai_chat.py` & `bpm_ai_core-2.1.0/bpm_ai_core/llm/openai_chat/openai_chat.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/llm/openai_chat/util.py` & `bpm_ai_core-2.1.0/bpm_ai_core/llm/openai_chat/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/ocr/amazon_textract.py` & `bpm_ai_core-2.1.0/bpm_ai_core/ocr/amazon_textract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/ocr/azure_doc_intelligence.py` & `bpm_ai_core-2.1.0/bpm_ai_core/ocr/azure_doc_intelligence.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/ocr/ocr.py` & `bpm_ai_core-2.1.0/bpm_ai_core/ocr/ocr.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/pos/pos_tagger.py` & `bpm_ai_core-2.1.0/bpm_ai_core/pos/pos_tagger.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/prompt/prompt.py` & `bpm_ai_core-2.1.0/bpm_ai_core/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py` & `bpm_ai_core-2.1.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py` & `bpm_ai_core-2.1.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/question_answering/question_answering.py` & `bpm_ai_core-2.1.0/bpm_ai_core/question_answering/question_answering.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/speech_recognition/openai_whisper.py` & `bpm_ai_core-2.1.0/bpm_ai_core/speech_recognition/openai_whisper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 import logging
 from typing import Optional
 
 from typing_extensions import override
 
-from bpm_ai_core.speech_recognition.asr import ASRModel
+from bpm_ai_core.speech_recognition.asr import ASRModel, ASRResult
 
 logger = logging.getLogger(__name__)
 
 try:
     from openai import AsyncOpenAI, OpenAIError
     import httpx
 
@@ -38,14 +38,14 @@
         whisper_model: str = "whisper-1"
     ):
         if not has_openai:
             raise ImportError('openai is not installed')
         self.whisper_model = whisper_model
 
     @override
-    async def _do_transcribe(self, audio: io.BytesIO, language: Optional[str] = None) -> str:
+    async def _do_transcribe(self, audio: io.BytesIO, language: Optional[str] = None) -> ASRResult:
         transcript = await client.audio.transcriptions.create(
             model=self.whisper_model,
             file=audio,
             **{"language": language} if language else {}
         )
-        return transcript.text
+        return ASRResult(text=transcript.text)
```

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/testing/fake_llm.py` & `bpm_ai_core-2.1.0/bpm_ai_core/testing/fake_llm.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/tracing/decorators.py` & `bpm_ai_core-2.1.0/bpm_ai_core/tracing/decorators.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/tracing/delegate.py` & `bpm_ai_core-2.1.0/bpm_ai_core/tracing/delegate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/tracing/langfuse.py` & `bpm_ai_core-2.1.0/bpm_ai_core/tracing/langfuse.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/tracing/logging.py` & `bpm_ai_core-2.1.0/bpm_ai_core/tracing/logging.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/tracing/tracer.py` & `bpm_ai_core-2.1.0/bpm_ai_core/tracing/tracer.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/tracing/tracing.py` & `bpm_ai_core-2.1.0/bpm_ai_core/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/translation/amazon_translate.py` & `bpm_ai_core-2.1.0/bpm_ai_core/translation/amazon_translate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/translation/azure_translation.py` & `bpm_ai_core-2.1.0/bpm_ai_core/translation/azure_translation.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/util/audio.py` & `bpm_ai_core-2.1.0/bpm_ai_core/util/audio.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/util/file.py` & `bpm_ai_core-2.1.0/bpm_ai_core/util/file.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/util/image.py` & `bpm_ai_core-2.1.0/bpm_ai_core/util/image.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/util/json_schema.py` & `bpm_ai_core-2.1.0/bpm_ai_core/util/json_schema.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/util/linguistics.py` & `bpm_ai_core-2.1.0/bpm_ai_core/util/linguistics.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/util/markdown.py` & `bpm_ai_core-2.1.0/bpm_ai_core/util/markdown.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/util/remote_object.py` & `bpm_ai_core-2.1.0/bpm_ai_core/util/remote_object.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/util/storage.py` & `bpm_ai_core-2.1.0/bpm_ai_core/util/storage.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/bpm_ai_core/util/xml_convert.py` & `bpm_ai_core-2.1.0/bpm_ai_core/util/xml_convert.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.0.0/pyproject.toml` & `bpm_ai_core-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpm-ai-core"
-version = "2.0.0"
+version = "2.1.0"
 description = "Core AI abstractions and helpers."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `bpm_ai_core-2.0.0/PKG-INFO` & `bpm_ai_core-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpm-ai-core
-Version: 2.0.0
+Version: 2.1.0
 Summary: Core AI abstractions and helpers.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

