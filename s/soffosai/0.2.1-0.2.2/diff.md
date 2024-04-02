# Comparing `tmp/soffosai-0.2.1.tar.gz` & `tmp/soffosai-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soffosai-0.2.1.tar", last modified: Tue Mar 26 09:06:42 2024, max compression
+gzip compressed data, was "soffosai-0.2.2.tar", last modified: Tue Apr  2 07:46:50 2024, max compression
```

## Comparing `soffosai-0.2.1.tar` & `soffosai-0.2.2.tar`

### file list

```diff
@@ -1,128 +1,130 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 09:06:42.010676 soffosai-0.2.1/
--rw-rw-rw-   0        0        0     1070 2024-03-01 11:45:47.000000 soffosai-0.2.1/LICENSE
--rw-rw-rw-   0        0        0    16342 2024-03-26 09:06:42.010676 soffosai-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    15698 2024-03-03 11:15:17.000000 soffosai-0.2.1/README.md
--rw-rw-rw-   0        0        0      749 2024-03-26 09:03:38.000000 soffosai-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-26 09:06:42.010676 soffosai-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      358 2024-03-26 08:58:56.000000 soffosai-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-26 09:06:41.912799 soffosai-0.2.1/soffosai/
--rw-rw-rw-   0        0        0     3269 2024-03-01 11:45:47.000000 soffosai-0.2.1/soffosai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 09:06:41.943733 soffosai-0.2.1/soffosai/client/
--rw-rw-rw-   0        0        0       43 2024-03-01 11:45:47.000000 soffosai-0.2.1/soffosai/client/__init__.py
--rw-rw-rw-   0        0        0     3170 2024-03-01 11:45:47.000000 soffosai-0.2.1/soffosai/client/ai_response.py
-drwxrwxrwx   0        0        0        0 2024-03-26 09:06:41.945732 soffosai-0.2.1/soffosai/common/
--rw-rw-rw-   0        0        0      137 2024-03-01 11:45:47.000000 soffosai-0.2.1/soffosai/common/__init__.py
--rw-rw-rw-   0        0        0     3763 2024-03-20 11:29:55.000000 soffosai-0.2.1/soffosai/common/constants.py
--rw-rw-rw-   0        0        0      444 2024-03-01 11:45:47.000000 soffosai-0.2.1/soffosai/common/service_io_map.py
-drwxrwxrwx   0        0        0        0 2024-03-26 09:06:41.976116 soffosai-0.2.1/soffosai/common/serviceio_fields/
--rw-rw-rw-   0        0        0     2043 2024-03-20 11:12:52.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/__init__.py
--rw-rw-rw-   0        0        0      751 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/answer_scoring.py
--rw-rw-rw-   0        0        0     1443 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/audio_converter.py
--rw-rw-rw-   0        0        0     1037 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/chat_bot.py
--rw-rw-rw-   0        0        0      695 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/chat_bot_create.py
--rw-rw-rw-   0        0        0      738 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/chat_bot_delete_user_sessions.py
--rw-rw-rw-   0        0        0      730 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/chat_bot_get_user_sessions.py
--rw-rw-rw-   0        0        0      623 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/chat_bots_delete.py
--rw-rw-rw-   0        0        0      616 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/chat_bots_get.py
--rw-rw-rw-   0        0        0      655 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/discuss_count.py
--rw-rw-rw-   0        0        0      583 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/discuss_create.py
--rw-rw-rw-   0        0        0      619 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/discuss_delete.py
--rw-rw-rw-   0        0        0      697 2024-03-04 16:19:49.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/discuss_query.py
--rw-rw-rw-   0        0        0      721 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/documents_count.py
--rw-rw-rw-   0        0        0      626 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/documents_delete.py
--rw-rw-rw-   0        0        0     4365 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/documents_ingest.py
--rw-rw-rw-   0        0        0      891 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/documents_search.py
--rw-rw-rw-   0        0        0      604 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/email_analysis.py
--rw-rw-rw-   0        0        0     1413 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/emotion_detection.py
--rw-rw-rw-   0        0        0      827 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/file_converter.py
--rw-rw-rw-   0        0        0      623 2024-03-20 08:40:42.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/image_analysis.py
--rw-rw-rw-   0        0        0      696 2024-03-20 08:40:42.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/image_generation.py
--rw-rw-rw-   0        0        0      616 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/language_detection.py
--rw-rw-rw-   0        0        0      636 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/logical_error_detection.py
--rw-rw-rw-   0        0        0     1356 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/microlesson.py
--rw-rw-rw-   0        0        0      723 2024-03-20 09:50:35.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/multiple_choice_qn_a_generator.py
--rw-rw-rw-   0        0        0      647 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/named_entity_recognition.py
--rw-rw-rw-   0        0        0     1494 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/natural_s_q_l_generation.py
--rw-rw-rw-   0        0        0      594 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/paraphrase.py
--rw-rw-rw-   0        0        0      673 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/profanity.py
--rw-rw-rw-   0        0        0     1049 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/qna_generation.py
--rw-rw-rw-   0        0        0     1643 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/question_answering.py
--rw-rw-rw-   0        0        0      645 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/review_tagger.py
--rw-rw-rw-   0        0        0      724 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/search_recommendations.py
--rw-rw-rw-   0        0        0     1081 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/sentiment_analysis.py
--rw-rw-rw-   0        0        0     1206 2024-03-01 11:45:47.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/service_io.py
--rw-rw-rw-   0        0        0      612 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/simplify.py
--rw-rw-rw-   0        0        0      658 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/string_similarity.py
--rw-rw-rw-   0        0        0      642 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/summarization.py
--rw-rw-rw-   0        0        0      608 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/table_delete.py
--rw-rw-rw-   0        0        0      683 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/table_generator.py
--rw-rw-rw-   0        0        0      558 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/table_get.py
--rw-rw-rw-   0        0        0      674 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/table_ingest.py
--rw-rw-rw-   0        0        0      623 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/tag.py
--rw-rw-rw-   0        0        0      625 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/transcript_correction.py
--rw-rw-rw-   0        0        0     1631 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/translation.py
--rw-rw-rw-   0        0        0      630 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/common/serviceio_fields/website_converter.py
-drwxrwxrwx   0        0        0        0 2024-03-26 09:06:41.976116 soffosai-0.2.1/soffosai/core/
--rw-rw-rw-   0        0        0      113 2024-03-01 11:45:47.000000 soffosai-0.2.1/soffosai/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 09:06:41.980040 soffosai-0.2.1/soffosai/core/pipelines/
--rw-rw-rw-   0        0        0      245 2024-03-01 11:45:47.000000 soffosai-0.2.1/soffosai/core/pipelines/__init__.py
--rw-rw-rw-   0        0        0     1599 2024-03-01 11:45:47.000000 soffosai-0.2.1/soffosai/core/pipelines/document_summary.py
--rw-rw-rw-   0        0        0     1335 2024-03-01 11:45:47.000000 soffosai-0.2.1/soffosai/core/pipelines/file_ingest.py
--rw-rw-rw-   0        0        0     1362 2024-03-01 11:45:47.000000 soffosai-0.2.1/soffosai/core/pipelines/file_summary.py
--rw-rw-rw-   0        0        0     1695 2024-03-01 11:45:47.000000 soffosai-0.2.1/soffosai/core/pipelines/file_summary_ingest.py
--rw-rw-rw-   0        0        0    19493 2024-03-01 11:45:47.000000 soffosai-0.2.1/soffosai/core/pipelines/pipeline.py
-drwxrwxrwx   0        0        0        0 2024-03-26 09:06:42.010676 soffosai-0.2.1/soffosai/core/services/
--rw-rw-rw-   0        0        0     2637 2024-03-20 11:15:27.000000 soffosai-0.2.1/soffosai/core/services/__init__.py
--rw-rw-rw-   0        0        0     4838 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/answer_scoring.py
--rw-rw-rw-   0        0        0     3891 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/audio_converter.py
--rw-rw-rw-   0        0        0     7262 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/chat_bot.py
--rw-rw-rw-   0        0        0     4154 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/chat_bot_create.py
--rw-rw-rw-   0        0        0     3361 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/chat_bot_delete_user_sessions.py
--rw-rw-rw-   0        0        0     3243 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/chat_bot_get_user_sessions.py
--rw-rw-rw-   0        0        0     2801 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/chat_bots_delete.py
--rw-rw-rw-   0        0        0     3035 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/chat_bots_get.py
--rw-rw-rw-   0        0        0     4838 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/discuss_count.py
--rw-rw-rw-   0        0        0     3106 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/discuss_create.py
--rw-rw-rw-   0        0        0     3370 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/discuss_delete.py
--rw-rw-rw-   0        0        0     4207 2024-03-04 16:18:15.000000 soffosai-0.2.1/soffosai/core/services/discuss_query.py
--rw-rw-rw-   0        0        0     4126 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/documents_count.py
--rw-rw-rw-   0        0        0     2790 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/documents_delete.py
--rw-rw-rw-   0        0        0     5727 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/documents_ingest.py
--rw-rw-rw-   0        0        0     6304 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/documents_search.py
--rw-rw-rw-   0        0        0     3039 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/email_analysis.py
--rw-rw-rw-   0        0        0     5672 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/emotion_detection.py
--rw-rw-rw-   0        0        0     6551 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/file_converter.py
--rw-rw-rw-   0        0        0     3094 2024-03-20 11:20:06.000000 soffosai-0.2.1/soffosai/core/services/image_analysis.py
--rw-rw-rw-   0        0        0     3654 2024-03-21 05:30:43.000000 soffosai-0.2.1/soffosai/core/services/image_generation.py
--rw-rw-rw-   0        0        0     1167 2024-03-01 11:45:47.000000 soffosai-0.2.1/soffosai/core/services/input_config.py
--rw-rw-rw-   0        0        0     2713 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/language_detection.py
--rw-rw-rw-   0        0        0     3401 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/logical_error_detection.py
--rw-rw-rw-   0        0        0     3624 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/microlesson.py
--rw-rw-rw-   0        0        0     3483 2024-03-20 09:50:35.000000 soffosai-0.2.1/soffosai/core/services/multiple_choice_qn_a_generator.py
--rw-rw-rw-   0        0        0     4580 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/named_entity_recognition.py
--rw-rw-rw-   0        0        0    11501 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/natural_s_q_l_generation.py
--rw-rw-rw-   0        0        0     2826 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/paraphrase.py
--rw-rw-rw-   0        0        0     3749 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/profanity.py
--rw-rw-rw-   0        0        0     5711 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/qna_generation.py
--rw-rw-rw-   0        0        0    12201 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/question_answering.py
--rw-rw-rw-   0        0        0     3526 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/review_tagger.py
--rw-rw-rw-   0        0        0     2855 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/search_recommendations.py
--rw-rw-rw-   0        0        0     4963 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/sentiment_analysis.py
--rw-rw-rw-   0        0        0    13761 2024-03-01 11:45:47.000000 soffosai-0.2.1/soffosai/core/services/service.py
--rw-rw-rw-   0        0        0     3133 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/simplify.py
--rw-rw-rw-   0        0        0     4803 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/string_similarity.py
--rw-rw-rw-   0        0        0     3601 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/summarization.py
--rw-rw-rw-   0        0        0     2521 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/table_delete.py
--rw-rw-rw-   0        0        0     4020 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/table_generator.py
--rw-rw-rw-   0        0        0     2303 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/table_get.py
--rw-rw-rw-   0        0        0     2896 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/table_ingest.py
--rw-rw-rw-   0        0        0     4166 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/tag.py
--rw-rw-rw-   0        0        0     2952 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/transcript_correction.py
--rw-rw-rw-   0        0        0     3425 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/translation.py
--rw-rw-rw-   0        0        0     3463 2024-03-03 11:15:17.000000 soffosai-0.2.1/soffosai/core/services/website_converter.py
-drwxrwxrwx   0        0        0        0 2024-03-26 09:06:42.010676 soffosai-0.2.1/soffosai.egg-info/
--rw-rw-rw-   0        0        0    16342 2024-03-26 09:06:41.000000 soffosai-0.2.1/soffosai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5119 2024-03-26 09:06:41.000000 soffosai-0.2.1/soffosai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 09:06:41.000000 soffosai-0.2.1/soffosai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-26 09:06:41.000000 soffosai-0.2.1/soffosai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-26 09:06:41.000000 soffosai-0.2.1/soffosai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 07:46:50.920957 soffosai-0.2.2/
+-rw-rw-rw-   0        0        0     1070 2024-03-01 11:45:47.000000 soffosai-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0    16478 2024-04-02 07:46:50.919958 soffosai-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    15834 2024-03-27 10:23:08.000000 soffosai-0.2.2/README.md
+-rw-rw-rw-   0        0        0      749 2024-03-27 10:18:29.000000 soffosai-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 07:46:50.920957 soffosai-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      358 2024-03-27 10:18:37.000000 soffosai-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:46:50.828226 soffosai-0.2.2/soffosai/
+-rw-rw-rw-   0        0        0     3269 2024-03-01 11:45:47.000000 soffosai-0.2.2/soffosai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:46:50.853196 soffosai-0.2.2/soffosai/client/
+-rw-rw-rw-   0        0        0       43 2024-03-01 11:45:47.000000 soffosai-0.2.2/soffosai/client/__init__.py
+-rw-rw-rw-   0        0        0     3170 2024-03-01 11:45:47.000000 soffosai-0.2.2/soffosai/client/ai_response.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:46:50.855209 soffosai-0.2.2/soffosai/common/
+-rw-rw-rw-   0        0        0      137 2024-03-01 11:45:47.000000 soffosai-0.2.2/soffosai/common/__init__.py
+-rw-rw-rw-   0        0        0     3822 2024-03-27 10:24:25.000000 soffosai-0.2.2/soffosai/common/constants.py
+-rw-rw-rw-   0        0        0      444 2024-03-01 11:45:47.000000 soffosai-0.2.2/soffosai/common/service_io_map.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:46:50.886235 soffosai-0.2.2/soffosai/common/serviceio_fields/
+-rw-rw-rw-   0        0        0     2100 2024-03-27 10:08:32.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/__init__.py
+-rw-rw-rw-   0        0        0      751 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/answer_scoring.py
+-rw-rw-rw-   0        0        0      724 2024-03-27 10:06:40.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/assessment_generator.py
+-rw-rw-rw-   0        0        0     1443 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/audio_converter.py
+-rw-rw-rw-   0        0        0     1037 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/chat_bot.py
+-rw-rw-rw-   0        0        0      695 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/chat_bot_create.py
+-rw-rw-rw-   0        0        0      738 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/chat_bot_delete_user_sessions.py
+-rw-rw-rw-   0        0        0      730 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/chat_bot_get_user_sessions.py
+-rw-rw-rw-   0        0        0      623 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/chat_bots_delete.py
+-rw-rw-rw-   0        0        0      616 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/chat_bots_get.py
+-rw-rw-rw-   0        0        0      655 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/discuss_count.py
+-rw-rw-rw-   0        0        0      583 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/discuss_create.py
+-rw-rw-rw-   0        0        0      619 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/discuss_delete.py
+-rw-rw-rw-   0        0        0      697 2024-03-04 16:19:49.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/discuss_query.py
+-rw-rw-rw-   0        0        0      721 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/documents_count.py
+-rw-rw-rw-   0        0        0      626 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/documents_delete.py
+-rw-rw-rw-   0        0        0     4365 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/documents_ingest.py
+-rw-rw-rw-   0        0        0      891 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/documents_search.py
+-rw-rw-rw-   0        0        0      604 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/email_analysis.py
+-rw-rw-rw-   0        0        0     1413 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/emotion_detection.py
+-rw-rw-rw-   0        0        0      827 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/file_converter.py
+-rw-rw-rw-   0        0        0      623 2024-03-20 08:40:42.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/image_analysis.py
+-rw-rw-rw-   0        0        0      696 2024-03-20 08:40:42.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/image_generation.py
+-rw-rw-rw-   0        0        0      616 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/language_detection.py
+-rw-rw-rw-   0        0        0      636 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/logical_error_detection.py
+-rw-rw-rw-   0        0        0     1356 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/microlesson.py
+-rw-rw-rw-   0        0        0      723 2024-03-20 09:50:35.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/multiple_choice_qn_a_generator.py
+-rw-rw-rw-   0        0        0      647 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/named_entity_recognition.py
+-rw-rw-rw-   0        0        0     1494 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/natural_s_q_l_generation.py
+-rw-rw-rw-   0        0        0      594 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/paraphrase.py
+-rw-rw-rw-   0        0        0      673 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/profanity.py
+-rw-rw-rw-   0        0        0     1049 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/qna_generation.py
+-rw-rw-rw-   0        0        0     1643 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/question_answering.py
+-rw-rw-rw-   0        0        0      645 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/review_tagger.py
+-rw-rw-rw-   0        0        0      724 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/search_recommendations.py
+-rw-rw-rw-   0        0        0     1081 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/sentiment_analysis.py
+-rw-rw-rw-   0        0        0     1206 2024-03-01 11:45:47.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/service_io.py
+-rw-rw-rw-   0        0        0      612 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/simplify.py
+-rw-rw-rw-   0        0        0      658 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/string_similarity.py
+-rw-rw-rw-   0        0        0      642 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/summarization.py
+-rw-rw-rw-   0        0        0      608 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/table_delete.py
+-rw-rw-rw-   0        0        0      683 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/table_generator.py
+-rw-rw-rw-   0        0        0      558 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/table_get.py
+-rw-rw-rw-   0        0        0      674 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/table_ingest.py
+-rw-rw-rw-   0        0        0      623 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/tag.py
+-rw-rw-rw-   0        0        0      625 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/transcript_correction.py
+-rw-rw-rw-   0        0        0     1631 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/translation.py
+-rw-rw-rw-   0        0        0      630 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/common/serviceio_fields/website_converter.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:46:50.887236 soffosai-0.2.2/soffosai/core/
+-rw-rw-rw-   0        0        0      113 2024-03-01 11:45:47.000000 soffosai-0.2.2/soffosai/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:46:50.890759 soffosai-0.2.2/soffosai/core/pipelines/
+-rw-rw-rw-   0        0        0      245 2024-03-01 11:45:47.000000 soffosai-0.2.2/soffosai/core/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     1599 2024-03-01 11:45:47.000000 soffosai-0.2.2/soffosai/core/pipelines/document_summary.py
+-rw-rw-rw-   0        0        0     1335 2024-03-01 11:45:47.000000 soffosai-0.2.2/soffosai/core/pipelines/file_ingest.py
+-rw-rw-rw-   0        0        0     1362 2024-03-01 11:45:47.000000 soffosai-0.2.2/soffosai/core/pipelines/file_summary.py
+-rw-rw-rw-   0        0        0     1695 2024-03-01 11:45:47.000000 soffosai-0.2.2/soffosai/core/pipelines/file_summary_ingest.py
+-rw-rw-rw-   0        0        0    19493 2024-03-01 11:45:47.000000 soffosai-0.2.2/soffosai/core/pipelines/pipeline.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:46:50.918958 soffosai-0.2.2/soffosai/core/services/
+-rw-rw-rw-   0        0        0     2699 2024-03-27 10:11:29.000000 soffosai-0.2.2/soffosai/core/services/__init__.py
+-rw-rw-rw-   0        0        0     4838 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/answer_scoring.py
+-rw-rw-rw-   0        0        0     3639 2024-03-27 10:10:14.000000 soffosai-0.2.2/soffosai/core/services/assessment_generator.py
+-rw-rw-rw-   0        0        0     3891 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/audio_converter.py
+-rw-rw-rw-   0        0        0     7262 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/chat_bot.py
+-rw-rw-rw-   0        0        0     4154 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/chat_bot_create.py
+-rw-rw-rw-   0        0        0     3361 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/chat_bot_delete_user_sessions.py
+-rw-rw-rw-   0        0        0     3243 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/chat_bot_get_user_sessions.py
+-rw-rw-rw-   0        0        0     2801 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/chat_bots_delete.py
+-rw-rw-rw-   0        0        0     3035 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/chat_bots_get.py
+-rw-rw-rw-   0        0        0     4838 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/discuss_count.py
+-rw-rw-rw-   0        0        0     3106 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/discuss_create.py
+-rw-rw-rw-   0        0        0     3370 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/discuss_delete.py
+-rw-rw-rw-   0        0        0     4207 2024-03-04 16:18:15.000000 soffosai-0.2.2/soffosai/core/services/discuss_query.py
+-rw-rw-rw-   0        0        0     4126 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/documents_count.py
+-rw-rw-rw-   0        0        0     2790 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/documents_delete.py
+-rw-rw-rw-   0        0        0     5727 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/documents_ingest.py
+-rw-rw-rw-   0        0        0     6304 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/documents_search.py
+-rw-rw-rw-   0        0        0     3039 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/email_analysis.py
+-rw-rw-rw-   0        0        0     5672 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/emotion_detection.py
+-rw-rw-rw-   0        0        0     6551 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/file_converter.py
+-rw-rw-rw-   0        0        0     2902 2024-03-27 10:11:58.000000 soffosai-0.2.2/soffosai/core/services/image_analysis.py
+-rw-rw-rw-   0        0        0     3462 2024-03-27 10:12:12.000000 soffosai-0.2.2/soffosai/core/services/image_generation.py
+-rw-rw-rw-   0        0        0     1167 2024-03-01 11:45:47.000000 soffosai-0.2.2/soffosai/core/services/input_config.py
+-rw-rw-rw-   0        0        0     2713 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/language_detection.py
+-rw-rw-rw-   0        0        0     3401 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/logical_error_detection.py
+-rw-rw-rw-   0        0        0     3624 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/microlesson.py
+-rw-rw-rw-   0        0        0     3291 2024-03-27 10:12:30.000000 soffosai-0.2.2/soffosai/core/services/multiple_choice_qn_a_generator.py
+-rw-rw-rw-   0        0        0     4580 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/named_entity_recognition.py
+-rw-rw-rw-   0        0        0    11501 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/natural_s_q_l_generation.py
+-rw-rw-rw-   0        0        0     2826 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/paraphrase.py
+-rw-rw-rw-   0        0        0     3749 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/profanity.py
+-rw-rw-rw-   0        0        0     5711 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/qna_generation.py
+-rw-rw-rw-   0        0        0    12201 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/question_answering.py
+-rw-rw-rw-   0        0        0     3526 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/review_tagger.py
+-rw-rw-rw-   0        0        0     2855 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/search_recommendations.py
+-rw-rw-rw-   0        0        0     4963 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/sentiment_analysis.py
+-rw-rw-rw-   0        0        0    13761 2024-03-01 11:45:47.000000 soffosai-0.2.2/soffosai/core/services/service.py
+-rw-rw-rw-   0        0        0     3133 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/simplify.py
+-rw-rw-rw-   0        0        0     4803 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/string_similarity.py
+-rw-rw-rw-   0        0        0     3601 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/summarization.py
+-rw-rw-rw-   0        0        0     2521 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/table_delete.py
+-rw-rw-rw-   0        0        0     4020 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/table_generator.py
+-rw-rw-rw-   0        0        0     2303 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/table_get.py
+-rw-rw-rw-   0        0        0     2896 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/table_ingest.py
+-rw-rw-rw-   0        0        0     4166 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/tag.py
+-rw-rw-rw-   0        0        0     2952 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/transcript_correction.py
+-rw-rw-rw-   0        0        0     3425 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/translation.py
+-rw-rw-rw-   0        0        0     3463 2024-03-03 11:15:17.000000 soffosai-0.2.2/soffosai/core/services/website_converter.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:46:50.918958 soffosai-0.2.2/soffosai.egg-info/
+-rw-rw-rw-   0        0        0    16478 2024-04-02 07:46:50.000000 soffosai-0.2.2/soffosai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5223 2024-04-02 07:46:50.000000 soffosai-0.2.2/soffosai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 07:46:50.000000 soffosai-0.2.2/soffosai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 07:46:50.000000 soffosai-0.2.2/soffosai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 07:46:50.000000 soffosai-0.2.2/soffosai.egg-info/top_level.txt
```

### Comparing `soffosai-0.2.1/LICENSE` & `soffosai-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/PKG-INFO` & `soffosai-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soffosai
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python SDK for Soffos AI
 Author: Soffosai
 Author-email: "Soffos.ai" <Soffos@Soffos.ai>, Franco Such <franco.such@Soffos.ai>, Andreas Christofi <andreas.christofi@Soffos.ai>
 Project-URL: Homepage, https://github.com/Soffos-Inc/soffos_ai
 Project-URL: Bug Tracker, https://github.com/Soffos-Inc/soffos_ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -53,14 +53,15 @@
 
 ## SoffosAIService
 The SoffosAIService class handles validation and execution of specified endpoint vs payload.
 Here is the list of SoffosAIService Subclasses:
 ```
 [
     "AnswerScoringService",
+    "AssessmentGeneratorService"
     "AudioConverterService",
     "ChatBotCreateService",
     "ChatBotDeleteUserSessionsService",
     "ChatBotGetUserSessionsService",
     "ChatBotsDeleteService",
     "ChatBotService",
     "ChatBotsGetService",
@@ -70,15 +71,18 @@
     "DiscussDeleteService",
     "DocumentsCountService",
     "DocumentsIngestService", 
     "DocumentsSearchService", 
     "DocumentsDeleteService", 
     "EmailAnalysisService",
     "FileConverterService",
+    "ImageAnalysisService",
+    "ImageGenerationService",
     "MicrolessonService",
+    "MultipleChoiceQnAGeneratorService",
     "NERService",
     "NaturalSQLGenerationService",
     "ParaphraseService",
     "QnAGenerationService",
     "SearchRecommendationsService",
     "SentimentAnalysisService",
     "SimplifyService",
```

### Comparing `soffosai-0.2.1/README.md` & `soffosai-0.2.2/soffosai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: soffosai
+Version: 0.2.2
+Summary: Python SDK for Soffos AI
+Author: Soffosai
+Author-email: "Soffos.ai" <Soffos@Soffos.ai>, Franco Such <franco.such@Soffos.ai>, Andreas Christofi <andreas.christofi@Soffos.ai>
+Project-URL: Homepage, https://github.com/Soffos-Inc/soffos_ai
+Project-URL: Bug Tracker, https://github.com/Soffos-Inc/soffos_ai/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+
 # Welcome to the Soffos Platform SDK
 At Soffos Inc., our specialty is helping organizations create pioneering apps with conversational artificial intelligence (CAI) and natural language processing (NLP) at their core.
 
 NLP and conversational AI are at the heart of everything Soffos does. Using Soffos’ technology, we offer a suite of unique application programming interfaces (APIs) so businesses can choose the natural language and generative AI functionalities they would like to include in any kind of application.
 
 What sets Soffos apart is we’ve taken the most advanced technology, enhanced it with our own R&D, and made it easy to use and accessible to everyone.
 
@@ -37,14 +53,15 @@
 
 ## SoffosAIService
 The SoffosAIService class handles validation and execution of specified endpoint vs payload.
 Here is the list of SoffosAIService Subclasses:
 ```
 [
     "AnswerScoringService",
+    "AssessmentGeneratorService"
     "AudioConverterService",
     "ChatBotCreateService",
     "ChatBotDeleteUserSessionsService",
     "ChatBotGetUserSessionsService",
     "ChatBotsDeleteService",
     "ChatBotService",
     "ChatBotsGetService",
@@ -54,15 +71,18 @@
     "DiscussDeleteService",
     "DocumentsCountService",
     "DocumentsIngestService", 
     "DocumentsSearchService", 
     "DocumentsDeleteService", 
     "EmailAnalysisService",
     "FileConverterService",
+    "ImageAnalysisService",
+    "ImageGenerationService",
     "MicrolessonService",
+    "MultipleChoiceQnAGeneratorService",
     "NERService",
     "NaturalSQLGenerationService",
     "ParaphraseService",
     "QnAGenerationService",
     "SearchRecommendationsService",
     "SentimentAnalysisService",
     "SimplifyService",
@@ -362,8 +382,8 @@
         super().__init__(services, **kwargs)
 
 
     def __call__(self, user, file, sent_length, question):
         return super().__call__(user=user, file=file, sent_length=sent_length, question=question)
 ```
 
-Copyright (c)2023 - Soffos.ai - All rights reserved
+Copyright (c)2023 - Soffos.ai - All rights reserved
```

### Comparing `soffosai-0.2.1/pyproject.toml` & `soffosai-0.2.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools >= 40.9.0",
     "wheel >= 0.36.2",
 ]
 
 [project]
 name = "soffosai"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Soffos.ai", email="Soffos@Soffos.ai" },
   { name="Franco Such", email="franco.such@Soffos.ai" },
   { name="Andreas Christofi", email="andreas.christofi@Soffos.ai" }
 
 ]
 description = "Python SDK for Soffos AI"
```

### Comparing `soffosai-0.2.1/soffosai/__init__.py` & `soffosai-0.2.2/soffosai/__init__.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/client/ai_response.py` & `soffosai-0.2.2/soffosai/client/ai_response.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/constants.py` & `soffosai-0.2.2/soffosai/common/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 Created at: 2023-04-19
 Purpose: Organize the constants
 -----------------------------------------------------
 '''
 SOFFOS_SERVICE_URL = "https://api.soffos.ai/service/"
 
 SERVICES_LIST = [
-    'answer-scoring', 
+    'answer-scoring',
+    'assessment',
     'audio_converter',
     'chatbot/create',
     'chatbot',
     'chatbot/get',
     'chatbot/delete',
     'chatbot/sessions/get',
     'chatbot/sessions/delete',
@@ -59,14 +60,15 @@
 ]
 
 class ServiceString:
     '''
     Contains the list of Soffos services as attributes
     '''
     ANSWER_SCORING = 'answer-scoring'
+    ASSESSMENT_GENERATOR = 'assessment'
     AUDIO_CONVERTER = 'audio-converter'
     CHAT_BOT_CREATE = 'chatbot/create'
     CHAT_BOT = 'chatbot'
     CHAT_BOTS_GET = 'chatbot/get'
     CHAT_BOTS_DELETE = 'chatbot/delete'
     CHAT_BOT_GET_USER_SESSIONS = 'chatbot/sessions/get'
     CHAT_BOT_DELETE_USER_SESSIONS = 'chatbot/sessions/delete'
```

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/__init__.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .service_io import ServiceIO
 from .answer_scoring import AnswerScoringIO
+from .assessment_generator import AssessmentGeneratorIO
 from .audio_converter import AudioConverterIO
 from .chat_bot_create import ChatBotCreateIO
 from .chat_bot import ChatBotIO
 from .chat_bots_get import ChatBotsGetIO
 from .chat_bots_delete import ChatBotsDeleteIO
 from .chat_bot_delete_user_sessions import ChatBotDeleteUserSessionsIO
 from .discuss_count import DiscussCountIO
```

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/answer_scoring.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/answer_scoring.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/audio_converter.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/audio_converter.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/chat_bot.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/chat_bot.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/chat_bot_create.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/chat_bot_create.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/chat_bot_delete_user_sessions.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/chat_bot_delete_user_sessions.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/chat_bot_get_user_sessions.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/chat_bot_get_user_sessions.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/chat_bots_delete.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/chat_bots_delete.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/chat_bots_get.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/chat_bots_get.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/discuss_count.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/discuss_count.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/discuss_create.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/discuss_create.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/discuss_delete.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/discuss_delete.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/discuss_query.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/discuss_query.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/documents_count.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/documents_count.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/documents_delete.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/documents_delete.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/documents_ingest.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/documents_ingest.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/documents_search.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/documents_search.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/email_analysis.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/email_analysis.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/emotion_detection.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/emotion_detection.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/file_converter.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/file_converter.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/image_analysis.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/image_analysis.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/image_generation.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/image_generation.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/language_detection.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/language_detection.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/logical_error_detection.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/logical_error_detection.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/microlesson.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/microlesson.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/multiple_choice_qn_a_generator.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/multiple_choice_qn_a_generator.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/named_entity_recognition.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/named_entity_recognition.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/natural_s_q_l_generation.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/natural_s_q_l_generation.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/paraphrase.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/paraphrase.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/profanity.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/profanity.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/qna_generation.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/qna_generation.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/question_answering.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/question_answering.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/review_tagger.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/review_tagger.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/search_recommendations.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/search_recommendations.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/sentiment_analysis.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/service_io.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/service_io.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/simplify.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/simplify.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/string_similarity.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/string_similarity.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/summarization.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/summarization.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/table_delete.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/table_delete.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/table_generator.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/table_generator.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/table_get.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/table_get.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/table_ingest.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/table_ingest.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/tag.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/tag.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/transcript_correction.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/transcript_correction.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/translation.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/translation.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/common/serviceio_fields/website_converter.py` & `soffosai-0.2.2/soffosai/common/serviceio_fields/website_converter.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/pipelines/document_summary.py` & `soffosai-0.2.2/soffosai/core/pipelines/document_summary.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/pipelines/file_ingest.py` & `soffosai-0.2.2/soffosai/core/pipelines/file_ingest.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/pipelines/file_summary.py` & `soffosai-0.2.2/soffosai/core/pipelines/file_summary.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/pipelines/file_summary_ingest.py` & `soffosai-0.2.2/soffosai/core/pipelines/file_summary_ingest.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/pipelines/pipeline.py` & `soffosai-0.2.2/soffosai/core/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/__init__.py` & `soffosai-0.2.2/soffosai/core/services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 -----------------------------------------------------
 '''
 
 from .service import SoffosAIService, inspect_arguments
 from .input_config import InputConfig
 
 from .answer_scoring import AnswerScoringService
+from .assessment_generator import AssessmentGeneratorService
 from .audio_converter import AudioConverterService
 from .chat_bot_create import ChatBotCreateService
 from .chat_bot import ChatBotService
 from .chat_bots_get import ChatBotsGetService
 from .chat_bots_delete import ChatBotsDeleteService
 from .chat_bot_get_user_sessions import ChatBotGetUserSessionsService
 from .chat_bot_delete_user_sessions import ChatBotDeleteUserSessionsService
```

### Comparing `soffosai-0.2.1/soffosai/core/services/answer_scoring.py` & `soffosai-0.2.2/soffosai/core/services/answer_scoring.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/audio_converter.py` & `soffosai-0.2.2/soffosai/core/services/audio_converter.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/chat_bot.py` & `soffosai-0.2.2/soffosai/core/services/chat_bot.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/chat_bot_create.py` & `soffosai-0.2.2/soffosai/core/services/chat_bot_create.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/chat_bot_delete_user_sessions.py` & `soffosai-0.2.2/soffosai/core/services/chat_bot_delete_user_sessions.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/chat_bot_get_user_sessions.py` & `soffosai-0.2.2/soffosai/core/services/chat_bot_get_user_sessions.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/chat_bots_delete.py` & `soffosai-0.2.2/soffosai/core/services/chat_bots_delete.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/chat_bots_get.py` & `soffosai-0.2.2/soffosai/core/services/chat_bots_get.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/discuss_count.py` & `soffosai-0.2.2/soffosai/core/services/discuss_count.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/discuss_create.py` & `soffosai-0.2.2/soffosai/core/services/discuss_create.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/discuss_delete.py` & `soffosai-0.2.2/soffosai/core/services/discuss_delete.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/discuss_query.py` & `soffosai-0.2.2/soffosai/core/services/discuss_query.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/documents_count.py` & `soffosai-0.2.2/soffosai/core/services/documents_count.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/documents_delete.py` & `soffosai-0.2.2/soffosai/core/services/documents_delete.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/documents_ingest.py` & `soffosai-0.2.2/soffosai/core/services/documents_ingest.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/documents_search.py` & `soffosai-0.2.2/soffosai/core/services/documents_search.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/email_analysis.py` & `soffosai-0.2.2/soffosai/core/services/email_analysis.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/emotion_detection.py` & `soffosai-0.2.2/soffosai/core/services/emotion_detection.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/file_converter.py` & `soffosai-0.2.2/soffosai/core/services/file_converter.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/image_analysis.py` & `soffosai-0.2.2/soffosai/core/services/table_get.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,57 @@
 '''
 Copyright (c)2022 - Soffos.ai - All rights reserved
-Updated at: 2024-03-20
-Purpose: Easily use Image Analysis Service
+Updated at: 2024-03-03
+Purpose: Easily use Table Get Service
 -----------------------------------------------------
 '''
 from .service import SoffosAIService
 from .input_config import InputConfig
 from soffosai.common.constants import ServiceString
 from typing import Union
 
 
-class ImageAnalysisService(SoffosAIService):
+class TableGetService(SoffosAIService):
     '''
-    The base service for all Image Analyzation Services
-    ----------------------------------------------------------- 
-    Describes an image
+    General HTTP service client.
     '''
 
     def __init__(self, **kwargs) -> None:
-        service = ServiceString.IMAGE_ANALYSIS
+        service = ServiceString.TABLE_GET
         super().__init__(service, **kwargs)
     
-    def __call__(self, user:str, prompt:str, image_url:str, engine:str=None) -> dict:
+    def __call__(self, user:str, engine:str=None) -> dict:
         '''
-        Call the Image Analysis Service
+        Call the Table Get Service
         
         :param user: The ID of the user accessing the Soffos API.
             This string will be used for throttling and profanity tracking.
             Soffos assumes that the owner of the api is an application (app) and that app has users.
             Soffos API will accept any string."
-        :param prompt: the prompt to be sent to the LLM
-        :param image_url: the location of the image to be processed
-        :param engine: The LLM engine to be used. Currently supports:
-            ['gpt-4-1106-preview', 'gpt-3.5-turbo-1106', 'gemini-1.0-pro']
-        :return: analysis: the analysis of the image
+        :param engine: The LLM engine to be used.
+        :return: engine: The LLM engine used.
+        tables: None
         :Examples
-        Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/image_analysis.py>`_
+        Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/table_get.py>`_
         '''
-        return super().__call__(user=user, prompt=prompt, image_url=image_url, engine=engine)
+        return super().__call__(user=user, engine=engine)
 
-    def set_input_configs(self, name:str, prompt:Union[str, InputConfig], image_url:Union[str, InputConfig], engine:Union[str, InputConfig]=None):
-        super().set_input_configs(name=name, prompt=prompt, image_url=image_url, engine=engine)
+    def set_input_configs(self, name:str, engine:Union[str, InputConfig]=None):
+        super().set_input_configs(name=name, engine=engine)
 
     @classmethod
-    def call(self, user:str, prompt:str, image_url:str, engine:str=None) -> dict:
+    def call(self, user:str, engine:str=None) -> dict:
         '''
-        Call the Image Analysis Service
+        Call the Table Get Service
         
         :param user: The ID of the user accessing the Soffos API.
             This string will be used for throttling and profanity tracking.
             Soffos assumes that the owner of the api is an application (app) and that app has users.
             Soffos API will accept any string."
-        :param prompt: the prompt to be sent to the LLM
-        :param image_url: the location of the image to be processed
-        :param engine: The LLM engine to be used. Currently supports:
-            ['gpt-4-1106-preview', 'gpt-3.5-turbo-1106', 'gemini-1.0-pro']
-        :return: analysis: the analysis of the image
+        :param engine: The LLM engine to be used.
+        :return: engine: The LLM engine used.
+        tables: None
         :Examples
-        Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/image_analysis.py>`_
+        Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/table_get.py>`_
         '''
-        return super().call(user=user, prompt=prompt, image_url=image_url, engine=engine)
+        return super().call(user=user, engine=engine)
```

### Comparing `soffosai-0.2.1/soffosai/core/services/image_generation.py` & `soffosai-0.2.2/soffosai/core/services/image_generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,16 +27,15 @@
         Call the Image Generation Service
         
         :param user: The ID of the user accessing the Soffos API.
             This string will be used for throttling and profanity tracking.
             Soffos assumes that the owner of the api is an application (app) and that app has users.
             Soffos API will accept any string."
         :param prompt: the prompt to be sent to the LLM.
-        :param engine: The LLM engine to be used. Currently supports:
-            ['gpt-4-1106-preview', 'gpt-3.5-turbo-1106', 'gemini-1.0-pro']
+        :param engine: The LLM engine to be used.
         :param size: the required size of the image.
         :param quality: the quality of the image
         :param quantity: how many images should be created
         :return: image_urls: list of image URLs
         :Examples
         Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/image_generation.py>`_
         '''
@@ -51,16 +50,15 @@
         Call the Image Generation Service
         
         :param user: The ID of the user accessing the Soffos API.
             This string will be used for throttling and profanity tracking.
             Soffos assumes that the owner of the api is an application (app) and that app has users.
             Soffos API will accept any string."
         :param prompt: the prompt to be sent to the LLM.
-        :param engine: The LLM engine to be used. Currently supports:
-            ['gpt-4-1106-preview', 'gpt-3.5-turbo-1106', 'gemini-1.0-pro']
+        :param engine: The LLM engine to be used.
         :param size: the required size of the image.
         :param quality: the quality of the image
         :param quantity: how many images should be created
         :return: image_urls: list of image URLs
         :Examples
         Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/image_generation.py>`_
         '''
```

### Comparing `soffosai-0.2.1/soffosai/core/services/input_config.py` & `soffosai-0.2.2/soffosai/core/services/input_config.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/language_detection.py` & `soffosai-0.2.2/soffosai/core/services/language_detection.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/logical_error_detection.py` & `soffosai-0.2.2/soffosai/core/services/logical_error_detection.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/microlesson.py` & `soffosai-0.2.2/soffosai/core/services/microlesson.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/multiple_choice_qn_a_generator.py` & `soffosai-0.2.2/soffosai/core/services/multiple_choice_qn_a_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,16 +26,15 @@
         :param user: The ID of the user accessing the Soffos API.
             This string will be used for throttling and profanity tracking.
             Soffos assumes that the owner of the api is an application (app) and that app has users.
             Soffos API will accept any string."
         :param context: the prompt to be sent to the LLM
         :param num_questions: the location of the image to be processed
         :param num_choices: the location of the image to be processed
-        :param engine: The LLM engine to be used. Currently supports:
-            ['gpt-4-1106-preview', 'gpt-3.5-turbo-1106', 'gemini-1.0-pro']
+        :param engine: The LLM engine to be used.
         :return: qna_sets: The question and answer sets
         :Examples
         Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/multiple_choice_qn_a_generator.py>`_
         '''
         return super().__call__(user=user, context=context, num_questions=num_questions, num_choices=num_choices, engine=engine)
 
     def set_input_configs(self, name:str, context:Union[str, InputConfig], num_questions:Union[int, InputConfig], num_choices:Union[int, InputConfig], engine:Union[str, InputConfig]=None):
@@ -49,15 +48,14 @@
         :param user: The ID of the user accessing the Soffos API.
             This string will be used for throttling and profanity tracking.
             Soffos assumes that the owner of the api is an application (app) and that app has users.
             Soffos API will accept any string."
         :param context: the prompt to be sent to the LLM
         :param num_questions: the location of the image to be processed
         :param num_choices: the location of the image to be processed
-        :param engine: The LLM engine to be used. Currently supports:
-            ['gpt-4-1106-preview', 'gpt-3.5-turbo-1106', 'gemini-1.0-pro']
+        :param engine: The LLM engine to be used.
         :return: qna_sets: The question and answer sets
         :Examples
         Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/multiple_choice_qn_a_generator.py>`_
         '''
         return super().call(user=user, context=context, num_questions=num_questions, num_choices=num_choices, engine=engine)
```

### Comparing `soffosai-0.2.1/soffosai/core/services/named_entity_recognition.py` & `soffosai-0.2.2/soffosai/core/services/named_entity_recognition.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/natural_s_q_l_generation.py` & `soffosai-0.2.2/soffosai/core/services/natural_s_q_l_generation.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/paraphrase.py` & `soffosai-0.2.2/soffosai/core/services/paraphrase.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/profanity.py` & `soffosai-0.2.2/soffosai/core/services/profanity.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/qna_generation.py` & `soffosai-0.2.2/soffosai/core/services/qna_generation.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/question_answering.py` & `soffosai-0.2.2/soffosai/core/services/question_answering.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/review_tagger.py` & `soffosai-0.2.2/soffosai/core/services/review_tagger.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/search_recommendations.py` & `soffosai-0.2.2/soffosai/core/services/search_recommendations.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/sentiment_analysis.py` & `soffosai-0.2.2/soffosai/core/services/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/service.py` & `soffosai-0.2.2/soffosai/core/services/service.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/simplify.py` & `soffosai-0.2.2/soffosai/core/services/simplify.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/string_similarity.py` & `soffosai-0.2.2/soffosai/core/services/string_similarity.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/summarization.py` & `soffosai-0.2.2/soffosai/core/services/summarization.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/table_delete.py` & `soffosai-0.2.2/soffosai/core/services/table_delete.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/table_generator.py` & `soffosai-0.2.2/soffosai/core/services/table_generator.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/table_get.py` & `soffosai-0.2.2/soffosai/core/services/transcript_correction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 '''
 Copyright (c)2022 - Soffos.ai - All rights reserved
 Updated at: 2024-03-03
-Purpose: Easily use Table Get Service
+Purpose: Easily use Transcript Correction Service
 -----------------------------------------------------
 '''
 from .service import SoffosAIService
 from .input_config import InputConfig
 from soffosai.common.constants import ServiceString
 from typing import Union
 
 
-class TableGetService(SoffosAIService):
+class TranscriptCorrectionService(SoffosAIService):
     '''
-    General HTTP service client.
+    This module cleans up and corrects poorly transcribed text from Speech-To-Text
+    (STT) systems. It can handle cases where STT produced the wrong word or phrase
+    by taking into account the surrounding context and choosing the most fitting
+    replacement. Although this is meant for correcting STT outpus, it can also be
+    used to correct grammar, misspellings and syntactical errors.
     '''
 
     def __init__(self, **kwargs) -> None:
-        service = ServiceString.TABLE_GET
+        service = ServiceString.TRANSCRIPT_CORRECTION
         super().__init__(service, **kwargs)
     
-    def __call__(self, user:str, engine:str=None) -> dict:
+    def __call__(self, user:str, text:str, engine:str=None) -> dict:
         '''
-        Call the Table Get Service
+        Call the Transcript Correction Service
         
         :param user: The ID of the user accessing the Soffos API.
             This string will be used for throttling and profanity tracking.
             Soffos assumes that the owner of the api is an application (app) and that app has users.
             Soffos API will accept any string."
+        :param text: Text to be corrected.
         :param engine: The LLM engine to be used.
         :return: engine: The LLM engine used.
-        tables: None
+        corrected: Corrected text.
         :Examples
-        Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/table_get.py>`_
+        Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/transcript_correction.py>`_
         '''
-        return super().__call__(user=user, engine=engine)
+        return super().__call__(user=user, text=text, engine=engine)
 
-    def set_input_configs(self, name:str, engine:Union[str, InputConfig]=None):
-        super().set_input_configs(name=name, engine=engine)
+    def set_input_configs(self, name:str, text:Union[str, InputConfig], engine:Union[str, InputConfig]=None):
+        super().set_input_configs(name=name, text=text, engine=engine)
 
     @classmethod
-    def call(self, user:str, engine:str=None) -> dict:
+    def call(self, user:str, text:str, engine:str=None) -> dict:
         '''
-        Call the Table Get Service
+        Call the Transcript Correction Service
         
         :param user: The ID of the user accessing the Soffos API.
             This string will be used for throttling and profanity tracking.
             Soffos assumes that the owner of the api is an application (app) and that app has users.
             Soffos API will accept any string."
+        :param text: Text to be corrected.
         :param engine: The LLM engine to be used.
         :return: engine: The LLM engine used.
-        tables: None
+        corrected: Corrected text.
         :Examples
-        Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/table_get.py>`_
+        Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/transcript_correction.py>`_
         '''
-        return super().call(user=user, engine=engine)
+        return super().call(user=user, text=text, engine=engine)
```

### Comparing `soffosai-0.2.1/soffosai/core/services/table_ingest.py` & `soffosai-0.2.2/soffosai/core/services/table_ingest.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/tag.py` & `soffosai-0.2.2/soffosai/core/services/tag.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai/core/services/transcript_correction.py` & `soffosai-0.2.2/soffosai/core/services/website_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 '''
 Copyright (c)2022 - Soffos.ai - All rights reserved
 Updated at: 2024-03-03
-Purpose: Easily use Transcript Correction Service
+Purpose: Easily use Website Converter Service
 -----------------------------------------------------
 '''
 from .service import SoffosAIService
 from .input_config import InputConfig
 from soffosai.common.constants import ServiceString
 from typing import Union
 
 
-class TranscriptCorrectionService(SoffosAIService):
+class WebsiteConverterService(SoffosAIService):
     '''
-    This module cleans up and corrects poorly transcribed text from Speech-To-Text
-    (STT) systems. It can handle cases where STT produced the wrong word or phrase
-    by taking into account the surrounding context and choosing the most fitting
-    replacement. Although this is meant for correcting STT outpus, it can also be
-    used to correct grammar, misspellings and syntactical errors.
+    The Website Converter module offers basic functionality for extracting
+    meaningful text from websites. This can be a useful tool for processing website
+    content with other modules. Note: Character volume is not charged for this
+    module.
     '''
 
     def __init__(self, **kwargs) -> None:
-        service = ServiceString.TRANSCRIPT_CORRECTION
+        service = ServiceString.WEBSITE_CONVERTER
         super().__init__(service, **kwargs)
     
-    def __call__(self, user:str, text:str, engine:str=None) -> dict:
+    def __call__(self, user:str, url:str, engine:str=None) -> dict:
         '''
-        Call the Transcript Correction Service
+        Call the Website Converter Service
         
         :param user: The ID of the user accessing the Soffos API.
             This string will be used for throttling and profanity tracking.
             Soffos assumes that the owner of the api is an application (app) and that app has users.
             Soffos API will accept any string."
-        :param text: Text to be corrected.
+        :param url: The url to extract text from.
         :param engine: The LLM engine to be used.
         :return: engine: The LLM engine used.
-        corrected: Corrected text.
+        text: Raw text extracted from the website.
+        links: A dictionary containing a list of `internal` and a list of
+            `external` links found on the website. `internal`: Links found
+            on the page that are under the same domain as the provided url.
+            `external`: Links found on the page that belong to different
+            domains.
         :Examples
-        Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/transcript_correction.py>`_
+        Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/website_converter.py>`_
         '''
-        return super().__call__(user=user, text=text, engine=engine)
+        return super().__call__(user=user, url=url, engine=engine)
 
-    def set_input_configs(self, name:str, text:Union[str, InputConfig], engine:Union[str, InputConfig]=None):
-        super().set_input_configs(name=name, text=text, engine=engine)
+    def set_input_configs(self, name:str, url:Union[str, InputConfig], engine:Union[str, InputConfig]=None):
+        super().set_input_configs(name=name, url=url, engine=engine)
 
     @classmethod
-    def call(self, user:str, text:str, engine:str=None) -> dict:
+    def call(self, user:str, url:str, engine:str=None) -> dict:
         '''
-        Call the Transcript Correction Service
+        Call the Website Converter Service
         
         :param user: The ID of the user accessing the Soffos API.
             This string will be used for throttling and profanity tracking.
             Soffos assumes that the owner of the api is an application (app) and that app has users.
             Soffos API will accept any string."
-        :param text: Text to be corrected.
+        :param url: The url to extract text from.
         :param engine: The LLM engine to be used.
         :return: engine: The LLM engine used.
-        corrected: Corrected text.
+        text: Raw text extracted from the website.
+        links: A dictionary containing a list of `internal` and a list of
+            `external` links found on the website. `internal`: Links found
+            on the page that are under the same domain as the provided url.
+            `external`: Links found on the page that belong to different
+            domains.
         :Examples
-        Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/transcript_correction.py>`_
+        Detailed examples can be found at `Soffos Github Repository <https://github.com/Soffos-Inc/soffosai-python/tree/master/samples/services/website_converter.py>`_
         '''
-        return super().call(user=user, text=text, engine=engine)
+        return super().call(user=user, url=url, engine=engine)
```

### Comparing `soffosai-0.2.1/soffosai/core/services/translation.py` & `soffosai-0.2.2/soffosai/core/services/translation.py`

 * *Files identical despite different names*

### Comparing `soffosai-0.2.1/soffosai.egg-info/PKG-INFO` & `soffosai-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: soffosai
-Version: 0.2.1
-Summary: Python SDK for Soffos AI
-Author: Soffosai
-Author-email: "Soffos.ai" <Soffos@Soffos.ai>, Franco Such <franco.such@Soffos.ai>, Andreas Christofi <andreas.christofi@Soffos.ai>
-Project-URL: Homepage, https://github.com/Soffos-Inc/soffos_ai
-Project-URL: Bug Tracker, https://github.com/Soffos-Inc/soffos_ai/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-
 # Welcome to the Soffos Platform SDK
 At Soffos Inc., our specialty is helping organizations create pioneering apps with conversational artificial intelligence (CAI) and natural language processing (NLP) at their core.
 
 NLP and conversational AI are at the heart of everything Soffos does. Using Soffos’ technology, we offer a suite of unique application programming interfaces (APIs) so businesses can choose the natural language and generative AI functionalities they would like to include in any kind of application.
 
 What sets Soffos apart is we’ve taken the most advanced technology, enhanced it with our own R&D, and made it easy to use and accessible to everyone.
 
@@ -53,14 +37,15 @@
 
 ## SoffosAIService
 The SoffosAIService class handles validation and execution of specified endpoint vs payload.
 Here is the list of SoffosAIService Subclasses:
 ```
 [
     "AnswerScoringService",
+    "AssessmentGeneratorService"
     "AudioConverterService",
     "ChatBotCreateService",
     "ChatBotDeleteUserSessionsService",
     "ChatBotGetUserSessionsService",
     "ChatBotsDeleteService",
     "ChatBotService",
     "ChatBotsGetService",
@@ -70,15 +55,18 @@
     "DiscussDeleteService",
     "DocumentsCountService",
     "DocumentsIngestService", 
     "DocumentsSearchService", 
     "DocumentsDeleteService", 
     "EmailAnalysisService",
     "FileConverterService",
+    "ImageAnalysisService",
+    "ImageGenerationService",
     "MicrolessonService",
+    "MultipleChoiceQnAGeneratorService",
     "NERService",
     "NaturalSQLGenerationService",
     "ParaphraseService",
     "QnAGenerationService",
     "SearchRecommendationsService",
     "SentimentAnalysisService",
     "SimplifyService",
@@ -378,8 +366,8 @@
         super().__init__(services, **kwargs)
 
 
     def __call__(self, user, file, sent_length, question):
         return super().__call__(user=user, file=file, sent_length=sent_length, question=question)
 ```
 
-Copyright (c)2023 - Soffos.ai - All rights reserved
+Copyright (c)2023 - Soffos.ai - All rights reserved
```

### Comparing `soffosai-0.2.1/soffosai.egg-info/SOURCES.txt` & `soffosai-0.2.2/soffosai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 soffosai/client/__init__.py
 soffosai/client/ai_response.py
 soffosai/common/__init__.py
 soffosai/common/constants.py
 soffosai/common/service_io_map.py
 soffosai/common/serviceio_fields/__init__.py
 soffosai/common/serviceio_fields/answer_scoring.py
+soffosai/common/serviceio_fields/assessment_generator.py
 soffosai/common/serviceio_fields/audio_converter.py
 soffosai/common/serviceio_fields/chat_bot.py
 soffosai/common/serviceio_fields/chat_bot_create.py
 soffosai/common/serviceio_fields/chat_bot_delete_user_sessions.py
 soffosai/common/serviceio_fields/chat_bot_get_user_sessions.py
 soffosai/common/serviceio_fields/chat_bots_delete.py
 soffosai/common/serviceio_fields/chat_bots_get.py
@@ -65,14 +66,15 @@
 soffosai/core/pipelines/document_summary.py
 soffosai/core/pipelines/file_ingest.py
 soffosai/core/pipelines/file_summary.py
 soffosai/core/pipelines/file_summary_ingest.py
 soffosai/core/pipelines/pipeline.py
 soffosai/core/services/__init__.py
 soffosai/core/services/answer_scoring.py
+soffosai/core/services/assessment_generator.py
 soffosai/core/services/audio_converter.py
 soffosai/core/services/chat_bot.py
 soffosai/core/services/chat_bot_create.py
 soffosai/core/services/chat_bot_delete_user_sessions.py
 soffosai/core/services/chat_bot_get_user_sessions.py
 soffosai/core/services/chat_bots_delete.py
 soffosai/core/services/chat_bots_get.py
```

