# Comparing `tmp/notdiamond_openai-0.1.2.tar.gz` & `tmp/notdiamond_openai-0.1.3.tar.gz`

## Comparing `notdiamond_openai-0.1.2.tar` & `notdiamond_openai-0.1.3.tar`

### file list

```diff
@@ -1,237 +1,237 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/__init__.py
--rw-r--r--   0        0        0     9372 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/__main__.py
--rw-r--r--   0        0        0    63372 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_base_client.py
--rw-r--r--   0        0        0    20780 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_compat.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_constants.py
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_exceptions.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_files.py
--rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_legacy_response.py
--rw-r--r--   0        0        0    22361 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_models.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_module_client.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_qs.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_resource.py
--rw-r--r--   0        0        0    28577 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_response.py
--rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_streaming.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_types.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_version.py
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/py.typed
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/version.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_extras/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_extras/_common.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_extras/numpy_proxy.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_extras/pandas_proxy.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_utils/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_utils/_logs.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_utils/_typing.py
--rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/_utils/_utils.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/__init__.py
--rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_cli.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_errors.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_models.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_progress.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_utils.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_api/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_api/_main.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_api/audio.py
--rw-r--r--   0        0        0     6412 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_api/completions.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_api/files.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_api/image.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_api/models.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_api/chat/__init__.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_api/chat/completions.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_tools/__init__.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_tools/_main.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_tools/fine_tunes.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/cli/_tools/migrate.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/lib/.keep
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/lib/_old_api.py
--rw-r--r--   0        0        0    35189 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/lib/_validators.py
--rw-r--r--   0        0        0    21021 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/lib/azure.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/lib/notdiamond/model_select.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/lib/streaming/__init__.py
--rw-r--r--   0        0        0    40467 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/lib/streaming/_assistants.py
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/__init__.py
--rw-r--r--   0        0        0    57139 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/completions.py
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/embeddings.py
--rw-r--r--   0        0        0    26089 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/files.py
--rw-r--r--   0        0        0    24782 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/images.py
--rw-r--r--   0        0        0    10183 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/models.py
--rw-r--r--   0        0        0     6639 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/moderations.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/audio/__init__.py
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/audio/audio.py
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/audio/speech.py
--rw-r--r--   0        0        0    11088 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/audio/transcriptions.py
--rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/audio/translations.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/beta/__init__.py
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/beta/beta.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/beta/assistants/__init__.py
--rw-r--r--   0        0        0    30704 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/beta/assistants/assistants.py
--rw-r--r--   0        0        0    19513 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/beta/assistants/files.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/beta/threads/__init__.py
--rw-r--r--   0        0        0    48295 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/beta/threads/threads.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/beta/threads/messages/__init__.py
--rw-r--r--   0        0        0    12300 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/beta/threads/messages/files.py
--rw-r--r--   0        0        0    22804 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/beta/threads/messages/messages.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/beta/threads/runs/__init__.py
--rw-r--r--   0        0        0    73259 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/beta/threads/runs/runs.py
--rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/beta/threads/runs/steps.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/chat/__init__.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/chat/chat.py
--rw-r--r--   0        0        0    72380 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/chat/completions.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/fine_tuning/__init__.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/fine_tuning/fine_tuning.py
--rw-r--r--   0        0        0    24536 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/resources/fine_tuning/jobs.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/__init__.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/completion.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/completion_choice.py
--rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/completion_create_params.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/completion_usage.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/create_embedding_response.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/embedding.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/embedding_create_params.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/file_content.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/file_create_params.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/file_deleted.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/file_list_params.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/file_object.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/image.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/image_create_variation_params.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/image_edit_params.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/image_generate_params.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/images_response.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/model.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/model_deleted.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/moderation.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/moderation_create_params.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/moderation_create_response.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/audio/__init__.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/audio/speech_create_params.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/audio/transcription.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/audio/transcription_create_params.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/audio/translation.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/audio/translation_create_params.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/__init__.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/assistant.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/assistant_create_params.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/assistant_deleted.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/assistant_list_params.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/assistant_stream_event.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/assistant_tool.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/assistant_tool_param.py
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/assistant_update_params.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/code_interpreter_tool.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/code_interpreter_tool_param.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/function_tool.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/function_tool_param.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/retrieval_tool.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/retrieval_tool_param.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/thread.py
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/thread_create_and_run_params.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/thread_create_params.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/thread_deleted.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/thread_update_params.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/assistants/__init__.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/assistants/assistant_file.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/assistants/file_create_params.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/assistants/file_delete_response.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/assistants/file_list_params.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/chat/__init__.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/__init__.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/annotation.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/annotation_delta.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/file_citation_annotation.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/file_citation_delta_annotation.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/file_path_annotation.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/file_path_delta_annotation.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/image_file.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/image_file_content_block.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/image_file_delta.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/image_file_delta_block.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/message.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/message_content.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/message_content_delta.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/message_create_params.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/message_delta.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/message_delta_event.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/message_list_params.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/message_update_params.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/required_action_function_tool_call.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/run.py
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/run_create_params.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/run_list_params.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/run_status.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/run_submit_tool_outputs_params.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/run_update_params.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/text.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/text_content_block.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/text_delta.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/text_delta_block.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/messages/__init__.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/messages/file_list_params.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/messages/message_file.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/__init__.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/code_interpreter_logs.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/code_interpreter_output_image.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/code_interpreter_tool_call.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/code_interpreter_tool_call_delta.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/function_tool_call.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/function_tool_call_delta.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/message_creation_step_details.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/retrieval_tool_call.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/retrieval_tool_call_delta.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/run_step.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/run_step_delta.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/run_step_delta_event.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/run_step_delta_message_delta.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/step_list_params.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/tool_call.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/tool_call_delta.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/tool_call_delta_object.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/tool_calls_step_details.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/__init__.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_assistant_message_param.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_chunk.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_content_part_image_param.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_content_part_param.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_content_part_text_param.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_function_call_option_param.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_function_message_param.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_message.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_message_param.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_message_tool_call.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_message_tool_call_param.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_named_tool_choice_param.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_role.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_system_message_param.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_token_logprob.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_tool_choice_option_param.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_tool_message_param.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_tool_param.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_user_message_param.py
--rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/chat/completion_create_params.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/fine_tuning/__init__.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/fine_tuning/fine_tuning_job.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/fine_tuning/fine_tuning_job_event.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/fine_tuning/job_create_params.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/fine_tuning/job_list_events_params.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/fine_tuning/job_list_params.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/shared/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/shared/error_object.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/shared/function_definition.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/shared/function_parameters.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/shared_params/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/shared_params/function_definition.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/src/openai/types/shared_params/function_parameters.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/.gitignore
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/LICENSE
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/README.md
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/__init__.py
+-rw-r--r--   0        0        0     9372 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/__main__.py
+-rw-r--r--   0        0        0    63372 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_base_client.py
+-rw-r--r--   0        0        0    20780 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_compat.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_constants.py
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_exceptions.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_files.py
+-rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_legacy_response.py
+-rw-r--r--   0        0        0    22361 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_models.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_module_client.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_qs.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_resource.py
+-rw-r--r--   0        0        0    28577 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_response.py
+-rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_streaming.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_types.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_version.py
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/py.typed
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/version.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_extras/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_extras/_common.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_extras/numpy_proxy.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_extras/pandas_proxy.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_utils/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_utils/_logs.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_utils/_typing.py
+-rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/_utils/_utils.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/__init__.py
+-rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_cli.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_errors.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_models.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_progress.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_utils.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_api/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_api/_main.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_api/audio.py
+-rw-r--r--   0        0        0     6412 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_api/completions.py
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_api/files.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_api/image.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_api/models.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_api/chat/__init__.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_api/chat/completions.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_tools/__init__.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_tools/_main.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_tools/fine_tunes.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_tools/migrate.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/lib/.keep
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/lib/_old_api.py
+-rw-r--r--   0        0        0    35189 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/lib/_validators.py
+-rw-r--r--   0        0        0    21021 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/lib/azure.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/lib/notdiamond/model_select.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/lib/streaming/__init__.py
+-rw-r--r--   0        0        0    40467 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/lib/streaming/_assistants.py
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/__init__.py
+-rw-r--r--   0        0        0    57139 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/completions.py
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/embeddings.py
+-rw-r--r--   0        0        0    26089 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/files.py
+-rw-r--r--   0        0        0    24782 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/images.py
+-rw-r--r--   0        0        0    10183 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/models.py
+-rw-r--r--   0        0        0     6639 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/moderations.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/audio/__init__.py
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/audio/audio.py
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/audio/speech.py
+-rw-r--r--   0        0        0    11088 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/audio/transcriptions.py
+-rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/audio/translations.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/__init__.py
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/beta.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/assistants/__init__.py
+-rw-r--r--   0        0        0    30704 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/assistants/assistants.py
+-rw-r--r--   0        0        0    19513 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/assistants/files.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/__init__.py
+-rw-r--r--   0        0        0    48295 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/threads.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/messages/__init__.py
+-rw-r--r--   0        0        0    12300 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/messages/files.py
+-rw-r--r--   0        0        0    22804 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/messages/messages.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/runs/__init__.py
+-rw-r--r--   0        0        0    73259 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/runs/runs.py
+-rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/runs/steps.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/chat/chat.py
+-rw-r--r--   0        0        0    72380 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/chat/completions.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/fine_tuning/__init__.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/fine_tuning/fine_tuning.py
+-rw-r--r--   0        0        0    24536 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/resources/fine_tuning/jobs.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/__init__.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/completion.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/completion_choice.py
+-rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/completion_create_params.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/completion_usage.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/create_embedding_response.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/embedding.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/embedding_create_params.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/file_content.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/file_create_params.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/file_deleted.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/file_list_params.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/file_object.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/image.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/image_create_variation_params.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/image_edit_params.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/image_generate_params.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/images_response.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/model.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/model_deleted.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/moderation.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/moderation_create_params.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/moderation_create_response.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/audio/__init__.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/audio/speech_create_params.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/audio/transcription.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/audio/transcription_create_params.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/audio/translation.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/audio/translation_create_params.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/__init__.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistant.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistant_create_params.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistant_deleted.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistant_list_params.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistant_stream_event.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistant_tool.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistant_tool_param.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistant_update_params.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/code_interpreter_tool.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/code_interpreter_tool_param.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/function_tool.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/function_tool_param.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/retrieval_tool.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/retrieval_tool_param.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/thread.py
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/thread_create_and_run_params.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/thread_create_params.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/thread_deleted.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/thread_update_params.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistants/__init__.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistants/assistant_file.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistants/file_create_params.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistants/file_delete_response.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistants/file_list_params.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/chat/__init__.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/__init__.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/annotation.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/annotation_delta.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/file_citation_annotation.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/file_citation_delta_annotation.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/file_path_annotation.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/file_path_delta_annotation.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/image_file.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/image_file_content_block.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/image_file_delta.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/image_file_delta_block.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/message.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/message_content.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/message_content_delta.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/message_create_params.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/message_delta.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/message_delta_event.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/message_list_params.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/message_update_params.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/required_action_function_tool_call.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/run.py
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/run_create_params.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/run_list_params.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/run_status.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/run_submit_tool_outputs_params.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/run_update_params.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/text.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/text_content_block.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/text_delta.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/text_delta_block.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/messages/__init__.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/messages/file_list_params.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/messages/message_file.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/__init__.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/code_interpreter_logs.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/code_interpreter_output_image.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/code_interpreter_tool_call.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/code_interpreter_tool_call_delta.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/function_tool_call.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/function_tool_call_delta.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/message_creation_step_details.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/retrieval_tool_call.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/retrieval_tool_call_delta.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/run_step.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/run_step_delta.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/run_step_delta_event.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/run_step_delta_message_delta.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/step_list_params.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/tool_call.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/tool_call_delta.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/tool_call_delta_object.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/tool_calls_step_details.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/__init__.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_assistant_message_param.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_chunk.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_content_part_image_param.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_content_part_param.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_content_part_text_param.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_function_call_option_param.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_function_message_param.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_message.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_message_param.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_message_tool_call.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_message_tool_call_param.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_named_tool_choice_param.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_role.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_system_message_param.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_token_logprob.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_tool_choice_option_param.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_tool_message_param.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_tool_param.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_user_message_param.py
+-rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/completion_create_params.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/fine_tuning/__init__.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/fine_tuning/fine_tuning_job.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/fine_tuning/fine_tuning_job_event.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/fine_tuning/job_create_params.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/fine_tuning/job_list_events_params.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/fine_tuning/job_list_params.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/shared/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/shared/error_object.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/shared/function_definition.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/shared/function_parameters.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/shared_params/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/shared_params/function_definition.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/src/notdiamond_openai/types/shared_params/function_parameters.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/.gitignore
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/README.md
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 notdiamond_openai-0.1.3/PKG-INFO
```

### Comparing `notdiamond_openai-0.1.2/src/openai/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_base_client.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_base_client.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_client.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_client.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_compat.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_compat.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_exceptions.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_exceptions.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_files.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_files.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_legacy_response.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_legacy_response.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_models.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_models.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_module_client.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_module_client.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_qs.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_qs.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_resource.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_resource.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_response.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_response.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_streaming.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_streaming.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_types.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_types.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/pagination.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/pagination.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_extras/numpy_proxy.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_extras/numpy_proxy.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_extras/pandas_proxy.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_extras/pandas_proxy.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_utils/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_utils/_logs.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_utils/_proxy.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_utils/_sync.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_utils/_transform.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_utils/_typing.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/_utils/_utils.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/cli/_cli.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_cli.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/cli/_progress.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_progress.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/cli/_utils.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/cli/_api/audio.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_api/audio.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/cli/_api/completions.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_api/completions.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/cli/_api/files.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_api/files.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/cli/_api/image.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_api/image.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/cli/_api/models.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_api/models.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/cli/_api/chat/completions.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_api/chat/completions.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/cli/_tools/fine_tunes.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_tools/fine_tunes.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/cli/_tools/migrate.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/cli/_tools/migrate.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/lib/_old_api.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/lib/_old_api.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/lib/_validators.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/lib/_validators.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/lib/azure.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/lib/azure.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/lib/notdiamond/model_select.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/lib/notdiamond/model_select.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/lib/streaming/_assistants.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/lib/streaming/_assistants.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/completions.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/completions.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/embeddings.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/embeddings.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/files.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/files.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/images.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/images.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/models.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/models.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/moderations.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/moderations.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/audio/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/audio/audio.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/audio/audio.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/audio/speech.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/audio/speech.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/audio/transcriptions.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/audio/transcriptions.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/audio/translations.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/audio/translations.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/beta/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/beta/beta.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/beta.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/beta/assistants/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/assistants/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/beta/assistants/assistants.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/assistants/assistants.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/beta/assistants/files.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/assistants/files.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/beta/threads/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/beta/threads/threads.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/threads.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/beta/threads/messages/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/beta/threads/messages/files.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/messages/files.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/beta/threads/messages/messages.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/messages/messages.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/beta/threads/runs/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/beta/threads/runs/runs.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/runs/runs.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/beta/threads/runs/steps.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/beta/threads/runs/steps.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/chat/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/chat/chat.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/chat/completions.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/chat/completions.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/fine_tuning/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/fine_tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/fine_tuning/fine_tuning.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/fine_tuning/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/resources/fine_tuning/jobs.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/resources/fine_tuning/jobs.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/completion.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/completion.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/completion_choice.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/completion_choice.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/completion_create_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/create_embedding_response.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/create_embedding_response.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/embedding.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/embedding.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/embedding_create_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/embedding_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/file_create_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/file_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/file_object.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/file_object.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/image.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/image.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/image_create_variation_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/image_create_variation_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/image_edit_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/image_edit_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/image_generate_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/image_generate_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/model.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/model.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/moderation.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/moderation.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/moderation_create_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/moderation_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/audio/speech_create_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/audio/speech_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/audio/transcription_create_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/audio/transcription_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/audio/translation_create_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/audio/translation_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/assistant.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistant.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/assistant_create_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistant_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/assistant_list_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistant_list_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/assistant_stream_event.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistant_stream_event.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/assistant_update_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistant_update_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/thread.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/thread.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/thread_create_and_run_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/thread_create_and_run_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/thread_create_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/thread_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/thread_update_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/thread_update_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/assistants/assistant_file.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistants/assistant_file.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/assistants/file_create_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistants/file_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/assistants/file_list_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/assistants/file_list_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/file_citation_annotation.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/file_citation_annotation.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/file_citation_delta_annotation.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/file_citation_delta_annotation.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/file_path_annotation.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/file_path_annotation.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/file_path_delta_annotation.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/file_path_delta_annotation.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/message.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/message.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/message_create_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/message_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/message_delta.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/message_delta.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/message_delta_event.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/message_delta_event.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/message_list_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/message_list_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/message_update_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/message_update_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/required_action_function_tool_call.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/required_action_function_tool_call.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/run.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/run.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/run_create_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/run_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/run_list_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/run_list_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/run_submit_tool_outputs_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/run_submit_tool_outputs_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/run_update_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/run_update_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/messages/file_list_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/messages/file_list_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/messages/message_file.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/messages/message_file.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/code_interpreter_output_image.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/code_interpreter_output_image.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/code_interpreter_tool_call.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/code_interpreter_tool_call.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/code_interpreter_tool_call_delta.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/code_interpreter_tool_call_delta.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/function_tool_call.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/function_tool_call.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/function_tool_call_delta.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/function_tool_call_delta.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/retrieval_tool_call.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/retrieval_tool_call.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/retrieval_tool_call_delta.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/retrieval_tool_call_delta.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/run_step.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/run_step.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/run_step_delta.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/run_step_delta.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/run_step_delta_event.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/run_step_delta_event.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/run_step_delta_message_delta.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/run_step_delta_message_delta.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/step_list_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/step_list_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/tool_call_delta.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/tool_call_delta.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/tool_call_delta_object.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/tool_call_delta_object.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/beta/threads/runs/tool_calls_step_details.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/beta/threads/runs/tool_calls_step_details.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/__init__.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_assistant_message_param.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_assistant_message_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_chunk.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_content_part_image_param.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_content_part_image_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_function_message_param.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_function_message_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_message.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_message.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_message_param.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_message_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_message_tool_call.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_message_tool_call.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_message_tool_call_param.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_message_tool_call_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_named_tool_choice_param.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_named_tool_choice_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_system_message_param.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_system_message_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_token_logprob.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_token_logprob.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_tool_message_param.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_tool_message_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/chat_completion_user_message_param.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/chat_completion_user_message_param.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/chat/completion_create_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/chat/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/fine_tuning/fine_tuning_job.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/fine_tuning/fine_tuning_job.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/fine_tuning/job_create_params.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/fine_tuning/job_create_params.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/shared/function_definition.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/shared/function_definition.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/src/openai/types/shared_params/function_definition.py` & `notdiamond_openai-0.1.3/src/notdiamond_openai/types/shared_params/function_definition.py`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/LICENSE` & `notdiamond_openai-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/README.md` & `notdiamond_openai-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `notdiamond_openai-0.1.2/pyproject.toml` & `notdiamond_openai-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "notdiamond-openai"
-version = "0.1.2"
+version = "0.1.3"
 description = "NotDiamond Python library for easy OpenAI integration."
 readme = "README.md"
 license = "Apache-2.0"
 authors = [
 { name = "NotDiamond", email = "t7@notdiamond.ai" },
 ]
 dependencies = [
```

### Comparing `notdiamond_openai-0.1.2/PKG-INFO` & `notdiamond_openai-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: notdiamond-openai
-Version: 0.1.2
+Version: 0.1.3
 Summary: NotDiamond Python library for easy OpenAI integration.
 Project-URL: Homepage, https://notdiamond.ai/
 Project-URL: Repository, https://github.com/Not-Diamond/openai-python
 Author-email: NotDiamond <t7@notdiamond.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

