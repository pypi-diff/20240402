# Comparing `tmp/metagpt-0.7.7.tar.gz` & `tmp/metagpt-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metagpt-0.7.7.tar", last modified: Fri Mar 29 04:02:23 2024, max compression
+gzip compressed data, was "metagpt-0.8.0.tar", last modified: Fri Mar 29 12:19:04 2024, max compression
```

## Comparing `metagpt-0.7.7.tar` & `metagpt-0.8.0.tar`

### file list

```diff
@@ -1,277 +1,385 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.602405 metagpt-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-29 04:00:53.000000 metagpt-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-03-29 04:02:23.602405 metagpt-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-03-29 04:00:53.000000 metagpt-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.558405 metagpt-0.7.7/metagpt/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.566404 metagpt-0.7.7/metagpt/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/action_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    27537 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/action_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/action_outcls_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/action_output.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/add_requirement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/debug_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/design_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/design_api_an.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/design_api_review.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.566404 metagpt-0.7.7/metagpt/actions/di/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/di/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/di/ask_review.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/di/debug_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/di/execute_nb_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/di/ml_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/di/write_analysis_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/di/write_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/execute_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/fix_bug.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/generate_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/invoice_ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/prepare_documents.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/prepare_interview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/project_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/project_management_an.py
--rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/rebuild_class_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/rebuild_sequence_view.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/rebuild_sequence_view_an.py
--rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/research.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/run_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/search_and_summarize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/skill_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/summarize_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/talk_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/write_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    18013 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/write_code_an_draft.py
--rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/write_code_plan_and_change_an.py
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/write_code_review.py
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/write_docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/write_prd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/write_prd_an.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/write_prd_review.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/write_review.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/write_teaching_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/write_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/actions/write_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/config2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.570405 metagpt-0.7.7/metagpt/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/configs/browser_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/configs/llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/configs/mermaid_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/configs/redis_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/configs/s3_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/configs/search_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/configs/workspace_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/context_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8170 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.570405 metagpt-0.7.7/metagpt/document_store/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/document_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/document_store/base_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/document_store/chromadb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/document_store/faiss_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/document_store/lancedb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/document_store/qdrant_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.570405 metagpt-0.7.7/metagpt/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.570405 metagpt-0.7.7/metagpt/environment/android_env/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/android_env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/android_env/android_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/android_env/android_ext_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/android_env/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.570405 metagpt-0.7.7/metagpt/environment/api/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/api/env_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/base_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.570405 metagpt-0.7.7/metagpt/environment/mincraft_env/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/mincraft_env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/mincraft_env/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    16366 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/mincraft_env/mincraft_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/mincraft_env/mincraft_ext_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/mincraft_env/process_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.574405 metagpt-0.7.7/metagpt/environment/software_env/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/software_env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/software_env/software_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.574405 metagpt-0.7.7/metagpt/environment/stanford_town_env/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/stanford_town_env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/stanford_town_env/stanford_town_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    14873 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/stanford_town_env/stanford_town_ext_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.574405 metagpt-0.7.7/metagpt/environment/werewolf_env/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/werewolf_env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/werewolf_env/werewolf_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    14833 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/environment/werewolf_env/werewolf_ext_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.574405 metagpt-0.7.7/metagpt/learn/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/learn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/learn/google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/learn/skill_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/learn/text_to_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/learn/text_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/learn/text_to_speech.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.574405 metagpt-0.7.7/metagpt/management/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/management/skill_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.574405 metagpt-0.7.7/metagpt/memory/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/memory/brain_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/memory/longterm_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/memory/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/memory/memory_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.578405 metagpt-0.7.7/metagpt/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/prompts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.578405 metagpt-0.7.7/metagpt/prompts/di/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/prompts/di/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/prompts/di/ml_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/prompts/di/write_analysis_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/prompts/invoice_ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/prompts/metagpt_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/prompts/sales.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/prompts/summarize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/prompts/tool_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/prompts/tutorial_assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.582404 metagpt-0.7.7/metagpt/provider/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/anthropic_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/azure_openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/base_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/fireworks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    19443 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/general_api_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/general_api_requestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/google_gemini_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/human_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/llm_provider_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/metagpt_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/ollama_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/open_llm_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/openai_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.582404 metagpt-0.7.7/metagpt/provider/postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/postprocess/base_postprocess_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/postprocess/llm_output_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/spark_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.582404 metagpt-0.7.7/metagpt/provider/zhipuai/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/zhipuai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/zhipuai/async_sse_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/zhipuai/zhipu_model_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/provider/zhipuai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15669 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/repo_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.586405 metagpt-0.7.7/metagpt/roles/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/architect.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/customer_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.586405 metagpt-0.7.7/metagpt/roles/di/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/di/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/di/data_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/di/ml_engineer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16607 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/engineer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/invoice_ocr_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/product_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/project_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/qa_engineer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/researcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    25043 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/sales.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/sk_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/teacher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/roles/tutorial_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)    24930 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/software_company.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.586405 metagpt-0.7.7/metagpt/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/strategy/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/strategy/planner.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/strategy/search_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/strategy/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10017 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/strategy/tot.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/strategy/tot_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/team.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.594405 metagpt-0.7.7/metagpt/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/azure_tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/iflytek_tts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.594405 metagpt-0.7.7/metagpt/tools/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/libs/data_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/libs/email_login.py
--rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/libs/feature_engineering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/libs/gpt_v_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/libs/sd_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/libs/web_scraping.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/metagpt_oas3_api_svc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/metagpt_text_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/moderation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/openai_text_to_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/openai_text_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/openapi_v3_hello.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/prompt_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/search_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/search_engine_ddg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/search_engine_googleapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/search_engine_meilisearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/search_engine_serpapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/search_engine_serper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/tool_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/tool_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/tool_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/tool_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/ut_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/web_browser_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/web_browser_engine_playwright.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/tools/web_browser_engine_selenium.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.602405 metagpt-0.7.7/metagpt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/ahttp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24249 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/cost_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/custom_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/dependency_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/di_graph_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/file_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/git_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/graph_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/highlight.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/human_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/json_to_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/make_sk_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/mmdc_ink.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/mmdc_playwright.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/mmdc_pyppeteer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/parse_docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/parse_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/project_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/pycst.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/read_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/recovery_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/repair_llm_raw_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/save_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/special_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/token_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-29 04:00:53.000000 metagpt-0.7.7/metagpt/utils/yaml_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:02:23.558405 metagpt-0.7.7/metagpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-03-29 04:02:23.000000 metagpt-0.7.7/metagpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-03-29 04:02:23.000000 metagpt-0.7.7/metagpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 04:02:23.000000 metagpt-0.7.7/metagpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-29 04:02:23.000000 metagpt-0.7.7/metagpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-29 04:02:23.000000 metagpt-0.7.7/metagpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-29 04:02:23.000000 metagpt-0.7.7/metagpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 04:02:23.602405 metagpt-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-03-29 04:02:22.000000 metagpt-0.7.7/setup.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:04.009691 metagpt-0.8.0/
+-rw-r--r--   0 vk         (501) staff       (20)     1072 2024-01-31 08:12:12.000000 metagpt-0.8.0/LICENSE
+-rw-r--r--   0 vk         (501) staff       (20)    10890 2024-03-29 12:19:04.008226 metagpt-0.8.0/PKG-INFO
+-rw-r--r--   0 vk         (501) staff       (20)    10333 2024-03-29 12:17:47.000000 metagpt-0.8.0/README.md
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.794296 metagpt-0.8.0/metagpt/
+-rw-r--r--   0 vk         (501) staff       (20)      173 2023-12-19 03:15:31.000000 metagpt-0.8.0/metagpt/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)      846 2023-12-19 03:15:31.000000 metagpt-0.8.0/metagpt/_compat.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.828542 metagpt-0.8.0/metagpt/actions/
+-rw-r--r--   0 vk         (501) staff       (20)     1942 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     3209 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/action.py
+-rw-r--r--   0 vk         (501) staff       (20)     1324 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/action_graph.py
+-rw-r--r--   0 vk         (501) staff       (20)    27539 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/action_node.py
+-rw-r--r--   0 vk         (501) staff       (20)     1460 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/action_outcls_registry.py
+-rw-r--r--   0 vk         (501) staff       (20)      371 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/actions/action_output.py
+-rw-r--r--   0 vk         (501) staff       (20)      264 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/actions/add_requirement.py
+-rw-r--r--   0 vk         (501) staff       (20)     2621 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/debug_error.py
+-rw-r--r--   0 vk         (501) staff       (20)     5405 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/design_api.py
+-rw-r--r--   0 vk         (501) staff       (20)     4154 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/design_api_an.py
+-rw-r--r--   0 vk         (501) staff       (20)      754 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/design_api_review.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.831578 metagpt-0.8.0/metagpt/actions/di/
+-rw-r--r--   0 vk         (501) staff       (20)        0 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/di/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     2465 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/di/ask_review.py
+-rw-r--r--   0 vk         (501) staff       (20)     9952 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/di/execute_nb_code.py
+-rw-r--r--   0 vk         (501) staff       (20)     2403 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/di/write_analysis_code.py
+-rw-r--r--   0 vk         (501) staff       (20)     3162 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/di/write_plan.py
+-rw-r--r--   0 vk         (501) staff       (20)      352 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/execute_task.py
+-rw-r--r--   0 vk         (501) staff       (20)      243 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/actions/fix_bug.py
+-rw-r--r--   0 vk         (501) staff       (20)      895 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/generate_questions.py
+-rw-r--r--   0 vk         (501) staff       (20)     6397 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/invoice_ocr.py
+-rw-r--r--   0 vk         (501) staff       (20)     2063 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/prepare_documents.py
+-rw-r--r--   0 vk         (501) staff       (20)      853 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/actions/prepare_interview.py
+-rw-r--r--   0 vk         (501) staff       (20)     4169 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/project_management.py
+-rw-r--r--   0 vk         (501) staff       (20)     4475 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/project_management_an.py
+-rw-r--r--   0 vk         (501) staff       (20)     9960 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/rebuild_class_view.py
+-rw-r--r--   0 vk         (501) staff       (20)    26309 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/rebuild_sequence_view.py
+-rw-r--r--   0 vk         (501) staff       (20)    11163 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/research.py
+-rw-r--r--   0 vk         (501) staff       (20)     6991 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/run_code.py
+-rw-r--r--   0 vk         (501) staff       (20)     5452 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/search_and_summarize.py
+-rw-r--r--   0 vk         (501) staff       (20)     4032 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/skill_action.py
+-rw-r--r--   0 vk         (501) staff       (20)     3274 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/summarize_code.py
+-rw-r--r--   0 vk         (501) staff       (20)     6557 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/talk_action.py
+-rw-r--r--   0 vk         (501) staff       (20)     9742 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/write_code.py
+-rw-r--r--   0 vk         (501) staff       (20)    18013 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/write_code_an_draft.py
+-rw-r--r--   0 vk         (501) staff       (20)     7749 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/write_code_plan_and_change_an.py
+-rw-r--r--   0 vk         (501) staff       (20)     7583 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/write_code_review.py
+-rw-r--r--   0 vk         (501) staff       (20)     6392 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/write_docstring.py
+-rw-r--r--   0 vk         (501) staff       (20)     7243 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/write_prd.py
+-rw-r--r--   0 vk         (501) staff       (20)     7741 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/actions/write_prd_an.py
+-rw-r--r--   0 vk         (501) staff       (20)      800 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/write_prd_review.py
+-rw-r--r--   0 vk         (501) staff       (20)     1116 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/actions/write_review.py
+-rw-r--r--   0 vk         (501) staff       (20)     7380 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/write_teaching_plan.py
+-rw-r--r--   0 vk         (501) staff       (20)     3705 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/actions/write_test.py
+-rw-r--r--   0 vk         (501) staff       (20)     2002 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/actions/write_tutorial.py
+-rw-r--r--   0 vk         (501) staff       (20)     4842 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/config2.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.837411 metagpt-0.8.0/metagpt/configs/
+-rw-r--r--   0 vk         (501) staff       (20)      126 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/configs/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)      682 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/configs/browser_config.py
+-rw-r--r--   0 vk         (501) staff       (20)     2704 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/configs/llm_config.py
+-rw-r--r--   0 vk         (501) staff       (20)      466 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/configs/mermaid_config.py
+-rw-r--r--   0 vk         (501) staff       (20)      549 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/configs/redis_config.py
+-rw-r--r--   0 vk         (501) staff       (20)      305 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/configs/s3_config.py
+-rw-r--r--   0 vk         (501) staff       (20)      712 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/configs/search_config.py
+-rw-r--r--   0 vk         (501) staff       (20)     1012 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/configs/workspace_config.py
+-rw-r--r--   0 vk         (501) staff       (20)     4309 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/const.py
+-rw-r--r--   0 vk         (501) staff       (20)     3445 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/context.py
+-rw-r--r--   0 vk         (501) staff       (20)     3481 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/context_mixin.py
+-rw-r--r--   0 vk         (501) staff       (20)     8323 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/document.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.841980 metagpt-0.8.0/metagpt/document_store/
+-rw-r--r--   0 vk         (501) staff       (20)      212 2023-12-19 03:15:31.000000 metagpt-0.8.0/metagpt/document_store/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     1462 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/document_store/base_store.py
+-rw-r--r--   0 vk         (501) staff       (20)     1796 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/document_store/chromadb_store.py
+-rw-r--r--   0 vk         (501) staff       (20)     3935 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/document_store/faiss_store.py
+-rw-r--r--   0 vk         (501) staff       (20)     2930 2023-12-19 03:15:31.000000 metagpt-0.8.0/metagpt/document_store/lancedb_store.py
+-rw-r--r--   0 vk         (501) staff       (20)     3734 2023-12-23 08:47:00.000000 metagpt-0.8.0/metagpt/document_store/qdrant_store.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.843476 metagpt-0.8.0/metagpt/environment/
+-rw-r--r--   0 vk         (501) staff       (20)      494 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/__init__.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.846067 metagpt-0.8.0/metagpt/environment/android_env/
+-rw-r--r--   0 vk         (501) staff       (20)       58 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/android_env/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)      439 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/android_env/android_env.py
+-rw-r--r--   0 vk         (501) staff       (20)     5940 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/android_env/android_ext_env.py
+-rw-r--r--   0 vk         (501) staff       (20)      114 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/android_env/const.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.848015 metagpt-0.8.0/metagpt/environment/api/
+-rw-r--r--   0 vk         (501) staff       (20)       58 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/environment/api/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     1823 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/environment/api/env_api.py
+-rw-r--r--   0 vk         (501) staff       (20)     7526 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/base_env.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.850524 metagpt-0.8.0/metagpt/environment/minecraft_env/
+-rw-r--r--   0 vk         (501) staff       (20)       58 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/minecraft_env/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     1056 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/minecraft_env/const.py
+-rw-r--r--   0 vk         (501) staff       (20)    16291 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/minecraft_env/minecraft_env.py
+-rw-r--r--   0 vk         (501) staff       (20)     6632 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/minecraft_env/minecraft_ext_env.py
+-rw-r--r--   0 vk         (501) staff       (20)     2443 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/minecraft_env/process_monitor.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.851997 metagpt-0.8.0/metagpt/environment/software_env/
+-rw-r--r--   0 vk         (501) staff       (20)       58 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/software_env/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)      205 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/software_env/software_env.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.854049 metagpt-0.8.0/metagpt/environment/stanford_town_env/
+-rw-r--r--   0 vk         (501) staff       (20)       58 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/stanford_town_env/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)      299 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/stanford_town_env/stanford_town_env.py
+-rw-r--r--   0 vk         (501) staff       (20)    14873 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/stanford_town_env/stanford_town_ext_env.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.855831 metagpt-0.8.0/metagpt/environment/werewolf_env/
+-rw-r--r--   0 vk         (501) staff       (20)       58 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/werewolf_env/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     1241 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/werewolf_env/werewolf_env.py
+-rw-r--r--   0 vk         (501) staff       (20)    14833 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/environment/werewolf_env/werewolf_ext_env.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.860232 metagpt-0.8.0/metagpt/learn/
+-rw-r--r--   0 vk         (501) staff       (20)      356 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/learn/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)      551 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/learn/google_search.py
+-rw-r--r--   0 vk         (501) staff       (20)     2631 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/learn/skill_loader.py
+-rw-r--r--   0 vk         (501) staff       (20)     1102 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/learn/text_to_embedding.py
+-rw-r--r--   0 vk         (501) staff       (20)     1668 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/learn/text_to_image.py
+-rw-r--r--   0 vk         (501) staff       (20)     3749 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/learn/text_to_speech.py
+-rw-r--r--   0 vk         (501) staff       (20)      576 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/llm.py
+-rw-r--r--   0 vk         (501) staff       (20)      970 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/logs.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.861781 metagpt-0.8.0/metagpt/management/
+-rw-r--r--   0 vk         (501) staff       (20)      127 2023-07-10 02:22:27.000000 metagpt-0.8.0/metagpt/management/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     2351 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/management/skill_manager.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.864980 metagpt-0.8.0/metagpt/memory/
+-rw-r--r--   0 vk         (501) staff       (20)      284 2023-12-23 08:47:00.000000 metagpt-0.8.0/metagpt/memory/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)    12259 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/memory/brain_memory.py
+-rw-r--r--   0 vk         (501) staff       (20)     2865 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/memory/longterm_memory.py
+-rw-r--r--   0 vk         (501) staff       (20)     3915 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/memory/memory.py
+-rw-r--r--   0 vk         (501) staff       (20)     2827 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/memory/memory_storage.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.869757 metagpt-0.8.0/metagpt/prompts/
+-rw-r--r--   0 vk         (501) staff       (20)      127 2023-07-10 02:22:27.000000 metagpt-0.8.0/metagpt/prompts/__init__.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.870826 metagpt-0.8.0/metagpt/prompts/di/
+-rw-r--r--   0 vk         (501) staff       (20)        0 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/prompts/di/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     3458 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/prompts/di/write_analysis_code.py
+-rw-r--r--   0 vk         (501) staff       (20)     1314 2023-12-23 08:47:00.000000 metagpt-0.8.0/metagpt/prompts/invoice_ocr.py
+-rw-r--r--   0 vk         (501) staff       (20)     2308 2023-12-19 03:15:31.000000 metagpt-0.8.0/metagpt/prompts/metagpt_sample.py
+-rw-r--r--   0 vk         (501) staff       (20)     4818 2023-12-23 08:47:00.000000 metagpt-0.8.0/metagpt/prompts/sales.py
+-rw-r--r--   0 vk         (501) staff       (20)     5406 2023-12-19 03:15:31.000000 metagpt-0.8.0/metagpt/prompts/summarize.py
+-rw-r--r--   0 vk         (501) staff       (20)     3423 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/prompts/task_type.py
+-rw-r--r--   0 vk         (501) staff       (20)     1844 2023-12-23 08:47:00.000000 metagpt-0.8.0/metagpt/prompts/tutorial_assistant.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.883178 metagpt-0.8.0/metagpt/provider/
+-rw-r--r--   0 vk         (501) staff       (20)      938 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     3138 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/anthropic_api.py
+-rw-r--r--   0 vk         (501) staff       (20)     1476 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/azure_openai_api.py
+-rw-r--r--   0 vk         (501) staff       (20)    10812 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/base_llm.py
+-rw-r--r--   0 vk         (501) staff       (20)     1258 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/constant.py
+-rw-r--r--   0 vk         (501) staff       (20)     8196 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/dashscope_api.py
+-rw-r--r--   0 vk         (501) staff       (20)    19422 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/general_api_base.py
+-rw-r--r--   0 vk         (501) staff       (20)     3906 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/general_api_requestor.py
+-rw-r--r--   0 vk         (501) staff       (20)     7380 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/google_gemini_api.py
+-rw-r--r--   0 vk         (501) staff       (20)     1928 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/human_provider.py
+-rw-r--r--   0 vk         (501) staff       (20)     1076 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/llm_provider_registry.py
+-rw-r--r--   0 vk         (501) staff       (20)      744 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/metagpt_api.py
+-rw-r--r--   0 vk         (501) staff       (20)     3619 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/ollama_api.py
+-rw-r--r--   0 vk         (501) staff       (20)    12504 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/openai_api.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.884698 metagpt-0.8.0/metagpt/provider/postprocess/
+-rw-r--r--   0 vk         (501) staff       (20)       58 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/provider/postprocess/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     2984 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/provider/postprocess/base_postprocess_plugin.py
+-rw-r--r--   0 vk         (501) staff       (20)      700 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/provider/postprocess/llm_output_postprocess.py
+-rw-r--r--   0 vk         (501) staff       (20)     6242 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/qianfan_api.py
+-rw-r--r--   0 vk         (501) staff       (20)     7013 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/spark_api.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.886252 metagpt-0.8.0/metagpt/provider/zhipuai/
+-rw-r--r--   0 vk         (501) staff       (20)       58 2023-12-19 03:15:31.000000 metagpt-0.8.0/metagpt/provider/zhipuai/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     1078 2024-01-31 08:12:12.000000 metagpt-0.8.0/metagpt/provider/zhipuai/async_sse_client.py
+-rw-r--r--   0 vk         (501) staff       (20)     2235 2024-01-31 08:12:12.000000 metagpt-0.8.0/metagpt/provider/zhipuai/zhipu_model_api.py
+-rw-r--r--   0 vk         (501) staff       (20)     3088 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/provider/zhipuai_api.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.887701 metagpt-0.8.0/metagpt/rag/
+-rw-r--r--   0 vk         (501) staff       (20)        0 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/__init__.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.889318 metagpt-0.8.0/metagpt/rag/engines/
+-rw-r--r--   0 vk         (501) staff       (20)      165 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/engines/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)      299 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/engines/flare.py
+-rw-r--r--   0 vk         (501) staff       (20)    10788 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/engines/simple.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.894054 metagpt-0.8.0/metagpt/rag/factories/
+-rw-r--r--   0 vk         (501) staff       (20)      387 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/factories/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     1925 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/factories/base.py
+-rw-r--r--   0 vk         (501) staff       (20)     1235 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/factories/embedding.py
+-rw-r--r--   0 vk         (501) staff       (20)     3494 2024-03-29 11:46:45.000000 metagpt-0.8.0/metagpt/rag/factories/index.py
+-rw-r--r--   0 vk         (501) staff       (20)     1921 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/factories/llm.py
+-rw-r--r--   0 vk         (501) staff       (20)     2115 2024-03-29 11:46:45.000000 metagpt-0.8.0/metagpt/rag/factories/ranker.py
+-rw-r--r--   0 vk         (501) staff       (20)     4439 2024-03-29 11:46:45.000000 metagpt-0.8.0/metagpt/rag/factories/retriever.py
+-rw-r--r--   0 vk         (501) staff       (20)      540 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/interface.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.895787 metagpt-0.8.0/metagpt/rag/rankers/
+-rw-r--r--   0 vk         (501) staff       (20)       19 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/rankers/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)      505 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/rankers/base.py
+-rw-r--r--   0 vk         (501) staff       (20)     1813 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/rankers/object_ranker.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.899960 metagpt-0.8.0/metagpt/rag/retrievers/
+-rw-r--r--   0 vk         (501) staff       (20)      135 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/retrievers/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     1309 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/retrievers/base.py
+-rw-r--r--   0 vk         (501) staff       (20)     1641 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/retrievers/bm25_retriever.py
+-rw-r--r--   0 vk         (501) staff       (20)      520 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/retrievers/chroma_retriever.py
+-rw-r--r--   0 vk         (501) staff       (20)      546 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/retrievers/es_retriever.py
+-rw-r--r--   0 vk         (501) staff       (20)      501 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/retrievers/faiss_retriever.py
+-rw-r--r--   0 vk         (501) staff       (20)     1640 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/retrievers/hybrid_retriever.py
+-rw-r--r--   0 vk         (501) staff       (20)     6728 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/rag/schema.py
+-rw-r--r--   0 vk         (501) staff       (20)    35487 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/repo_parser.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.911370 metagpt-0.8.0/metagpt/roles/
+-rw-r--r--   0 vk         (501) staff       (20)      651 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/roles/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     1210 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/roles/architect.py
+-rw-r--r--   0 vk         (501) staff       (20)     5971 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/roles/assistant.py
+-rw-r--r--   0 vk         (501) staff       (20)     1456 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/roles/customer_service.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.912240 metagpt-0.8.0/metagpt/roles/di/
+-rw-r--r--   0 vk         (501) staff       (20)        0 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/roles/di/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     7114 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/roles/di/data_interpreter.py
+-rw-r--r--   0 vk         (501) staff       (20)    17814 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/roles/engineer.py
+-rw-r--r--   0 vk         (501) staff       (20)     3689 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/roles/invoice_ocr_assistant.py
+-rw-r--r--   0 vk         (501) staff       (20)     1835 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/roles/product_manager.py
+-rw-r--r--   0 vk         (501) staff       (20)     1136 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/roles/project_manager.py
+-rw-r--r--   0 vk         (501) staff       (20)    10360 2023-12-23 08:47:00.000000 metagpt-0.8.0/metagpt/roles/prompt.py
+-rw-r--r--   0 vk         (501) staff       (20)     8226 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/roles/qa_engineer.py
+-rw-r--r--   0 vk         (501) staff       (20)     4796 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/roles/researcher.py
+-rw-r--r--   0 vk         (501) staff       (20)    24684 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/roles/role.py
+-rw-r--r--   0 vk         (501) staff       (20)     1541 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/roles/sales.py
+-rw-r--r--   0 vk         (501) staff       (20)     2469 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/roles/searcher.py
+-rw-r--r--   0 vk         (501) staff       (20)     3563 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/roles/sk_agent.py
+-rw-r--r--   0 vk         (501) staff       (20)     4106 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/roles/teacher.py
+-rw-r--r--   0 vk         (501) staff       (20)     3404 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/roles/tutorial_assistant.py
+-rw-r--r--   0 vk         (501) staff       (20)    26628 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/schema.py
+-rw-r--r--   0 vk         (501) staff       (20)     5142 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/software_company.py
+-rw-r--r--   0 vk         (501) staff       (20)      270 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/startup.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.917035 metagpt-0.8.0/metagpt/strategy/
+-rw-r--r--   0 vk         (501) staff       (20)      115 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/strategy/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     3429 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/strategy/base.py
+-rw-r--r--   0 vk         (501) staff       (20)     6776 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/strategy/planner.py
+-rw-r--r--   0 vk         (501) staff       (20)      452 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/strategy/search_space.py
+-rw-r--r--   0 vk         (501) staff       (20)     1913 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/strategy/solver.py
+-rw-r--r--   0 vk         (501) staff       (20)     2377 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/strategy/task_type.py
+-rw-r--r--   0 vk         (501) staff       (20)    10017 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/strategy/tot.py
+-rw-r--r--   0 vk         (501) staff       (20)      772 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/strategy/tot_schema.py
+-rw-r--r--   0 vk         (501) staff       (20)     3299 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/subscription.py
+-rw-r--r--   0 vk         (501) staff       (20)     4665 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/team.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.932728 metagpt-0.8.0/metagpt/tools/
+-rw-r--r--   0 vk         (501) staff       (20)      799 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/tools/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     4790 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/tools/azure_tts.py
+-rw-r--r--   0 vk         (501) staff       (20)     5404 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/tools/iflytek_tts.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.936856 metagpt-0.8.0/metagpt/tools/libs/
+-rw-r--r--   0 vk         (501) staff       (20)      441 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/tools/libs/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     7410 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/tools/libs/data_preprocess.py
+-rw-r--r--   0 vk         (501) staff       (20)     2017 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/tools/libs/email_login.py
+-rw-r--r--   0 vk         (501) staff       (20)    14873 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/tools/libs/feature_engineering.py
+-rw-r--r--   0 vk         (501) staff       (20)     4604 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/tools/libs/gpt_v_generator.py
+-rw-r--r--   0 vk         (501) staff       (20)     6316 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/tools/libs/sd_engine.py
+-rw-r--r--   0 vk         (501) staff       (20)      766 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/tools/libs/web_scraping.py
+-rw-r--r--   0 vk         (501) staff       (20)      837 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/tools/metagpt_oas3_api_svc.py
+-rw-r--r--   0 vk         (501) staff       (20)     3011 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/tools/metagpt_text_to_image.py
+-rw-r--r--   0 vk         (501) staff       (20)     1259 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/tools/moderation.py
+-rw-r--r--   0 vk         (501) staff       (20)     3242 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/tools/openai_text_to_embedding.py
+-rw-r--r--   0 vk         (501) staff       (20)     2161 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/tools/openai_text_to_image.py
+-rw-r--r--   0 vk         (501) staff       (20)      850 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/tools/openapi_v3_hello.py
+-rw-r--r--   0 vk         (501) staff       (20)     5146 2023-12-23 08:47:00.000000 metagpt-0.8.0/metagpt/tools/prompt_writer.py
+-rw-r--r--   0 vk         (501) staff       (20)     6002 2024-03-29 12:17:47.000000 metagpt-0.8.0/metagpt/tools/search_engine.py
+-rw-r--r--   0 vk         (501) staff       (20)     2636 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/tools/search_engine_ddg.py
+-rw-r--r--   0 vk         (501) staff       (20)     4681 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/tools/search_engine_googleapi.py
+-rw-r--r--   0 vk         (501) staff       (20)     1175 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/tools/search_engine_meilisearch.py
+-rw-r--r--   0 vk         (501) staff       (20)     4593 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/tools/search_engine_serpapi.py
+-rw-r--r--   0 vk         (501) staff       (20)     5008 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/tools/search_engine_serper.py
+-rw-r--r--   0 vk         (501) staff       (20)     2647 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/tools/tool_convert.py
+-rw-r--r--   0 vk         (501) staff       (20)      203 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/tools/tool_data_type.py
+-rw-r--r--   0 vk         (501) staff       (20)     8044 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/tools/tool_recommend.py
+-rw-r--r--   0 vk         (501) staff       (20)     4511 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/tools/tool_registry.py
+-rw-r--r--   0 vk         (501) staff       (20)      666 2023-12-23 08:47:00.000000 metagpt-0.8.0/metagpt/tools/translator.py
+-rw-r--r--   0 vk         (501) staff       (20)    10878 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/tools/ut_writer.py
+-rw-r--r--   0 vk         (501) staff       (20)     4816 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/tools/web_browser_engine.py
+-rw-r--r--   0 vk         (501) staff       (20)     5112 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/tools/web_browser_engine_playwright.py
+-rw-r--r--   0 vk         (501) staff       (20)     5463 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/tools/web_browser_engine_selenium.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.963433 metagpt-0.8.0/metagpt/utils/
+-rw-r--r--   0 vk         (501) staff       (20)      460 2023-12-19 03:15:31.000000 metagpt-0.8.0/metagpt/utils/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     1462 2023-12-23 08:47:00.000000 metagpt-0.8.0/metagpt/utils/ahttp_client.py
+-rw-r--r--   0 vk         (501) staff       (20)      693 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/async_helper.py
+-rw-r--r--   0 vk         (501) staff       (20)    29032 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/common.py
+-rw-r--r--   0 vk         (501) staff       (20)     5270 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/cost_manager.py
+-rw-r--r--   0 vk         (501) staff       (20)    11393 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/utils/custom_decoder.py
+-rw-r--r--   0 vk         (501) staff       (20)     3279 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/dependency_file.py
+-rw-r--r--   0 vk         (501) staff       (20)     5817 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/di_graph_repository.py
+-rw-r--r--   0 vk         (501) staff       (20)      536 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/embedding.py
+-rw-r--r--   0 vk         (501) staff       (20)     1866 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/utils/exceptions.py
+-rw-r--r--   0 vk         (501) staff       (20)     2238 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/utils/file.py
+-rw-r--r--   0 vk         (501) staff       (20)     9073 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/file_repository.py
+-rw-r--r--   0 vk         (501) staff       (20)    11076 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/utils/git_repository.py
+-rw-r--r--   0 vk         (501) staff       (20)    16139 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/graph_repository.py
+-rw-r--r--   0 vk         (501) staff       (20)      851 2023-12-23 08:47:00.000000 metagpt-0.8.0/metagpt/utils/highlight.py
+-rw-r--r--   0 vk         (501) staff       (20)     4092 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/utils/human_interaction.py
+-rw-r--r--   0 vk         (501) staff       (20)     1355 2023-12-19 03:15:31.000000 metagpt-0.8.0/metagpt/utils/json_to_markdown.py
+-rw-r--r--   0 vk         (501) staff       (20)      845 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/utils/make_sk_kernel.py
+-rw-r--r--   0 vk         (501) staff       (20)     4399 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/mermaid.py
+-rw-r--r--   0 vk         (501) staff       (20)     1416 2023-12-23 08:47:00.000000 metagpt-0.8.0/metagpt/utils/mmdc_ink.py
+-rw-r--r--   0 vk         (501) staff       (20)     5090 2023-12-29 03:56:57.000000 metagpt-0.8.0/metagpt/utils/mmdc_playwright.py
+-rw-r--r--   0 vk         (501) staff       (20)     4993 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/utils/mmdc_pyppeteer.py
+-rw-r--r--   0 vk         (501) staff       (20)     1112 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/parse_docstring.py
+-rw-r--r--   0 vk         (501) staff       (20)     1579 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/utils/parse_html.py
+-rw-r--r--   0 vk         (501) staff       (20)     5877 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/project_repo.py
+-rw-r--r--   0 vk         (501) staff       (20)     5673 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/utils/pycst.py
+-rw-r--r--   0 vk         (501) staff       (20)      529 2023-12-23 08:47:00.000000 metagpt-0.8.0/metagpt/utils/read_document.py
+-rw-r--r--   0 vk         (501) staff       (20)     1775 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/recovery_util.py
+-rw-r--r--   0 vk         (501) staff       (20)     1835 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/utils/redis.py
+-rw-r--r--   0 vk         (501) staff       (20)      639 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/reflection.py
+-rw-r--r--   0 vk         (501) staff       (20)    13827 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/repair_llm_raw_output.py
+-rw-r--r--   0 vk         (501) staff       (20)     2928 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/repo_to_markdown.py
+-rw-r--r--   0 vk         (501) staff       (20)     6058 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/utils/s3.py
+-rw-r--r--   0 vk         (501) staff       (20)     1403 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/utils/save_code.py
+-rw-r--r--   0 vk         (501) staff       (20)     2721 2024-01-24 02:55:48.000000 metagpt-0.8.0/metagpt/utils/serialize.py
+-rw-r--r--   0 vk         (501) staff       (20)      532 2023-12-23 08:47:00.000000 metagpt-0.8.0/metagpt/utils/singleton.py
+-rw-r--r--   0 vk         (501) staff       (20)      198 2023-12-23 08:47:00.000000 metagpt-0.8.0/metagpt/utils/special_tokens.py
+-rw-r--r--   0 vk         (501) staff       (20)     4037 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/text.py
+-rw-r--r--   0 vk         (501) staff       (20)    13338 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/token_counter.py
+-rw-r--r--   0 vk         (501) staff       (20)     4366 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/tree.py
+-rw-r--r--   0 vk         (501) staff       (20)     6087 2024-03-27 07:26:42.000000 metagpt-0.8.0/metagpt/utils/visual_graph_repo.py
+-rw-r--r--   0 vk         (501) staff       (20)     1483 2024-02-07 02:23:19.000000 metagpt-0.8.0/metagpt/utils/yaml_model.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.797582 metagpt-0.8.0/metagpt.egg-info/
+-rw-r--r--   0 vk         (501) staff       (20)    10890 2024-03-29 12:19:03.000000 metagpt-0.8.0/metagpt.egg-info/PKG-INFO
+-rw-r--r--   0 vk         (501) staff       (20)    11581 2024-03-29 12:19:03.000000 metagpt-0.8.0/metagpt.egg-info/SOURCES.txt
+-rw-r--r--   0 vk         (501) staff       (20)        1 2024-03-29 12:19:03.000000 metagpt-0.8.0/metagpt.egg-info/dependency_links.txt
+-rw-r--r--   0 vk         (501) staff       (20)       57 2024-03-29 12:19:03.000000 metagpt-0.8.0/metagpt.egg-info/entry_points.txt
+-rw-r--r--   0 vk         (501) staff       (20)     2255 2024-03-29 12:19:03.000000 metagpt-0.8.0/metagpt.egg-info/requires.txt
+-rw-r--r--   0 vk         (501) staff       (20)        8 2024-03-29 12:19:03.000000 metagpt-0.8.0/metagpt.egg-info/top_level.txt
+-rw-r--r--   0 vk         (501) staff       (20)       38 2024-03-29 12:19:04.009855 metagpt-0.8.0/setup.cfg
+-rw-r--r--   0 vk         (501) staff       (20)     2878 2024-03-29 12:17:47.000000 metagpt-0.8.0/setup.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.964216 metagpt-0.8.0/tests/
+-rw-r--r--   0 vk         (501) staff       (20)      127 2023-07-10 02:22:27.000000 metagpt-0.8.0/tests/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     9256 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/conftest.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.968094 metagpt-0.8.0/tests/metagpt/
+-rw-r--r--   0 vk         (501) staff       (20)      127 2023-07-10 02:22:27.000000 metagpt-0.8.0/tests/metagpt/__init__.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.977802 metagpt-0.8.0/tests/metagpt/actions/
+-rw-r--r--   0 vk         (501) staff       (20)      127 2023-07-10 02:22:27.000000 metagpt-0.8.0/tests/metagpt/actions/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     1094 2024-01-24 02:55:48.000000 metagpt-0.8.0/tests/metagpt/actions/test_action.py
+-rw-r--r--   0 vk         (501) staff       (20)     4913 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/actions/test_debug_error.py
+-rw-r--r--   0 vk         (501) staff       (20)     1336 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/actions/test_design_api.py
+-rw-r--r--   0 vk         (501) staff       (20)     1225 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/actions/test_design_api_review.py
+-rw-r--r--   0 vk         (501) staff       (20)     1377 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/actions/test_project_management.py
+-rw-r--r--   0 vk         (501) staff       (20)     1849 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/actions/test_run_code.py
+-rw-r--r--   0 vk         (501) staff       (20)     6224 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/actions/test_write_code.py
+-rw-r--r--   0 vk         (501) staff       (20)     1732 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/actions/test_write_code_review.py
+-rw-r--r--   0 vk         (501) staff       (20)      916 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/actions/test_write_docstring.py
+-rw-r--r--   0 vk         (501) staff       (20)     2890 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/actions/test_write_prd.py
+-rw-r--r--   0 vk         (501) staff       (20)     1276 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/actions/test_write_prd_review.py
+-rw-r--r--   0 vk         (501) staff       (20)     1864 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/actions/test_write_test.py
+-rw-r--r--   0 vk         (501) staff       (20)     1277 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/actions/test_write_tutorial.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.981476 metagpt-0.8.0/tests/metagpt/document_store/
+-rw-r--r--   0 vk         (501) staff       (20)      127 2023-07-10 02:22:27.000000 metagpt-0.8.0/tests/metagpt/document_store/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)      922 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/document_store/test_chromadb_store.py
+-rw-r--r--   0 vk         (501) staff       (20)      944 2023-12-23 08:47:00.000000 metagpt-0.8.0/tests/metagpt/document_store/test_document.py
+-rw-r--r--   0 vk         (501) staff       (20)     2429 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/document_store/test_faiss_store.py
+-rw-r--r--   0 vk         (501) staff       (20)      993 2024-01-24 02:55:48.000000 metagpt-0.8.0/tests/metagpt/document_store/test_lancedb_store.py
+-rw-r--r--   0 vk         (501) staff       (20)     3029 2024-01-31 08:12:12.000000 metagpt-0.8.0/tests/metagpt/document_store/test_qdrant_store.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.982788 metagpt-0.8.0/tests/metagpt/management/
+-rw-r--r--   0 vk         (501) staff       (20)      126 2023-12-29 10:06:26.000000 metagpt-0.8.0/tests/metagpt/management/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     1029 2024-01-24 02:55:48.000000 metagpt-0.8.0/tests/metagpt/management/test_skill_manager.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.985150 metagpt-0.8.0/tests/metagpt/memory/
+-rw-r--r--   0 vk         (501) staff       (20)       58 2023-12-19 03:15:31.000000 metagpt-0.8.0/tests/metagpt/memory/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     2017 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/memory/test_longterm_memory.py
+-rw-r--r--   0 vk         (501) staff       (20)     4130 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/memory/test_memory_storage.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.986948 metagpt-0.8.0/tests/metagpt/planner/
+-rw-r--r--   0 vk         (501) staff       (20)      127 2023-12-29 10:06:26.000000 metagpt-0.8.0/tests/metagpt/planner/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     1168 2023-12-29 10:06:26.000000 metagpt-0.8.0/tests/metagpt/planner/test_action_planner.py
+-rw-r--r--   0 vk         (501) staff       (20)     1491 2023-12-29 10:06:26.000000 metagpt-0.8.0/tests/metagpt/planner/test_basic_planner.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.987459 metagpt-0.8.0/tests/metagpt/provider/
+-rw-r--r--   0 vk         (501) staff       (20)      126 2023-07-22 01:05:00.000000 metagpt-0.8.0/tests/metagpt/provider/__init__.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.993188 metagpt-0.8.0/tests/metagpt/roles/
+-rw-r--r--   0 vk         (501) staff       (20)      127 2023-07-10 02:22:27.000000 metagpt-0.8.0/tests/metagpt/roles/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)    11906 2024-01-31 08:12:12.000000 metagpt-0.8.0/tests/metagpt/roles/mock.py
+-rw-r--r--   0 vk         (501) staff       (20)     1321 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/roles/test_architect.py
+-rw-r--r--   0 vk         (501) staff       (20)     5035 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/roles/test_engineer.py
+-rw-r--r--   0 vk         (501) staff       (20)     1639 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/roles/test_product_manager.py
+-rw-r--r--   0 vk         (501) staff       (20)      480 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/roles/test_project_manager.py
+-rw-r--r--   0 vk         (501) staff       (20)     1960 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/roles/test_qa_engineer.py
+-rw-r--r--   0 vk         (501) staff       (20)     2330 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/roles/test_researcher.py
+-rw-r--r--   0 vk         (501) staff       (20)      781 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/roles/test_tutorial_assistant.py
+-rw-r--r--   0 vk         (501) staff       (20)     2072 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/test_environment.py
+-rw-r--r--   0 vk         (501) staff       (20)      759 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/test_llm.py
+-rw-r--r--   0 vk         (501) staff       (20)      781 2024-01-24 02:55:48.000000 metagpt-0.8.0/tests/metagpt/test_message.py
+-rw-r--r--   0 vk         (501) staff       (20)     5000 2024-02-07 02:23:19.000000 metagpt-0.8.0/tests/metagpt/test_role.py
+-rw-r--r--   0 vk         (501) staff       (20)    12412 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/test_schema.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:03.998493 metagpt-0.8.0/tests/metagpt/tools/
+-rw-r--r--   0 vk         (501) staff       (20)      127 2023-07-10 02:22:27.000000 metagpt-0.8.0/tests/metagpt/tools/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     2888 2024-03-29 12:17:47.000000 metagpt-0.8.0/tests/metagpt/tools/test_search_engine.py
+-rw-r--r--   0 vk         (501) staff       (20)     2032 2024-01-31 08:12:12.000000 metagpt-0.8.0/tests/metagpt/tools/test_search_engine_meilisearch.py
+-rw-r--r--   0 vk         (501) staff       (20)    10649 2023-12-23 08:47:00.000000 metagpt-0.8.0/tests/metagpt/tools/test_summarize.py
+-rw-r--r--   0 vk         (501) staff       (20)      638 2024-01-31 08:12:12.000000 metagpt-0.8.0/tests/metagpt/tools/test_translate.py
+-rw-r--r--   0 vk         (501) staff       (20)      986 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/tools/test_web_browser_engine.py
+-rw-r--r--   0 vk         (501) staff       (20)     1494 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/tools/test_web_browser_engine_playwright.py
+-rw-r--r--   0 vk         (501) staff       (20)     1790 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/tools/test_web_browser_engine_selenium.py
+drwxr-xr-x   0 vk         (501) staff       (20)        0 2024-03-29 12:19:04.007329 metagpt-0.8.0/tests/metagpt/utils/
+-rw-r--r--   0 vk         (501) staff       (20)      127 2023-07-10 02:22:27.000000 metagpt-0.8.0/tests/metagpt/utils/__init__.py
+-rw-r--r--   0 vk         (501) staff       (20)     3810 2024-01-24 02:55:48.000000 metagpt-0.8.0/tests/metagpt/utils/test_code_parser.py
+-rw-r--r--   0 vk         (501) staff       (20)     7738 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/utils/test_common.py
+-rw-r--r--   0 vk         (501) staff       (20)     2947 2023-12-23 08:47:00.000000 metagpt-0.8.0/tests/metagpt/utils/test_custom_decoder.py
+-rw-r--r--   0 vk         (501) staff       (20)     1064 2024-01-24 02:55:48.000000 metagpt-0.8.0/tests/metagpt/utils/test_file.py
+-rw-r--r--   0 vk         (501) staff       (20)     1216 2023-12-19 03:15:31.000000 metagpt-0.8.0/tests/metagpt/utils/test_json_to_markdown.py
+-rw-r--r--   0 vk         (501) staff       (20)     8000 2024-01-24 02:55:48.000000 metagpt-0.8.0/tests/metagpt/utils/test_output_parser.py
+-rw-r--r--   0 vk         (501) staff       (20)     2093 2023-12-23 08:47:00.000000 metagpt-0.8.0/tests/metagpt/utils/test_parse_html.py
+-rw-r--r--   0 vk         (501) staff       (20)     2802 2023-12-23 08:47:00.000000 metagpt-0.8.0/tests/metagpt/utils/test_pycst.py
+-rw-r--r--   0 vk         (501) staff       (20)      554 2024-01-31 08:12:12.000000 metagpt-0.8.0/tests/metagpt/utils/test_read_docx.py
+-rw-r--r--   0 vk         (501) staff       (20)     2146 2024-01-24 02:55:48.000000 metagpt-0.8.0/tests/metagpt/utils/test_serialize.py
+-rw-r--r--   0 vk         (501) staff       (20)     2860 2024-03-27 07:26:42.000000 metagpt-0.8.0/tests/metagpt/utils/test_text.py
+-rw-r--r--   0 vk         (501) staff       (20)     2014 2024-01-24 02:55:48.000000 metagpt-0.8.0/tests/metagpt/utils/test_token_counter.py
```

### Comparing `metagpt-0.7.7/LICENSE` & `metagpt-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/PKG-INFO` & `metagpt-0.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: metagpt
-Version: 0.7.7
+Version: 0.8.0
 Summary: The Multi-Agent Framework
 Home-page: https://github.com/geekan/MetaGPT
 Author: Alexander Wu
 Author-email: alexanderwu@deepwisdom.ai
 License: MIT
 Keywords: metagpt multi-agent multi-role programming gpt llm metaprogramming
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: selenium
 Provides-Extra: search-google
 Provides-Extra: search-ddg
 Provides-Extra: ocr
+Provides-Extra: rag
 Provides-Extra: test
 Provides-Extra: pyppeteer
 Provides-Extra: dev
 License-File: LICENSE
 
 
 # MetaGPT: The Multi-Agent Framework
@@ -42,15 +43,17 @@
 <p align="center">
    <a href="https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/geekan/MetaGPT"><img src="https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode" alt="Open in Dev Containers"></a>
    <a href="https://codespaces.new/geekan/MetaGPT"><img src="https://img.shields.io/badge/Github_Codespace-Open-blue?logo=github" alt="Open in GitHub Codespaces"></a>
    <a href="https://huggingface.co/spaces/deepwisdom/MetaGPT" target="_blank"><img alt="Hugging Face" src="https://img.shields.io/badge/%F0%9F%A4%97%20-Hugging%20Face-blue?color=blue&logoColor=white" /></a>
 </p>
 
 ## News
-🚀 March. 01, 2024: Our Data Interpreter paper is on arxiv. Find all design and benchmark details [here](https://arxiv.org/abs/2402.18679)!
+🚀 Mar. 29, 2024: [v0.8.0](https://github.com/geekan/MetaGPT/releases/tag/v0.8.0) released. Now you can use Data Interpreter via pypi package import. Meanwhile, we integrated RAG module and supported multiple new LLMs.
+
+🚀 Mar. 14, 2024: Our **Data Interpreter** paper is on [arxiv](https://arxiv.org/abs/2402.18679). Check the [example](https://docs.deepwisdom.ai/main/en/DataInterpreter/) and [code](https://github.com/geekan/MetaGPT/tree/main/examples/di)!
 
 🚀 Feb. 08, 2024: [v0.7.0](https://github.com/geekan/MetaGPT/releases/tag/v0.7.0) released, supporting assigning different LLMs to different Roles. We also introduced [Data Interpreter](https://github.com/geekan/MetaGPT/blob/main/examples/di/README.md), a powerful agent capable of solving a wide range of real-world problems.
 
 🚀 Jan. 16, 2024: Our paper [MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework
 ](https://arxiv.org/abs/2308.00352) accepted for oral presentation **(top 1.2%)** at ICLR 2024, **ranking #1** in the LLM-based Agent category.
 
 🚀 Jan. 03, 2024: [v0.6.0](https://github.com/geekan/MetaGPT/releases/tag/v0.6.0) released, new features include serialization, upgraded OpenAI package and supported multiple LLM, provided [minimal example for debate](https://github.com/geekan/MetaGPT/blob/main/examples/debate_simple.py) etc.
@@ -71,57 +74,77 @@
 2. Internally, MetaGPT includes **product managers / architects / project managers / engineers.** It provides the entire process of a **software company along with carefully orchestrated SOPs.**
    1. `Code = SOP(Team)` is the core philosophy. We materialize SOP and apply it to teams composed of LLMs.
 
 ![A software company consists of LLM-based roles](docs/resources/software_company_cd.jpeg)
 
 <p align="center">Software Company Multi-Agent Schematic (Gradually Implementing)</p>
 
-## Install
+## Get Started
 
-### Pip installation
+### Installation
 
 > Ensure that Python 3.9+ is installed on your system. You can check this by using: `python --version`.  
 > You can use conda like this: `conda create -n metagpt python=3.9 && conda activate metagpt`
 
 ```bash
-pip install metagpt
-metagpt --init-config  # create ~/.metagpt/config2.yaml, modify it to your own config
+pip install --upgrade metagpt
+# or `pip install --upgrade git+https://github.com/geekan/MetaGPT.git`
+# or `git clone https://github.com/geekan/MetaGPT && cd MetaGPT && pip install --upgrade -e .`
+```
+
+For detailed installation guidance, please refer to [cli_install](https://docs.deepwisdom.ai/main/en/guide/get_started/installation.html#install-stable-version)
+ or [docker_install](https://docs.deepwisdom.ai/main/en/guide/get_started/installation.html#install-with-docker)
+
+### Configuration
+
+You can init the config of MetaGPT by running the following command, or manually create `~/.metagpt/config2.yaml` file:
+```bash
+# Check https://docs.deepwisdom.ai/main/en/guide/get_started/configuration.html for more details
+metagpt --init-config  # it will create ~/.metagpt/config2.yaml, just modify it to your needs
+```
+
+You can configure `~/.metagpt/config2.yaml` according to the [example](https://github.com/geekan/MetaGPT/blob/main/config/config2.example.yaml) and [doc](https://docs.deepwisdom.ai/main/en/guide/get_started/configuration.html):
+
+```yaml
+llm:
+  api_type: "openai"  # or azure / ollama / open_llm etc. Check LLMType for more options
+  model: "gpt-4-turbo-preview"  # or gpt-3.5-turbo-1106 / gpt-4-1106-preview
+  base_url: "https://api.openai.com/v1"  # or forward url / other llm url
+  api_key: "YOUR_API_KEY"
+```
+
+### Usage
+
+After installation, you can use MetaGPT at CLI
+
+```bash
 metagpt "Create a 2048 game"  # this will create a repo in ./workspace
 ```
 
-or you can use it as library
+or use it as library
 
 ```python
 from metagpt.software_company import generate_repo, ProjectRepo
 repo: ProjectRepo = generate_repo("Create a 2048 game")  # or ProjectRepo("<path>")
 print(repo)  # it will print the repo structure with files
 ```
 
-detail installation please refer to [cli_install](https://docs.deepwisdom.ai/main/en/guide/get_started/installation.html#install-stable-version)
+You can also use its [Data Interpreter](https://github.com/geekan/MetaGPT/tree/main/examples/di)
+
+```python
+import asyncio
+from metagpt.roles.di.data_interpreter import DataInterpreter
 
-### Docker installation
-> Note: In the Windows, you need to replace "/opt/metagpt" with a directory that Docker has permission to create, such as "D:\Users\x\metagpt"
+async def main():
+    di = DataInterpreter()
+    await di.run("Run data analysis on sklearn Iris dataset, include a plot")
 
-```bash
-# Step 1: Download metagpt official image and prepare config2.yaml
-docker pull metagpt/metagpt:latest
-mkdir -p /opt/metagpt/{config,workspace}
-docker run --rm metagpt/metagpt:latest cat /app/metagpt/config/config2.yaml > /opt/metagpt/config/config2.yaml
-vim /opt/metagpt/config/config2.yaml # Change the config
-
-# Step 2: Run metagpt demo with container
-docker run --rm \
-    --privileged \
-    -v /opt/metagpt/config/config2.yaml:/app/metagpt/config/config2.yaml \
-    -v /opt/metagpt/workspace:/app/metagpt/workspace \
-    metagpt/metagpt:latest \
-    metagpt "Create a 2048 game"
+asyncio.run(main())  # or await main() in a jupyter notebook setting
 ```
 
-detail installation please refer to [docker_install](https://docs.deepwisdom.ai/main/en/guide/get_started/installation.html#install-with-docker)
 
 ### QuickStart & Demo Video
 - Try it on [MetaGPT Huggingface Space](https://huggingface.co/spaces/deepwisdom/MetaGPT)
 - [Matthew Berman: How To Install MetaGPT - Build A Startup With One Prompt!!](https://youtu.be/uT75J_KG_aY)
 - [Official Demo Video](https://github.com/geekan/MetaGPT/assets/2707039/5e8c1062-8c35-440f-bb20-2b0320f8d27d)
 
 https://github.com/geekan/MetaGPT/assets/34952977/34345016-5d13-489d-b9f9-b82ace413419
@@ -133,14 +156,15 @@
 - 🔎 [What can MetaGPT do?](https://docs.deepwisdom.ai/main/en/guide/get_started/introduction.html)
 - 🛠 How to build your own agents? 
   - [MetaGPT Usage & Development Guide | Agent 101](https://docs.deepwisdom.ai/main/en/guide/tutorials/agent_101.html)
   - [MetaGPT Usage & Development Guide | MultiAgent 101](https://docs.deepwisdom.ai/main/en/guide/tutorials/multi_agent_101.html)
 - 🧑‍💻 Contribution
   - [Develop Roadmap](docs/ROADMAP.md)
 - 🔖 Use Cases
+  - [Data Interpreter](https://docs.deepwisdom.ai/main/en/guide/use_cases/agent/interpreter/intro.html)
   - [Debate](https://docs.deepwisdom.ai/main/en/guide/use_cases/multi_agent/debate.html)
   - [Researcher](https://docs.deepwisdom.ai/main/en/guide/use_cases/agent/researcher.html)
   - [Recepit Assistant](https://docs.deepwisdom.ai/main/en/guide/use_cases/agent/receipt_assistant.html)
 - ❓ [FAQs](https://docs.deepwisdom.ai/main/en/guide/faq.html)
 
 ## Support
 
@@ -156,19 +180,31 @@
 - **Email:** alexanderwu@deepwisdom.ai
 - **GitHub Issues:** For more technical inquiries, you can also create a new issue in our [GitHub repository](https://github.com/geekan/metagpt/issues).
 
 We will respond to all questions within 2-3 business days.
 
 ## Citation
 
-For now, cite the [arXiv paper](https://arxiv.org/abs/2308.00352):
+To stay updated with the latest research and development, follow [@MetaGPT_](https://twitter.com/MetaGPT_) on Twitter. 
+
+To cite [MetaGPT](https://arxiv.org/abs/2308.00352) or [Data Interpreter](https://arxiv.org/abs/2402.18679) in publications, please use the following BibTeX entries.
 
 ```bibtex
 @misc{hong2023metagpt,
       title={MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework}, 
       author={Sirui Hong and Mingchen Zhuge and Jonathan Chen and Xiawu Zheng and Yuheng Cheng and Ceyao Zhang and Jinlin Wang and Zili Wang and Steven Ka Shing Yau and Zijuan Lin and Liyang Zhou and Chenyu Ran and Lingfeng Xiao and Chenglin Wu and Jürgen Schmidhuber},
       year={2023},
       eprint={2308.00352},
       archivePrefix={arXiv},
       primaryClass={cs.AI}
 }
+@misc{hong2024data,
+      title={Data Interpreter: An LLM Agent For Data Science}, 
+      author={Sirui Hong and Yizhang Lin and Bang Liu and Bangbang Liu and Binhao Wu and Danyang Li and Jiaqi Chen and Jiayi Zhang and Jinlin Wang and Li Zhang and Lingyao Zhang and Min Yang and Mingchen Zhuge and Taicheng Guo and Tuo Zhou and Wei Tao and Wenyi Wang and Xiangru Tang and Xiangtao Lu and Xiawu Zheng and Xinbing Liang and Yaying Fei and Yuheng Cheng and Zongze Xu and Chenglin Wu},
+      year={2024},
+      eprint={2402.18679},
+      archivePrefix={arXiv},
+      primaryClass={cs.AI}
+}
+
 ```
+
```

#### html2text {}

```diff
@@ -1,35 +1,39 @@
-Metadata-Version: 2.1 Name: metagpt Version: 0.7.7 Summary: The Multi-Agent
+Metadata-Version: 2.1 Name: metagpt Version: 0.8.0 Summary: The Multi-Agent
 Framework Home-page: https://github.com/geekan/MetaGPT Author: Alexander Wu
 Author-email: alexanderwu@deepwisdom.ai License: MIT Keywords: metagpt multi-
 agent multi-role programming gpt llm metaprogramming Requires-Python: >=3.9
 Description-Content-Type: text/markdown Provides-Extra: selenium Provides-
 Extra: search-google Provides-Extra: search-ddg Provides-Extra: ocr Provides-
-Extra: test Provides-Extra: pyppeteer Provides-Extra: dev License-File: LICENSE
-# MetaGPT: The Multi-Agent Framework
+Extra: rag Provides-Extra: test Provides-Extra: pyppeteer Provides-Extra: dev
+License-File: LICENSE # MetaGPT: The Multi-Agent Framework
 [MetaGPT logo: Enable GPT to work in software company, collaborating to tackle
                              more complex tasks.]
    AAssssiiggnn ddiiffffeerreenntt rroolleess ttoo GGPPTTss ttoo ffoorrmm aa ccoollllaabboorraattiivvee eennttiittyy ffoorr ccoommpplleexx
                                     ttaasskkss..
 _[_C_N_ _d_o_c_]_[_E_N_ _d_o_c_]_[_J_A_ _d_o_c_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]_[_r_o_a_d_m_a_p_]_[_D_i_s_c_o_r_d_ _F_o_l_l_o_w_]_[_T_w_i_t_t_e_r_ _F_o_l_l_o_w_]
        _[_O_p_e_n_ _i_n_ _D_e_v_ _C_o_n_t_a_i_n_e_r_s_]_[_O_p_e_n_ _i_n_ _G_i_t_H_u_b_ _C_o_d_e_s_p_a_c_e_s_]_[_H_u_g_g_i_n_g_ _F_a_c_e_]
-## News ð March. 01, 2024: Our Data Interpreter paper is on arxiv. Find all
-design and benchmark details [here](https://arxiv.org/abs/2402.18679)! ð
-Feb. 08, 2024: [v0.7.0](https://github.com/geekan/MetaGPT/releases/tag/v0.7.0)
-released, supporting assigning different LLMs to different Roles. We also
-introduced [Data Interpreter](https://github.com/geekan/MetaGPT/blob/main/
-examples/di/README.md), a powerful agent capable of solving a wide range of
-real-world problems. ð Jan. 16, 2024: Our paper [MetaGPT: Meta Programming
-for A Multi-Agent Collaborative Framework ](https://arxiv.org/abs/2308.00352)
-accepted for oral presentation **(top 1.2%)** at ICLR 2024, **ranking #1** in
-the LLM-based Agent category. ð Jan. 03, 2024: [v0.6.0](https://github.com/
-geekan/MetaGPT/releases/tag/v0.6.0) released, new features include
-serialization, upgraded OpenAI package and supported multiple LLM, provided
-[minimal example for debate](https://github.com/geekan/MetaGPT/blob/main/
-examples/debate_simple.py) etc. ð Dec. 15, 2023: [v0.5.0](https://
+## News ð Mar. 29, 2024: [v0.8.0](https://github.com/geekan/MetaGPT/
+releases/tag/v0.8.0) released. Now you can use Data Interpreter via pypi
+package import. Meanwhile, we integrated RAG module and supported multiple new
+LLMs. ð Mar. 14, 2024: Our **Data Interpreter** paper is on [arxiv](https://
+arxiv.org/abs/2402.18679). Check the [example](https://docs.deepwisdom.ai/main/
+en/DataInterpreter/) and [code](https://github.com/geekan/MetaGPT/tree/main/
+examples/di)! ð Feb. 08, 2024: [v0.7.0](https://github.com/geekan/MetaGPT/
+releases/tag/v0.7.0) released, supporting assigning different LLMs to different
+Roles. We also introduced [Data Interpreter](https://github.com/geekan/MetaGPT/
+blob/main/examples/di/README.md), a powerful agent capable of solving a wide
+range of real-world problems. ð Jan. 16, 2024: Our paper [MetaGPT: Meta
+Programming for A Multi-Agent Collaborative Framework ](https://arxiv.org/abs/
+2308.00352) accepted for oral presentation **(top 1.2%)** at ICLR 2024,
+**ranking #1** in the LLM-based Agent category. ð Jan. 03, 2024: [v0.6.0]
+(https://github.com/geekan/MetaGPT/releases/tag/v0.6.0) released, new features
+include serialization, upgraded OpenAI package and supported multiple LLM,
+provided [minimal example for debate](https://github.com/geekan/MetaGPT/blob/
+main/examples/debate_simple.py) etc. ð Dec. 15, 2023: [v0.5.0](https://
 github.com/geekan/MetaGPT/releases/tag/v0.5.0) released, introducing some
 experimental features such as **incremental development**, **multilingual**,
 **multiple programming languages**, etc. ð¥ Nov. 08, 2023: MetaGPT is
 selected into [Open100: Top 100 Open Source achievements](https://
 www.benchcouncil.org/evaluation/opencs/annual.html). ð¥ Sep. 01, 2023:
 MetaGPT tops GitHub Trending Monthly for the **17th time** in August 2023. ð
 Jun. 30, 2023: MetaGPT is now open source. ð Apr. 24, 2023: First line of
@@ -39,63 +43,82 @@
 etc.** 2. Internally, MetaGPT includes **product managers / architects /
 project managers / engineers.** It provides the entire process of a **software
 company along with carefully orchestrated SOPs.** 1. `Code = SOP(Team)` is the
 core philosophy. We materialize SOP and apply it to teams composed of LLMs. ![A
 software company consists of LLM-based roles](docs/resources/
 software_company_cd.jpeg)
         Software Company Multi-Agent Schematic (Gradually Implementing)
-## Install ### Pip installation > Ensure that Python 3.9+ is installed on your
+## Get Started ### Installation > Ensure that Python 3.9+ is installed on your
 system. You can check this by using: `python --version`. > You can use conda
 like this: `conda create -n metagpt python=3.9 && conda activate metagpt`
-```bash pip install metagpt metagpt --init-config # create ~/.metagpt/
-config2.yaml, modify it to your own config metagpt "Create a 2048 game" # this
-will create a repo in ./workspace ``` or you can use it as library ```python
-from metagpt.software_company import generate_repo, ProjectRepo repo:
-ProjectRepo = generate_repo("Create a 2048 game") # or ProjectRepo("") print
-(repo) # it will print the repo structure with files ``` detail installation
-please refer to [cli_install](https://docs.deepwisdom.ai/main/en/guide/
-get_started/installation.html#install-stable-version) ### Docker installation >
-Note: In the Windows, you need to replace "/opt/metagpt" with a directory that
-Docker has permission to create, such as "D:\Users\x\metagpt" ```bash # Step 1:
-Download metagpt official image and prepare config2.yaml docker pull metagpt/
-metagpt:latest mkdir -p /opt/metagpt/{config,workspace} docker run --rm
-metagpt/metagpt:latest cat /app/metagpt/config/config2.yaml > /opt/metagpt/
-config/config2.yaml vim /opt/metagpt/config/config2.yaml # Change the config #
-Step 2: Run metagpt demo with container docker run --rm \ --privileged \ -v /
-opt/metagpt/config/config2.yaml:/app/metagpt/config/config2.yaml \ -v /opt/
-metagpt/workspace:/app/metagpt/workspace \ metagpt/metagpt:latest \ metagpt
-"Create a 2048 game" ``` detail installation please refer to [docker_install]
-(https://docs.deepwisdom.ai/main/en/guide/get_started/
-installation.html#install-with-docker) ### QuickStart & Demo Video - Try it on
-[MetaGPT Huggingface Space](https://huggingface.co/spaces/deepwisdom/MetaGPT) -
-[Matthew Berman: How To Install MetaGPT - Build A Startup With One Prompt!!]
-(https://youtu.be/uT75J_KG_aY) - [Official Demo Video](https://github.com/
-geekan/MetaGPT/assets/2707039/5e8c1062-8c35-440f-bb20-2b0320f8d27d) https://
+```bash pip install --upgrade metagpt # or `pip install --upgrade git+https://
+github.com/geekan/MetaGPT.git` # or `git clone https://github.com/geekan/
+MetaGPT && cd MetaGPT && pip install --upgrade -e .` ``` For detailed
+installation guidance, please refer to [cli_install](https://
+docs.deepwisdom.ai/main/en/guide/get_started/installation.html#install-stable-
+version) or [docker_install](https://docs.deepwisdom.ai/main/en/guide/
+get_started/installation.html#install-with-docker) ### Configuration You can
+init the config of MetaGPT by running the following command, or manually create
+`~/.metagpt/config2.yaml` file: ```bash # Check https://docs.deepwisdom.ai/
+main/en/guide/get_started/configuration.html for more details metagpt --init-
+config # it will create ~/.metagpt/config2.yaml, just modify it to your needs
+``` You can configure `~/.metagpt/config2.yaml` according to the [example]
+(https://github.com/geekan/MetaGPT/blob/main/config/config2.example.yaml) and
+[doc](https://docs.deepwisdom.ai/main/en/guide/get_started/configuration.html):
+```yaml llm: api_type: "openai" # or azure / ollama / open_llm etc. Check
+LLMType for more options model: "gpt-4-turbo-preview" # or gpt-3.5-turbo-1106 /
+gpt-4-1106-preview base_url: "https://api.openai.com/v1" # or forward url /
+other llm url api_key: "YOUR_API_KEY" ``` ### Usage After installation, you can
+use MetaGPT at CLI ```bash metagpt "Create a 2048 game" # this will create a
+repo in ./workspace ``` or use it as library ```python from
+metagpt.software_company import generate_repo, ProjectRepo repo: ProjectRepo =
+generate_repo("Create a 2048 game") # or ProjectRepo("") print(repo) # it will
+print the repo structure with files ``` You can also use its [Data Interpreter]
+(https://github.com/geekan/MetaGPT/tree/main/examples/di) ```python import
+asyncio from metagpt.roles.di.data_interpreter import DataInterpreter async def
+main(): di = DataInterpreter() await di.run("Run data analysis on sklearn Iris
+dataset, include a plot") asyncio.run(main()) # or await main() in a jupyter
+notebook setting ``` ### QuickStart & Demo Video - Try it on [MetaGPT
+Huggingface Space](https://huggingface.co/spaces/deepwisdom/MetaGPT) - [Matthew
+Berman: How To Install MetaGPT - Build A Startup With One Prompt!!](https://
+youtu.be/uT75J_KG_aY) - [Official Demo Video](https://github.com/geekan/
+MetaGPT/assets/2707039/5e8c1062-8c35-440f-bb20-2b0320f8d27d) https://
 github.com/geekan/MetaGPT/assets/34952977/34345016-5d13-489d-b9f9-b82ace413419
 ## Tutorial - ð [Online Document](https://docs.deepwisdom.ai/main/en/) -
 ð» [Usage](https://docs.deepwisdom.ai/main/en/guide/get_started/
 quickstart.html) - ð [What can MetaGPT do?](https://docs.deepwisdom.ai/main/
 en/guide/get_started/introduction.html) - ð  How to build your own agents? -
 [MetaGPT Usage & Development Guide | Agent 101](https://docs.deepwisdom.ai/
 main/en/guide/tutorials/agent_101.html) - [MetaGPT Usage & Development Guide |
 MultiAgent 101](https://docs.deepwisdom.ai/main/en/guide/tutorials/
 multi_agent_101.html) - ð§âð» Contribution - [Develop Roadmap](docs/
-ROADMAP.md) - ð Use Cases - [Debate](https://docs.deepwisdom.ai/main/en/
-guide/use_cases/multi_agent/debate.html) - [Researcher](https://
-docs.deepwisdom.ai/main/en/guide/use_cases/agent/researcher.html) - [Recepit
-Assistant](https://docs.deepwisdom.ai/main/en/guide/use_cases/agent/
-receipt_assistant.html) - â [FAQs](https://docs.deepwisdom.ai/main/en/guide/
-faq.html) ## Support ### Discard Join US ð¢ Join Our [Discord Channel](https:
-//discord.gg/ZRHeExS6xv)! Looking forward to seeing you there! ð ### Contact
-Information If you have any questions or feedback about this project, please
-feel free to contact us. We highly appreciate your suggestions! - **Email:**
-alexanderwu@deepwisdom.ai - **GitHub Issues:** For more technical inquiries,
-you can also create a new issue in our [GitHub repository](https://github.com/
-geekan/metagpt/issues). We will respond to all questions within 2-3 business
-days. ## Citation For now, cite the [arXiv paper](https://arxiv.org/abs/
-2308.00352): ```bibtex @misc{hong2023metagpt, title={MetaGPT: Meta Programming
-for A Multi-Agent Collaborative Framework}, author={Sirui Hong and Mingchen
-Zhuge and Jonathan Chen and Xiawu Zheng and Yuheng Cheng and Ceyao Zhang and
-Jinlin Wang and Zili Wang and Steven Ka Shing Yau and Zijuan Lin and Liyang
-Zhou and Chenyu Ran and Lingfeng Xiao and Chenglin Wu and JÃ¼rgen Schmidhuber},
-year={2023}, eprint={2308.00352}, archivePrefix={arXiv}, primaryClass={cs.AI} }
-```
+ROADMAP.md) - ð Use Cases - [Data Interpreter](https://docs.deepwisdom.ai/
+main/en/guide/use_cases/agent/interpreter/intro.html) - [Debate](https://
+docs.deepwisdom.ai/main/en/guide/use_cases/multi_agent/debate.html) -
+[Researcher](https://docs.deepwisdom.ai/main/en/guide/use_cases/agent/
+researcher.html) - [Recepit Assistant](https://docs.deepwisdom.ai/main/en/
+guide/use_cases/agent/receipt_assistant.html) - â [FAQs](https://
+docs.deepwisdom.ai/main/en/guide/faq.html) ## Support ### Discard Join US ð¢
+Join Our [Discord Channel](https://discord.gg/ZRHeExS6xv)! Looking forward to
+seeing you there! ð ### Contact Information If you have any questions or
+feedback about this project, please feel free to contact us. We highly
+appreciate your suggestions! - **Email:** alexanderwu@deepwisdom.ai - **GitHub
+Issues:** For more technical inquiries, you can also create a new issue in our
+[GitHub repository](https://github.com/geekan/metagpt/issues). We will respond
+to all questions within 2-3 business days. ## Citation To stay updated with the
+latest research and development, follow [@MetaGPT_](https://twitter.com/
+MetaGPT_) on Twitter. To cite [MetaGPT](https://arxiv.org/abs/2308.00352) or
+[Data Interpreter](https://arxiv.org/abs/2402.18679) in publications, please
+use the following BibTeX entries. ```bibtex @misc{hong2023metagpt, title=
+{MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework}, author=
+{Sirui Hong and Mingchen Zhuge and Jonathan Chen and Xiawu Zheng and Yuheng
+Cheng and Ceyao Zhang and Jinlin Wang and Zili Wang and Steven Ka Shing Yau and
+Zijuan Lin and Liyang Zhou and Chenyu Ran and Lingfeng Xiao and Chenglin Wu and
+JÃ¼rgen Schmidhuber}, year={2023}, eprint={2308.00352}, archivePrefix={arXiv},
+primaryClass={cs.AI} } @misc{hong2024data, title={Data Interpreter: An LLM
+Agent For Data Science}, author={Sirui Hong and Yizhang Lin and Bang Liu and
+Bangbang Liu and Binhao Wu and Danyang Li and Jiaqi Chen and Jiayi Zhang and
+Jinlin Wang and Li Zhang and Lingyao Zhang and Min Yang and Mingchen Zhuge and
+Taicheng Guo and Tuo Zhou and Wei Tao and Wenyi Wang and Xiangru Tang and
+Xiangtao Lu and Xiawu Zheng and Xinbing Liang and Yaying Fei and Yuheng Cheng
+and Zongze Xu and Chenglin Wu}, year={2024}, eprint={2402.18679},
+archivePrefix={arXiv}, primaryClass={cs.AI} } ```
```

### Comparing `metagpt-0.7.7/README.md` & `metagpt-0.8.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 <p align="center">
    <a href="https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/geekan/MetaGPT"><img src="https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode" alt="Open in Dev Containers"></a>
    <a href="https://codespaces.new/geekan/MetaGPT"><img src="https://img.shields.io/badge/Github_Codespace-Open-blue?logo=github" alt="Open in GitHub Codespaces"></a>
    <a href="https://huggingface.co/spaces/deepwisdom/MetaGPT" target="_blank"><img alt="Hugging Face" src="https://img.shields.io/badge/%F0%9F%A4%97%20-Hugging%20Face-blue?color=blue&logoColor=white" /></a>
 </p>
 
 ## News
-🚀 March. 01, 2024: Our Data Interpreter paper is on arxiv. Find all design and benchmark details [here](https://arxiv.org/abs/2402.18679)!
+🚀 Mar. 29, 2024: [v0.8.0](https://github.com/geekan/MetaGPT/releases/tag/v0.8.0) released. Now you can use Data Interpreter via pypi package import. Meanwhile, we integrated RAG module and supported multiple new LLMs.
+
+🚀 Mar. 14, 2024: Our **Data Interpreter** paper is on [arxiv](https://arxiv.org/abs/2402.18679). Check the [example](https://docs.deepwisdom.ai/main/en/DataInterpreter/) and [code](https://github.com/geekan/MetaGPT/tree/main/examples/di)!
 
 🚀 Feb. 08, 2024: [v0.7.0](https://github.com/geekan/MetaGPT/releases/tag/v0.7.0) released, supporting assigning different LLMs to different Roles. We also introduced [Data Interpreter](https://github.com/geekan/MetaGPT/blob/main/examples/di/README.md), a powerful agent capable of solving a wide range of real-world problems.
 
 🚀 Jan. 16, 2024: Our paper [MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework
 ](https://arxiv.org/abs/2308.00352) accepted for oral presentation **(top 1.2%)** at ICLR 2024, **ranking #1** in the LLM-based Agent category.
 
 🚀 Jan. 03, 2024: [v0.6.0](https://github.com/geekan/MetaGPT/releases/tag/v0.6.0) released, new features include serialization, upgraded OpenAI package and supported multiple LLM, provided [minimal example for debate](https://github.com/geekan/MetaGPT/blob/main/examples/debate_simple.py) etc.
@@ -51,57 +53,77 @@
 2. Internally, MetaGPT includes **product managers / architects / project managers / engineers.** It provides the entire process of a **software company along with carefully orchestrated SOPs.**
    1. `Code = SOP(Team)` is the core philosophy. We materialize SOP and apply it to teams composed of LLMs.
 
 ![A software company consists of LLM-based roles](docs/resources/software_company_cd.jpeg)
 
 <p align="center">Software Company Multi-Agent Schematic (Gradually Implementing)</p>
 
-## Install
+## Get Started
 
-### Pip installation
+### Installation
 
 > Ensure that Python 3.9+ is installed on your system. You can check this by using: `python --version`.  
 > You can use conda like this: `conda create -n metagpt python=3.9 && conda activate metagpt`
 
 ```bash
-pip install metagpt
-metagpt --init-config  # create ~/.metagpt/config2.yaml, modify it to your own config
+pip install --upgrade metagpt
+# or `pip install --upgrade git+https://github.com/geekan/MetaGPT.git`
+# or `git clone https://github.com/geekan/MetaGPT && cd MetaGPT && pip install --upgrade -e .`
+```
+
+For detailed installation guidance, please refer to [cli_install](https://docs.deepwisdom.ai/main/en/guide/get_started/installation.html#install-stable-version)
+ or [docker_install](https://docs.deepwisdom.ai/main/en/guide/get_started/installation.html#install-with-docker)
+
+### Configuration
+
+You can init the config of MetaGPT by running the following command, or manually create `~/.metagpt/config2.yaml` file:
+```bash
+# Check https://docs.deepwisdom.ai/main/en/guide/get_started/configuration.html for more details
+metagpt --init-config  # it will create ~/.metagpt/config2.yaml, just modify it to your needs
+```
+
+You can configure `~/.metagpt/config2.yaml` according to the [example](https://github.com/geekan/MetaGPT/blob/main/config/config2.example.yaml) and [doc](https://docs.deepwisdom.ai/main/en/guide/get_started/configuration.html):
+
+```yaml
+llm:
+  api_type: "openai"  # or azure / ollama / open_llm etc. Check LLMType for more options
+  model: "gpt-4-turbo-preview"  # or gpt-3.5-turbo-1106 / gpt-4-1106-preview
+  base_url: "https://api.openai.com/v1"  # or forward url / other llm url
+  api_key: "YOUR_API_KEY"
+```
+
+### Usage
+
+After installation, you can use MetaGPT at CLI
+
+```bash
 metagpt "Create a 2048 game"  # this will create a repo in ./workspace
 ```
 
-or you can use it as library
+or use it as library
 
 ```python
 from metagpt.software_company import generate_repo, ProjectRepo
 repo: ProjectRepo = generate_repo("Create a 2048 game")  # or ProjectRepo("<path>")
 print(repo)  # it will print the repo structure with files
 ```
 
-detail installation please refer to [cli_install](https://docs.deepwisdom.ai/main/en/guide/get_started/installation.html#install-stable-version)
+You can also use its [Data Interpreter](https://github.com/geekan/MetaGPT/tree/main/examples/di)
+
+```python
+import asyncio
+from metagpt.roles.di.data_interpreter import DataInterpreter
 
-### Docker installation
-> Note: In the Windows, you need to replace "/opt/metagpt" with a directory that Docker has permission to create, such as "D:\Users\x\metagpt"
+async def main():
+    di = DataInterpreter()
+    await di.run("Run data analysis on sklearn Iris dataset, include a plot")
 
-```bash
-# Step 1: Download metagpt official image and prepare config2.yaml
-docker pull metagpt/metagpt:latest
-mkdir -p /opt/metagpt/{config,workspace}
-docker run --rm metagpt/metagpt:latest cat /app/metagpt/config/config2.yaml > /opt/metagpt/config/config2.yaml
-vim /opt/metagpt/config/config2.yaml # Change the config
-
-# Step 2: Run metagpt demo with container
-docker run --rm \
-    --privileged \
-    -v /opt/metagpt/config/config2.yaml:/app/metagpt/config/config2.yaml \
-    -v /opt/metagpt/workspace:/app/metagpt/workspace \
-    metagpt/metagpt:latest \
-    metagpt "Create a 2048 game"
+asyncio.run(main())  # or await main() in a jupyter notebook setting
 ```
 
-detail installation please refer to [docker_install](https://docs.deepwisdom.ai/main/en/guide/get_started/installation.html#install-with-docker)
 
 ### QuickStart & Demo Video
 - Try it on [MetaGPT Huggingface Space](https://huggingface.co/spaces/deepwisdom/MetaGPT)
 - [Matthew Berman: How To Install MetaGPT - Build A Startup With One Prompt!!](https://youtu.be/uT75J_KG_aY)
 - [Official Demo Video](https://github.com/geekan/MetaGPT/assets/2707039/5e8c1062-8c35-440f-bb20-2b0320f8d27d)
 
 https://github.com/geekan/MetaGPT/assets/34952977/34345016-5d13-489d-b9f9-b82ace413419
@@ -113,14 +135,15 @@
 - 🔎 [What can MetaGPT do?](https://docs.deepwisdom.ai/main/en/guide/get_started/introduction.html)
 - 🛠 How to build your own agents? 
   - [MetaGPT Usage & Development Guide | Agent 101](https://docs.deepwisdom.ai/main/en/guide/tutorials/agent_101.html)
   - [MetaGPT Usage & Development Guide | MultiAgent 101](https://docs.deepwisdom.ai/main/en/guide/tutorials/multi_agent_101.html)
 - 🧑‍💻 Contribution
   - [Develop Roadmap](docs/ROADMAP.md)
 - 🔖 Use Cases
+  - [Data Interpreter](https://docs.deepwisdom.ai/main/en/guide/use_cases/agent/interpreter/intro.html)
   - [Debate](https://docs.deepwisdom.ai/main/en/guide/use_cases/multi_agent/debate.html)
   - [Researcher](https://docs.deepwisdom.ai/main/en/guide/use_cases/agent/researcher.html)
   - [Recepit Assistant](https://docs.deepwisdom.ai/main/en/guide/use_cases/agent/receipt_assistant.html)
 - ❓ [FAQs](https://docs.deepwisdom.ai/main/en/guide/faq.html)
 
 ## Support
 
@@ -136,19 +159,31 @@
 - **Email:** alexanderwu@deepwisdom.ai
 - **GitHub Issues:** For more technical inquiries, you can also create a new issue in our [GitHub repository](https://github.com/geekan/metagpt/issues).
 
 We will respond to all questions within 2-3 business days.
 
 ## Citation
 
-For now, cite the [arXiv paper](https://arxiv.org/abs/2308.00352):
+To stay updated with the latest research and development, follow [@MetaGPT_](https://twitter.com/MetaGPT_) on Twitter. 
+
+To cite [MetaGPT](https://arxiv.org/abs/2308.00352) or [Data Interpreter](https://arxiv.org/abs/2402.18679) in publications, please use the following BibTeX entries.
 
 ```bibtex
 @misc{hong2023metagpt,
       title={MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework}, 
       author={Sirui Hong and Mingchen Zhuge and Jonathan Chen and Xiawu Zheng and Yuheng Cheng and Ceyao Zhang and Jinlin Wang and Zili Wang and Steven Ka Shing Yau and Zijuan Lin and Liyang Zhou and Chenyu Ran and Lingfeng Xiao and Chenglin Wu and Jürgen Schmidhuber},
       year={2023},
       eprint={2308.00352},
       archivePrefix={arXiv},
       primaryClass={cs.AI}
 }
+@misc{hong2024data,
+      title={Data Interpreter: An LLM Agent For Data Science}, 
+      author={Sirui Hong and Yizhang Lin and Bang Liu and Bangbang Liu and Binhao Wu and Danyang Li and Jiaqi Chen and Jiayi Zhang and Jinlin Wang and Li Zhang and Lingyao Zhang and Min Yang and Mingchen Zhuge and Taicheng Guo and Tuo Zhou and Wei Tao and Wenyi Wang and Xiangru Tang and Xiangtao Lu and Xiawu Zheng and Xinbing Liang and Yaying Fei and Yuheng Cheng and Zongze Xu and Chenglin Wu},
+      year={2024},
+      eprint={2402.18679},
+      archivePrefix={arXiv},
+      primaryClass={cs.AI}
+}
+
 ```
+
```

#### html2text {}

```diff
@@ -1,28 +1,32 @@
 # MetaGPT: The Multi-Agent Framework
 [MetaGPT logo: Enable GPT to work in software company, collaborating to tackle
                              more complex tasks.]
    AAssssiiggnn ddiiffffeerreenntt rroolleess ttoo GGPPTTss ttoo ffoorrmm aa ccoollllaabboorraattiivvee eennttiittyy ffoorr ccoommpplleexx
                                     ttaasskkss..
 _[_C_N_ _d_o_c_]_[_E_N_ _d_o_c_]_[_J_A_ _d_o_c_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]_[_r_o_a_d_m_a_p_]_[_D_i_s_c_o_r_d_ _F_o_l_l_o_w_]_[_T_w_i_t_t_e_r_ _F_o_l_l_o_w_]
        _[_O_p_e_n_ _i_n_ _D_e_v_ _C_o_n_t_a_i_n_e_r_s_]_[_O_p_e_n_ _i_n_ _G_i_t_H_u_b_ _C_o_d_e_s_p_a_c_e_s_]_[_H_u_g_g_i_n_g_ _F_a_c_e_]
-## News ð March. 01, 2024: Our Data Interpreter paper is on arxiv. Find all
-design and benchmark details [here](https://arxiv.org/abs/2402.18679)! ð
-Feb. 08, 2024: [v0.7.0](https://github.com/geekan/MetaGPT/releases/tag/v0.7.0)
-released, supporting assigning different LLMs to different Roles. We also
-introduced [Data Interpreter](https://github.com/geekan/MetaGPT/blob/main/
-examples/di/README.md), a powerful agent capable of solving a wide range of
-real-world problems. ð Jan. 16, 2024: Our paper [MetaGPT: Meta Programming
-for A Multi-Agent Collaborative Framework ](https://arxiv.org/abs/2308.00352)
-accepted for oral presentation **(top 1.2%)** at ICLR 2024, **ranking #1** in
-the LLM-based Agent category. ð Jan. 03, 2024: [v0.6.0](https://github.com/
-geekan/MetaGPT/releases/tag/v0.6.0) released, new features include
-serialization, upgraded OpenAI package and supported multiple LLM, provided
-[minimal example for debate](https://github.com/geekan/MetaGPT/blob/main/
-examples/debate_simple.py) etc. ð Dec. 15, 2023: [v0.5.0](https://
+## News ð Mar. 29, 2024: [v0.8.0](https://github.com/geekan/MetaGPT/
+releases/tag/v0.8.0) released. Now you can use Data Interpreter via pypi
+package import. Meanwhile, we integrated RAG module and supported multiple new
+LLMs. ð Mar. 14, 2024: Our **Data Interpreter** paper is on [arxiv](https://
+arxiv.org/abs/2402.18679). Check the [example](https://docs.deepwisdom.ai/main/
+en/DataInterpreter/) and [code](https://github.com/geekan/MetaGPT/tree/main/
+examples/di)! ð Feb. 08, 2024: [v0.7.0](https://github.com/geekan/MetaGPT/
+releases/tag/v0.7.0) released, supporting assigning different LLMs to different
+Roles. We also introduced [Data Interpreter](https://github.com/geekan/MetaGPT/
+blob/main/examples/di/README.md), a powerful agent capable of solving a wide
+range of real-world problems. ð Jan. 16, 2024: Our paper [MetaGPT: Meta
+Programming for A Multi-Agent Collaborative Framework ](https://arxiv.org/abs/
+2308.00352) accepted for oral presentation **(top 1.2%)** at ICLR 2024,
+**ranking #1** in the LLM-based Agent category. ð Jan. 03, 2024: [v0.6.0]
+(https://github.com/geekan/MetaGPT/releases/tag/v0.6.0) released, new features
+include serialization, upgraded OpenAI package and supported multiple LLM,
+provided [minimal example for debate](https://github.com/geekan/MetaGPT/blob/
+main/examples/debate_simple.py) etc. ð Dec. 15, 2023: [v0.5.0](https://
 github.com/geekan/MetaGPT/releases/tag/v0.5.0) released, introducing some
 experimental features such as **incremental development**, **multilingual**,
 **multiple programming languages**, etc. ð¥ Nov. 08, 2023: MetaGPT is
 selected into [Open100: Top 100 Open Source achievements](https://
 www.benchcouncil.org/evaluation/opencs/annual.html). ð¥ Sep. 01, 2023:
 MetaGPT tops GitHub Trending Monthly for the **17th time** in August 2023. ð
 Jun. 30, 2023: MetaGPT is now open source. ð Apr. 24, 2023: First line of
@@ -32,63 +36,82 @@
 etc.** 2. Internally, MetaGPT includes **product managers / architects /
 project managers / engineers.** It provides the entire process of a **software
 company along with carefully orchestrated SOPs.** 1. `Code = SOP(Team)` is the
 core philosophy. We materialize SOP and apply it to teams composed of LLMs. ![A
 software company consists of LLM-based roles](docs/resources/
 software_company_cd.jpeg)
         Software Company Multi-Agent Schematic (Gradually Implementing)
-## Install ### Pip installation > Ensure that Python 3.9+ is installed on your
+## Get Started ### Installation > Ensure that Python 3.9+ is installed on your
 system. You can check this by using: `python --version`. > You can use conda
 like this: `conda create -n metagpt python=3.9 && conda activate metagpt`
-```bash pip install metagpt metagpt --init-config # create ~/.metagpt/
-config2.yaml, modify it to your own config metagpt "Create a 2048 game" # this
-will create a repo in ./workspace ``` or you can use it as library ```python
-from metagpt.software_company import generate_repo, ProjectRepo repo:
-ProjectRepo = generate_repo("Create a 2048 game") # or ProjectRepo("") print
-(repo) # it will print the repo structure with files ``` detail installation
-please refer to [cli_install](https://docs.deepwisdom.ai/main/en/guide/
-get_started/installation.html#install-stable-version) ### Docker installation >
-Note: In the Windows, you need to replace "/opt/metagpt" with a directory that
-Docker has permission to create, such as "D:\Users\x\metagpt" ```bash # Step 1:
-Download metagpt official image and prepare config2.yaml docker pull metagpt/
-metagpt:latest mkdir -p /opt/metagpt/{config,workspace} docker run --rm
-metagpt/metagpt:latest cat /app/metagpt/config/config2.yaml > /opt/metagpt/
-config/config2.yaml vim /opt/metagpt/config/config2.yaml # Change the config #
-Step 2: Run metagpt demo with container docker run --rm \ --privileged \ -v /
-opt/metagpt/config/config2.yaml:/app/metagpt/config/config2.yaml \ -v /opt/
-metagpt/workspace:/app/metagpt/workspace \ metagpt/metagpt:latest \ metagpt
-"Create a 2048 game" ``` detail installation please refer to [docker_install]
-(https://docs.deepwisdom.ai/main/en/guide/get_started/
-installation.html#install-with-docker) ### QuickStart & Demo Video - Try it on
-[MetaGPT Huggingface Space](https://huggingface.co/spaces/deepwisdom/MetaGPT) -
-[Matthew Berman: How To Install MetaGPT - Build A Startup With One Prompt!!]
-(https://youtu.be/uT75J_KG_aY) - [Official Demo Video](https://github.com/
-geekan/MetaGPT/assets/2707039/5e8c1062-8c35-440f-bb20-2b0320f8d27d) https://
+```bash pip install --upgrade metagpt # or `pip install --upgrade git+https://
+github.com/geekan/MetaGPT.git` # or `git clone https://github.com/geekan/
+MetaGPT && cd MetaGPT && pip install --upgrade -e .` ``` For detailed
+installation guidance, please refer to [cli_install](https://
+docs.deepwisdom.ai/main/en/guide/get_started/installation.html#install-stable-
+version) or [docker_install](https://docs.deepwisdom.ai/main/en/guide/
+get_started/installation.html#install-with-docker) ### Configuration You can
+init the config of MetaGPT by running the following command, or manually create
+`~/.metagpt/config2.yaml` file: ```bash # Check https://docs.deepwisdom.ai/
+main/en/guide/get_started/configuration.html for more details metagpt --init-
+config # it will create ~/.metagpt/config2.yaml, just modify it to your needs
+``` You can configure `~/.metagpt/config2.yaml` according to the [example]
+(https://github.com/geekan/MetaGPT/blob/main/config/config2.example.yaml) and
+[doc](https://docs.deepwisdom.ai/main/en/guide/get_started/configuration.html):
+```yaml llm: api_type: "openai" # or azure / ollama / open_llm etc. Check
+LLMType for more options model: "gpt-4-turbo-preview" # or gpt-3.5-turbo-1106 /
+gpt-4-1106-preview base_url: "https://api.openai.com/v1" # or forward url /
+other llm url api_key: "YOUR_API_KEY" ``` ### Usage After installation, you can
+use MetaGPT at CLI ```bash metagpt "Create a 2048 game" # this will create a
+repo in ./workspace ``` or use it as library ```python from
+metagpt.software_company import generate_repo, ProjectRepo repo: ProjectRepo =
+generate_repo("Create a 2048 game") # or ProjectRepo("") print(repo) # it will
+print the repo structure with files ``` You can also use its [Data Interpreter]
+(https://github.com/geekan/MetaGPT/tree/main/examples/di) ```python import
+asyncio from metagpt.roles.di.data_interpreter import DataInterpreter async def
+main(): di = DataInterpreter() await di.run("Run data analysis on sklearn Iris
+dataset, include a plot") asyncio.run(main()) # or await main() in a jupyter
+notebook setting ``` ### QuickStart & Demo Video - Try it on [MetaGPT
+Huggingface Space](https://huggingface.co/spaces/deepwisdom/MetaGPT) - [Matthew
+Berman: How To Install MetaGPT - Build A Startup With One Prompt!!](https://
+youtu.be/uT75J_KG_aY) - [Official Demo Video](https://github.com/geekan/
+MetaGPT/assets/2707039/5e8c1062-8c35-440f-bb20-2b0320f8d27d) https://
 github.com/geekan/MetaGPT/assets/34952977/34345016-5d13-489d-b9f9-b82ace413419
 ## Tutorial - ð [Online Document](https://docs.deepwisdom.ai/main/en/) -
 ð» [Usage](https://docs.deepwisdom.ai/main/en/guide/get_started/
 quickstart.html) - ð [What can MetaGPT do?](https://docs.deepwisdom.ai/main/
 en/guide/get_started/introduction.html) - ð  How to build your own agents? -
 [MetaGPT Usage & Development Guide | Agent 101](https://docs.deepwisdom.ai/
 main/en/guide/tutorials/agent_101.html) - [MetaGPT Usage & Development Guide |
 MultiAgent 101](https://docs.deepwisdom.ai/main/en/guide/tutorials/
 multi_agent_101.html) - ð§âð» Contribution - [Develop Roadmap](docs/
-ROADMAP.md) - ð Use Cases - [Debate](https://docs.deepwisdom.ai/main/en/
-guide/use_cases/multi_agent/debate.html) - [Researcher](https://
-docs.deepwisdom.ai/main/en/guide/use_cases/agent/researcher.html) - [Recepit
-Assistant](https://docs.deepwisdom.ai/main/en/guide/use_cases/agent/
-receipt_assistant.html) - â [FAQs](https://docs.deepwisdom.ai/main/en/guide/
-faq.html) ## Support ### Discard Join US ð¢ Join Our [Discord Channel](https:
-//discord.gg/ZRHeExS6xv)! Looking forward to seeing you there! ð ### Contact
-Information If you have any questions or feedback about this project, please
-feel free to contact us. We highly appreciate your suggestions! - **Email:**
-alexanderwu@deepwisdom.ai - **GitHub Issues:** For more technical inquiries,
-you can also create a new issue in our [GitHub repository](https://github.com/
-geekan/metagpt/issues). We will respond to all questions within 2-3 business
-days. ## Citation For now, cite the [arXiv paper](https://arxiv.org/abs/
-2308.00352): ```bibtex @misc{hong2023metagpt, title={MetaGPT: Meta Programming
-for A Multi-Agent Collaborative Framework}, author={Sirui Hong and Mingchen
-Zhuge and Jonathan Chen and Xiawu Zheng and Yuheng Cheng and Ceyao Zhang and
-Jinlin Wang and Zili Wang and Steven Ka Shing Yau and Zijuan Lin and Liyang
-Zhou and Chenyu Ran and Lingfeng Xiao and Chenglin Wu and JÃ¼rgen Schmidhuber},
-year={2023}, eprint={2308.00352}, archivePrefix={arXiv}, primaryClass={cs.AI} }
-```
+ROADMAP.md) - ð Use Cases - [Data Interpreter](https://docs.deepwisdom.ai/
+main/en/guide/use_cases/agent/interpreter/intro.html) - [Debate](https://
+docs.deepwisdom.ai/main/en/guide/use_cases/multi_agent/debate.html) -
+[Researcher](https://docs.deepwisdom.ai/main/en/guide/use_cases/agent/
+researcher.html) - [Recepit Assistant](https://docs.deepwisdom.ai/main/en/
+guide/use_cases/agent/receipt_assistant.html) - â [FAQs](https://
+docs.deepwisdom.ai/main/en/guide/faq.html) ## Support ### Discard Join US ð¢
+Join Our [Discord Channel](https://discord.gg/ZRHeExS6xv)! Looking forward to
+seeing you there! ð ### Contact Information If you have any questions or
+feedback about this project, please feel free to contact us. We highly
+appreciate your suggestions! - **Email:** alexanderwu@deepwisdom.ai - **GitHub
+Issues:** For more technical inquiries, you can also create a new issue in our
+[GitHub repository](https://github.com/geekan/metagpt/issues). We will respond
+to all questions within 2-3 business days. ## Citation To stay updated with the
+latest research and development, follow [@MetaGPT_](https://twitter.com/
+MetaGPT_) on Twitter. To cite [MetaGPT](https://arxiv.org/abs/2308.00352) or
+[Data Interpreter](https://arxiv.org/abs/2402.18679) in publications, please
+use the following BibTeX entries. ```bibtex @misc{hong2023metagpt, title=
+{MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework}, author=
+{Sirui Hong and Mingchen Zhuge and Jonathan Chen and Xiawu Zheng and Yuheng
+Cheng and Ceyao Zhang and Jinlin Wang and Zili Wang and Steven Ka Shing Yau and
+Zijuan Lin and Liyang Zhou and Chenyu Ran and Lingfeng Xiao and Chenglin Wu and
+JÃ¼rgen Schmidhuber}, year={2023}, eprint={2308.00352}, archivePrefix={arXiv},
+primaryClass={cs.AI} } @misc{hong2024data, title={Data Interpreter: An LLM
+Agent For Data Science}, author={Sirui Hong and Yizhang Lin and Bang Liu and
+Bangbang Liu and Binhao Wu and Danyang Li and Jiaqi Chen and Jiayi Zhang and
+Jinlin Wang and Li Zhang and Lingyao Zhang and Min Yang and Mingchen Zhuge and
+Taicheng Guo and Tuo Zhou and Wei Tao and Wenyi Wang and Xiangru Tang and
+Xiangtao Lu and Xiawu Zheng and Xinbing Liang and Yaying Fei and Yuheng Cheng
+and Zongze Xu and Chenglin Wu}, year={2024}, eprint={2402.18679},
+archivePrefix={arXiv}, primaryClass={cs.AI} } ```
```

### Comparing `metagpt-0.7.7/metagpt/_compat.py` & `metagpt-0.8.0/metagpt/_compat.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/__init__.py` & `metagpt-0.8.0/metagpt/actions/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from metagpt.actions.search_and_summarize import SearchAndSummarize
 from metagpt.actions.write_code import WriteCode
 from metagpt.actions.write_code_review import WriteCodeReview
 from metagpt.actions.write_prd import WritePRD
 from metagpt.actions.write_prd_review import WritePRDReview
 from metagpt.actions.write_test import WriteTest
 from metagpt.actions.di.execute_nb_code import ExecuteNbCode
-from metagpt.actions.di.write_analysis_code import WriteCodeWithoutTools, WriteCodeWithTools
+from metagpt.actions.di.write_analysis_code import WriteAnalysisCode
 from metagpt.actions.di.write_plan import WritePlan
 
 
 class ActionType(Enum):
     """All types of Actions, used for indexing."""
 
     ADD_REQUIREMENT = UserRequirement
@@ -42,16 +42,15 @@
     DEBUG_ERROR = DebugError
     WRITE_TASKS = WriteTasks
     SEARCH_AND_SUMMARIZE = SearchAndSummarize
     COLLECT_LINKS = CollectLinks
     WEB_BROWSE_AND_SUMMARIZE = WebBrowseAndSummarize
     CONDUCT_RESEARCH = ConductResearch
     EXECUTE_NB_CODE = ExecuteNbCode
-    WRITE_CODE_WITHOUT_TOOLS = WriteCodeWithoutTools
-    WRITE_CODE_WITH_TOOLS = WriteCodeWithTools
+    WRITE_ANALYSIS_CODE = WriteAnalysisCode
     WRITE_PLAN = WritePlan
 
 
 __all__ = [
     "ActionType",
     "Action",
     "ActionOutput",
```

### Comparing `metagpt-0.7.7/metagpt/actions/action.py` & `metagpt-0.8.0/metagpt/actions/action.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/action_graph.py` & `metagpt-0.8.0/metagpt/actions/action_graph.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/action_node.py` & `metagpt-0.8.0/metagpt/actions/action_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 from pydantic import BaseModel, Field, create_model, model_validator
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 
 from metagpt.actions.action_outcls_registry import register_action_outcls
+from metagpt.const import USE_CONFIG_TIMEOUT
 from metagpt.llm import BaseLLM
 from metagpt.logs import logger
 from metagpt.provider.postprocess.llm_output_postprocess import llm_output_postprocess
 from metagpt.utils.common import OutputParser, general_after_log
 from metagpt.utils.human_interaction import HumanInteraction
 
 
@@ -326,27 +327,24 @@
 
         for _, child_node in self.children.items():
             keys.append(child_node.key)
         return keys
 
     def compile_to(self, i: Dict, schema, kv_sep) -> str:
         if schema == "json":
-            return json.dumps(i, indent=4)
+            return json.dumps(i, indent=4, ensure_ascii=False)
         elif schema == "markdown":
             return dict_to_markdown(i, kv_sep=kv_sep)
         else:
             return str(i)
 
     def tagging(self, text, schema, tag="") -> str:
         if not tag:
             return text
-        if schema == "json":
-            return f"[{tag}]\n" + text + f"\n[/{tag}]"
-        else:  # markdown
-            return f"[{tag}]\n" + text + f"\n[/{tag}]"
+        return f"[{tag}]\n{text}\n[/{tag}]"
 
     def _compile_f(self, schema, mode, tag, format_func, kv_sep, exclude=None) -> str:
         nodes = self.to_dict(format_func=format_func, mode=mode, exclude=exclude)
         text = self.compile_to(nodes, schema, kv_sep)
         return self.tagging(text, schema, tag)
 
     def compile_instruction(self, schema="markdown", mode="children", tag="", exclude=None) -> str:
@@ -370,15 +368,15 @@
             mode="root": NotImplemented
         schmea: raw/json/markdown
             schema="raw": 不编译，context, lang_constaint, instruction
             schema="json"：编译context, example(json), instruction(markdown), constraint, action
             schema="markdown": 编译context, example(markdown), instruction(markdown), constraint, action
         """
         if schema == "raw":
-            return context + "\n\n## Actions\n" + LANGUAGE_CONSTRAINT + "\n" + self.instruction
+            return f"{context}\n\n## Actions\n{LANGUAGE_CONSTRAINT}\n{self.instruction}"
 
         ### 直接使用 pydantic BaseModel 生成 instruction 与 example，仅限 JSON
         # child_class = self._create_children_class()
         # node_schema = child_class.model_json_schema()
         # defaults = {
         #     k: str(v)
         #     for k, v in child_class.model_fields.items()
@@ -412,15 +410,15 @@
         self,
         prompt: str,
         output_class_name: str,
         output_data_mapping: dict,
         images: Optional[Union[str, list[str]]] = None,
         system_msgs: Optional[list[str]] = None,
         schema="markdown",  # compatible to original format
-        timeout=3,
+        timeout=USE_CONFIG_TIMEOUT,
     ) -> (str, BaseModel):
         """Use ActionOutput to wrap the output of aask"""
         content = await self.llm.aask(prompt, system_msgs, images=images, timeout=timeout)
         logger.debug(f"llm raw output:\n{content}")
         output_class = self.create_model_class(output_class_name, output_data_mapping)
 
         if schema == "json":
@@ -444,15 +442,17 @@
 
     def set_llm(self, llm):
         self.set_recursive("llm", llm)
 
     def set_context(self, context):
         self.set_recursive("context", context)
 
-    async def simple_fill(self, schema, mode, images: Optional[Union[str, list[str]]] = None, timeout=3, exclude=None):
+    async def simple_fill(
+        self, schema, mode, images: Optional[Union[str, list[str]]] = None, timeout=USE_CONFIG_TIMEOUT, exclude=None
+    ):
         prompt = self.compile(context=self.context, schema=schema, mode=mode, exclude=exclude)
 
         if schema != "raw":
             mapping = self.get_mapping(mode, exclude=exclude)
             class_name = f"{self.key}_AN"
             content, scontent = await self._aask_v1(
                 prompt, class_name, mapping, images=images, schema=schema, timeout=timeout
@@ -469,15 +469,15 @@
         self,
         context,
         llm,
         schema="json",
         mode="auto",
         strgy="simple",
         images: Optional[Union[str, list[str]]] = None,
-        timeout=3,
+        timeout=USE_CONFIG_TIMEOUT,
         exclude=[],
     ):
         """Fill the node(s) with mode.
 
         :param context: Everything we should know when filling node.
         :param llm: Large Language Model with pre-defined system message.
         :param schema: json/markdown, determine example and output format.
```

### Comparing `metagpt-0.7.7/metagpt/actions/action_outcls_registry.py` & `metagpt-0.8.0/metagpt/actions/action_outcls_registry.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/debug_error.py` & `metagpt-0.8.0/metagpt/actions/debug_error.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/design_api.py` & `metagpt-0.8.0/metagpt/actions/design_api.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/design_api_an.py` & `metagpt-0.8.0/metagpt/actions/design_api_an.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 @Time    : 2023/12/12 22:24
 @Author  : alexanderwu
 @File    : design_api_an.py
 """
 from typing import List
 
 from metagpt.actions.action_node import ActionNode
-from metagpt.logs import logger
 from metagpt.utils.mermaid import MMC1, MMC2
 
 IMPLEMENTATION_APPROACH = ActionNode(
     key="Implementation approach",
     expected_type=str,
     instruction="Analyze the difficult points of the requirements, select the appropriate open-source framework",
     example="We will ...",
@@ -105,18 +104,7 @@
     REFINED_DATA_STRUCTURES_AND_INTERFACES,
     REFINED_PROGRAM_CALL_FLOW,
     ANYTHING_UNCLEAR,
 ]
 
 DESIGN_API_NODE = ActionNode.from_children("DesignAPI", NODES)
 REFINED_DESIGN_NODE = ActionNode.from_children("RefinedDesignAPI", REFINED_NODES)
-
-
-def main():
-    prompt = DESIGN_API_NODE.compile(context="")
-    logger.info(prompt)
-    prompt = REFINED_DESIGN_NODE.compile(context="")
-    logger.info(prompt)
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `metagpt-0.7.7/metagpt/actions/design_api_review.py` & `metagpt-0.8.0/metagpt/actions/design_api_review.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/di/ask_review.py` & `metagpt-0.8.0/metagpt/actions/di/ask_review.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/di/execute_nb_code.py` & `metagpt-0.8.0/metagpt/actions/di/execute_nb_code.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 @File    :   execute_nb_code.py
 """
 from __future__ import annotations
 
 import asyncio
 import base64
 import re
-import traceback
 from typing import Literal, Tuple
 
 import nbformat
 from nbclient import NotebookClient
 from nbclient.exceptions import CellTimeoutError, DeadKernelError
 from nbformat import NotebookNode
 from nbformat.v4 import new_code_cell, new_markdown_cell, new_output
@@ -54,15 +53,31 @@
         if self.nb_client.kc is None or not await self.nb_client.kc.is_alive():
             self.nb_client.create_kernel_manager()
             self.nb_client.start_new_kernel()
             self.nb_client.start_new_kernel_client()
 
     async def terminate(self):
         """kill NotebookClient"""
-        await self.nb_client._async_cleanup_kernel()
+        if self.nb_client.km is not None and await self.nb_client.km.is_alive():
+            await self.nb_client.km.shutdown_kernel(now=True)
+            await self.nb_client.km.cleanup_resources()
+
+            channels = [
+                self.nb_client.kc.stdin_channel,  # The channel for handling standard input to the kernel.
+                self.nb_client.kc.hb_channel,  # The channel for heartbeat communication between the kernel and client.
+                self.nb_client.kc.control_channel,  # The channel for controlling the kernel.
+            ]
+
+            # Stops all the running channels for this kernel
+            for channel in channels:
+                if channel.is_alive():
+                    channel.stop()
+
+            self.nb_client.kc = None
+            self.nb_client.km = None
 
     async def reset(self):
         """reset NotebookClient"""
         await self.terminate()
 
         # sleep 1s to wait for the kernel to be cleaned up completely
         await asyncio.sleep(1)
@@ -87,35 +102,49 @@
     def add_output_to_cell(self, cell: NotebookNode, output: str):
         """add outputs of code execution to notebook cell."""
         if "outputs" not in cell:
             cell["outputs"] = []
         else:
             cell["outputs"].append(new_output(output_type="stream", name="stdout", text=str(output)))
 
-    def parse_outputs(self, outputs: list[str]) -> str:
+    def parse_outputs(self, outputs: list[str], keep_len: int = 2000) -> Tuple[bool, str]:
         """Parses the outputs received from notebook execution."""
         assert isinstance(outputs, list)
-        parsed_output = ""
-
+        parsed_output, is_success = [], True
         for i, output in enumerate(outputs):
+            output_text = ""
             if output["output_type"] == "stream" and not any(
                 tag in output["text"]
                 for tag in ["| INFO     | metagpt", "| ERROR    | metagpt", "| WARNING  | metagpt", "DEBUG"]
             ):
-                parsed_output += output["text"]
+                output_text = output["text"]
             elif output["output_type"] == "display_data":
                 if "image/png" in output["data"]:
                     self.show_bytes_figure(output["data"]["image/png"], self.interaction)
                 else:
                     logger.info(
                         f"{i}th output['data'] from nbclient outputs dont have image/png, continue next output ..."
                     )
             elif output["output_type"] == "execute_result":
-                parsed_output += output["data"]["text/plain"]
-        return parsed_output
+                output_text = output["data"]["text/plain"]
+            elif output["output_type"] == "error":
+                output_text, is_success = "\n".join(output["traceback"]), False
+
+            # handle coroutines that are not executed asynchronously
+            if output_text.strip().startswith("<coroutine object"):
+                output_text = "Executed code failed, you need use key word 'await' to run a async code."
+                is_success = False
+
+            output_text = remove_escape_and_color_codes(output_text)
+            # The useful information of the exception is at the end,
+            # the useful information of normal output is at the begining.
+            output_text = output_text[:keep_len] if is_success else output_text[-keep_len:]
+
+            parsed_output.append(output_text)
+        return is_success, ",".join(parsed_output)
 
     def show_bytes_figure(self, image_base64: str, interaction_type: Literal["ipython", None]):
         image_bytes = base64.b64decode(image_base64)
         if interaction_type == "ipython":
             from IPython.display import Image, display
 
             display(Image(data=image_bytes))
@@ -141,26 +170,26 @@
 
     async def run_cell(self, cell: NotebookNode, cell_index: int) -> Tuple[bool, str]:
         """set timeout for run code.
         returns the success or failure of the cell execution, and an optional error message.
         """
         try:
             await self.nb_client.async_execute_cell(cell, cell_index)
-            return True, ""
+            return self.parse_outputs(self.nb.cells[-1].outputs)
         except CellTimeoutError:
             assert self.nb_client.km is not None
             await self.nb_client.km.interrupt_kernel()
             await asyncio.sleep(1)
             error_msg = "Cell execution timed out: Execution exceeded the time limit and was stopped; consider optimizing your code for better performance."
             return False, error_msg
         except DeadKernelError:
             await self.reset()
             return False, "DeadKernelError"
         except Exception:
-            return False, f"{traceback.format_exc()}"
+            return self.parse_outputs(self.nb.cells[-1].outputs)
 
     async def run(self, code: str, language: Literal["python", "markdown"] = "python") -> Tuple[str, bool]:
         """
         return the output of code execution, and a success indicator (bool) of code execution.
         """
         self._display(code, language)
 
@@ -169,22 +198,15 @@
             self.add_code_cell(code=code)
 
             # build code executor
             await self.build()
 
             # run code
             cell_index = len(self.nb.cells) - 1
-            success, error_message = await self.run_cell(self.nb.cells[-1], cell_index)
-
-            if not success:
-                return truncate(remove_escape_and_color_codes(error_message), is_success=success)
-
-            # code success
-            outputs = self.parse_outputs(self.nb.cells[-1].outputs)
-            outputs, success = truncate(remove_escape_and_color_codes(outputs), is_success=success)
+            success, outputs = await self.run_cell(self.nb.cells[-1], cell_index)
 
             if "!pip" in code:
                 success = False
 
             return outputs, success
 
         elif language == "markdown":
@@ -192,58 +214,43 @@
             self.add_markdown_cell(code)
             # return True, beacuse there is no execution failure for markdown cell.
             return code, True
         else:
             raise ValueError(f"Only support for language: python, markdown, but got {language}, ")
 
 
-def truncate(result: str, keep_len: int = 2000, is_success: bool = True):
-    """对于超出keep_len个字符的result: 执行失败的代码, 展示result后keep_len个字符; 执行成功的代码, 展示result前keep_len个字符。"""
-    if is_success:
-        desc = f"Executed code successfully. Truncated to show only first {keep_len} characters\n"
-    else:
-        desc = f"Executed code failed, please reflect the cause of bug and then debug. Truncated to show only last {keep_len} characters\n"
-
-    if result.strip().startswith("<coroutine object"):
-        result = "Executed code failed, you need use key word 'await' to run a async code."
-        return result, False
-
-    if len(result) > keep_len:
-        result = result[-keep_len:] if not is_success else result[:keep_len]
-        return desc + result, is_success
-
-    return result, is_success
-
-
 def remove_escape_and_color_codes(input_str: str):
-    # 使用正则表达式去除转义字符和颜色代码
+    # 使用正则表达式去除jupyter notebook输出结果中的转义字符和颜色代码
+    # Use regular expressions to get rid of escape characters and color codes in jupyter notebook output.
     pattern = re.compile(r"\x1b\[[0-9;]*[mK]")
     result = pattern.sub("", input_str)
     return result
 
 
 def display_markdown(content: str):
-    # 使用正则表达式逐个匹配代码块
+    # Use regular expressions to match blocks of code one by one.
     matches = re.finditer(r"```(.+?)```", content, re.DOTALL)
     start_index = 0
     content_panels = []
-    # 逐个打印匹配到的文本和代码
+    # Set the text background color and text color.
+    style = "black on white"
+    # Print the matching text and code one by one.
     for match in matches:
         text_content = content[start_index : match.start()].strip()
         code_content = match.group(0).strip()[3:-3]  # Remove triple backticks
 
         if text_content:
-            content_panels.append(Panel(Markdown(text_content), box=MINIMAL))
+            content_panels.append(Panel(Markdown(text_content), style=style, box=MINIMAL))
 
         if code_content:
-            content_panels.append(Panel(Markdown(f"```{code_content}"), box=MINIMAL))
+            content_panels.append(Panel(Markdown(f"```{code_content}"), style=style, box=MINIMAL))
         start_index = match.end()
 
-    # 打印剩余文本（如果有）
+    # Print remaining text (if any).
     remaining_text = content[start_index:].strip()
     if remaining_text:
-        content_panels.append(Panel(Markdown(remaining_text), box=MINIMAL))
+        content_panels.append(Panel(Markdown(remaining_text), style=style, box=MINIMAL))
 
-    # 在Live模式中显示所有Panel
+    # Display all panels in Live mode.
     with Live(auto_refresh=False, console=Console(), vertical_overflow="visible") as live:
         live.update(Group(*content_panels))
         live.refresh()
```

### Comparing `metagpt-0.7.7/metagpt/actions/di/write_analysis_code.py` & `metagpt-0.8.0/metagpt/environment/base_env.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,155 +1,212 @@
-# -*- encoding: utf-8 -*-
-"""
-@Date    :   2023/11/20 13:19:39
-@Author  :   orange-crow
-@File    :   write_analysis_code.py
-"""
-from __future__ import annotations
-
-from typing import Tuple
-
-from metagpt.actions import Action
-from metagpt.logs import logger
-from metagpt.prompts.di.write_analysis_code import (
-    CODE_GENERATOR_WITH_TOOLS,
-    SELECT_FUNCTION_TOOLS,
-    TOOL_RECOMMENDATION_PROMPT,
-    TOOL_USAGE_PROMPT,
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# @Desc   : base env of executing environment
+
+import asyncio
+from enum import Enum
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Set, Union
+
+from pydantic import BaseModel, ConfigDict, Field, SerializeAsAny, model_validator
+
+from metagpt.context import Context
+from metagpt.environment.api.env_api import (
+    EnvAPIAbstract,
+    ReadAPIRegistry,
+    WriteAPIRegistry,
 )
-from metagpt.schema import Message, Plan, SystemMessage
-from metagpt.tools import TOOL_REGISTRY
-from metagpt.tools.tool_registry import validate_tool_names
-from metagpt.utils.common import create_func_call_config
-
-
-class BaseWriteAnalysisCode(Action):
-    DEFAULT_SYSTEM_MSG: str = """You are Code Interpreter, a world-class programmer that can complete any goal by executing code. Strictly follow the plan and generate code step by step. Each step of the code will be executed on the user's machine, and the user will provide the code execution results to you.**Notice: The code for the next step depends on the code for the previous step. Must reuse variables in the lastest other code directly, dont creat it again, it is very import for you. Use !pip install in a standalone block to install missing packages.Usually the libraries you need are already installed.Dont check if packages already imported.**"""  # prompt reference: https://github.com/KillianLucas/open-interpreter/blob/v0.1.4/interpreter/system_message.txt
-    # REUSE_CODE_INSTRUCTION = """ATTENTION: DONT include codes from previous tasks in your current code block, include new codes only, DONT repeat codes!"""
-
-    def insert_system_message(self, context: list[Message], system_msg: str = None):
-        system_msg = system_msg or self.DEFAULT_SYSTEM_MSG
-        context.insert(0, SystemMessage(content=system_msg)) if context[0].role != "system" else None
-        return context
-
-    async def run(self, context: list[Message], plan: Plan = None) -> dict:
-        """Run of a code writing action, used in data analysis or modeling
-
-        Args:
-            context (list[Message]): Action output history, source action denoted by Message.cause_by
-            plan (Plan, optional): Overall plan. Defaults to None.
-
-        Returns:
-            dict: code result in the format of {"code": "print('hello world')", "language": "python"}
-        """
-        raise NotImplementedError
-
-
-class WriteCodeWithoutTools(BaseWriteAnalysisCode):
-    """Ask LLM to generate codes purely by itself without local user-defined tools"""
-
-    async def run(self, context: list[Message], plan: Plan = None, system_msg: str = None, **kwargs) -> dict:
-        messages = self.insert_system_message(context, system_msg)
-        rsp = await self.llm.aask_code(messages, **kwargs)
-        return rsp
-
-
-class WriteCodeWithTools(BaseWriteAnalysisCode):
-    """Write code with help of local available tools. Choose tools first, then generate code to use the tools"""
-
-    # selected tools to choose from, listed by their names. An empty list means selection from all tools.
-    selected_tools: list[str] = []
-
-    def _get_tools_by_type(self, tool_type: str) -> dict:
-        """
-        Retreive tools by tool type from registry, but filtered by pre-selected tool list
-
-        Args:
-            tool_type (str): Tool type to retrieve from the registry
-
-        Returns:
-            dict: A dict of tool name to Tool object, representing available tools under the type
-        """
-        candidate_tools = TOOL_REGISTRY.get_tools_by_type(tool_type)
-        if self.selected_tools:
-            candidate_tool_names = set(self.selected_tools) & candidate_tools.keys()
-            candidate_tools = {tool_name: candidate_tools[tool_name] for tool_name in candidate_tool_names}
-        return candidate_tools
-
-    async def _recommend_tool(
-        self,
-        task: str,
-        available_tools: dict,
-    ) -> dict:
-        """
-        Recommend tools for the specified task.
-
-        Args:
-            task (str): the task to recommend tools for
-            available_tools (dict): the available tools description
-
-        Returns:
-            dict: schemas of recommended tools for the specified task
-        """
-        prompt = TOOL_RECOMMENDATION_PROMPT.format(
-            current_task=task,
-            available_tools=available_tools,
-        )
-        tool_config = create_func_call_config(SELECT_FUNCTION_TOOLS)
-        rsp = await self.llm.aask_code(prompt, **tool_config)
-        recommend_tools = rsp["recommend_tools"]
-        logger.info(f"Recommended tools: \n{recommend_tools}")
-
-        # Parses and validates the  recommended tools, for LLM might hallucinate and recommend non-existing tools
-        valid_tools = validate_tool_names(recommend_tools, return_tool_object=True)
-
-        tool_schemas = {tool.name: tool.schemas for tool in valid_tools}
-
-        return tool_schemas
-
-    async def _prepare_tools(self, plan: Plan) -> Tuple[dict, str]:
-        """Prepare tool schemas and usage instructions according to current task
-
-        Args:
-            plan (Plan): The overall plan containing task information.
-
-        Returns:
-            Tuple[dict, str]: A tool schemas ({tool_name: tool_schema_dict}) and a usage prompt for the type of tools selected
-        """
-        # find tool type from task type through exact match, can extend to retrieval in the future
-        tool_type = plan.current_task.task_type
-
-        # prepare tool-type-specific instruction
-        tool_type_usage_prompt = (
-            TOOL_REGISTRY.get_tool_type(tool_type).usage_prompt if TOOL_REGISTRY.has_tool_type(tool_type) else ""
-        )
+from metagpt.logs import logger
+from metagpt.schema import Message
+from metagpt.utils.common import get_function_schema, is_coroutine_func, is_send_to
 
-        # prepare schemas of available tools
-        tool_schemas = {}
-        available_tools = self._get_tools_by_type(tool_type)
-        if available_tools:
-            available_tools = {tool_name: tool.schemas["description"] for tool_name, tool in available_tools.items()}
-            tool_schemas = await self._recommend_tool(plan.current_task.instruction, available_tools)
+if TYPE_CHECKING:
+    from metagpt.roles.role import Role  # noqa: F401
 
-        return tool_schemas, tool_type_usage_prompt
 
-    async def run(
-        self,
-        context: list[Message],
-        plan: Plan,
-        **kwargs,
-    ) -> str:
-        # prepare tool schemas and tool-type-specific instruction
-        tool_schemas, tool_type_usage_prompt = await self._prepare_tools(plan=plan)
+class EnvType(Enum):
+    ANDROID = "Android"
+    GYM = "Gym"
+    WEREWOLF = "Werewolf"
+    MINECRAFT = "Minecraft"
+    STANFORDTOWN = "StanfordTown"
+
+
+env_write_api_registry = WriteAPIRegistry()
+env_read_api_registry = ReadAPIRegistry()
+
+
+def mark_as_readable(func):
+    """mark functionn as a readable one in ExtEnv, it observes something from ExtEnv"""
+    env_read_api_registry[func.__name__] = get_function_schema(func)
+    return func
+
+
+def mark_as_writeable(func):
+    """mark functionn as a writeable one in ExtEnv, it does something to ExtEnv"""
+    env_write_api_registry[func.__name__] = get_function_schema(func)
+    return func
+
+
+class ExtEnv(BaseModel):
+    """External Env to integrate actual game environment"""
+
+    def _check_api_exist(self, rw_api: Optional[str] = None):
+        if not rw_api:
+            raise ValueError(f"{rw_api} not exists")
+
+    def get_all_available_apis(self, mode: str = "read") -> list[Any]:
+        """get available read/write apis definition"""
+        assert mode in ["read", "write"]
+        if mode == "read":
+            return env_read_api_registry.get_apis()
+        else:
+            return env_write_api_registry.get_apis()
+
+    async def observe(self, env_action: Union[str, EnvAPIAbstract]):
+        """get observation from particular api of ExtEnv"""
+        if isinstance(env_action, str):
+            read_api = env_read_api_registry.get(api_name=env_action)["func"]
+            self._check_api_exist(read_api)
+            if is_coroutine_func(read_api):
+                res = await read_api(self)
+            else:
+                res = read_api(self)
+        elif isinstance(env_action, EnvAPIAbstract):
+            read_api = env_read_api_registry.get(api_name=env_action.api_name)["func"]
+            self._check_api_exist(read_api)
+            if is_coroutine_func(read_api):
+                res = await read_api(self, *env_action.args, **env_action.kwargs)
+            else:
+                res = read_api(self, *env_action.args, **env_action.kwargs)
+        return res
+
+    async def step(self, env_action: Union[str, Message, EnvAPIAbstract, list[EnvAPIAbstract]]):
+        """execute through particular api of ExtEnv"""
+        res = None
+        if isinstance(env_action, Message):
+            self.publish_message(env_action)
+        elif isinstance(env_action, EnvAPIAbstract):
+            write_api = env_write_api_registry.get(env_action.api_name)["func"]
+            self._check_api_exist(write_api)
+            if is_coroutine_func(write_api):
+                res = await write_api(self, *env_action.args, **env_action.kwargs)
+            else:
+                res = write_api(self, *env_action.args, **env_action.kwargs)
+
+        return res
+
+
+class Environment(ExtEnv):
+    """环境，承载一批角色，角色可以向环境发布消息，可以被其他角色观察到
+    Environment, hosting a batch of roles, roles can publish messages to the environment, and can be observed by other roles
+    """
+
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
+    desc: str = Field(default="")  # 环境描述
+    roles: dict[str, SerializeAsAny["Role"]] = Field(default_factory=dict, validate_default=True)
+    member_addrs: Dict["Role", Set] = Field(default_factory=dict, exclude=True)
+    history: str = ""  # For debug
+    context: Context = Field(default_factory=Context, exclude=True)
+
+    @model_validator(mode="after")
+    def init_roles(self):
+        self.add_roles(self.roles.values())
+        return self
+
+    def add_role(self, role: "Role"):
+        """增加一个在当前环境的角色
+        Add a role in the current environment
+        """
+        self.roles[role.profile] = role
+        role.set_env(self)
+        role.context = self.context
+
+    def add_roles(self, roles: Iterable["Role"]):
+        """增加一批在当前环境的角色
+        Add a batch of characters in the current environment
+        """
+        for role in roles:
+            self.roles[role.profile] = role
+
+        for role in roles:  # setup system message with roles
+            role.context = self.context
+            role.set_env(self)
+
+    def publish_message(self, message: Message, peekable: bool = True) -> bool:
+        """
+        Distribute the message to the recipients.
+        In accordance with the Message routing structure design in Chapter 2.2.1 of RFC 116, as already planned
+        in RFC 113 for the entire system, the routing information in the Message is only responsible for
+        specifying the message recipient, without concern for where the message recipient is located. How to
+        route the message to the message recipient is a problem addressed by the transport framework designed
+        in RFC 113.
+        """
+        logger.debug(f"publish_message: {message.dump()}")
+        found = False
+        # According to the routing feature plan in Chapter 2.2.3.2 of RFC 113
+        for role, addrs in self.member_addrs.items():
+            if is_send_to(message, addrs):
+                role.put_message(message)
+                found = True
+        if not found:
+            logger.warning(f"Message no recipients: {message.dump()}")
+        self.history += f"\n{message}"  # For debug
+
+        return True
+
+    async def run(self, k=1):
+        """处理一次所有信息的运行
+        Process all Role runs at once
+        """
+        for _ in range(k):
+            futures = []
+            for role in self.roles.values():
+                future = role.run()
+                futures.append(future)
+
+            await asyncio.gather(*futures)
+            logger.debug(f"is idle: {self.is_idle}")
+
+    def get_roles(self) -> dict[str, "Role"]:
+        """获得环境内的所有角色
+        Process all Role runs at once
+        """
+        return self.roles
+
+    def get_role(self, name: str) -> "Role":
+        """获得环境内的指定角色
+        get all the environment roles
+        """
+        return self.roles.get(name, None)
+
+    def role_names(self) -> list[str]:
+        return [i.name for i in self.roles.values()]
+
+    @property
+    def is_idle(self):
+        """If true, all actions have been executed."""
+        for r in self.roles.values():
+            if not r.is_idle:
+                return False
+        return True
+
+    def get_addresses(self, obj):
+        """Get the addresses of the object."""
+        return self.member_addrs.get(obj, {})
+
+    def set_addresses(self, obj, addresses):
+        """Set the addresses of the object"""
+        self.member_addrs[obj] = addresses
+
+    def archive(self, auto_archive=True):
+        if auto_archive and self.context.git_repo:
+            self.context.git_repo.archive()
+
+    @classmethod
+    def model_rebuild(cls, **kwargs):
+        from metagpt.roles.role import Role  # noqa: F401
 
-        # form a complete tool usage instruction and include it as a message in context
-        tools_instruction = TOOL_USAGE_PROMPT.format(
-            tool_schemas=tool_schemas, tool_type_usage_prompt=tool_type_usage_prompt
-        )
-        context.append(Message(content=tools_instruction, role="user"))
+        super().model_rebuild(**kwargs)
 
-        # prepare prompt & LLM call
-        prompt = self.insert_system_message(context)
-        tool_config = create_func_call_config(CODE_GENERATOR_WITH_TOOLS)
-        rsp = await self.llm.aask_code(prompt, **tool_config)
 
-        return rsp
+Environment.model_rebuild()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `metagpt-0.7.7/metagpt/actions/generate_questions.py` & `metagpt-0.8.0/metagpt/actions/generate_questions.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/invoice_ocr.py` & `metagpt-0.8.0/metagpt/actions/invoice_ocr.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/prepare_documents.py` & `metagpt-0.8.0/metagpt/actions/prepare_documents.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/prepare_interview.py` & `metagpt-0.8.0/metagpt/actions/prepare_interview.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/project_management.py` & `metagpt-0.8.0/metagpt/actions/project_management.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/project_management_an.py` & `metagpt-0.8.0/metagpt/actions/project_management_an.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 @Time    : 2023/12/14 15:28
 @Author  : alexanderwu
 @File    : project_management_an.py
 """
 from typing import List
 
 from metagpt.actions.action_node import ActionNode
-from metagpt.logs import logger
 
 REQUIRED_PYTHON_PACKAGES = ActionNode(
     key="Required Python packages",
     expected_type=List[str],
     instruction="Provide required Python packages in requirements.txt format.",
     example=["flask==1.1.2", "bcrypt==3.2.0"],
 )
@@ -115,18 +114,7 @@
     FULL_API_SPEC,
     REFINED_SHARED_KNOWLEDGE,
     ANYTHING_UNCLEAR_PM,
 ]
 
 PM_NODE = ActionNode.from_children("PM_NODE", NODES)
 REFINED_PM_NODE = ActionNode.from_children("REFINED_PM_NODE", REFINED_NODES)
-
-
-def main():
-    prompt = PM_NODE.compile(context="")
-    logger.info(prompt)
-    prompt = REFINED_PM_NODE.compile(context="")
-    logger.info(prompt)
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `metagpt-0.7.7/metagpt/actions/research.py` & `metagpt-0.8.0/metagpt/actions/research.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                 yield prompt
                 remove = max(results, key=len)
                 remove.pop()
                 if len(remove) == 0:
                     break
 
         model_name = config.llm.model
-        prompt = reduce_message_length(gen_msg(), model_name, system_text, 4096)
+        prompt = reduce_message_length(gen_msg(), model_name, system_text, config.llm.max_token)
         logger.debug(prompt)
         queries = await self._aask(prompt, [system_text])
         try:
             queries = OutputParser.extract_struct(queries, list)
             queries = TypeAdapter(list[str]).validate_python(queries)
         except Exception as e:
             logger.exception(f"fail to break down the research question due to {e}")
```

### Comparing `metagpt-0.7.7/metagpt/actions/run_code.py` & `metagpt-0.8.0/metagpt/actions/run_code.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/search_and_summarize.py` & `metagpt-0.8.0/metagpt/actions/search_and_summarize.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/skill_action.py` & `metagpt-0.8.0/metagpt/actions/skill_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         return prompt
 
     async def run(self, with_message=None, **kwargs) -> Message:
         prompt = self.prompt
         rsp = await self.llm.aask(
             msg=prompt,
             system_msgs=["You are a function parser.", "You can convert spoken words into function parameters."],
+            stream=False,
         )
         logger.debug(f"SKILL:{prompt}\n, RESULT:{rsp}")
         self.args = ArgumentsParingAction.parse_arguments(skill_name=self.skill.name, txt=rsp)
         self.rsp = Message(content=rsp, role="assistant", instruct_content=self.args, cause_by=self)
         return self.rsp
 
     @staticmethod
```

### Comparing `metagpt-0.7.7/metagpt/actions/summarize_code.py` & `metagpt-0.8.0/metagpt/actions/summarize_code.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/talk_action.py` & `metagpt-0.8.0/metagpt/actions/talk_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             format_msgs.append({"role": "assistant", "content": self.knowledge})
         if self.history_summary:
             format_msgs.append({"role": "assistant", "content": self.history_summary})
         return self.i_context, format_msgs, system_msgs
 
     async def run(self, with_message=None, **kwargs) -> Message:
         msg, format_msgs, system_msgs = self.aask_args
-        rsp = await self.llm.aask(msg=msg, format_msgs=format_msgs, system_msgs=system_msgs)
+        rsp = await self.llm.aask(msg=msg, format_msgs=format_msgs, system_msgs=system_msgs, stream=False)
         self.rsp = Message(content=rsp, role="assistant", cause_by=self)
         return self.rsp
 
 
 class TalkActionPrompt:
     FORMATION = """Formation: "Capacity and role" defines the role you are currently playing;
   "[HISTORY_BEGIN]" and "[HISTORY_END]" tags enclose the historical conversation;
```

### Comparing `metagpt-0.7.7/metagpt/actions/write_code.py` & `metagpt-0.8.0/metagpt/actions/write_code.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,19 +19,15 @@
 
 from pydantic import Field
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 
 from metagpt.actions.action import Action
 from metagpt.actions.project_management_an import REFINED_TASK_LIST, TASK_LIST
 from metagpt.actions.write_code_plan_and_change_an import REFINED_TEMPLATE
-from metagpt.const import (
-    BUGFIX_FILENAME,
-    CODE_PLAN_AND_CHANGE_FILENAME,
-    REQUIREMENT_FILENAME,
-)
+from metagpt.const import BUGFIX_FILENAME, REQUIREMENT_FILENAME
 from metagpt.logs import logger
 from metagpt.schema import CodingContext, Document, RunCodeResult
 from metagpt.utils.common import CodeParser
 from metagpt.utils.project_repo import ProjectRepo
 
 PROMPT_TEMPLATE = """
 NOTICE
@@ -94,42 +90,40 @@
         code = CodeParser.parse_code(block="", text=code_rsp)
         return code
 
     async def run(self, *args, **kwargs) -> CodingContext:
         bug_feedback = await self.repo.docs.get(filename=BUGFIX_FILENAME)
         coding_context = CodingContext.loads(self.i_context.content)
         test_doc = await self.repo.test_outputs.get(filename="test_" + coding_context.filename + ".json")
-        code_plan_and_change_doc = await self.repo.docs.code_plan_and_change.get(filename=CODE_PLAN_AND_CHANGE_FILENAME)
-        code_plan_and_change = code_plan_and_change_doc.content if code_plan_and_change_doc else ""
         requirement_doc = await self.repo.docs.get(filename=REQUIREMENT_FILENAME)
         summary_doc = None
         if coding_context.design_doc and coding_context.design_doc.filename:
             summary_doc = await self.repo.docs.code_summary.get(filename=coding_context.design_doc.filename)
         logs = ""
         if test_doc:
             test_detail = RunCodeResult.loads(test_doc.content)
             logs = test_detail.stderr
 
         if bug_feedback:
             code_context = coding_context.code_doc.content
-        elif code_plan_and_change:
+        elif self.config.inc:
             code_context = await self.get_codes(
                 coding_context.task_doc, exclude=self.i_context.filename, project_repo=self.repo, use_inc=True
             )
         else:
             code_context = await self.get_codes(
                 coding_context.task_doc,
                 exclude=self.i_context.filename,
                 project_repo=self.repo.with_src_path(self.context.src_workspace),
             )
 
-        if code_plan_and_change:
+        if self.config.inc:
             prompt = REFINED_TEMPLATE.format(
                 user_requirement=requirement_doc.content if requirement_doc else "",
-                code_plan_and_change=code_plan_and_change,
+                code_plan_and_change=str(coding_context.code_plan_and_change_doc),
                 design=coding_context.design_doc.content if coding_context.design_doc else "",
                 task=coding_context.task_doc.content if coding_context.task_doc else "",
                 code=code_context,
                 logs=logs,
                 feedback=bug_feedback.content if bug_feedback else "",
                 filename=self.i_context.filename,
                 summary_log=summary_doc.content if summary_doc else "",
```

### Comparing `metagpt-0.7.7/metagpt/actions/write_code_an_draft.py` & `metagpt-0.8.0/metagpt/actions/write_code_an_draft.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/write_code_plan_and_change_an.py` & `metagpt-0.8.0/metagpt/actions/write_code_plan_and_change_an.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,87 +2,102 @@
 # -*- coding: utf-8 -*-
 """
 @Time    : 2023/12/26
 @Author  : mannaandpoem
 @File    : write_code_plan_and_change_an.py
 """
 import os
+from typing import List
 
 from pydantic import Field
 
 from metagpt.actions.action import Action
 from metagpt.actions.action_node import ActionNode
+from metagpt.logs import logger
 from metagpt.schema import CodePlanAndChangeContext
 
-CODE_PLAN_AND_CHANGE = ActionNode(
-    key="Code Plan And Change",
-    expected_type=str,
-    instruction="Developing comprehensive and step-by-step incremental development plan, and write Incremental "
-    "Change by making a code draft that how to implement incremental development including detailed steps based on the "
-    "context. Note: Track incremental changes using mark of '+' or '-' for add/modify/delete code, and conforms to the "
-    "output format of git diff",
-    example="""
-1. Plan for calculator.py: Enhance the functionality of `calculator.py` by extending it to incorporate methods for subtraction, multiplication, and division. Additionally, implement robust error handling for the division operation to mitigate potential issues related to division by zero. 
-```python
+DEVELOPMENT_PLAN = ActionNode(
+    key="Development Plan",
+    expected_type=List[str],
+    instruction="Develop a comprehensive and step-by-step incremental development plan, providing the detail "
+    "changes to be implemented at each step based on the order of 'Task List'",
+    example=[
+        "Enhance the functionality of `calculator.py` by extending it to incorporate methods for subtraction, ...",
+        "Update the existing codebase in main.py to incorporate new API endpoints for subtraction, ...",
+    ],
+)
+
+INCREMENTAL_CHANGE = ActionNode(
+    key="Incremental Change",
+    expected_type=List[str],
+    instruction="Write Incremental Change by making a code draft that how to implement incremental development "
+    "including detailed steps based on the context. Note: Track incremental changes using the marks `+` and `-` to "
+    "indicate additions and deletions, and ensure compliance with the output format of `git diff`",
+    example=[
+        '''```diff
+--- Old/calculator.py
++++ New/calculator.py
+
 class Calculator:
          self.result = number1 + number2
          return self.result
 
 -    def sub(self, number1, number2) -> float:
 +    def subtract(self, number1: float, number2: float) -> float:
-+        '''
++        """
 +        Subtracts the second number from the first and returns the result.
 +
 +        Args:
 +            number1 (float): The number to be subtracted from.
 +            number2 (float): The number to subtract.
 +
 +        Returns:
 +            float: The difference of number1 and number2.
-+        '''
++        """
 +        self.result = number1 - number2
 +        return self.result
 +
     def multiply(self, number1: float, number2: float) -> float:
 -        pass
-+        '''
++        """
 +        Multiplies two numbers and returns the result.
 +
 +        Args:
 +            number1 (float): The first number to multiply.
 +            number2 (float): The second number to multiply.
 +
 +        Returns:
 +            float: The product of number1 and number2.
-+        '''
++        """
 +        self.result = number1 * number2
 +        return self.result
 +
     def divide(self, number1: float, number2: float) -> float:
 -        pass
-+        '''
++        """
 +            ValueError: If the second number is zero.
-+        '''
++        """
 +        if number2 == 0:
 +            raise ValueError('Cannot divide by zero')
 +        self.result = number1 / number2
 +        return self.result
 +
 -    def reset_result(self):
 +    def clear(self):
 +        if self.result != 0.0:
 +            print("Result is not zero, clearing...")
 +        else:
 +            print("Result is already zero, no need to clear.")
 +
          self.result = 0.0
-```
+```''',
+        """```diff
+--- Old/main.py
++++ New/main.py
 
-2. Plan for main.py: Integrate new API endpoints for subtraction, multiplication, and division into the existing codebase of `main.py`. Then, ensure seamless integration with the overall application architecture and maintain consistency with coding standards.
-```python
 def add_numbers():
      result = calculator.add_numbers(num1, num2)
      return jsonify({'result': result}), 200
 
 -# TODO: Implement subtraction, multiplication, and division operations
 +@app.route('/subtract_numbers', methods=['POST'])
 +def subtract_numbers():
@@ -102,14 +117,15 @@
 +    except ValueError as e:
 +        return jsonify({'error': str(e)}), 400
 +    return jsonify({'result': result}), 200
 +
  if __name__ == '__main__':
      app.run()
 ```""",
+    ],
 )
 
 CODE_PLAN_AND_CHANGE_CONTEXT = """
 ## User New Requirements
 {requirement}
 
 ## PRD
@@ -168,42 +184,44 @@
 
 # Instruction: Based on the context, follow "Format example", write or rewrite code.
 ## Write/Rewrite Code: Only write one file {filename}, write or rewrite complete code using triple quotes based on the following attentions and context.
 1. Only One file: do your best to implement THIS ONLY ONE FILE.
 2. COMPLETE CODE: Your code will be part of the entire project, so please implement complete, reliable, reusable code snippets.
 3. Set default value: If there is any setting, ALWAYS SET A DEFAULT VALUE, ALWAYS USE STRONG TYPE AND EXPLICIT VARIABLE. AVOID circular import.
 4. Follow design: YOU MUST FOLLOW "Data structures and interfaces". DONT CHANGE ANY DESIGN. Do not use public member functions that do not exist in your design.
-5. Follow Code Plan And Change: If there is any Incremental Change that is marked by the git diff format using '+' and '-' for add/modify/delete code, or Legacy Code files contain "{filename} to be rewritten", you must merge it into the code file according to the plan. 
+5. Follow Code Plan And Change: If there is any "Incremental Change" that is marked by the git diff format with '+' and '-' symbols, or Legacy Code files contain "{filename} to be rewritten", you must merge it into the code file according to the "Development Plan". 
 6. CAREFULLY CHECK THAT YOU DONT MISS ANY NECESSARY CLASS/FUNCTION IN THIS FILE.
 7. Before using a external variable/module, make sure you import it first.
 8. Write out EVERY CODE DETAIL, DON'T LEAVE TODO.
 9. Attention: Retain details that are not related to incremental development but are important for maintaining the consistency and clarity of the old code.
 """
 
-WRITE_CODE_PLAN_AND_CHANGE_NODE = ActionNode.from_children("WriteCodePlanAndChange", [CODE_PLAN_AND_CHANGE])
+CODE_PLAN_AND_CHANGE = [DEVELOPMENT_PLAN, INCREMENTAL_CHANGE]
+
+WRITE_CODE_PLAN_AND_CHANGE_NODE = ActionNode.from_children("WriteCodePlanAndChange", CODE_PLAN_AND_CHANGE)
 
 
 class WriteCodePlanAndChange(Action):
     name: str = "WriteCodePlanAndChange"
     i_context: CodePlanAndChangeContext = Field(default_factory=CodePlanAndChangeContext)
 
     async def run(self, *args, **kwargs):
         self.llm.system_prompt = "You are a professional software engineer, your primary responsibility is to "
         "meticulously craft comprehensive incremental development plan and deliver detailed incremental change"
         prd_doc = await self.repo.docs.prd.get(filename=self.i_context.prd_filename)
         design_doc = await self.repo.docs.system_design.get(filename=self.i_context.design_filename)
         task_doc = await self.repo.docs.task.get(filename=self.i_context.task_filename)
-        code_text = await self.get_old_codes()
         context = CODE_PLAN_AND_CHANGE_CONTEXT.format(
             requirement=self.i_context.requirement,
             prd=prd_doc.content,
             design=design_doc.content,
             task=task_doc.content,
-            code=code_text,
+            code=await self.get_old_codes(),
         )
+        logger.info("Writing code plan and change..")
         return await WRITE_CODE_PLAN_AND_CHANGE_NODE.fill(context=context, llm=self.llm, schema="json")
 
     async def get_old_codes(self) -> str:
         self.repo.old_workspace = self.repo.git_repo.workdir / os.path.basename(self.config.project_path)
         old_file_repo = self.repo.git_repo.new_file_repository(relative_path=self.repo.old_workspace)
         old_codes = await old_file_repo.get_all()
         codes = [f"----- {code.filename}\n```{code.content}```" for code in old_codes]
```

### Comparing `metagpt-0.7.7/metagpt/actions/write_code_review.py` & `metagpt-0.8.0/metagpt/actions/write_code_review.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 
 from pydantic import Field
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 
 from metagpt.actions import WriteCode
 from metagpt.actions.action import Action
-from metagpt.const import CODE_PLAN_AND_CHANGE_FILENAME, REQUIREMENT_FILENAME
+from metagpt.const import REQUIREMENT_FILENAME
 from metagpt.logs import logger
 from metagpt.schema import CodingContext
 from metagpt.utils.common import CodeParser
 
 PROMPT_TEMPLATE = """
 # System
 Role: You are a professional software engineer, and your main task is to review and revise the code. You need to ensure that the code conforms to the google-style standards, is elegantly designed and modularized, easy to read and maintain.
@@ -145,37 +145,29 @@
             code_context = await WriteCode.get_codes(
                 self.i_context.task_doc,
                 exclude=self.i_context.filename,
                 project_repo=self.repo.with_src_path(self.context.src_workspace),
                 use_inc=self.config.inc,
             )
 
-            if not self.config.inc:
-                context = "\n".join(
-                    [
-                        "## System Design\n" + str(self.i_context.design_doc) + "\n",
-                        "## Task\n" + task_content + "\n",
-                        "## Code Files\n" + code_context + "\n",
-                    ]
-                )
-            else:
+            ctx_list = [
+                "## System Design\n" + str(self.i_context.design_doc) + "\n",
+                "## Task\n" + task_content + "\n",
+                "## Code Files\n" + code_context + "\n",
+            ]
+            if self.config.inc:
                 requirement_doc = await self.repo.docs.get(filename=REQUIREMENT_FILENAME)
-                code_plan_and_change_doc = await self.repo.get(filename=CODE_PLAN_AND_CHANGE_FILENAME)
-                context = "\n".join(
-                    [
-                        "## User New Requirements\n" + str(requirement_doc) + "\n",
-                        "## Code Plan And Change\n" + str(code_plan_and_change_doc) + "\n",
-                        "## System Design\n" + str(self.i_context.design_doc) + "\n",
-                        "## Task\n" + task_content + "\n",
-                        "## Code Files\n" + code_context + "\n",
-                    ]
-                )
+                insert_ctx_list = [
+                    "## User New Requirements\n" + str(requirement_doc) + "\n",
+                    "## Code Plan And Change\n" + str(self.i_context.code_plan_and_change_doc) + "\n",
+                ]
+                ctx_list = insert_ctx_list + ctx_list
 
             context_prompt = PROMPT_TEMPLATE.format(
-                context=context,
+                context="\n".join(ctx_list),
                 code=iterative_code,
                 filename=self.i_context.code_doc.filename,
             )
             cr_prompt = EXAMPLE_AND_INSTRUCTION.format(
                 format_example=format_example,
             )
             len1 = len(iterative_code) if iterative_code else 0
```

### Comparing `metagpt-0.7.7/metagpt/actions/write_docstring.py` & `metagpt-0.8.0/metagpt/actions/write_docstring.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/write_prd.py` & `metagpt-0.8.0/metagpt/actions/write_prd.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/write_prd_an.py` & `metagpt-0.8.0/metagpt/actions/write_prd_an.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     example=["Create an engaging user experience", "Improve accessibility, be responsive", "More beautiful UI"],
 )
 
 REFINED_PRODUCT_GOALS = ActionNode(
     key="Refined Product Goals",
     expected_type=List[str],
     instruction="Update and expand the original product goals to reflect the evolving needs due to incremental "
-    "development.Ensure that the refined goals align with the current project direction and contribute to its success.",
+    "development. Ensure that the refined goals align with the current project direction and contribute to its success.",
     example=[
         "Enhance user engagement through new features",
         "Optimize performance for scalability",
         "Integrate innovative UI enhancements",
     ],
 )
```

### Comparing `metagpt-0.7.7/metagpt/actions/write_prd_review.py` & `metagpt-0.8.0/metagpt/actions/write_prd_review.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/write_review.py` & `metagpt-0.8.0/metagpt/actions/write_review.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/write_teaching_plan.py` & `metagpt-0.8.0/metagpt/actions/write_teaching_plan.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/write_test.py` & `metagpt-0.8.0/metagpt/actions/write_test.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/actions/write_tutorial.py` & `metagpt-0.8.0/metagpt/actions/write_tutorial.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/config2.py` & `metagpt-0.8.0/metagpt/config2.py`

 * *Files 13% similar despite different names*

```diff
@@ -88,22 +88,36 @@
     def default(cls):
         """Load default config
         - Priority: env < default_config_paths
         - Inside default_config_paths, the latter one overwrites the former one
         """
         default_config_paths: List[Path] = [
             METAGPT_ROOT / "config/config2.yaml",
-            Path.home() / ".metagpt/config2.yaml",
+            CONFIG_ROOT / "config2.yaml",
         ]
 
         dicts = [dict(os.environ)]
         dicts += [Config.read_yaml(path) for path in default_config_paths]
         final = merge_dict(dicts)
         return Config(**final)
 
+    @classmethod
+    def from_llm_config(cls, llm_config: dict):
+        """user config llm
+        example:
+        llm_config = {"api_type": "xxx", "api_key": "xxx", "model": "xxx"}
+        gpt4 = Config.from_llm_config(llm_config)
+        A = Role(name="A", profile="Democratic candidate", goal="Win the election", actions=[a1], watch=[a2], config=gpt4)
+        """
+        llm_config = LLMConfig.model_validate(llm_config)
+        dicts = [dict(os.environ)]
+        dicts += [{"llm": llm_config}]
+        final = merge_dict(dicts)
+        return Config(**final)
+
     def update_via_cli(self, project_path, project_name, inc, reqa_file, max_auto_summarize_code):
         """update config via cli"""
 
         # Use in the PrepareDocuments action according to Section 2.2.3.5.1 of RFC 135.
         if project_path:
             inc = True
             project_name = project_name or Path(project_path).name
```

### Comparing `metagpt-0.7.7/metagpt/configs/browser_config.py` & `metagpt-0.8.0/metagpt/configs/browser_config.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/configs/llm_config.py` & `metagpt-0.8.0/metagpt/configs/llm_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,46 +6,59 @@
 @File    : llm_config.py
 """
 from enum import Enum
 from typing import Optional
 
 from pydantic import field_validator
 
+from metagpt.const import LLM_API_TIMEOUT
 from metagpt.utils.yaml_model import YamlModel
 
 
 class LLMType(Enum):
     OPENAI = "openai"
     ANTHROPIC = "anthropic"
+    CLAUDE = "claude"  # alias name of anthropic
     SPARK = "spark"
     ZHIPUAI = "zhipuai"
     FIREWORKS = "fireworks"
     OPEN_LLM = "open_llm"
     GEMINI = "gemini"
     METAGPT = "metagpt"
     AZURE = "azure"
     OLLAMA = "ollama"
+    QIANFAN = "qianfan"  # Baidu BCE
+    DASHSCOPE = "dashscope"  # Aliyun LingJi DashScope
+    MOONSHOT = "moonshot"
+    MISTRAL = "mistral"
+    YI = "yi"  # lingyiwanwu
 
     def __missing__(self, key):
         return self.OPENAI
 
 
 class LLMConfig(YamlModel):
     """Config for LLM
 
     OpenAI: https://github.com/openai/openai-python/blob/main/src/openai/resources/chat/completions.py#L681
     Optional Fields in pydantic: https://docs.pydantic.dev/latest/migration/#required-optional-and-nullable-fields
     """
 
-    api_key: str
+    api_key: str = "sk-"
     api_type: LLMType = LLMType.OPENAI
     base_url: str = "https://api.openai.com/v1"
     api_version: Optional[str] = None
 
     model: Optional[str] = None  # also stands for DEPLOYMENT_NAME
+    pricing_plan: Optional[str] = None  # Cost Settlement Plan Parameters.
+
+    # For Cloud Service Provider like Baidu/ Alibaba
+    access_key: Optional[str] = None
+    secret_key: Optional[str] = None
+    endpoint: Optional[str] = None  # for self-deployed model on the cloud
 
     # For Spark(Xunfei), maybe remove later
     app_id: Optional[str] = None
     api_secret: Optional[str] = None
     domain: Optional[str] = None
 
     # For Chat Completion
@@ -58,21 +71,26 @@
     presence_penalty: float = 0.0
     frequency_penalty: float = 0.0
     best_of: Optional[int] = None
     n: Optional[int] = None
     stream: bool = False
     logprobs: Optional[bool] = None  # https://cookbook.openai.com/examples/using_logprobs
     top_logprobs: Optional[int] = None
-    timeout: int = 60
+    timeout: int = 600
 
     # For Network
     proxy: Optional[str] = None
 
     # Cost Control
     calc_usage: bool = True
 
     @field_validator("api_key")
     @classmethod
     def check_llm_key(cls, v):
         if v in ["", None, "YOUR_API_KEY"]:
             raise ValueError("Please set your API key in config2.yaml")
         return v
+
+    @field_validator("timeout")
+    @classmethod
+    def check_timeout(cls, v):
+        return v or LLM_API_TIMEOUT
```

### Comparing `metagpt-0.7.7/metagpt/configs/redis_config.py` & `metagpt-0.8.0/metagpt/configs/redis_config.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/configs/workspace_config.py` & `metagpt-0.8.0/metagpt/configs/workspace_config.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/const.py` & `metagpt-0.8.0/metagpt/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
 # METAGPT PROJECT ROOT AND VARS
 CONFIG_ROOT = Path.home() / ".metagpt"
 METAGPT_ROOT = get_metagpt_root()  # Dependent on METAGPT_PROJECT_ROOT
 DEFAULT_WORKSPACE_ROOT = METAGPT_ROOT / "workspace"
 
 EXAMPLE_PATH = METAGPT_ROOT / "examples"
+EXAMPLE_DATA_PATH = EXAMPLE_PATH / "data"
 DATA_PATH = METAGPT_ROOT / "data"
 TEST_DATA_PATH = METAGPT_ROOT / "tests/data"
 RESEARCH_PATH = DATA_PATH / "research"
 TUTORIAL_PATH = DATA_PATH / "tutorial_docx"
 INVOICE_OCR_TABLE_PATH = DATA_PATH / "invoice_table"
 
 UT_PATH = DATA_PATH / "ut"
@@ -80,15 +81,14 @@
 MESSAGE_META_ROLE = "role"
 MESSAGE_ROUTE_TO_ALL = "<all>"
 MESSAGE_ROUTE_TO_NONE = "<none>"
 
 REQUIREMENT_FILENAME = "requirement.txt"
 BUGFIX_FILENAME = "bugfix.txt"
 PACKAGE_REQUIREMENTS_FILENAME = "requirements.txt"
-CODE_PLAN_AND_CHANGE_FILENAME = "code_plan_and_change.json"
 
 DOCS_FILE_REPO = "docs"
 PRDS_FILE_REPO = "docs/prd"
 SYSTEM_DESIGN_FILE_REPO = "docs/system_design"
 TASK_FILE_REPO = "docs/task"
 CODE_PLAN_AND_CHANGE_FILE_REPO = "docs/code_plan_and_change"
 COMPETITIVE_ANALYSIS_FILE_REPO = "resources/competitive_analysis"
@@ -101,14 +101,15 @@
 TEST_CODES_FILE_REPO = "tests"
 TEST_OUTPUTS_FILE_REPO = "test_outputs"
 CODE_SUMMARIES_FILE_REPO = "docs/code_summary"
 CODE_SUMMARIES_PDF_FILE_REPO = "resources/code_summary"
 RESOURCES_FILE_REPO = "resources"
 SD_OUTPUT_FILE_REPO = "resources/sd_output"
 GRAPH_REPO_FILE_REPO = "docs/graph_repo"
+VISUAL_GRAPH_REPO_FILE_REPO = "resources/graph_db"
 CLASS_VIEW_FILE_REPO = "docs/class_view"
 
 YAPI_URL = "http://yapi.deepwisdomai.com/"
 
 DEFAULT_LANGUAGE = "English"
 DEFAULT_MAX_TOKENS = 1500
 COMMAND_TOKENS = 500
@@ -118,16 +119,19 @@
 DEFAULT_TOKEN_SIZE = 500
 
 # format
 BASE64_FORMAT = "base64"
 
 # REDIS
 REDIS_KEY = "REDIS_KEY"
-LLM_API_TIMEOUT = 300
 
 # Message id
 IGNORED_MESSAGE_ID = "0"
 
 # Class Relationship
 GENERALIZATION = "Generalize"
 COMPOSITION = "Composite"
 AGGREGATION = "Aggregate"
+
+# Timeout
+USE_CONFIG_TIMEOUT = 0  # Using llm.timeout configuration.
+LLM_API_TIMEOUT = 300
```

### Comparing `metagpt-0.7.7/metagpt/context.py` & `metagpt-0.8.0/metagpt/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 import os
 from pathlib import Path
 from typing import Any, Optional
 
 from pydantic import BaseModel, ConfigDict
 
 from metagpt.config2 import Config
-from metagpt.configs.llm_config import LLMConfig
+from metagpt.configs.llm_config import LLMConfig, LLMType
 from metagpt.provider.base_llm import BaseLLM
 from metagpt.provider.llm_provider_registry import create_llm_instance
-from metagpt.utils.cost_manager import CostManager
+from metagpt.utils.cost_manager import (
+    CostManager,
+    FireworksCostManager,
+    TokenCostManager,
+)
 from metagpt.utils.git_repository import GitRepository
 from metagpt.utils.project_repo import ProjectRepo
 
 
 class AttrDict(BaseModel):
     """A dict-like object that allows access to keys as attributes, compatible with Pydantic."""
 
@@ -76,22 +80,31 @@
 
     # def use_llm(self, name: Optional[str] = None, provider: LLMType = LLMType.OPENAI) -> BaseLLM:
     #     """Use a LLM instance"""
     #     self._llm_config = self.config.get_llm_config(name, provider)
     #     self._llm = None
     #     return self._llm
 
+    def _select_costmanager(self, llm_config: LLMConfig) -> CostManager:
+        """Return a CostManager instance"""
+        if llm_config.api_type == LLMType.FIREWORKS:
+            return FireworksCostManager()
+        elif llm_config.api_type == LLMType.OPEN_LLM:
+            return TokenCostManager()
+        else:
+            return self.cost_manager
+
     def llm(self) -> BaseLLM:
         """Return a LLM instance, fixme: support cache"""
         # if self._llm is None:
         self._llm = create_llm_instance(self.config.llm)
         if self._llm.cost_manager is None:
-            self._llm.cost_manager = self.cost_manager
+            self._llm.cost_manager = self._select_costmanager(self.config.llm)
         return self._llm
 
     def llm_with_cost_manager_from_llm_config(self, llm_config: LLMConfig) -> BaseLLM:
         """Return a LLM instance, fixme: support cache"""
         # if self._llm is None:
         llm = create_llm_instance(llm_config)
         if llm.cost_manager is None:
-            llm.cost_manager = self.cost_manager
+            llm.cost_manager = self._select_costmanager(llm_config)
         return llm
```

### Comparing `metagpt-0.7.7/metagpt/context_mixin.py` & `metagpt-0.8.0/metagpt/context_mixin.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/document.py` & `metagpt-0.8.0/metagpt/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,45 @@
 @Desc    : Classes and Operations Related to Files in the File System.
 """
 from enum import Enum
 from pathlib import Path
 from typing import Optional, Union
 
 import pandas as pd
-from langchain.document_loaders import (
-    TextLoader,
-    UnstructuredPDFLoader,
-    UnstructuredWordDocumentLoader,
-)
-from langchain.text_splitter import CharacterTextSplitter
+from llama_index.core import Document, SimpleDirectoryReader
+from llama_index.core.node_parser import SimpleNodeParser
+from llama_index.readers.file import PDFReader
 from pydantic import BaseModel, ConfigDict, Field
 from tqdm import tqdm
 
+from metagpt.logs import logger
 from metagpt.repo_parser import RepoParser
 
 
 def validate_cols(content_col: str, df: pd.DataFrame):
     if content_col not in df.columns:
         raise ValueError("Content column not found in DataFrame.")
 
 
-def read_data(data_path: Path):
+def read_data(data_path: Path) -> Union[pd.DataFrame, list[Document]]:
     suffix = data_path.suffix
     if ".xlsx" == suffix:
         data = pd.read_excel(data_path)
     elif ".csv" == suffix:
         data = pd.read_csv(data_path)
     elif ".json" == suffix:
         data = pd.read_json(data_path)
     elif suffix in (".docx", ".doc"):
-        data = UnstructuredWordDocumentLoader(str(data_path), mode="elements").load()
+        data = SimpleDirectoryReader(input_files=[str(data_path)]).load_data()
     elif ".txt" == suffix:
-        data = TextLoader(str(data_path)).load()
-        text_splitter = CharacterTextSplitter(separator="\n", chunk_size=256, chunk_overlap=0)
-        texts = text_splitter.split_documents(data)
-        data = texts
+        data = SimpleDirectoryReader(input_files=[str(data_path)]).load_data()
+        node_parser = SimpleNodeParser.from_defaults(separator="\n", chunk_size=256, chunk_overlap=0)
+        data = node_parser.get_nodes_from_documents(data)
     elif ".pdf" == suffix:
-        data = UnstructuredPDFLoader(str(data_path), mode="elements").load()
+        data = PDFReader.load_data(str(data_path))
     else:
         raise NotImplementedError("File format not supported.")
     return data
 
 
 class DocumentStatus(Enum):
     """Indicates document status, a mechanism similar to RFC/PEP"""
@@ -126,41 +123,44 @@
     def from_path(cls, data_path: Path, content_col="content", meta_col="metadata"):
         if not data_path.exists():
             raise FileNotFoundError(f"File {data_path} not found.")
         data = read_data(data_path)
         if isinstance(data, pd.DataFrame):
             validate_cols(content_col, data)
             return cls(data=data, content=str(data), content_col=content_col, meta_col=meta_col)
-        else:
+        try:
             content = data_path.read_text()
-            return cls(data=data, content=content, content_col=content_col, meta_col=meta_col)
+        except Exception as e:
+            logger.debug(f"Load {str(data_path)} error: {e}")
+            content = ""
+        return cls(data=data, content=content, content_col=content_col, meta_col=meta_col)
 
     def _get_docs_and_metadatas_by_df(self) -> (list, list):
         df = self.data
         docs = []
         metadatas = []
         for i in tqdm(range(len(df))):
             docs.append(df[self.content_col].iloc[i])
             if self.meta_col:
                 metadatas.append({self.meta_col: df[self.meta_col].iloc[i]})
             else:
                 metadatas.append({})
         return docs, metadatas
 
-    def _get_docs_and_metadatas_by_langchain(self) -> (list, list):
+    def _get_docs_and_metadatas_by_llamaindex(self) -> (list, list):
         data = self.data
-        docs = [i.page_content for i in data]
+        docs = [i.text for i in data]
         metadatas = [i.metadata for i in data]
         return docs, metadatas
 
     def get_docs_and_metadatas(self) -> (list, list):
         if isinstance(self.data, pd.DataFrame):
             return self._get_docs_and_metadatas_by_df()
         elif isinstance(self.data, list):
-            return self._get_docs_and_metadatas_by_langchain()
+            return self._get_docs_and_metadatas_by_llamaindex()
         else:
             raise NotImplementedError("Data type not supported for metadata extraction.")
 
 
 class RepoMetadata(BaseModel):
     name: str = Field(default="")
     n_docs: int = Field(default=0)
```

### Comparing `metagpt-0.7.7/metagpt/document_store/base_store.py` & `metagpt-0.8.0/metagpt/document_store/base_store.py`

 * *Files 26% similar despite different names*

```diff
@@ -34,17 +34,17 @@
         if not cache_dir:
             cache_dir = raw_data_path.parent
         self.cache_dir = cache_dir
         self.store = self._load()
         if not self.store:
             self.store = self.write()
 
-    def _get_index_and_store_fname(self, index_ext=".index", pkl_ext=".pkl"):
-        index_file = self.cache_dir / f"{self.fname}{index_ext}"
-        store_file = self.cache_dir / f"{self.fname}{pkl_ext}"
+    def _get_index_and_store_fname(self, index_ext=".json", docstore_ext=".json"):
+        index_file = self.cache_dir / "default__vector_store" / index_ext
+        store_file = self.cache_dir / "docstore" / docstore_ext
         return index_file, store_file
 
     @abstractmethod
     def _load(self):
         raise NotImplementedError
 
     @abstractmethod
```

### Comparing `metagpt-0.7.7/metagpt/document_store/chromadb_store.py` & `metagpt-0.8.0/metagpt/document_store/chromadb_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 """
 import chromadb
 
 
 class ChromaStore:
     """If inherited from BaseStore, or importing other modules from metagpt, a Python exception occurs, which is strange."""
 
-    def __init__(self, name):
+    def __init__(self, name: str, get_or_create: bool = False):
         client = chromadb.Client()
-        collection = client.create_collection(name)
+        collection = client.create_collection(name, get_or_create=get_or_create)
         self.client = client
         self.collection = collection
 
     def search(self, query, n_results=2, metadata_filter=None, document_filter=None):
         # kwargs can be used for optional filtering
         results = self.collection.query(
             query_texts=[query],
```

### Comparing `metagpt-0.7.7/metagpt/document_store/faiss_store.py` & `metagpt-0.8.0/metagpt/document_store/faiss_store.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,57 +3,75 @@
 """
 @Time    : 2023/5/25 10:20
 @Author  : alexanderwu
 @File    : faiss_store.py
 """
 import asyncio
 from pathlib import Path
-from typing import Optional
+from typing import Any, Optional
 
-from langchain.vectorstores import FAISS
-from langchain_core.embeddings import Embeddings
+import faiss
+from llama_index.core import VectorStoreIndex, load_index_from_storage
+from llama_index.core.embeddings import BaseEmbedding
+from llama_index.core.schema import Document, QueryBundle, TextNode
+from llama_index.core.storage import StorageContext
+from llama_index.vector_stores.faiss import FaissVectorStore
 
 from metagpt.document import IndexableDocument
 from metagpt.document_store.base_store import LocalStore
 from metagpt.logs import logger
 from metagpt.utils.embedding import get_embedding
 
 
 class FaissStore(LocalStore):
     def __init__(
-        self, raw_data: Path, cache_dir=None, meta_col="source", content_col="output", embedding: Embeddings = None
+        self, raw_data: Path, cache_dir=None, meta_col="source", content_col="output", embedding: BaseEmbedding = None
     ):
         self.meta_col = meta_col
         self.content_col = content_col
         self.embedding = embedding or get_embedding()
+        self.store: VectorStoreIndex
         super().__init__(raw_data, cache_dir)
 
-    def _load(self) -> Optional["FaissStore"]:
-        index_file, store_file = self._get_index_and_store_fname(index_ext=".faiss")  # langchain FAISS using .faiss
+    def _load(self) -> Optional["VectorStoreIndex"]:
+        index_file, store_file = self._get_index_and_store_fname()
 
         if not (index_file.exists() and store_file.exists()):
             logger.info("Missing at least one of index_file/store_file, load failed and return None")
             return None
+        vector_store = FaissVectorStore.from_persist_dir(persist_dir=self.cache_dir)
+        storage_context = StorageContext.from_defaults(persist_dir=self.cache_dir, vector_store=vector_store)
+        index = load_index_from_storage(storage_context, embed_model=self.embedding)
+
+        return index
+
+    def _write(self, docs: list[str], metadatas: list[dict[str, Any]]) -> VectorStoreIndex:
+        assert len(docs) == len(metadatas)
+        documents = [Document(text=doc, metadata=metadatas[idx]) for idx, doc in enumerate(docs)]
+
+        vector_store = FaissVectorStore(faiss_index=faiss.IndexFlatL2(1536))
+        storage_context = StorageContext.from_defaults(vector_store=vector_store)
+        index = VectorStoreIndex.from_documents(
+            documents=documents, storage_context=storage_context, embed_model=self.embedding
+        )
 
-        return FAISS.load_local(self.raw_data_path.parent, self.embedding, self.fname)
-
-    def _write(self, docs, metadatas):
-        store = FAISS.from_texts(docs, self.embedding, metadatas=metadatas)
-        return store
+        return index
 
     def persist(self):
-        self.store.save_local(self.raw_data_path.parent, self.fname)
+        self.store.storage_context.persist(self.cache_dir)
+
+    def search(self, query: str, expand_cols=False, sep="\n", *args, k=5, **kwargs):
+        retriever = self.store.as_retriever(similarity_top_k=k)
+        rsp = retriever.retrieve(QueryBundle(query_str=query, embedding=self.embedding.get_text_embedding(query)))
 
-    def search(self, query, expand_cols=False, sep="\n", *args, k=5, **kwargs):
-        rsp = self.store.similarity_search(query, k=k, **kwargs)
         logger.debug(rsp)
         if expand_cols:
-            return str(sep.join([f"{x.page_content}: {x.metadata}" for x in rsp]))
+            return str(sep.join([f"{x.node.text}: {x.node.metadata}" for x in rsp]))
         else:
-            return str(sep.join([f"{x.page_content}" for x in rsp]))
+            return str(sep.join([f"{x.node.text}" for x in rsp]))
 
     async def asearch(self, *args, **kwargs):
         return await asyncio.to_thread(self.search, *args, **kwargs)
 
     def write(self):
         """Initialize the index and library based on the Document (JSON / XLSX, etc.) file provided by the user."""
         if not self.raw_data_path.exists():
@@ -63,12 +81,16 @@
 
         self.store = self._write(docs, metadatas)
         self.persist()
         return self.store
 
     def add(self, texts: list[str], *args, **kwargs) -> list[str]:
         """FIXME: Currently, the store is not updated after adding."""
-        return self.store.add_texts(texts)
+        texts_embeds = self.embedding.get_text_embedding_batch(texts)
+        nodes = [TextNode(text=texts[idx], embedding=embed) for idx, embed in enumerate(texts_embeds)]
+        self.store.insert_nodes(nodes)
+
+        return []
 
     def delete(self, *args, **kwargs):
-        """Currently, langchain does not provide a delete interface."""
+        """Currently, faiss does not provide a delete interface."""
         raise NotImplementedError
```

### Comparing `metagpt-0.7.7/metagpt/document_store/lancedb_store.py` & `metagpt-0.8.0/metagpt/document_store/lancedb_store.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/document_store/qdrant_store.py` & `metagpt-0.8.0/metagpt/document_store/qdrant_store.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/environment/android_env/android_ext_env.py` & `metagpt-0.8.0/metagpt/environment/android_env/android_ext_env.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/environment/api/env_api.py` & `metagpt-0.8.0/metagpt/environment/api/env_api.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/environment/base_env.py` & `metagpt-0.8.0/metagpt/roles/di/data_interpreter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,212 +1,184 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# @Desc   : base env of executing environment
-
-import asyncio
-from enum import Enum
-from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Set, Union
-
-from pydantic import BaseModel, ConfigDict, Field, SerializeAsAny, model_validator
-
-from metagpt.context import Context
-from metagpt.environment.api.env_api import (
-    EnvAPIAbstract,
-    ReadAPIRegistry,
-    WriteAPIRegistry,
-)
-from metagpt.logs import logger
-from metagpt.schema import Message
-from metagpt.utils.common import get_function_schema, is_coroutine_func, is_send_to
-
-if TYPE_CHECKING:
-    from metagpt.roles.role import Role  # noqa: F401
-
-
-class EnvType(Enum):
-    ANDROID = "Android"
-    GYM = "Gym"
-    WEREWOLF = "Werewolf"
-    MINCRAFT = "Mincraft"
-    STANFORDTOWN = "StanfordTown"
-
-
-env_write_api_registry = WriteAPIRegistry()
-env_read_api_registry = ReadAPIRegistry()
-
-
-def mark_as_readable(func):
-    """mark functionn as a readable one in ExtEnv, it observes something from ExtEnv"""
-    env_read_api_registry[func.__name__] = get_function_schema(func)
-    return func
-
-
-def mark_as_writeable(func):
-    """mark functionn as a writeable one in ExtEnv, it does something to ExtEnv"""
-    env_write_api_registry[func.__name__] = get_function_schema(func)
-    return func
-
+from __future__ import annotations
 
-class ExtEnv(BaseModel):
-    """External Env to intergate actual game environment"""
+import json
+from typing import Literal, Union
 
-    def _check_api_exist(self, rw_api: Optional[str] = None):
-        if not rw_api:
-            raise ValueError(f"{rw_api} not exists")
+from pydantic import Field, model_validator
 
-    def get_all_available_apis(self, mode: str = "read") -> list[Any]:
-        """get available read/write apis definition"""
-        assert mode in ["read", "write"]
-        if mode == "read":
-            return env_read_api_registry.get_apis()
-        else:
-            return env_write_api_registry.get_apis()
-
-    async def observe(self, env_action: Union[str, EnvAPIAbstract]):
-        """get observation from particular api of ExtEnv"""
-        if isinstance(env_action, str):
-            read_api = env_read_api_registry.get(api_name=env_action)["func"]
-            self._check_api_exist(read_api)
-            if is_coroutine_func(read_api):
-                res = await read_api(self)
-            else:
-                res = read_api(self)
-        elif isinstance(env_action, EnvAPIAbstract):
-            read_api = env_read_api_registry.get(api_name=env_action.api_name)["func"]
-            self._check_api_exist(read_api)
-            if is_coroutine_func(read_api):
-                res = await read_api(self, *env_action.args, **env_action.kwargs)
-            else:
-                res = read_api(self, *env_action.args, **env_action.kwargs)
-        return res
-
-    async def step(self, env_action: Union[str, Message, EnvAPIAbstract, list[EnvAPIAbstract]]):
-        """execute through particular api of ExtEnv"""
-        res = None
-        if isinstance(env_action, Message):
-            self.publish_message(env_action)
-        elif isinstance(env_action, EnvAPIAbstract):
-            write_api = env_write_api_registry.get(env_action.api_name)["func"]
-            self._check_api_exist(write_api)
-            if is_coroutine_func(write_api):
-                res = await write_api(self, *env_action.args, **env_action.kwargs)
-            else:
-                res = write_api(self, *env_action.args, **env_action.kwargs)
-
-        return res
-
-
-class Environment(ExtEnv):
-    """环境，承载一批角色，角色可以向环境发布消息，可以被其他角色观察到
-    Environment, hosting a batch of roles, roles can publish messages to the environment, and can be observed by other roles
-    """
-
-    model_config = ConfigDict(arbitrary_types_allowed=True)
-
-    desc: str = Field(default="")  # 环境描述
-    roles: dict[str, SerializeAsAny["Role"]] = Field(default_factory=dict, validate_default=True)
-    member_addrs: Dict["Role", Set] = Field(default_factory=dict, exclude=True)
-    history: str = ""  # For debug
-    context: Context = Field(default_factory=Context, exclude=True)
+from metagpt.actions.di.ask_review import ReviewConst
+from metagpt.actions.di.execute_nb_code import ExecuteNbCode
+from metagpt.actions.di.write_analysis_code import CheckData, WriteAnalysisCode
+from metagpt.logs import logger
+from metagpt.prompts.di.write_analysis_code import DATA_INFO
+from metagpt.roles import Role
+from metagpt.schema import Message, Task, TaskResult
+from metagpt.strategy.task_type import TaskType
+from metagpt.tools.tool_recommend import BM25ToolRecommender, ToolRecommender
+from metagpt.utils.common import CodeParser
+
+REACT_THINK_PROMPT = """
+# User Requirement
+{user_requirement}
+# Context
+{context}
+
+Output a json following the format:
+```json
+{{
+    "thoughts": str = "Thoughts on current situation, reflect on how you should proceed to fulfill the user requirement",
+    "state": bool = "Decide whether you need to take more actions to complete the user requirement. Return true if you think so. Return false if you think the requirement has been completely fulfilled."
+}}
+```
+"""
+
+
+class DataInterpreter(Role):
+    name: str = "David"
+    profile: str = "DataInterpreter"
+    auto_run: bool = True
+    use_plan: bool = True
+    use_reflection: bool = False
+    execute_code: ExecuteNbCode = Field(default_factory=ExecuteNbCode, exclude=True)
+    tools: Union[str, list[str]] = []  # Use special symbol ["<all>"] to indicate use of all registered tools
+    tool_recommender: ToolRecommender = None
+    react_mode: Literal["plan_and_act", "react"] = "plan_and_act"
+    max_react_loop: int = 10  # used for react mode
 
     @model_validator(mode="after")
-    def init_roles(self):
-        self.add_roles(self.roles.values())
+    def set_plan_and_tool(self) -> "Interpreter":
+        self._set_react_mode(react_mode=self.react_mode, max_react_loop=self.max_react_loop, auto_run=self.auto_run)
+        self.use_plan = (
+            self.react_mode == "plan_and_act"
+        )  # create a flag for convenience, overwrite any passed-in value
+        if self.tools:
+            self.tool_recommender = BM25ToolRecommender(tools=self.tools)
+        self.set_actions([WriteAnalysisCode])
+        self._set_state(0)
         return self
 
-    def add_role(self, role: "Role"):
-        """增加一个在当前环境的角色
-        Add a role in the current environment
-        """
-        self.roles[role.profile] = role
-        role.set_env(self)
-        role.context = self.context
-
-    def add_roles(self, roles: Iterable["Role"]):
-        """增加一批在当前环境的角色
-        Add a batch of characters in the current environment
-        """
-        for role in roles:
-            self.roles[role.profile] = role
-
-        for role in roles:  # setup system message with roles
-            role.set_env(self)
-            role.context = self.context
-
-    def publish_message(self, message: Message, peekable: bool = True) -> bool:
-        """
-        Distribute the message to the recipients.
-        In accordance with the Message routing structure design in Chapter 2.2.1 of RFC 116, as already planned
-        in RFC 113 for the entire system, the routing information in the Message is only responsible for
-        specifying the message recipient, without concern for where the message recipient is located. How to
-        route the message to the message recipient is a problem addressed by the transport framework designed
-        in RFC 113.
-        """
-        logger.debug(f"publish_message: {message.dump()}")
-        found = False
-        # According to the routing feature plan in Chapter 2.2.3.2 of RFC 113
-        for role, addrs in self.member_addrs.items():
-            if is_send_to(message, addrs):
-                role.put_message(message)
-                found = True
-        if not found:
-            logger.warning(f"Message no recipients: {message.dump()}")
-        self.history += f"\n{message}"  # For debug
-
-        return True
-
-    async def run(self, k=1):
-        """处理一次所有信息的运行
-        Process all Role runs at once
-        """
-        for _ in range(k):
-            futures = []
-            for role in self.roles.values():
-                future = role.run()
-                futures.append(future)
-
-            await asyncio.gather(*futures)
-            logger.debug(f"is idle: {self.is_idle}")
-
-    def get_roles(self) -> dict[str, "Role"]:
-        """获得环境内的所有角色
-        Process all Role runs at once
-        """
-        return self.roles
-
-    def get_role(self, name: str) -> "Role":
-        """获得环境内的指定角色
-        get all the environment roles
-        """
-        return self.roles.get(name, None)
-
-    def role_names(self) -> list[str]:
-        return [i.name for i in self.roles.values()]
-
     @property
-    def is_idle(self):
-        """If true, all actions have been executed."""
-        for r in self.roles.values():
-            if not r.is_idle:
-                return False
-        return True
+    def working_memory(self):
+        return self.rc.working_memory
 
-    def get_addresses(self, obj):
-        """Get the addresses of the object."""
-        return self.member_addrs.get(obj, {})
-
-    def set_addresses(self, obj, addresses):
-        """Set the addresses of the object"""
-        self.member_addrs[obj] = addresses
-
-    def archive(self, auto_archive=True):
-        if auto_archive and self.context.git_repo:
-            self.context.git_repo.archive()
-
-    @classmethod
-    def model_rebuild(cls, **kwargs):
-        from metagpt.roles.role import Role  # noqa: F401
-
-        super().model_rebuild(**kwargs)
+    async def _think(self) -> bool:
+        """Useful in 'react' mode. Use LLM to decide whether and what to do next."""
+        user_requirement = self.get_memories()[0].content
+        context = self.working_memory.get()
+
+        if not context:
+            # just started the run, we need action certainly
+            self.working_memory.add(self.get_memories()[0])  # add user requirement to working memory
+            self._set_state(0)
+            return True
+
+        prompt = REACT_THINK_PROMPT.format(user_requirement=user_requirement, context=context)
+        rsp = await self.llm.aask(prompt)
+        rsp_dict = json.loads(CodeParser.parse_code(block=None, text=rsp))
+        self.working_memory.add(Message(content=rsp_dict["thoughts"], role="assistant"))
+        need_action = rsp_dict["state"]
+        self._set_state(0) if need_action else self._set_state(-1)
+
+        return need_action
+
+    async def _act(self) -> Message:
+        """Useful in 'react' mode. Return a Message conforming to Role._act interface."""
+        code, _, _ = await self._write_and_exec_code()
+        return Message(content=code, role="assistant", cause_by=WriteAnalysisCode)
+
+    async def _plan_and_act(self) -> Message:
+        rsp = await super()._plan_and_act()
+        await self.execute_code.terminate()
+        return rsp
+
+    async def _act_on_task(self, current_task: Task) -> TaskResult:
+        """Useful in 'plan_and_act' mode. Wrap the output in a TaskResult for review and confirmation."""
+        code, result, is_success = await self._write_and_exec_code()
+        task_result = TaskResult(code=code, result=result, is_success=is_success)
+        return task_result
+
+    async def _write_and_exec_code(self, max_retry: int = 3):
+        counter = 0
+        success = False
+
+        # plan info
+        plan_status = self.planner.get_plan_status() if self.use_plan else ""
+
+        # tool info
+        if self.tools:
+            context = (
+                self.working_memory.get()[-1].content if self.working_memory.get() else ""
+            )  # thoughts from _think stage in 'react' mode
+            plan = self.planner.plan if self.use_plan else None
+            tool_info = await self.tool_recommender.get_recommended_tool_info(context=context, plan=plan)
+        else:
+            tool_info = ""
 
+        # data info
+        await self._check_data()
 
-Environment.model_rebuild()
+        while not success and counter < max_retry:
+            ### write code ###
+            code, cause_by = await self._write_code(counter, plan_status, tool_info)
+
+            self.working_memory.add(Message(content=code, role="assistant", cause_by=cause_by))
+
+            ### execute code ###
+            result, success = await self.execute_code.run(code)
+            print(result)
+
+            self.working_memory.add(Message(content=result, role="user", cause_by=ExecuteNbCode))
+
+            ### process execution result ###
+            counter += 1
+
+            if not success and counter >= max_retry:
+                logger.info("coding failed!")
+                review, _ = await self.planner.ask_review(auto_run=False, trigger=ReviewConst.CODE_REVIEW_TRIGGER)
+                if ReviewConst.CHANGE_WORDS[0] in review:
+                    counter = 0  # redo the task again with help of human suggestions
+
+        return code, result, success
+
+    async def _write_code(
+        self,
+        counter: int,
+        plan_status: str = "",
+        tool_info: str = "",
+    ):
+        todo = self.rc.todo  # todo is WriteAnalysisCode
+        logger.info(f"ready to {todo.name}")
+        use_reflection = counter > 0 and self.use_reflection  # only use reflection after the first trial
+
+        user_requirement = self.get_memories()[0].content
+
+        code = await todo.run(
+            user_requirement=user_requirement,
+            plan_status=plan_status,
+            tool_info=tool_info,
+            working_memory=self.working_memory.get(),
+            use_reflection=use_reflection,
+        )
+
+        return code, todo
+
+    async def _check_data(self):
+        if (
+            not self.use_plan
+            or not self.planner.plan.get_finished_tasks()
+            or self.planner.plan.current_task.task_type
+            not in [
+                TaskType.DATA_PREPROCESS.type_name,
+                TaskType.FEATURE_ENGINEERING.type_name,
+                TaskType.MODEL_TRAIN.type_name,
+            ]
+        ):
+            return
+        logger.info("Check updated data")
+        code = await CheckData().run(self.planner.plan)
+        if not code.strip():
+            return
+        result, success = await self.execute_code.run(code)
+        if success:
+            print(result)
+            data_info = DATA_INFO.format(info=result)
+            self.working_memory.add(Message(content=data_info, role="user", cause_by=CheckData))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `metagpt-0.7.7/metagpt/environment/mincraft_env/const.py` & `metagpt-0.8.0/metagpt/environment/minecraft_env/const.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # @Desc   :
 
 from metagpt.const import METAGPT_ROOT
 
-# For Mincraft Game Agent
-MC_CKPT_DIR = METAGPT_ROOT / "data/mincraft/ckpt"
+# For Minecraft Game Agent
+MC_CKPT_DIR = METAGPT_ROOT / "data/minecraft/ckpt"
 MC_LOG_DIR = METAGPT_ROOT / "logs"
 MC_DEFAULT_WARMUP = {
     "context": 15,
     "biome": 10,
     "time": 15,
     "nearby_blocks": 0,
     "other_blocks": 10,
```

### Comparing `metagpt-0.7.7/metagpt/environment/mincraft_env/mincraft_env.py` & `metagpt-0.8.0/metagpt/environment/minecraft_env/minecraft_env.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# @Desc   : MG Mincraft Env
+# @Desc   : MG Minecraft Env
 #           refs to `voyager voyager.py`
 
 import json
 import re
 import time
 from typing import Any, Iterable
 
-from langchain.embeddings.openai import OpenAIEmbeddings
-from langchain.vectorstores import Chroma
+from llama_index.vector_stores.chroma import ChromaVectorStore
 from pydantic import ConfigDict, Field
 
 from metagpt.config2 import config as CONFIG
 from metagpt.environment.base_env import Environment
-from metagpt.environment.mincraft_env.const import MC_CKPT_DIR
-from metagpt.environment.mincraft_env.mincraft_ext_env import MincraftExtEnv
+from metagpt.environment.minecraft_env.const import MC_CKPT_DIR
+from metagpt.environment.minecraft_env.minecraft_ext_env import MinecraftExtEnv
 from metagpt.logs import logger
 from metagpt.utils.common import load_mc_skills_code, read_json_file, write_json_file
 
 
-class MincraftEnv(Environment, MincraftExtEnv):
-    """MincraftEnv, including shared memory of cache and infomation between roles"""
+class MinecraftEnv(Environment, MinecraftExtEnv):
+    """MinecraftEnv, including shared memory of cache and information between roles"""
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     event: dict[str, Any] = Field(default_factory=dict)
     current_task: str = Field(default="Mine 1 wood log")
     task_execution_time: float = Field(default=float)
     context: str = Field(default="You can mine one of oak, birch, spruce, jungle, acacia, dark oak, or mangrove logs.")
@@ -44,17 +43,17 @@
     skill_desp: str = Field(default="")
 
     chest_memory: dict[str, Any] = Field(default_factory=dict)  # eg: {'(1344, 64, 1381)': 'Unknown'}
     chest_observation: str = Field(default="")  # eg: "Chests: None\n\n"
 
     runtime_status: bool = False  # equal to action execution status: success or failed
 
-    vectordb: Chroma = Field(default_factory=Chroma)
+    vectordb: ChromaVectorStore = Field(default_factory=ChromaVectorStore)
 
-    qa_cache_questions_vectordb: Chroma = Field(default_factory=Chroma)
+    qa_cache_questions_vectordb: ChromaVectorStore = Field(default_factory=ChromaVectorStore)
 
     @property
     def progress(self):
         # return len(self.completed_tasks) + 10 # Test only
         return len(self.completed_tasks)
 
     @property
@@ -69,24 +68,22 @@
         return programs
 
     def set_mc_port(self, mc_port):
         super().set_mc_port(mc_port)
         self.set_mc_resume()
 
     def set_mc_resume(self):
-        self.qa_cache_questions_vectordb = Chroma(
+        self.qa_cache_questions_vectordb = ChromaVectorStore(
             collection_name="qa_cache_questions_vectordb",
-            embedding_function=OpenAIEmbeddings(),
-            persist_directory=f"{MC_CKPT_DIR}/curriculum/vectordb",
+            persist_dir=f"{MC_CKPT_DIR}/curriculum/vectordb",
         )
 
-        self.vectordb = Chroma(
+        self.vectordb = ChromaVectorStore(
             collection_name="skill_vectordb",
-            embedding_function=OpenAIEmbeddings(),
-            persist_directory=f"{MC_CKPT_DIR}/skill/vectordb",
+            persist_dir=f"{MC_CKPT_DIR}/skill/vectordb",
         )
 
         if CONFIG.resume:
             logger.info(f"Loading Action Developer from {MC_CKPT_DIR}/action")
             self.chest_memory = read_json_file(f"{MC_CKPT_DIR}/action/chest_memory.json")
 
             logger.info(f"Loading Curriculum Agent from {MC_CKPT_DIR}/curriculum")
```

### Comparing `metagpt-0.7.7/metagpt/environment/mincraft_env/mincraft_ext_env.py` & `metagpt-0.8.0/metagpt/environment/minecraft_env/minecraft_ext_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# @Desc   : The Mincraft external environment to integrate with Mincraft game
+# @Desc   : The Minecraft external environment to integrate with Minecraft game
 #           refs to `voyager bridge.py`
 
 import json
 import time
 from typing import Optional
 
 import requests
 from pydantic import ConfigDict, Field, model_validator
 
 from metagpt.environment.base_env import ExtEnv, mark_as_writeable
-from metagpt.environment.mincraft_env.const import (
+from metagpt.environment.minecraft_env.const import (
     MC_CKPT_DIR,
     MC_CORE_INVENTORY_ITEMS,
     MC_CURRICULUM_OB,
     MC_DEFAULT_WARMUP,
     METAGPT_ROOT,
 )
-from metagpt.environment.mincraft_env.process_monitor import SubprocessMonitor
+from metagpt.environment.minecraft_env.process_monitor import SubprocessMonitor
 from metagpt.logs import logger
 
 
-class MincraftExtEnv(ExtEnv):
+class MinecraftExtEnv(ExtEnv):
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     mc_port: Optional[int] = Field(default=None)
     server_host: str = Field(default="http://127.0.0.1")
     server_port: str = Field(default=3000)
     request_timeout: int = Field(default=600)
 
@@ -44,15 +44,15 @@
 
     @model_validator(mode="after")
     def _post_init_ext_env(self):
         if not self.mineflayer:
             self.mineflayer = SubprocessMonitor(
                 commands=[
                     "node",
-                    METAGPT_ROOT.joinpath("metagpt", "environment", "mincraft_env", "mineflayer", "index.js"),
+                    METAGPT_ROOT.joinpath("metagpt", "environment", "minecraft_env", "mineflayer", "index.js"),
                     str(self.server_port),
                 ],
                 name="mineflayer",
                 ready_match=r"Server started on port (\d+)",
             )
         if not self.warm_up:
             warm_up = MC_DEFAULT_WARMUP
```

### Comparing `metagpt-0.7.7/metagpt/environment/mincraft_env/process_monitor.py` & `metagpt-0.8.0/metagpt/environment/minecraft_env/process_monitor.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/environment/stanford_town_env/stanford_town_ext_env.py` & `metagpt-0.8.0/metagpt/environment/stanford_town_env/stanford_town_ext_env.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/environment/werewolf_env/werewolf_env.py` & `metagpt-0.8.0/metagpt/environment/werewolf_env/werewolf_env.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/environment/werewolf_env/werewolf_ext_env.py` & `metagpt-0.8.0/metagpt/environment/werewolf_env/werewolf_ext_env.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/learn/google_search.py` & `metagpt-0.8.0/metagpt/learn/google_search.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/learn/skill_loader.py` & `metagpt-0.8.0/metagpt/learn/skill_loader.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/learn/text_to_embedding.py` & `metagpt-0.8.0/metagpt/learn/text_to_embedding.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/learn/text_to_image.py` & `metagpt-0.8.0/metagpt/learn/text_to_image.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/learn/text_to_speech.py` & `metagpt-0.8.0/metagpt/learn/text_to_speech.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/llm.py` & `metagpt-0.8.0/metagpt/llm.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/logs.py` & `metagpt-0.8.0/metagpt/logs.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/management/skill_manager.py` & `metagpt-0.8.0/metagpt/management/skill_manager.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/memory/brain_memory.py` & `metagpt-0.8.0/metagpt/memory/brain_memory.py`

 * *Files 11% similar despite different names*

```diff
@@ -182,34 +182,38 @@
         summary = await self.summarize(llm=llm, max_words=500)
 
         language = config.language
         command = f"Translate the above summary into a {language} title of less than {max_words} words."
         summaries = [summary, command]
         msg = "\n".join(summaries)
         logger.debug(f"title ask:{msg}")
-        response = await llm.aask(msg=msg, system_msgs=[])
+        response = await llm.aask(msg=msg, system_msgs=[], stream=False)
         logger.debug(f"title rsp: {response}")
         return response
 
     async def is_related(self, text1, text2, llm):
         if isinstance(llm, MetaGPTLLM):
             return await self._metagpt_is_related(text1=text1, text2=text2, llm=llm)
         return await self._openai_is_related(text1=text1, text2=text2, llm=llm)
 
     @staticmethod
     async def _metagpt_is_related(**kwargs):
         return False
 
     @staticmethod
     async def _openai_is_related(text1, text2, llm, **kwargs):
-        command = (
-            f"{text2}\n\nIs there any sentence above related to the following sentence: {text1}.\nIf is there "
-            "any relevance, return [TRUE] brief and clear. Otherwise, return [FALSE] brief and clear."
+        context = f"## Paragraph 1\n{text2}\n---\n## Paragraph 2\n{text1}\n"
+        rsp = await llm.aask(
+            msg=context,
+            system_msgs=[
+                "You are a tool capable of determining whether two paragraphs are semantically related."
+                'Return "TRUE" if "Paragraph 1" is semantically relevant to "Paragraph 2", otherwise return "FALSE".'
+            ],
+            stream=False,
         )
-        rsp = await llm.aask(msg=command, system_msgs=[])
         result = True if "TRUE" in rsp else False
         p2 = text2.replace("\n", "")
         p1 = text1.replace("\n", "")
         logger.info(f"IS_RELATED:\nParagraph 1: {p2}\nParagraph 2: {p1}\nRESULT: {result}\n")
         return result
 
     async def rewrite(self, sentence: str, context: str, llm):
@@ -219,20 +223,25 @@
 
     @staticmethod
     async def _metagpt_rewrite(sentence: str, **kwargs):
         return sentence
 
     @staticmethod
     async def _openai_rewrite(sentence: str, context: str, llm):
-        command = (
-            f"{context}\n\nExtract relevant information from every preceding sentence and use it to succinctly "
-            f"supplement or rewrite the following text in brief and clear:\n{sentence}"
+        prompt = f"## Context\n{context}\n---\n## Sentence\n{sentence}\n"
+        rsp = await llm.aask(
+            msg=prompt,
+            system_msgs=[
+                'You are a tool augmenting the "Sentence" with information from the "Context".',
+                "Do not supplement the context with information that is not present, especially regarding the subject and object.",
+                "Return the augmented sentence.",
+            ],
+            stream=False,
         )
-        rsp = await llm.aask(msg=command, system_msgs=[])
-        logger.info(f"REWRITE:\nCommand: {command}\nRESULT: {rsp}\n")
+        logger.info(f"REWRITE:\nCommand: {prompt}\nRESULT: {rsp}\n")
         return rsp
 
     @staticmethod
     def extract_info(input_string, pattern=r"\[([A-Z]+)\]:\s*(.+)"):
         match = re.match(pattern, input_string)
         if match:
             return match.group(1), match.group(2)
@@ -289,22 +298,22 @@
             max_count -= 1  # safeguard
         return summary
 
     async def _get_summary(self, text: str, max_words=20, keep_language: bool = False):
         """Generate text summary"""
         if len(text) < max_words:
             return text
+        system_msgs = [
+            "You are a tool for summarizing and abstracting text.",
+            f"Return the summarized text to less than {max_words} words.",
+        ]
         if keep_language:
-            command = f".Translate the above content into a summary of less than {max_words} words in language of the content strictly."
-        else:
-            command = f"Translate the above content into a summary of less than {max_words} words."
-        msg = text + "\n\n" + command
-        logger.debug(f"summary ask:{msg}")
-        response = await self.llm.aask(msg=msg, system_msgs=[])
-        logger.debug(f"summary rsp: {response}")
+            system_msgs.append("The generated summary should be in the same language as the original text.")
+        response = await self.llm.aask(msg=text, system_msgs=system_msgs, stream=False)
+        logger.debug(f"{text}\nsummary rsp: {response}")
         return response
 
     @staticmethod
     def split_texts(text: str, window_size) -> List[str]:
         """Splitting long text into sliding windows text"""
         if window_size <= 0:
             window_size = DEFAULT_TOKEN_SIZE
```

### Comparing `metagpt-0.7.7/metagpt/memory/longterm_memory.py` & `metagpt-0.8.0/metagpt/memory/longterm_memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,53 +25,54 @@
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     memory_storage: MemoryStorage = Field(default_factory=MemoryStorage)
     rc: Optional[RoleContext] = None
     msg_from_recover: bool = False
 
     def recover_memory(self, role_id: str, rc: RoleContext):
-        messages = self.memory_storage.recover_memory(role_id)
+        self.memory_storage.recover_memory(role_id)
         self.rc = rc
         if not self.memory_storage.is_initialized:
-            logger.warning(f"It may the first time to run Agent {role_id}, the long-term memory is empty")
+            logger.warning(f"It may the first time to run Role {role_id}, the long-term memory is empty")
         else:
-            logger.warning(
-                f"Agent {role_id} has existing memory storage with {len(messages)} messages " f"and has recovered them."
-            )
+            logger.warning(f"Role {role_id} has existing memory storage and has recovered them.")
         self.msg_from_recover = True
-        self.add_batch(messages)
+        # self.add_batch(messages) # TODO no need
         self.msg_from_recover = False
 
     def add(self, message: Message):
         super().add(message)
         for action in self.rc.watch:
             if message.cause_by == action and not self.msg_from_recover:
                 # currently, only add role's watching messages to its memory_storage
                 # and ignore adding messages from recover repeatedly
                 self.memory_storage.add(message)
 
-    def find_news(self, observed: list[Message], k=0) -> list[Message]:
+    async def find_news(self, observed: list[Message], k=0) -> list[Message]:
         """
         find news (previously unseen messages) from the the most recent k memories, from all memories when k=0
             1. find the short-term memory(stm) news
             2. furthermore, filter out similar messages based on ltm(long-term memory), get the final news
         """
         stm_news = super().find_news(observed, k=k)  # shot-term memory news
         if not self.memory_storage.is_initialized:
             # memory_storage hasn't initialized, use default `find_news` to get stm_news
             return stm_news
 
         ltm_news: list[Message] = []
         for mem in stm_news:
             # filter out messages similar to those seen previously in ltm, only keep fresh news
-            mem_searched = self.memory_storage.search_dissimilar(mem)
-            if len(mem_searched) > 0:
+            mem_searched = await self.memory_storage.search_similar(mem)
+            if len(mem_searched) == 0:
                 ltm_news.append(mem)
         return ltm_news[-k:]
 
+    def persist(self):
+        self.memory_storage.persist()
+
     def delete(self, message: Message):
         super().delete(message)
         # TODO delete message in memory_storage
 
     def clear(self):
         super().clear()
         self.memory_storage.clean()
```

### Comparing `metagpt-0.7.7/metagpt/memory/memory.py` & `metagpt-0.8.0/metagpt/memory/memory.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/prompts/invoice_ocr.py` & `metagpt-0.8.0/metagpt/prompts/invoice_ocr.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/prompts/metagpt_sample.py` & `metagpt-0.8.0/metagpt/prompts/metagpt_sample.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/prompts/sales.py` & `metagpt-0.8.0/metagpt/prompts/sales.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/prompts/summarize.py` & `metagpt-0.8.0/metagpt/prompts/summarize.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/prompts/tool_types.py` & `metagpt-0.8.0/metagpt/prompts/task_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,55 @@
-# Prompt for using tools of "eda" type
+# Prompt for taking on "eda" tasks
 EDA_PROMPT = """
 The current task is about exploratory data analysis, please note the following:
 - Distinguish column types with `select_dtypes` for tailored analysis and visualization, such as correlation.
 - Remember to `import numpy as np` before using Numpy functions.
 """
 
-# Prompt for using tools of "data_preprocess" type
+# Prompt for taking on "data_preprocess" tasks
 DATA_PREPROCESS_PROMPT = """
 The current task is about data preprocessing, please note the following:
 - Monitor data types per column, applying appropriate methods.
 - Ensure operations are on existing dataset columns.
 - Avoid writing processed data to files.
 - Avoid any change to label column, such as standardization, etc.
 - Prefer alternatives to one-hot encoding for categorical data.
 - Only encode or scale necessary columns to allow for potential feature-specific engineering tasks (like time_extract, binning, extraction, etc.) later.
 - Each step do data preprocessing to train, must do same for test separately at the same time.
+- Always copy the DataFrame before processing it and use the copy to process.
 """
 
-# Prompt for using tools of "feature_engineering" type
+# Prompt for taking on "feature_engineering" tasks
 FEATURE_ENGINEERING_PROMPT = """
 The current task is about feature engineering. when performing it, please adhere to the following principles:
 - Generate as diverse features as possible to improve the model's performance step-by-step. 
 - Use available feature engineering tools if they are potential impactful.
 - Avoid creating redundant or excessively numerous features in one step.
 - Exclude ID columns from feature generation and remove them.
 - Each feature engineering operation performed on the train set must also applies to the test separately at the same time.
 - Avoid using the label column to create features, except for cat encoding.
 - Use the data from previous task result if exist, do not mock or reload data yourself.
+- Always copy the DataFrame before processing it and use the copy to process.
 """
 
-# Prompt for using tools of "model_train" type
+# Prompt for taking on "model_train" tasks
 MODEL_TRAIN_PROMPT = """
 The current task is about training a model, please ensure high performance:
 - Keep in mind that your user prioritizes results and is highly focused on model performance. So, when needed, feel free to use models of any complexity to improve effectiveness, such as XGBoost, CatBoost, etc.
 - If non-numeric columns exist, perform label encode together with all steps.
 - Use the data from previous task result directly, do not mock or reload data yourself.
 - Set suitable hyperparameters for the model, make metrics as high as possible.
 """
 
-# Prompt for using tools of "model_evaluate" type
+# Prompt for taking on "model_evaluate" tasks
 MODEL_EVALUATE_PROMPT = """
 The current task is about evaluating a model, please note the following:
 - Ensure that the evaluated data is same processed as the training data. If not, remember use object in 'Done Tasks' to transform the data.
 - Use trained model from previous task result directly, do not mock or reload model yourself.
 """
 
-# Prompt for using tools of "vision" type
+# Prompt for taking on "image2webpage" tasks
 IMAGE2WEBPAGE_PROMPT = """
 The current task is about converting image into webpage code. please note the following:
 - Single-Step Code Generation: Execute the entire code generation process in a single step, encompassing HTML, CSS, and JavaScript. Avoid fragmenting the code generation into multiple separate steps to maintain consistency and simplify the development workflow.
 - Save webpages: Be sure to use the save method provided.
 """
```

### Comparing `metagpt-0.7.7/metagpt/prompts/tutorial_assistant.py` & `metagpt-0.8.0/metagpt/prompts/tutorial_assistant.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/provider/__init__.py` & `metagpt-0.8.0/metagpt/provider/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 # -*- coding: utf-8 -*-
 """
 @Time    : 2023/5/5 22:59
 @Author  : alexanderwu
 @File    : __init__.py
 """
 
-from metagpt.provider.fireworks_api import FireworksLLM
 from metagpt.provider.google_gemini_api import GeminiLLM
 from metagpt.provider.ollama_api import OllamaLLM
-from metagpt.provider.open_llm_api import OpenLLM
 from metagpt.provider.openai_api import OpenAILLM
 from metagpt.provider.zhipuai_api import ZhiPuAILLM
 from metagpt.provider.azure_openai_api import AzureOpenAILLM
 from metagpt.provider.metagpt_api import MetaGPTLLM
 from metagpt.provider.human_provider import HumanProvider
 from metagpt.provider.spark_api import SparkLLM
+from metagpt.provider.qianfan_api import QianFanLLM
+from metagpt.provider.dashscope_api import DashScopeLLM
+from metagpt.provider.anthropic_api import AnthropicLLM
 
 __all__ = [
-    "FireworksLLM",
     "GeminiLLM",
-    "OpenLLM",
     "OpenAILLM",
     "ZhiPuAILLM",
     "AzureOpenAILLM",
     "MetaGPTLLM",
     "OllamaLLM",
     "HumanProvider",
     "SparkLLM",
+    "QianFanLLM",
+    "DashScopeLLM",
+    "AnthropicLLM",
 ]
```

### Comparing `metagpt-0.7.7/metagpt/provider/azure_openai_api.py` & `metagpt-0.8.0/metagpt/provider/azure_openai_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 """
 @Time    : 2023/5/5 23:08
 @Author  : alexanderwu
 @File    : openai.py
 @Modified By: mashenquan, 2023/11/21. Fix bug: ReadTimeout.
 @Modified By: mashenquan, 2023/12/1. Fix bug: Unclosed connection caused by openai 0.x.
 """
-
-
 from openai import AsyncAzureOpenAI
 from openai._base_client import AsyncHttpxClientWrapper
 
 from metagpt.configs.llm_config import LLMType
 from metagpt.provider.llm_provider_registry import register_provider
 from metagpt.provider.openai_api import OpenAILLM
 
@@ -23,14 +21,15 @@
     """
 
     def _init_client(self):
         kwargs = self._make_client_kwargs()
         # https://learn.microsoft.com/zh-cn/azure/ai-services/openai/how-to/migration?tabs=python-new%2Cdalle-fix
         self.aclient = AsyncAzureOpenAI(**kwargs)
         self.model = self.config.model  # Used in _calc_usage & _cons_kwargs
+        self.pricing_plan = self.config.pricing_plan or self.model
 
     def _make_client_kwargs(self) -> dict:
         kwargs = dict(
             api_key=self.config.api_key,
             api_version=self.config.api_version,
             azure_endpoint=self.config.base_url,
         )
```

### Comparing `metagpt-0.7.7/metagpt/provider/base_llm.py` & `metagpt-0.8.0/metagpt/provider/base_llm.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,37 +2,50 @@
 # -*- coding: utf-8 -*-
 """
 @Time    : 2023/5/5 23:04
 @Author  : alexanderwu
 @File    : base_llm.py
 @Desc    : mashenquan, 2023/8/22. + try catch
 """
+from __future__ import annotations
+
 import json
 from abc import ABC, abstractmethod
 from typing import Optional, Union
 
 from openai import AsyncOpenAI
+from pydantic import BaseModel
+from tenacity import (
+    after_log,
+    retry,
+    retry_if_exception_type,
+    stop_after_attempt,
+    wait_random_exponential,
+)
 
 from metagpt.configs.llm_config import LLMConfig
+from metagpt.const import LLM_API_TIMEOUT, USE_CONFIG_TIMEOUT
 from metagpt.logs import logger
 from metagpt.schema import Message
-from metagpt.utils.cost_manager import CostManager
+from metagpt.utils.common import log_and_reraise
+from metagpt.utils.cost_manager import CostManager, Costs
 
 
 class BaseLLM(ABC):
     """LLM API abstract class, requiring all inheritors to provide a series of standard capabilities"""
 
     config: LLMConfig
     use_system_prompt: bool = True
     system_prompt = "You are a helpful assistant."
 
     # OpenAI / Azure / Others
     aclient: Optional[Union[AsyncOpenAI]] = None
     cost_manager: Optional[CostManager] = None
-    model: Optional[str] = None
+    model: Optional[str] = None  # deprecated
+    pricing_plan: Optional[str] = None
 
     @abstractmethod
     def __init__(self, config: LLMConfig):
         pass
 
     def _user_msg(self, msg: str, images: Optional[Union[str, list[str]]] = None) -> dict[str, Union[str, dict]]:
         if images:
@@ -57,73 +70,140 @@
 
     def _assistant_msg(self, msg: str) -> dict[str, str]:
         return {"role": "assistant", "content": msg}
 
     def _system_msg(self, msg: str) -> dict[str, str]:
         return {"role": "system", "content": msg}
 
+    def format_msg(self, messages: Union[str, Message, list[dict], list[Message], list[str]]) -> list[dict]:
+        """convert messages to list[dict]."""
+        from metagpt.schema import Message
+
+        if not isinstance(messages, list):
+            messages = [messages]
+
+        processed_messages = []
+        for msg in messages:
+            if isinstance(msg, str):
+                processed_messages.append({"role": "user", "content": msg})
+            elif isinstance(msg, dict):
+                assert set(msg.keys()) == set(["role", "content"])
+                processed_messages.append(msg)
+            elif isinstance(msg, Message):
+                processed_messages.append(msg.to_dict())
+            else:
+                raise ValueError(
+                    f"Only support message type are: str, Message, dict, but got {type(messages).__name__}!"
+                )
+        return processed_messages
+
     def _system_msgs(self, msgs: list[str]) -> list[dict[str, str]]:
         return [self._system_msg(msg) for msg in msgs]
 
     def _default_system_msg(self):
         return self._system_msg(self.system_prompt)
 
+    def _update_costs(self, usage: Union[dict, BaseModel], model: str = None, local_calc_usage: bool = True):
+        """update each request's token cost
+        Args:
+            model (str): model name or in some scenarios called endpoint
+            local_calc_usage (bool): some models don't calculate usage, it will overwrite LLMConfig.calc_usage
+        """
+        calc_usage = self.config.calc_usage and local_calc_usage
+        model = model or self.pricing_plan
+        model = model or self.model
+        usage = usage.model_dump() if isinstance(usage, BaseModel) else usage
+        if calc_usage and self.cost_manager:
+            try:
+                prompt_tokens = int(usage.get("prompt_tokens", 0))
+                completion_tokens = int(usage.get("completion_tokens", 0))
+                self.cost_manager.update_cost(prompt_tokens, completion_tokens, model)
+            except Exception as e:
+                logger.error(f"{self.__class__.__name__} updates costs failed! exp: {e}")
+
+    def get_costs(self) -> Costs:
+        if not self.cost_manager:
+            return Costs(0, 0, 0, 0)
+        return self.cost_manager.get_costs()
+
     async def aask(
         self,
-        msg: str,
+        msg: Union[str, list[dict[str, str]]],
         system_msgs: Optional[list[str]] = None,
         format_msgs: Optional[list[dict[str, str]]] = None,
         images: Optional[Union[str, list[str]]] = None,
-        timeout=3,
+        timeout=USE_CONFIG_TIMEOUT,
         stream=True,
     ) -> str:
         if system_msgs:
             message = self._system_msgs(system_msgs)
         else:
             message = [self._default_system_msg()]
         if not self.use_system_prompt:
             message = []
         if format_msgs:
             message.extend(format_msgs)
-        message.append(self._user_msg(msg, images=images))
+        if isinstance(msg, str):
+            message.append(self._user_msg(msg, images=images))
+        else:
+            message.extend(msg)
         logger.debug(message)
-        rsp = await self.acompletion_text(message, stream=stream, timeout=timeout)
+        rsp = await self.acompletion_text(message, stream=stream, timeout=self.get_timeout(timeout))
         return rsp
 
     def _extract_assistant_rsp(self, context):
         return "\n".join([i["content"] for i in context if i["role"] == "assistant"])
 
-    async def aask_batch(self, msgs: list, timeout=3) -> str:
+    async def aask_batch(self, msgs: list, timeout=USE_CONFIG_TIMEOUT) -> str:
         """Sequential questioning"""
         context = []
         for msg in msgs:
             umsg = self._user_msg(msg)
             context.append(umsg)
-            rsp_text = await self.acompletion_text(context, timeout=timeout)
+            rsp_text = await self.acompletion_text(context, timeout=self.get_timeout(timeout))
             context.append(self._assistant_msg(rsp_text))
         return self._extract_assistant_rsp(context)
 
-    async def aask_code(self, messages: Union[str, Message, list[dict]], timeout=3) -> dict:
-        """FIXME: No code segment filtering has been done here, and all results are actually displayed"""
+    async def aask_code(self, messages: Union[str, Message, list[dict]], timeout=USE_CONFIG_TIMEOUT, **kwargs) -> dict:
         raise NotImplementedError
 
     @abstractmethod
-    async def acompletion(self, messages: list[dict], timeout=3):
+    async def _achat_completion(self, messages: list[dict], timeout=USE_CONFIG_TIMEOUT):
+        """_achat_completion implemented by inherited class"""
+
+    @abstractmethod
+    async def acompletion(self, messages: list[dict], timeout=USE_CONFIG_TIMEOUT):
         """Asynchronous version of completion
         All GPTAPIs are required to provide the standard OpenAI completion interface
         [
             {"role": "system", "content": "You are a helpful assistant."},
             {"role": "user", "content": "hello, show me python hello world code"},
             # {"role": "assistant", "content": ...}, # If there is an answer in the history, also include it
         ]
         """
 
     @abstractmethod
-    async def acompletion_text(self, messages: list[dict], stream=False, timeout=3) -> str:
+    async def _achat_completion_stream(self, messages: list[dict], timeout: int = USE_CONFIG_TIMEOUT) -> str:
+        """_achat_completion_stream implemented by inherited class"""
+
+    @retry(
+        stop=stop_after_attempt(3),
+        wait=wait_random_exponential(min=1, max=60),
+        after=after_log(logger, logger.level("WARNING").name),
+        retry=retry_if_exception_type(ConnectionError),
+        retry_error_callback=log_and_reraise,
+    )
+    async def acompletion_text(
+        self, messages: list[dict], stream: bool = False, timeout: int = USE_CONFIG_TIMEOUT
+    ) -> str:
         """Asynchronous version of completion. Return str. Support stream-print"""
+        if stream:
+            return await self._achat_completion_stream(messages, timeout=self.get_timeout(timeout))
+        resp = await self._achat_completion(messages, timeout=self.get_timeout(timeout))
+        return self.get_choice_text(resp)
 
     def get_choice_text(self, rsp: dict) -> str:
         """Required to provide the first text of choice"""
         return rsp.get("choices")[0]["message"]["content"]
 
     def get_choice_delta_text(self, rsp: dict) -> str:
         """Required to provide the first text of stream choice"""
@@ -172,7 +252,15 @@
     def messages_to_prompt(self, messages: list[dict]):
         """[{"role": "user", "content": msg}] to user: <msg> etc."""
         return "\n".join([f"{i['role']}: {i['content']}" for i in messages])
 
     def messages_to_dict(self, messages):
         """objects to [{"role": "user", "content": msg}] etc."""
         return [i.to_dict() for i in messages]
+
+    def with_model(self, model: str):
+        """Set model and return self. For example, `with_model("gpt-3.5-turbo")`."""
+        self.config.model = model
+        return self
+
+    def get_timeout(self, timeout: int) -> int:
+        return timeout or self.config.timeout or LLM_API_TIMEOUT
```

### Comparing `metagpt-0.7.7/metagpt/provider/constant.py` & `metagpt-0.8.0/metagpt/provider/constant.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,10 +21,11 @@
             },
             "code": {"type": "string", "description": "The code to execute (required)"},
         },
         "required": ["language", "code"],
     },
 }
 
+
 # tool_choice value for general_function_schema
 # https://platform.openai.com/docs/api-reference/chat/create#chat-create-tool_choice
 GENERAL_TOOL_CHOICE = {"type": "function", "function": {"name": "execute"}}
```

### Comparing `metagpt-0.7.7/metagpt/provider/general_api_base.py` & `metagpt-0.8.0/metagpt/provider/general_api_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -569,15 +569,15 @@
 
         if isinstance(request_timeout, tuple):
             timeout = aiohttp.ClientTimeout(
                 connect=request_timeout[0],
                 total=request_timeout[1],
             )
         else:
-            timeout = aiohttp.ClientTimeout(total=request_timeout if request_timeout else TIMEOUT_SECS)
+            timeout = aiohttp.ClientTimeout(total=request_timeout or TIMEOUT_SECS)
 
         if files:
             # TODO: Use `aiohttp.MultipartWriter` to create the multipart form data here.
             # For now we use the private `requests` method that is known to have worked so far.
             data, content_type = requests.models.RequestEncodingMixin._encode_files(files, data)  # type: ignore
             headers["Content-Type"] = content_type
         request_kwargs = {
```

### Comparing `metagpt-0.7.7/metagpt/provider/general_api_requestor.py` & `metagpt-0.8.0/metagpt/provider/general_api_requestor.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/provider/google_gemini_api.py` & `metagpt-0.8.0/metagpt/provider/google_gemini_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # @Desc   : Google Gemini LLM from https://ai.google.dev/tutorials/python_quickstart
+import json
 import os
-from typing import Optional, Union
+from dataclasses import asdict
+from typing import List, Optional, Union
 
 import google.generativeai as genai
 from google.ai import generativelanguage as glm
 from google.generativeai.generative_models import GenerativeModel
 from google.generativeai.types import content_types
 from google.generativeai.types.generation_types import (
     AsyncGenerateContentResponse,
+    BlockedPromptException,
     GenerateContentResponse,
     GenerationConfig,
 )
-from tenacity import (
-    after_log,
-    retry,
-    retry_if_exception_type,
-    stop_after_attempt,
-    wait_random_exponential,
-)
 
 from metagpt.configs.llm_config import LLMConfig, LLMType
+from metagpt.const import USE_CONFIG_TIMEOUT
 from metagpt.logs import log_llm_stream, logger
 from metagpt.provider.base_llm import BaseLLM
 from metagpt.provider.llm_provider_registry import register_provider
-from metagpt.provider.openai_api import log_and_reraise
+from metagpt.schema import Message
 
 
 class GeminiGenerativeModel(GenerativeModel):
     """
     Due to `https://github.com/google/generative-ai-python/pull/123`, inherit a new class.
     Will use default GenerativeModel if it fixed.
     """
@@ -51,14 +48,15 @@
 
     def __init__(self, config: LLMConfig):
         self.use_system_prompt = False  # google gemini has no system prompt when use api
 
         self.__init_gemini(config)
         self.config = config
         self.model = "gemini-pro"  # so far only one model
+        self.pricing_plan = self.config.pricing_plan or self.model
         self.llm = GeminiGenerativeModel(model_name=self.model)
 
     def __init_gemini(self, config: LLMConfig):
         if config.proxy:
             logger.info(f"Use proxy: {config.proxy}")
             os.environ["http_proxy"] = config.proxy
             os.environ["https_proxy"] = config.proxy
@@ -68,28 +66,47 @@
         # Not to change BaseLLM default functions but update with Gemini's conversation format.
         # You should follow the format.
         return {"role": "user", "parts": [msg]}
 
     def _assistant_msg(self, msg: str) -> dict[str, str]:
         return {"role": "model", "parts": [msg]}
 
+    def _system_msg(self, msg: str) -> dict[str, str]:
+        return {"role": "user", "parts": [msg]}
+
+    def format_msg(self, messages: Union[str, Message, list[dict], list[Message], list[str]]) -> list[dict]:
+        """convert messages to list[dict]."""
+        from metagpt.schema import Message
+
+        if not isinstance(messages, list):
+            messages = [messages]
+
+        # REF: https://ai.google.dev/tutorials/python_quickstart
+        # As a dictionary, the message requires `role` and `parts` keys.
+        # The role in a conversation can either be the `user`, which provides the prompts,
+        # or `model`, which provides the responses.
+        processed_messages = []
+        for msg in messages:
+            if isinstance(msg, str):
+                processed_messages.append({"role": "user", "parts": [msg]})
+            elif isinstance(msg, dict):
+                assert set(msg.keys()) == set(["role", "parts"])
+                processed_messages.append(msg)
+            elif isinstance(msg, Message):
+                processed_messages.append({"role": "user" if msg.role == "user" else "model", "parts": [msg.content]})
+            else:
+                raise ValueError(
+                    f"Only support message type are: str, Message, dict, but got {type(messages).__name__}!"
+                )
+        return processed_messages
+
     def _const_kwargs(self, messages: list[dict], stream: bool = False) -> dict:
         kwargs = {"contents": messages, "generation_config": GenerationConfig(temperature=0.3), "stream": stream}
         return kwargs
 
-    def _update_costs(self, usage: dict):
-        """update each request's token cost"""
-        if self.config.calc_usage:
-            try:
-                prompt_tokens = int(usage.get("prompt_tokens", 0))
-                completion_tokens = int(usage.get("completion_tokens", 0))
-                self.cost_manager.update_cost(prompt_tokens, completion_tokens, self.model)
-            except Exception as e:
-                logger.error(f"google gemini updats costs failed! exp: {e}")
-
     def get_choice_text(self, resp: GenerateContentResponse) -> str:
         return resp.text
 
     def get_usage(self, messages: list[dict], resp_text: str) -> dict:
         req_text = messages[-1]["parts"][0] if messages else ""
         prompt_resp = self.llm.count_tokens(contents={"role": "user", "parts": [{"text": req_text}]})
         completion_resp = self.llm.count_tokens(contents={"role": "model", "parts": [{"text": resp_text}]})
@@ -105,45 +122,44 @@
 
     def completion(self, messages: list[dict]) -> "GenerateContentResponse":
         resp: GenerateContentResponse = self.llm.generate_content(**self._const_kwargs(messages))
         usage = self.get_usage(messages, resp.text)
         self._update_costs(usage)
         return resp
 
-    async def _achat_completion(self, messages: list[dict]) -> "AsyncGenerateContentResponse":
+    async def _achat_completion(
+        self, messages: list[dict], timeout: int = USE_CONFIG_TIMEOUT
+    ) -> "AsyncGenerateContentResponse":
         resp: AsyncGenerateContentResponse = await self.llm.generate_content_async(**self._const_kwargs(messages))
         usage = await self.aget_usage(messages, resp.text)
         self._update_costs(usage)
         return resp
 
-    async def acompletion(self, messages: list[dict], timeout=3) -> dict:
-        return await self._achat_completion(messages)
+    async def acompletion(self, messages: list[dict], timeout=USE_CONFIG_TIMEOUT) -> dict:
+        return await self._achat_completion(messages, timeout=self.get_timeout(timeout))
 
-    async def _achat_completion_stream(self, messages: list[dict]) -> str:
+    async def _achat_completion_stream(self, messages: list[dict], timeout: int = USE_CONFIG_TIMEOUT) -> str:
         resp: AsyncGenerateContentResponse = await self.llm.generate_content_async(
             **self._const_kwargs(messages, stream=True)
         )
         collected_content = []
         async for chunk in resp:
-            content = chunk.text
+            try:
+                content = chunk.text
+            except Exception as e:
+                logger.warning(f"messages: {messages}\nerrors: {e}\n{BlockedPromptException(str(chunk))}")
+                raise BlockedPromptException(str(chunk))
             log_llm_stream(content)
             collected_content.append(content)
         log_llm_stream("\n")
 
         full_content = "".join(collected_content)
         usage = await self.aget_usage(messages, full_content)
         self._update_costs(usage)
         return full_content
 
-    @retry(
-        stop=stop_after_attempt(3),
-        wait=wait_random_exponential(min=1, max=60),
-        after=after_log(logger, logger.level("WARNING").name),
-        retry=retry_if_exception_type(ConnectionError),
-        retry_error_callback=log_and_reraise,
-    )
-    async def acompletion_text(self, messages: list[dict], stream=False, timeout: int = 3) -> str:
-        """response in async with stream or non-stream mode"""
-        if stream:
-            return await self._achat_completion_stream(messages)
-        resp = await self._achat_completion(messages)
-        return self.get_choice_text(resp)
+    def list_models(self) -> List:
+        models = []
+        for model in genai.list_models(page_size=100):
+            models.append(asdict(model))
+        logger.info(json.dumps(models))
+        return models
```

### Comparing `metagpt-0.7.7/metagpt/provider/llm_provider_registry.py` & `metagpt-0.8.0/metagpt/provider/llm_provider_registry.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,19 +17,23 @@
         self.providers[key] = provider_cls
 
     def get_provider(self, enum: LLMType):
         """get provider instance according to the enum"""
         return self.providers[enum]
 
 
-def register_provider(key):
+def register_provider(keys):
     """register provider to registry"""
 
     def decorator(cls):
-        LLM_REGISTRY.register(key, cls)
+        if isinstance(keys, list):
+            for key in keys:
+                LLM_REGISTRY.register(key, cls)
+        else:
+            LLM_REGISTRY.register(keys, cls)
         return cls
 
     return decorator
 
 
 def create_llm_instance(config: LLMConfig) -> BaseLLM:
     """get the default llm provider"""
```

### Comparing `metagpt-0.7.7/metagpt/provider/ollama_api.py` & `metagpt-0.8.0/metagpt/roles/researcher.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,126 +1,126 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# @Desc   : self-host open llm model with ollama which isn't openai-api-compatible
-
-import json
-
-from requests import ConnectionError
-from tenacity import (
-    after_log,
-    retry,
-    retry_if_exception_type,
-    stop_after_attempt,
-    wait_random_exponential,
-)
-
-from metagpt.configs.llm_config import LLMConfig, LLMType
-from metagpt.const import LLM_API_TIMEOUT
-from metagpt.logs import log_llm_stream, logger
-from metagpt.provider.base_llm import BaseLLM
-from metagpt.provider.general_api_requestor import GeneralAPIRequestor
-from metagpt.provider.llm_provider_registry import register_provider
-from metagpt.provider.openai_api import log_and_reraise
-from metagpt.utils.cost_manager import TokenCostManager
-
-
-@register_provider(LLMType.OLLAMA)
-class OllamaLLM(BaseLLM):
-    """
-    Refs to `https://github.com/jmorganca/ollama/blob/main/docs/api.md#generate-a-chat-completion`
-    """
-
-    def __init__(self, config: LLMConfig):
-        self.__init_ollama(config)
-        self.client = GeneralAPIRequestor(base_url=config.base_url)
-        self.config = config
-        self.suffix_url = "/chat"
-        self.http_method = "post"
-        self.use_system_prompt = False
-        self._cost_manager = TokenCostManager()
-
-    def __init_ollama(self, config: LLMConfig):
-        assert config.base_url, "ollama base url is required!"
-        self.model = config.model
-
-    def _const_kwargs(self, messages: list[dict], stream: bool = False) -> dict:
-        kwargs = {"model": self.model, "messages": messages, "options": {"temperature": 0.3}, "stream": stream}
-        return kwargs
-
-    def _update_costs(self, usage: dict):
-        """update each request's token cost"""
-        if self.config.calc_usage:
-            try:
-                prompt_tokens = int(usage.get("prompt_tokens", 0))
-                completion_tokens = int(usage.get("completion_tokens", 0))
-                self._cost_manager.update_cost(prompt_tokens, completion_tokens, self.model)
-            except Exception as e:
-                logger.error(f"ollama updats costs failed! exp: {e}")
-
-    def get_choice_text(self, resp: dict) -> str:
-        """get the resp content from llm response"""
-        assist_msg = resp.get("message", {})
-        assert assist_msg.get("role", None) == "assistant"
-        return assist_msg.get("content")
-
-    def get_usage(self, resp: dict) -> dict:
-        return {"prompt_tokens": resp.get("prompt_eval_count", 0), "completion_tokens": resp.get("eval_count", 0)}
-
-    def _decode_and_load(self, chunk: bytes, encoding: str = "utf-8") -> dict:
-        chunk = chunk.decode(encoding)
-        return json.loads(chunk)
-
-    async def _achat_completion(self, messages: list[dict]) -> dict:
-        resp, _, _ = await self.client.arequest(
-            method=self.http_method,
-            url=self.suffix_url,
-            params=self._const_kwargs(messages),
-            request_timeout=LLM_API_TIMEOUT,
-        )
-        resp = self._decode_and_load(resp)
-        usage = self.get_usage(resp)
-        self._update_costs(usage)
-        return resp
-
-    async def acompletion(self, messages: list[dict], timeout=3) -> dict:
-        return await self._achat_completion(messages)
-
-    async def _achat_completion_stream(self, messages: list[dict]) -> str:
-        stream_resp, _, _ = await self.client.arequest(
-            method=self.http_method,
-            url=self.suffix_url,
-            stream=True,
-            params=self._const_kwargs(messages, stream=True),
-            request_timeout=LLM_API_TIMEOUT,
+"""
+@Modified By: mashenquan, 2023/8/22. A definition has been provided for the return value of _think: returning false indicates that further reasoning cannot continue.
+@Modified By: mashenquan, 2023-11-1. According to Chapter 2.2.1 and 2.2.2 of RFC 116, change the data type of
+        the `cause_by` value in the `Message` to a string to support the new message distribution feature.
+"""
+
+import asyncio
+import re
+
+from pydantic import BaseModel
+
+from metagpt.actions import Action, CollectLinks, ConductResearch, WebBrowseAndSummarize
+from metagpt.actions.research import get_research_system_text
+from metagpt.const import RESEARCH_PATH
+from metagpt.logs import logger
+from metagpt.roles.role import Role, RoleReactMode
+from metagpt.schema import Message
+
+
+class Report(BaseModel):
+    topic: str
+    links: dict[str, list[str]] = None
+    summaries: list[tuple[str, str]] = None
+    content: str = ""
+
+
+class Researcher(Role):
+    name: str = "David"
+    profile: str = "Researcher"
+    goal: str = "Gather information and conduct research"
+    constraints: str = "Ensure accuracy and relevance of information"
+    language: str = "en-us"
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.set_actions(
+            [CollectLinks(name=self.name), WebBrowseAndSummarize(name=self.name), ConductResearch(name=self.name)]
         )
+        self._set_react_mode(react_mode=RoleReactMode.BY_ORDER.value)
+        if self.language not in ("en-us", "zh-cn"):
+            logger.warning(f"The language `{self.language}` has not been tested, it may not work.")
+
+    async def _think(self) -> bool:
+        if self.rc.todo is None:
+            self._set_state(0)
+            return True
+
+        if self.rc.state + 1 < len(self.states):
+            self._set_state(self.rc.state + 1)
+        else:
+            self.set_todo(None)
+            return False
+
+    async def _act(self) -> Message:
+        logger.info(f"{self._setting}: to do {self.rc.todo}({self.rc.todo.name})")
+        todo = self.rc.todo
+        msg = self.rc.memory.get(k=1)[0]
+        if isinstance(msg.instruct_content, Report):
+            instruct_content = msg.instruct_content
+            topic = instruct_content.topic
+        else:
+            topic = msg.content
+
+        research_system_text = self.research_system_text(topic, todo)
+        if isinstance(todo, CollectLinks):
+            links = await todo.run(topic, 4, 4)
+            ret = Message(
+                content="", instruct_content=Report(topic=topic, links=links), role=self.profile, cause_by=todo
+            )
+        elif isinstance(todo, WebBrowseAndSummarize):
+            links = instruct_content.links
+            todos = (todo.run(*url, query=query, system_text=research_system_text) for (query, url) in links.items())
+            summaries = await asyncio.gather(*todos)
+            summaries = list((url, summary) for i in summaries for (url, summary) in i.items() if summary)
+            ret = Message(
+                content="", instruct_content=Report(topic=topic, summaries=summaries), role=self.profile, cause_by=todo
+            )
+        else:
+            summaries = instruct_content.summaries
+            summary_text = "\n---\n".join(f"url: {url}\nsummary: {summary}" for (url, summary) in summaries)
+            content = await self.rc.todo.run(topic, summary_text, system_text=research_system_text)
+            ret = Message(
+                content="",
+                instruct_content=Report(topic=topic, content=content),
+                role=self.profile,
+                cause_by=self.rc.todo,
+            )
+        self.rc.memory.add(ret)
+        return ret
+
+    def research_system_text(self, topic, current_task: Action) -> str:
+        """BACKWARD compatible
+        This allows sub-class able to define its own system prompt based on topic.
+        return the previous implementation to have backward compatible
+        Args:
+            topic:
+            language:
+
+        Returns: str
+        """
+        return get_research_system_text(topic, self.language)
+
+    async def react(self) -> Message:
+        msg = await super().react()
+        report = msg.instruct_content
+        self.write_report(report.topic, report.content)
+        return msg
+
+    def write_report(self, topic: str, content: str):
+        filename = re.sub(r'[\\/:"*?<>|]+', " ", topic)
+        filename = filename.replace("\n", "")
+        if not RESEARCH_PATH.exists():
+            RESEARCH_PATH.mkdir(parents=True)
+        filepath = RESEARCH_PATH / f"{filename}.md"
+        filepath.write_text(content)
+
+
+if __name__ == "__main__":
+    import fire
+
+    async def main(topic: str, language="en-us"):
+        role = Researcher(language=language)
+        await role.run(topic)
 
-        collected_content = []
-        usage = {}
-        async for raw_chunk in stream_resp:
-            chunk = self._decode_and_load(raw_chunk)
-
-            if not chunk.get("done", False):
-                content = self.get_choice_text(chunk)
-                collected_content.append(content)
-                log_llm_stream(content)
-            else:
-                # stream finished
-                usage = self.get_usage(chunk)
-        log_llm_stream("\n")
-
-        self._update_costs(usage)
-        full_content = "".join(collected_content)
-        return full_content
-
-    @retry(
-        stop=stop_after_attempt(3),
-        wait=wait_random_exponential(min=1, max=60),
-        after=after_log(logger, logger.level("WARNING").name),
-        retry=retry_if_exception_type(ConnectionError),
-        retry_error_callback=log_and_reraise,
-    )
-    async def acompletion_text(self, messages: list[dict], stream=False, timeout: int = 3) -> str:
-        """response in async with stream or non-stream mode"""
-        if stream:
-            return await self._achat_completion_stream(messages)
-        resp = await self._achat_completion(messages)
-        return self.get_choice_text(resp)
+    fire.Fire(main)
```

### Comparing `metagpt-0.7.7/metagpt/provider/openai_api.py` & `metagpt-0.8.0/metagpt/provider/openai_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,74 +2,62 @@
 """
 @Time    : 2023/5/5 23:08
 @Author  : alexanderwu
 @File    : openai.py
 @Modified By: mashenquan, 2023/11/21. Fix bug: ReadTimeout.
 @Modified By: mashenquan, 2023/12/1. Fix bug: Unclosed connection caused by openai 0.x.
 """
+from __future__ import annotations
 
 import json
 import re
-from typing import AsyncIterator, Optional, Union
+from typing import Optional, Union
 
 from openai import APIConnectionError, AsyncOpenAI, AsyncStream
 from openai._base_client import AsyncHttpxClientWrapper
 from openai.types import CompletionUsage
 from openai.types.chat import ChatCompletion, ChatCompletionChunk
 from tenacity import (
     after_log,
     retry,
     retry_if_exception_type,
     stop_after_attempt,
     wait_random_exponential,
 )
 
 from metagpt.configs.llm_config import LLMConfig, LLMType
+from metagpt.const import USE_CONFIG_TIMEOUT
 from metagpt.logs import log_llm_stream, logger
 from metagpt.provider.base_llm import BaseLLM
 from metagpt.provider.constant import GENERAL_FUNCTION_SCHEMA
 from metagpt.provider.llm_provider_registry import register_provider
-from metagpt.schema import Message
-from metagpt.utils.common import CodeParser, decode_image
-from metagpt.utils.cost_manager import CostManager, Costs
+from metagpt.utils.common import CodeParser, decode_image, log_and_reraise
+from metagpt.utils.cost_manager import CostManager
 from metagpt.utils.exceptions import handle_exception
 from metagpt.utils.token_counter import (
     count_message_tokens,
     count_string_tokens,
     get_max_completion_tokens,
 )
 
 
-def log_and_reraise(retry_state):
-    logger.error(f"Retry attempts exhausted. Last exception: {retry_state.outcome.exception()}")
-    logger.warning(
-        """
-Recommend going to https://deepwisdom.feishu.cn/wiki/MsGnwQBjiif9c3koSJNcYaoSnu4#part-XdatdVlhEojeAfxaaEZcMV3ZniQ
-See FAQ 5.8
-"""
-    )
-    raise retry_state.outcome.exception()
-
-
-@register_provider(LLMType.OPENAI)
+@register_provider([LLMType.OPENAI, LLMType.FIREWORKS, LLMType.OPEN_LLM, LLMType.MOONSHOT, LLMType.MISTRAL, LLMType.YI])
 class OpenAILLM(BaseLLM):
     """Check https://platform.openai.com/examples for examples"""
 
     def __init__(self, config: LLMConfig):
         self.config = config
-        self._init_model()
         self._init_client()
         self.auto_max_tokens = False
         self.cost_manager: Optional[CostManager] = None
 
-    def _init_model(self):
-        self.model = self.config.model  # Used in _calc_usage & _cons_kwargs
-
     def _init_client(self):
         """https://github.com/openai/openai-python#async-usage"""
+        self.model = self.config.model  # Used in _calc_usage & _cons_kwargs
+        self.pricing_plan = self.config.pricing_plan or self.model
         kwargs = self._make_client_kwargs()
         self.aclient = AsyncOpenAI(**kwargs)
 
     def _make_client_kwargs(self) -> dict:
         kwargs = {"api_key": self.config.api_key, "base_url": self.config.base_url}
 
         # to use proxy, openai v1 needs http_client
@@ -83,125 +71,110 @@
         if self.config.proxy:
             params = {"proxies": self.config.proxy}
             if self.config.base_url:
                 params["base_url"] = self.config.base_url
 
         return params
 
-    async def _achat_completion_stream(self, messages: list[dict], timeout=3) -> AsyncIterator[str]:
+    async def _achat_completion_stream(self, messages: list[dict], timeout=USE_CONFIG_TIMEOUT) -> str:
         response: AsyncStream[ChatCompletionChunk] = await self.aclient.chat.completions.create(
-            **self._cons_kwargs(messages, timeout=timeout), stream=True
+            **self._cons_kwargs(messages, timeout=self.get_timeout(timeout)), stream=True
         )
-
+        usage = None
+        collected_messages = []
         async for chunk in response:
             chunk_message = chunk.choices[0].delta.content or "" if chunk.choices else ""  # extract the message
-            yield chunk_message
+            finish_reason = (
+                chunk.choices[0].finish_reason if chunk.choices and hasattr(chunk.choices[0], "finish_reason") else None
+            )
+            log_llm_stream(chunk_message)
+            collected_messages.append(chunk_message)
+            if finish_reason:
+                if hasattr(chunk, "usage"):
+                    # Some services have usage as an attribute of the chunk, such as Fireworks
+                    usage = CompletionUsage(**chunk.usage)
+                elif hasattr(chunk.choices[0], "usage"):
+                    # The usage of some services is an attribute of chunk.choices[0], such as Moonshot
+                    usage = CompletionUsage(**chunk.choices[0].usage)
+
+        log_llm_stream("\n")
+        full_reply_content = "".join(collected_messages)
+        if not usage:
+            # Some services do not provide the usage attribute, such as OpenAI or OpenLLM
+            usage = self._calc_usage(messages, full_reply_content)
 
-    def _cons_kwargs(self, messages: list[dict], timeout=3, **extra_kwargs) -> dict:
+        self._update_costs(usage)
+        return full_reply_content
+
+    def _cons_kwargs(self, messages: list[dict], timeout=USE_CONFIG_TIMEOUT, **extra_kwargs) -> dict:
         kwargs = {
             "messages": messages,
             "max_tokens": self._get_max_tokens(messages),
-            "n": 1,
+            # "n": 1,  # Some services do not provide this parameter, such as mistral
             # "stop": None,  # default it's None and gpt4-v can't have this one
-            "temperature": 0.3,
+            "temperature": self.config.temperature,
             "model": self.model,
-            "timeout": max(self.config.timeout, timeout),
+            "timeout": self.get_timeout(timeout),
         }
         if extra_kwargs:
             kwargs.update(extra_kwargs)
         return kwargs
 
-    async def _achat_completion(self, messages: list[dict], timeout=3) -> ChatCompletion:
-        kwargs = self._cons_kwargs(messages, timeout=timeout)
+    async def _achat_completion(self, messages: list[dict], timeout=USE_CONFIG_TIMEOUT) -> ChatCompletion:
+        kwargs = self._cons_kwargs(messages, timeout=self.get_timeout(timeout))
         rsp: ChatCompletion = await self.aclient.chat.completions.create(**kwargs)
         self._update_costs(rsp.usage)
         return rsp
 
-    async def acompletion(self, messages: list[dict], timeout=3) -> ChatCompletion:
-        return await self._achat_completion(messages, timeout=timeout)
+    async def acompletion(self, messages: list[dict], timeout=USE_CONFIG_TIMEOUT) -> ChatCompletion:
+        return await self._achat_completion(messages, timeout=self.get_timeout(timeout))
 
     @retry(
         wait=wait_random_exponential(min=1, max=60),
         stop=stop_after_attempt(6),
         after=after_log(logger, logger.level("WARNING").name),
         retry=retry_if_exception_type(APIConnectionError),
         retry_error_callback=log_and_reraise,
     )
-    async def acompletion_text(self, messages: list[dict], stream=False, timeout=3) -> str:
+    async def acompletion_text(self, messages: list[dict], stream=False, timeout=USE_CONFIG_TIMEOUT) -> str:
         """when streaming, print each token in place."""
         if stream:
-            resp = self._achat_completion_stream(messages, timeout=timeout)
-
-            collected_messages = []
-            async for i in resp:
-                log_llm_stream(i)
-                collected_messages.append(i)
-            log_llm_stream("\n")
+            return await self._achat_completion_stream(messages, timeout=timeout)
 
-            full_reply_content = "".join(collected_messages)
-            usage = self._calc_usage(messages, full_reply_content)
-            self._update_costs(usage)
-            return full_reply_content
-
-        rsp = await self._achat_completion(messages, timeout=timeout)
+        rsp = await self._achat_completion(messages, timeout=self.get_timeout(timeout))
         return self.get_choice_text(rsp)
 
-    def _func_configs(self, messages: list[dict], timeout=3, **kwargs) -> dict:
-        """Note: Keep kwargs consistent with https://platform.openai.com/docs/api-reference/chat/create"""
-        if "tools" not in kwargs:
-            configs = {"tools": [{"type": "function", "function": GENERAL_FUNCTION_SCHEMA}]}
-            kwargs.update(configs)
-
-        return self._cons_kwargs(messages=messages, timeout=timeout, **kwargs)
-
-    def _process_message(self, messages: Union[str, Message, list[dict], list[Message], list[str]]) -> list[dict]:
-        """convert messages to list[dict]."""
-        # 全部转成list
-        if not isinstance(messages, list):
-            messages = [messages]
-
-        # 转成list[dict]
-        processed_messages = []
-        for msg in messages:
-            if isinstance(msg, str):
-                processed_messages.append({"role": "user", "content": msg})
-            elif isinstance(msg, dict):
-                assert set(msg.keys()) == set(["role", "content"])
-                processed_messages.append(msg)
-            elif isinstance(msg, Message):
-                processed_messages.append(msg.to_dict())
-            else:
-                raise ValueError(
-                    f"Only support message type are: str, Message, dict, but got {type(messages).__name__}!"
-                )
-        return processed_messages
-
-    async def _achat_completion_function(self, messages: list[dict], timeout=3, **chat_configs) -> ChatCompletion:
-        messages = self._process_message(messages)
-        kwargs = self._func_configs(messages=messages, timeout=timeout, **chat_configs)
+    async def _achat_completion_function(
+        self, messages: list[dict], timeout: int = USE_CONFIG_TIMEOUT, **chat_configs
+    ) -> ChatCompletion:
+        messages = self.format_msg(messages)
+        kwargs = self._cons_kwargs(messages=messages, timeout=self.get_timeout(timeout), **chat_configs)
         rsp: ChatCompletion = await self.aclient.chat.completions.create(**kwargs)
         self._update_costs(rsp.usage)
         return rsp
 
-    async def aask_code(self, messages: list[dict], **kwargs) -> dict:
+    async def aask_code(self, messages: list[dict], timeout: int = USE_CONFIG_TIMEOUT, **kwargs) -> dict:
         """Use function of tools to ask a code.
         Note: Keep kwargs consistent with https://platform.openai.com/docs/api-reference/chat/create
 
         Examples:
         >>> llm = OpenAILLM()
         >>> msg = [{'role': 'user', 'content': "Write a python hello world code."}]
         >>> rsp = await llm.aask_code(msg)
         # -> {'language': 'python', 'code': "print('Hello, World!')"}
         """
+        if "tools" not in kwargs:
+            configs = {"tools": [{"type": "function", "function": GENERAL_FUNCTION_SCHEMA}]}
+            kwargs.update(configs)
         rsp = await self._achat_completion_function(messages, **kwargs)
         return self.get_choice_function_arguments(rsp)
 
     def _parse_arguments(self, arguments: str) -> dict:
         """parse arguments in openai function call"""
-        if "langugae" not in arguments and "code" not in arguments:
+        if "language" not in arguments and "code" not in arguments:
             logger.warning(f"Not found `code`, `language`, We assume it is pure code:\n {arguments}\n. ")
             return {"language": "python", "code": arguments}
 
         # 匹配language
         language_pattern = re.compile(r'[\"\']?language[\"\']?\s*:\s*["\']([^"\']+?)["\']', re.DOTALL)
         language_match = language_pattern.search(arguments)
         language_value = language_match.group(1) if language_match else "python"
@@ -261,31 +234,21 @@
 
     def _calc_usage(self, messages: list[dict], rsp: str) -> CompletionUsage:
         usage = CompletionUsage(prompt_tokens=0, completion_tokens=0, total_tokens=0)
         if not self.config.calc_usage:
             return usage
 
         try:
-            usage.prompt_tokens = count_message_tokens(messages, self.model)
-            usage.completion_tokens = count_string_tokens(rsp, self.model)
+            usage.prompt_tokens = count_message_tokens(messages, self.pricing_plan)
+            usage.completion_tokens = count_string_tokens(rsp, self.pricing_plan)
         except Exception as e:
             logger.warning(f"usage calculation failed: {e}")
 
         return usage
 
-    @handle_exception
-    def _update_costs(self, usage: CompletionUsage):
-        if self.config.calc_usage and usage and self.cost_manager:
-            self.cost_manager.update_cost(usage.prompt_tokens, usage.completion_tokens, self.model)
-
-    def get_costs(self) -> Costs:
-        if not self.cost_manager:
-            return Costs(0, 0, 0, 0)
-        return self.cost_manager.get_costs()
-
     def _get_max_tokens(self, messages: list[dict]):
         if not self.auto_max_tokens:
             return self.config.max_token
         # FIXME
         # https://community.openai.com/t/why-is-gpt-3-5-turbo-1106-max-tokens-limited-to-4096/494973/3
         return min(get_max_completion_tokens(messages, self.model, self.config.max_token), 4096)
```

### Comparing `metagpt-0.7.7/metagpt/provider/postprocess/base_postprocess_plugin.py` & `metagpt-0.8.0/metagpt/provider/postprocess/base_postprocess_plugin.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/provider/postprocess/llm_output_postprocess.py` & `metagpt-0.8.0/metagpt/provider/postprocess/llm_output_postprocess.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/provider/spark_api.py` & `metagpt-0.8.0/metagpt/provider/spark_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,35 +13,42 @@
 from time import mktime
 from urllib.parse import urlencode, urlparse
 from wsgiref.handlers import format_date_time
 
 import websocket  # 使用websocket_client
 
 from metagpt.configs.llm_config import LLMConfig, LLMType
+from metagpt.const import USE_CONFIG_TIMEOUT
 from metagpt.logs import logger
 from metagpt.provider.base_llm import BaseLLM
 from metagpt.provider.llm_provider_registry import register_provider
 
 
 @register_provider(LLMType.SPARK)
 class SparkLLM(BaseLLM):
     def __init__(self, config: LLMConfig):
         self.config = config
         logger.warning("SparkLLM：当前方法无法支持异步运行。当你使用acompletion时，并不能并行访问。")
 
     def get_choice_text(self, rsp: dict) -> str:
         return rsp["payload"]["choices"]["text"][-1]["content"]
 
-    async def acompletion_text(self, messages: list[dict], stream=False, timeout: int = 3) -> str:
+    async def _achat_completion_stream(self, messages: list[dict], timeout: int = USE_CONFIG_TIMEOUT) -> str:
+        pass
+
+    async def acompletion_text(self, messages: list[dict], stream=False, timeout: int = USE_CONFIG_TIMEOUT) -> str:
         # 不支持
         # logger.warning("当前方法无法支持异步运行。当你使用acompletion时，并不能并行访问。")
         w = GetMessageFromWeb(messages, self.config)
         return w.run()
 
-    async def acompletion(self, messages: list[dict], timeout=3):
+    async def _achat_completion(self, messages: list[dict], timeout=USE_CONFIG_TIMEOUT):
+        pass
+
+    async def acompletion(self, messages: list[dict], timeout=USE_CONFIG_TIMEOUT):
         # 不支持异步
         w = GetMessageFromWeb(messages, self.config)
         return w.run()
 
 
 class GetMessageFromWeb:
     class WsParam:
```

### Comparing `metagpt-0.7.7/metagpt/provider/zhipuai/async_sse_client.py` & `metagpt-0.8.0/metagpt/provider/zhipuai/async_sse_client.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/provider/zhipuai/zhipu_model_api.py` & `metagpt-0.8.0/metagpt/provider/zhipuai/zhipu_model_api.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/provider/zhipuai_api.py` & `metagpt-0.8.0/metagpt/provider/ollama_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,112 +1,93 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# @Desc   : zhipuai LLM from https://open.bigmodel.cn/dev/api#sdk
+# @Desc   : self-host open llm model with ollama which isn't openai-api-compatible
 
-from enum import Enum
-from typing import Optional
-
-from requests import ConnectionError
-from tenacity import (
-    after_log,
-    retry,
-    retry_if_exception_type,
-    stop_after_attempt,
-    wait_random_exponential,
-)
-from zhipuai.types.chat.chat_completion import Completion
+import json
 
 from metagpt.configs.llm_config import LLMConfig, LLMType
-from metagpt.logs import log_llm_stream, logger
+from metagpt.const import USE_CONFIG_TIMEOUT
+from metagpt.logs import log_llm_stream
 from metagpt.provider.base_llm import BaseLLM
+from metagpt.provider.general_api_requestor import GeneralAPIRequestor
 from metagpt.provider.llm_provider_registry import register_provider
-from metagpt.provider.openai_api import log_and_reraise
-from metagpt.provider.zhipuai.zhipu_model_api import ZhiPuModelAPI
-from metagpt.utils.cost_manager import CostManager
-
-
-class ZhiPuEvent(Enum):
-    ADD = "add"
-    ERROR = "error"
-    INTERRUPTED = "interrupted"
-    FINISH = "finish"
+from metagpt.utils.cost_manager import TokenCostManager
 
 
-@register_provider(LLMType.ZHIPUAI)
-class ZhiPuAILLM(BaseLLM):
+@register_provider(LLMType.OLLAMA)
+class OllamaLLM(BaseLLM):
     """
-    Refs to `https://open.bigmodel.cn/dev/api#chatglm_turbo`
-    From now, support glm-3-turbo、glm-4, and also system_prompt.
+    Refs to `https://github.com/jmorganca/ollama/blob/main/docs/api.md#generate-a-chat-completion`
     """
 
     def __init__(self, config: LLMConfig):
+        self.__init_ollama(config)
+        self.client = GeneralAPIRequestor(base_url=config.base_url)
         self.config = config
-        self.__init_zhipuai()
-        self.cost_manager: Optional[CostManager] = None
-
-    def __init_zhipuai(self):
-        assert self.config.api_key
-        self.api_key = self.config.api_key
-        self.model = self.config.model  # so far, it support glm-3-turbo、glm-4
-        self.llm = ZhiPuModelAPI(api_key=self.api_key)
+        self.suffix_url = "/chat"
+        self.http_method = "post"
+        self.use_system_prompt = False
+        self.cost_manager = TokenCostManager()
+
+    def __init_ollama(self, config: LLMConfig):
+        assert config.base_url, "ollama base url is required!"
+        self.model = config.model
+        self.pricing_plan = self.model
 
     def _const_kwargs(self, messages: list[dict], stream: bool = False) -> dict:
-        kwargs = {"model": self.model, "messages": messages, "stream": stream, "temperature": 0.3}
+        kwargs = {"model": self.model, "messages": messages, "options": {"temperature": 0.3}, "stream": stream}
         return kwargs
 
-    def _update_costs(self, usage: dict):
-        """update each request's token cost"""
-        if self.config.calc_usage:
-            try:
-                prompt_tokens = int(usage.get("prompt_tokens", 0))
-                completion_tokens = int(usage.get("completion_tokens", 0))
-                self.cost_manager.update_cost(prompt_tokens, completion_tokens, self.model)
-            except Exception as e:
-                logger.error(f"zhipuai updats costs failed! exp: {e}")
-
-    def completion(self, messages: list[dict], timeout=3) -> dict:
-        resp: Completion = self.llm.chat.completions.create(**self._const_kwargs(messages))
-        usage = resp.usage.model_dump()
-        self._update_costs(usage)
-        return resp.model_dump()
-
-    async def _achat_completion(self, messages: list[dict], timeout=3) -> dict:
-        resp = await self.llm.acreate(**self._const_kwargs(messages))
-        usage = resp.get("usage", {})
+    def get_choice_text(self, resp: dict) -> str:
+        """get the resp content from llm response"""
+        assist_msg = resp.get("message", {})
+        assert assist_msg.get("role", None) == "assistant"
+        return assist_msg.get("content")
+
+    def get_usage(self, resp: dict) -> dict:
+        return {"prompt_tokens": resp.get("prompt_eval_count", 0), "completion_tokens": resp.get("eval_count", 0)}
+
+    def _decode_and_load(self, chunk: bytes, encoding: str = "utf-8") -> dict:
+        chunk = chunk.decode(encoding)
+        return json.loads(chunk)
+
+    async def _achat_completion(self, messages: list[dict], timeout: int = USE_CONFIG_TIMEOUT) -> dict:
+        resp, _, _ = await self.client.arequest(
+            method=self.http_method,
+            url=self.suffix_url,
+            params=self._const_kwargs(messages),
+            request_timeout=self.get_timeout(timeout),
+        )
+        resp = self._decode_and_load(resp)
+        usage = self.get_usage(resp)
         self._update_costs(usage)
         return resp
 
-    async def acompletion(self, messages: list[dict], timeout=3) -> dict:
-        return await self._achat_completion(messages, timeout=timeout)
+    async def acompletion(self, messages: list[dict], timeout=USE_CONFIG_TIMEOUT) -> dict:
+        return await self._achat_completion(messages, timeout=self.get_timeout(timeout))
+
+    async def _achat_completion_stream(self, messages: list[dict], timeout: int = USE_CONFIG_TIMEOUT) -> str:
+        stream_resp, _, _ = await self.client.arequest(
+            method=self.http_method,
+            url=self.suffix_url,
+            stream=True,
+            params=self._const_kwargs(messages, stream=True),
+            request_timeout=self.get_timeout(timeout),
+        )
 
-    async def _achat_completion_stream(self, messages: list[dict], timeout=3) -> str:
-        response = await self.llm.acreate_stream(**self._const_kwargs(messages, stream=True))
         collected_content = []
         usage = {}
-        async for chunk in response.stream():
-            finish_reason = chunk.get("choices")[0].get("finish_reason")
-            if finish_reason == "stop":
-                usage = chunk.get("usage", {})
-            else:
-                content = self.get_choice_delta_text(chunk)
+        async for raw_chunk in stream_resp:
+            chunk = self._decode_and_load(raw_chunk)
+
+            if not chunk.get("done", False):
+                content = self.get_choice_text(chunk)
                 collected_content.append(content)
                 log_llm_stream(content)
-
+            else:
+                # stream finished
+                usage = self.get_usage(chunk)
         log_llm_stream("\n")
 
         self._update_costs(usage)
         full_content = "".join(collected_content)
         return full_content
-
-    @retry(
-        stop=stop_after_attempt(3),
-        wait=wait_random_exponential(min=1, max=60),
-        after=after_log(logger, logger.level("WARNING").name),
-        retry=retry_if_exception_type(ConnectionError),
-        retry_error_callback=log_and_reraise,
-    )
-    async def acompletion_text(self, messages: list[dict], stream=False, timeout=3) -> str:
-        """response in async with stream or non-stream mode"""
-        if stream:
-            return await self._achat_completion_stream(messages)
-        resp = await self._achat_completion(messages)
-        return self.get_choice_text(resp)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `metagpt-0.7.7/metagpt/roles/architect.py` & `metagpt-0.8.0/metagpt/roles/architect.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/roles/assistant.py` & `metagpt-0.8.0/metagpt/roles/assistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
         prompt = ""
         skills = self.skills.get_skill_list(context=self.context)
         for desc, name in skills.items():
             prompt += f"If the text explicitly want you to {desc}, return `[SKILL]: {name}` brief and clear. For instance: [SKILL]: {name}\n"
         prompt += 'Otherwise, return `[TALK]: {talk}` brief and clear. For instance: if {talk} is "xxxx" return [TALK]: xxxx\n\n'
         prompt += f"Now what specific action is explicitly mentioned in the text: {last_talk}\n"
-        rsp = await self.llm.aask(prompt, ["You are an action classifier"])
+        rsp = await self.llm.aask(prompt, ["You are an action classifier"], stream=False)
         logger.info(f"THINK: {prompt}\n, THINK RESULT: {rsp}\n")
         return await self._plan(rsp, last_talk=last_talk)
 
     async def act(self) -> Message:
         result = await self.rc.todo.run()
         if not result:
             return None
```

### Comparing `metagpt-0.7.7/metagpt/roles/customer_service.py` & `metagpt-0.8.0/metagpt/roles/customer_service.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/roles/engineer.py` & `metagpt-0.8.0/metagpt/roles/engineer.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,25 @@
 @Modified By: mashenquan, 2023-12-5. Enhance the workflow to navigate to WriteCode or QaEngineer based on the results
     of SummarizeCode.
 """
 
 from __future__ import annotations
 
 import json
-import os
 from collections import defaultdict
 from pathlib import Path
 from typing import Set
 
 from metagpt.actions import Action, WriteCode, WriteCodeReview, WriteTasks
 from metagpt.actions.fix_bug import FixBug
 from metagpt.actions.project_management_an import REFINED_TASK_LIST, TASK_LIST
 from metagpt.actions.summarize_code import SummarizeCode
 from metagpt.actions.write_code_plan_and_change_an import WriteCodePlanAndChange
 from metagpt.const import (
     CODE_PLAN_AND_CHANGE_FILE_REPO,
-    CODE_PLAN_AND_CHANGE_FILENAME,
     REQUIREMENT_FILENAME,
     SYSTEM_DESIGN_FILE_REPO,
     TASK_FILE_REPO,
 )
 from metagpt.logs import logger
 from metagpt.roles import Role
 from metagpt.schema import (
@@ -115,18 +113,18 @@
             if review:
                 action = WriteCodeReview(i_context=coding_context, context=self.context, llm=self.llm)
                 self._init_action(action)
                 coding_context = await action.run()
 
             dependencies = {coding_context.design_doc.root_relative_path, coding_context.task_doc.root_relative_path}
             if self.config.inc:
-                dependencies.add(os.path.join(CODE_PLAN_AND_CHANGE_FILE_REPO, CODE_PLAN_AND_CHANGE_FILENAME))
+                dependencies.add(coding_context.code_plan_and_change_doc.root_relative_path)
             await self.project_repo.srcs.save(
                 filename=coding_context.filename,
-                dependencies=dependencies,
+                dependencies=list(dependencies),
                 content=coding_context.code_doc.content,
             )
             msg = Message(
                 content=coding_context.model_dump_json(),
                 instruct_content=coding_context,
                 role=self.profile,
                 cause_by=WriteCode,
@@ -202,28 +200,28 @@
         self.n_summarize += 1 if self.config.max_auto_summarize_code > self.n_summarize else 0
         return Message(
             content=json.dumps(tasks), role=self.profile, cause_by=SummarizeCode, send_to=self, sent_from=self
         )
 
     async def _act_code_plan_and_change(self):
         """Write code plan and change that guides subsequent WriteCode and WriteCodeReview"""
-        logger.info("Writing code plan and change..")
         node = await self.rc.todo.run()
         code_plan_and_change = node.instruct_content.model_dump_json()
         dependencies = {
             REQUIREMENT_FILENAME,
             self.rc.todo.i_context.prd_filename,
             self.rc.todo.i_context.design_filename,
             self.rc.todo.i_context.task_filename,
         }
+        code_plan_and_change_filepath = Path(self.rc.todo.i_context.design_filename)
         await self.project_repo.docs.code_plan_and_change.save(
-            filename=self.rc.todo.i_context.filename, content=code_plan_and_change, dependencies=dependencies
+            filename=code_plan_and_change_filepath.name, content=code_plan_and_change, dependencies=dependencies
         )
         await self.project_repo.resources.code_plan_and_change.save(
-            filename=Path(self.rc.todo.i_context.filename).with_suffix(".md").name,
+            filename=code_plan_and_change_filepath.with_suffix(".md").name,
             content=node.content,
             dependencies=dependencies,
         )
 
         return Message(
             content=code_plan_and_change,
             role=self.profile,
@@ -238,16 +236,16 @@
         if "YES" in rsp:
             return True, rsp
         return False, rsp
 
     async def _think(self) -> Action | None:
         if not self.src_workspace:
             self.src_workspace = self.git_repo.workdir / self.git_repo.workdir.name
-        write_plan_and_change_filters = any_to_str_set([WriteTasks])
-        write_code_filters = any_to_str_set([WriteTasks, WriteCodePlanAndChange, SummarizeCode, FixBug])
+        write_plan_and_change_filters = any_to_str_set([WriteTasks, FixBug])
+        write_code_filters = any_to_str_set([WriteTasks, WriteCodePlanAndChange, SummarizeCode])
         summarize_code_filters = any_to_str_set([WriteCode, WriteCodeReview])
         if not self.rc.news:
             return None
         msg = self.rc.news[0]
         if self.config.inc and msg.cause_by in write_plan_and_change_filters:
             logger.debug(f"TODO WriteCodePlanAndChange:{msg.model_dump_json()}")
             await self._new_code_plan_and_change_action()
@@ -265,23 +263,32 @@
     async def _new_coding_context(self, filename, dependency) -> CodingContext:
         old_code_doc = await self.project_repo.srcs.get(filename)
         if not old_code_doc:
             old_code_doc = Document(root_path=str(self.project_repo.src_relative_path), filename=filename, content="")
         dependencies = {Path(i) for i in await dependency.get(old_code_doc.root_relative_path)}
         task_doc = None
         design_doc = None
+        code_plan_and_change_doc = None
         for i in dependencies:
             if str(i.parent) == TASK_FILE_REPO:
                 task_doc = await self.project_repo.docs.task.get(i.name)
             elif str(i.parent) == SYSTEM_DESIGN_FILE_REPO:
                 design_doc = await self.project_repo.docs.system_design.get(i.name)
+            elif str(i.parent) == CODE_PLAN_AND_CHANGE_FILE_REPO:
+                code_plan_and_change_doc = await self.project_repo.docs.code_plan_and_change.get(i.name)
         if not task_doc or not design_doc:
             logger.error(f'Detected source code "{filename}" from an unknown origin.')
             raise ValueError(f'Detected source code "{filename}" from an unknown origin.')
-        context = CodingContext(filename=filename, design_doc=design_doc, task_doc=task_doc, code_doc=old_code_doc)
+        context = CodingContext(
+            filename=filename,
+            design_doc=design_doc,
+            task_doc=task_doc,
+            code_doc=old_code_doc,
+            code_plan_and_change_doc=code_plan_and_change_doc,
+        )
         return context
 
     async def _new_coding_doc(self, filename, dependency):
         context = await self._new_coding_context(filename, dependency)
         coding_doc = Document(
             root_path=str(self.project_repo.src_relative_path), filename=filename, content=context.model_dump_json()
         )
@@ -292,24 +299,34 @@
         changed_src_files = self.project_repo.srcs.all_files if bug_fix else self.project_repo.srcs.changed_files
         changed_task_files = self.project_repo.docs.task.changed_files
         changed_files = Documents()
         # Recode caused by upstream changes.
         for filename in changed_task_files:
             design_doc = await self.project_repo.docs.system_design.get(filename)
             task_doc = await self.project_repo.docs.task.get(filename)
+            code_plan_and_change_doc = await self.project_repo.docs.code_plan_and_change.get(filename)
             task_list = self._parse_tasks(task_doc)
             for task_filename in task_list:
                 old_code_doc = await self.project_repo.srcs.get(task_filename)
                 if not old_code_doc:
                     old_code_doc = Document(
                         root_path=str(self.project_repo.src_relative_path), filename=task_filename, content=""
                     )
-                context = CodingContext(
-                    filename=task_filename, design_doc=design_doc, task_doc=task_doc, code_doc=old_code_doc
-                )
+                if not code_plan_and_change_doc:
+                    context = CodingContext(
+                        filename=task_filename, design_doc=design_doc, task_doc=task_doc, code_doc=old_code_doc
+                    )
+                else:
+                    context = CodingContext(
+                        filename=task_filename,
+                        design_doc=design_doc,
+                        task_doc=task_doc,
+                        code_doc=old_code_doc,
+                        code_plan_and_change_doc=code_plan_and_change_doc,
+                    )
                 coding_doc = Document(
                     root_path=str(self.project_repo.src_relative_path),
                     filename=task_filename,
                     content=context.model_dump_json(),
                 )
                 if task_filename in changed_files.docs:
                     logger.warning(
@@ -338,17 +355,25 @@
         summarizations = defaultdict(list)
         for filename in src_files:
             dependencies = await self.project_repo.srcs.get_dependency(filename=filename)
             ctx = CodeSummarizeContext.loads(filenames=list(dependencies))
             summarizations[ctx].append(filename)
         for ctx, filenames in summarizations.items():
             ctx.codes_filenames = filenames
-            self.summarize_todos.append(SummarizeCode(i_context=ctx, context=self.context, llm=self.llm))
+            new_summarize = SummarizeCode(i_context=ctx, context=self.context, llm=self.llm)
+            for i, act in enumerate(self.summarize_todos):
+                if act.i_context.task_filename == new_summarize.i_context.task_filename:
+                    self.summarize_todos[i] = new_summarize
+                    new_summarize = None
+                    break
+            if new_summarize:
+                self.summarize_todos.append(new_summarize)
         if self.summarize_todos:
             self.set_todo(self.summarize_todos[0])
+            self.summarize_todos.pop(0)
 
     async def _new_code_plan_and_change_action(self):
         """Create a WriteCodePlanAndChange action for subsequent to-do actions."""
         files = self.project_repo.all_files
         requirement_doc = await self.project_repo.docs.get(REQUIREMENT_FILENAME)
         requirement = requirement_doc.content if requirement_doc else ""
         code_plan_and_change_ctx = CodePlanAndChangeContext.loads(files, requirement=requirement)
```

### Comparing `metagpt-0.7.7/metagpt/roles/invoice_ocr_assistant.py` & `metagpt-0.8.0/metagpt/roles/invoice_ocr_assistant.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/roles/product_manager.py` & `metagpt-0.8.0/metagpt/roles/product_manager.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/roles/project_manager.py` & `metagpt-0.8.0/metagpt/roles/project_manager.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/roles/prompt.py` & `metagpt-0.8.0/metagpt/roles/prompt.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/roles/qa_engineer.py` & `metagpt-0.8.0/metagpt/roles/qa_engineer.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/roles/role.py` & `metagpt-0.8.0/metagpt/roles/role.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,20 +104,14 @@
     watch: set[str] = Field(default_factory=set)
     news: list[Type[Message]] = Field(default=[], exclude=True)  # TODO not used
     react_mode: RoleReactMode = (
         RoleReactMode.REACT
     )  # see `Role._set_react_mode` for definitions of the following two attributes
     max_react_loop: int = 1
 
-    def check(self, role_id: str):
-        # if hasattr(CONFIG, "enable_longterm_memory") and CONFIG.enable_longterm_memory:
-        #     self.long_term_memory.recover_memory(role_id, self)
-        #     self.memory = self.long_term_memory  # use memory to act as long_term_memory for unify operation
-        pass
-
     @property
     def important_memory(self) -> list[Message]:
         """Retrieve information corresponding to the attention action."""
         return self.memory.get_by_actions(self.watch)
 
     @property
     def history(self) -> list[Message]:
@@ -171,14 +165,15 @@
         kwargs = self.model_extra or {}
 
         if self.is_human:
             self.llm = HumanProvider(None)
 
         self._check_actions()
         self.llm.system_prompt = self._get_prefix()
+        self.llm.cost_manager = self.context.cost_manager
         self._watch(kwargs.pop("watch", [UserRequirement]))
 
         if self.latest_observed_msg:
             self.recovered = True
 
     @property
     def todo(self) -> Action:
@@ -277,17 +272,17 @@
                         f"is_human attribute does not take effect, "
                         f"as Role's {str(action)} was initialized using LLM, "
                         f"try passing in Action classes instead of initialized instances"
                     )
                 i = action
             self._init_action(i)
             self.actions.append(i)
-            self.states.append(f"{len(self.actions)}. {action}")
+            self.states.append(f"{len(self.actions) - 1}. {action}")
 
-    def _set_react_mode(self, react_mode: str, max_react_loop: int = 1, auto_run: bool = True, use_tools: bool = False):
+    def _set_react_mode(self, react_mode: str, max_react_loop: int = 1, auto_run: bool = True):
         """Set strategy of the Role reacting to observed Message. Variation lies in how
         this Role elects action to perform during the _think stage, especially if it is capable of multiple Actions.
 
         Args:
             react_mode (str): Mode for choosing action during the _think stage, can be one of:
                         "react": standard think-act loop in the ReAct paper, alternating thinking and acting to solve the task, i.e. _think -> _act -> _think -> _act -> ...
                                  Use llm to select actions in _think dynamically;
@@ -300,25 +295,21 @@
                                   Defaults to 1, i.e. _think -> _act (-> return result and end)
         """
         assert react_mode in RoleReactMode.values(), f"react_mode must be one of {RoleReactMode.values()}"
         self.rc.react_mode = react_mode
         if react_mode == RoleReactMode.REACT:
             self.rc.max_react_loop = max_react_loop
         elif react_mode == RoleReactMode.PLAN_AND_ACT:
-            self.planner = Planner(
-                goal=self.goal, working_memory=self.rc.working_memory, auto_run=auto_run, use_tools=use_tools
-            )
+            self.planner = Planner(goal=self.goal, working_memory=self.rc.working_memory, auto_run=auto_run)
 
     def _watch(self, actions: Iterable[Type[Action]] | Iterable[Action]):
         """Watch Actions of interest. Role will select Messages caused by these Actions from its personal message
         buffer during _observe.
         """
         self.rc.watch = {any_to_str(t) for t in actions}
-        # check RoleContext after adding watch actions
-        self.rc.check(self.role_id)
 
     def is_watch(self, caused_by: str):
         return caused_by in self.rc.watch
 
     def set_addresses(self, addresses: Set[str]):
         """Used to receive Messages with certain tags from the environment. Message will be put into personal message
         buffer to be further processed in _observe. By default, a Role subscribes Messages with a tag of its own name
@@ -337,14 +328,15 @@
     def set_env(self, env: "Environment"):
         """Set the environment in which the role works. The role can talk to the environment and can also receive
         messages by observing."""
         self.rc.env = env
         if env:
             env.set_addresses(self, self.addresses)
             self.llm.system_prompt = self._get_prefix()
+            self.llm.cost_manager = self.context.cost_manager
             self.set_actions(self.actions)  # reset actions to update llm and prefix
 
     def _get_prefix(self):
         """Get the role prefix"""
         if self.desc:
             return self.desc
```

### Comparing `metagpt-0.7.7/metagpt/roles/sales.py` & `metagpt-0.8.0/metagpt/roles/sales.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 """
 
 from typing import Optional
 
 from pydantic import Field, model_validator
 
 from metagpt.actions import SearchAndSummarize, UserRequirement
-from metagpt.document_store.base_store import BaseStore
 from metagpt.roles import Role
 from metagpt.tools.search_engine import SearchEngine
 
 
 class Sales(Role):
     name: str = "John Smith"
     profile: str = "Retail Sales Guide"
@@ -23,15 +22,15 @@
         "As a Retail Sales Guide, my name is John Smith. I specialize in addressing customer inquiries with "
         "expertise and precision. My responses are based solely on the information available in our knowledge"
         " base. In instances where your query extends beyond this scope, I'll honestly indicate my inability "
         "to provide an answer, rather than speculate or assume. Please note, each of my replies will be "
         "delivered with the professionalism and courtesy expected of a seasoned sales guide."
     )
 
-    store: Optional[BaseStore] = Field(default=None, exclude=True)
+    store: Optional[object] = Field(default=None, exclude=True)  # must inplement tools.SearchInterface
 
     @model_validator(mode="after")
     def validate_stroe(self):
         if self.store:
             search_engine = SearchEngine.from_search_func(search_func=self.store.asearch, proxy=self.config.proxy)
             action = SearchAndSummarize(search_engine=search_engine, context=self.context)
         else:
```

### Comparing `metagpt-0.7.7/metagpt/roles/searcher.py` & `metagpt-0.8.0/metagpt/roles/searcher.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/roles/sk_agent.py` & `metagpt-0.8.0/metagpt/roles/sk_agent.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/roles/teacher.py` & `metagpt-0.8.0/metagpt/roles/teacher.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/roles/tutorial_assistant.py` & `metagpt-0.8.0/metagpt/roles/tutorial_assistant.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/schema.py` & `metagpt-0.8.0/metagpt/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,24 +33,24 @@
     field_serializer,
     field_validator,
     model_serializer,
     model_validator,
 )
 
 from metagpt.const import (
-    CODE_PLAN_AND_CHANGE_FILENAME,
     MESSAGE_ROUTE_CAUSE_BY,
     MESSAGE_ROUTE_FROM,
     MESSAGE_ROUTE_TO,
     MESSAGE_ROUTE_TO_ALL,
     PRDS_FILE_REPO,
     SYSTEM_DESIGN_FILE_REPO,
     TASK_FILE_REPO,
 )
 from metagpt.logs import logger
+from metagpt.repo_parser import DotClassInfo
 from metagpt.utils.common import any_to_str, any_to_str_set, import_class
 from metagpt.utils.exceptions import handle_exception
 from metagpt.utils.serialize import (
     actionoutout_schema_to_mapping,
     actionoutput_mapping_to_str,
     actionoutput_str_to_mapping,
 )
@@ -229,14 +229,18 @@
         return any_to_str(sent_from if sent_from else "")
 
     @field_validator("send_to", mode="before")
     @classmethod
     def check_send_to(cls, send_to: Any) -> set:
         return any_to_str_set(send_to if send_to else {MESSAGE_ROUTE_TO_ALL})
 
+    @field_serializer("send_to", mode="plain")
+    def ser_send_to(self, send_to: set) -> list:
+        return list(send_to)
+
     @field_serializer("instruct_content", mode="plain")
     def ser_instruct_content(self, ic: BaseModel) -> Union[dict, None]:
         ic_dict = None
         if ic:
             # compatible with custom-defined ActionOutput
             schema = ic.model_json_schema()
             ic_type = str(type(ic))
@@ -272,14 +276,18 @@
         if self.instruct_content:
             return f"{self.role}: {self.instruct_content.model_dump()}"
         return f"{self.role}: {self.content}"
 
     def __repr__(self):
         return self.__str__()
 
+    def rag_key(self) -> str:
+        """For search"""
+        return self.content
+
     def to_dict(self) -> dict:
         """Return a dict containing `role` and `content` for the LLM call.l"""
         return {"role": self.role, "content": self.content}
 
     def dump(self) -> str:
         """Convert the object to json string"""
         return self.model_dump_json(exclude_none=True, warnings=False)
@@ -609,14 +617,15 @@
 
 
 class CodingContext(BaseContext):
     filename: str
     design_doc: Optional[Document] = None
     task_doc: Optional[Document] = None
     code_doc: Optional[Document] = None
+    code_plan_and_change_doc: Optional[Document] = None
 
 
 class TestingContext(BaseContext):
     filename: str
     code_doc: Document
     test_doc: Optional[Document] = None
 
@@ -663,15 +672,14 @@
 
 
 class BugFixContext(BaseContext):
     filename: str = ""
 
 
 class CodePlanAndChangeContext(BaseModel):
-    filename: str = CODE_PLAN_AND_CHANGE_FILENAME
     requirement: str = ""
     prd_filename: str = ""
     design_filename: str = ""
     task_filename: str = ""
 
     @staticmethod
     def loads(filenames: List, **kwargs) -> CodePlanAndChangeContext:
@@ -687,64 +695,92 @@
             if filename.is_relative_to(TASK_FILE_REPO):
                 ctx.task_filename = filename.name
                 continue
         return ctx
 
 
 # mermaid class view
-class ClassMeta(BaseModel):
+class UMLClassMeta(BaseModel):
     name: str = ""
-    abstraction: bool = False
-    static: bool = False
     visibility: str = ""
 
+    @staticmethod
+    def name_to_visibility(name: str) -> str:
+        if name == "__init__":
+            return "+"
+        if name.startswith("__"):
+            return "-"
+        elif name.startswith("_"):
+            return "#"
+        return "+"
 
-class ClassAttribute(ClassMeta):
+
+class UMLClassAttribute(UMLClassMeta):
     value_type: str = ""
     default_value: str = ""
 
     def get_mermaid(self, align=1) -> str:
         content = "".join(["\t" for i in range(align)]) + self.visibility
         if self.value_type:
-            content += self.value_type + " "
-        content += self.name
+            content += self.value_type.replace(" ", "") + " "
+        name = self.name.split(":", 1)[1] if ":" in self.name else self.name
+        content += name
         if self.default_value:
             content += "="
             if self.value_type not in ["str", "string", "String"]:
                 content += self.default_value
             else:
                 content += '"' + self.default_value.replace('"', "") + '"'
-        if self.abstraction:
-            content += "*"
-        if self.static:
-            content += "$"
+        # if self.abstraction:
+        #     content += "*"
+        # if self.static:
+        #     content += "$"
         return content
 
 
-class ClassMethod(ClassMeta):
-    args: List[ClassAttribute] = Field(default_factory=list)
+class UMLClassMethod(UMLClassMeta):
+    args: List[UMLClassAttribute] = Field(default_factory=list)
     return_type: str = ""
 
     def get_mermaid(self, align=1) -> str:
         content = "".join(["\t" for i in range(align)]) + self.visibility
-        content += self.name + "(" + ",".join([v.get_mermaid(align=0) for v in self.args]) + ")"
+        name = self.name.split(":", 1)[1] if ":" in self.name else self.name
+        content += name + "(" + ",".join([v.get_mermaid(align=0) for v in self.args]) + ")"
         if self.return_type:
-            content += ":" + self.return_type
-        if self.abstraction:
-            content += "*"
-        if self.static:
-            content += "$"
+            content += " " + self.return_type.replace(" ", "")
+        # if self.abstraction:
+        #     content += "*"
+        # if self.static:
+        #     content += "$"
         return content
 
 
-class ClassView(ClassMeta):
-    attributes: List[ClassAttribute] = Field(default_factory=list)
-    methods: List[ClassMethod] = Field(default_factory=list)
+class UMLClassView(UMLClassMeta):
+    attributes: List[UMLClassAttribute] = Field(default_factory=list)
+    methods: List[UMLClassMethod] = Field(default_factory=list)
 
     def get_mermaid(self, align=1) -> str:
         content = "".join(["\t" for i in range(align)]) + "class " + self.name + "{\n"
         for v in self.attributes:
             content += v.get_mermaid(align=align + 1) + "\n"
         for v in self.methods:
             content += v.get_mermaid(align=align + 1) + "\n"
         content += "".join(["\t" for i in range(align)]) + "}\n"
         return content
+
+    @classmethod
+    def load_dot_class_info(cls, dot_class_info: DotClassInfo) -> UMLClassView:
+        visibility = UMLClassView.name_to_visibility(dot_class_info.name)
+        class_view = cls(name=dot_class_info.name, visibility=visibility)
+        for i in dot_class_info.attributes.values():
+            visibility = UMLClassAttribute.name_to_visibility(i.name)
+            attr = UMLClassAttribute(name=i.name, visibility=visibility, value_type=i.type_, default_value=i.default_)
+            class_view.attributes.append(attr)
+        for i in dot_class_info.methods.values():
+            visibility = UMLClassMethod.name_to_visibility(i.name)
+            method = UMLClassMethod(name=i.name, visibility=visibility, return_type=i.return_args.type_)
+            for j in i.args:
+                arg = UMLClassAttribute(name=j.name, value_type=j.type_, default_value=j.default_)
+                method.args.append(arg)
+            method.return_type = i.return_args.type_
+            class_view.methods.append(method)
+        return class_view
```

### Comparing `metagpt-0.7.7/metagpt/software_company.py` & `metagpt-0.8.0/metagpt/software_company.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/strategy/base.py` & `metagpt-0.8.0/metagpt/strategy/base.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/strategy/solver.py` & `metagpt-0.8.0/metagpt/strategy/solver.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/strategy/tot.py` & `metagpt-0.8.0/metagpt/strategy/tot.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/strategy/tot_schema.py` & `metagpt-0.8.0/metagpt/strategy/tot_schema.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/subscription.py` & `metagpt-0.8.0/metagpt/subscription.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/team.py` & `metagpt-0.8.0/metagpt/team.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/__init__.py` & `metagpt-0.8.0/metagpt/tools/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,7 +26,12 @@
     SELENIUM = "selenium"
     CUSTOM = "custom"
 
     @classmethod
     def __missing__(cls, key):
         """Default type conversion"""
         return cls.CUSTOM
+
+
+class SearchInterface:
+    async def asearch(self, *args, **kwargs):
+        ...
```

### Comparing `metagpt-0.7.7/metagpt/tools/azure_tts.py` & `metagpt-0.8.0/metagpt/tools/azure_tts.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/iflytek_tts.py` & `metagpt-0.8.0/metagpt/tools/iflytek_tts.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/libs/data_preprocess.py` & `metagpt-0.8.0/metagpt/tools/libs/data_preprocess.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import json
+from typing import Literal
 
 import numpy as np
 import pandas as pd
 from sklearn.impute import SimpleImputer
 from sklearn.preprocessing import (
     LabelEncoder,
     MaxAbsScaler,
@@ -12,17 +13,16 @@
     OneHotEncoder,
     OrdinalEncoder,
     RobustScaler,
     StandardScaler,
 )
 
 from metagpt.tools.tool_registry import register_tool
-from metagpt.tools.tool_type import ToolType
 
-TOOL_TYPE = ToolType.DATA_PREPROCESS.type_name
+TAGS = ["data preprocessing", "machine learning"]
 
 
 class MLProcess:
     def fit(self, df: pd.DataFrame):
         """
         Fit a model to be used in subsequent transform.
 
@@ -81,91 +81,93 @@
         if len(self.features) == 0:
             return df
         new_df = df.copy()
         new_df[self.features] = self.model.transform(new_df[self.features])
         return new_df
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class FillMissingValue(DataPreprocessTool):
     """
     Completing missing values with simple strategies.
     """
 
-    def __init__(self, features: list, strategy: str = "mean", fill_value=None):
+    def __init__(
+        self, features: list, strategy: Literal["mean", "median", "most_frequent", "constant"] = "mean", fill_value=None
+    ):
         """
         Initialize self.
 
         Args:
             features (list): Columns to be processed.
-            strategy (str, optional): The imputation strategy, notice 'mean' and 'median' can only
-                                      be used for numeric features. Enum: ['mean', 'median', 'most_frequent', 'constant']. Defaults to 'mean'.
+            strategy (Literal["mean", "median", "most_frequent", "constant"], optional): The imputation strategy, notice 'mean' and 'median' can only
+                                      be used for numeric features. Defaults to 'mean'.
             fill_value (int, optional): Fill_value is used to replace all occurrences of missing_values.
                                         Defaults to None.
         """
         self.features = features
         self.model = SimpleImputer(strategy=strategy, fill_value=fill_value)
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class MinMaxScale(DataPreprocessTool):
     """
     Transform features by scaling each feature to a range, which is (0, 1).
     """
 
     def __init__(self, features: list):
         self.features = features
         self.model = MinMaxScaler()
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class StandardScale(DataPreprocessTool):
     """
     Standardize features by removing the mean and scaling to unit variance.
     """
 
     def __init__(self, features: list):
         self.features = features
         self.model = StandardScaler()
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class MaxAbsScale(DataPreprocessTool):
     """
     Scale each feature by its maximum absolute value.
     """
 
     def __init__(self, features: list):
         self.features = features
         self.model = MaxAbsScaler()
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class RobustScale(DataPreprocessTool):
     """
     Apply the RobustScaler to scale features using statistics that are robust to outliers.
     """
 
     def __init__(self, features: list):
         self.features = features
         self.model = RobustScaler()
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class OrdinalEncode(DataPreprocessTool):
     """
     Encode categorical features as ordinal integers.
     """
 
     def __init__(self, features: list):
         self.features = features
         self.model = OrdinalEncoder()
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class OneHotEncode(DataPreprocessTool):
     """
     Apply one-hot encoding to specified categorical columns, the original columns will be dropped.
     """
 
     def __init__(self, features: list):
         self.features = features
@@ -176,15 +178,15 @@
         new_columns = self.model.get_feature_names_out(self.features)
         ts_data = pd.DataFrame(ts_data, columns=new_columns, index=df.index)
         new_df = df.drop(self.features, axis=1)
         new_df = pd.concat([new_df, ts_data], axis=1)
         return new_df
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class LabelEncode(DataPreprocessTool):
     """
     Apply label encoding to specified categorical columns in-place.
     """
 
     def __init__(self, features: list):
         """
```

### Comparing `metagpt-0.7.7/metagpt/tools/libs/email_login.py` & `metagpt-0.8.0/metagpt/tools/libs/email_login.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from imap_tools import MailBox
 
 from metagpt.tools.tool_registry import register_tool
-from metagpt.tools.tool_type import ToolType
 
 # Define a dictionary mapping email domains to their IMAP server addresses
 IMAP_SERVERS = {
     "outlook.com": "imap-mail.outlook.com",  # Outlook
     "163.com": "imap.163.com",  # 163 Mail
     "qq.com": "imap.qq.com",  # QQ Mail
     "gmail.com": "imap.gmail.com",  # Gmail
@@ -20,15 +19,15 @@
     "mail.ru": "imap.mail.ru",  # Mail.ru
     "aol.com": "imap.aol.com",  # AOL Mail
     "gmx.com": "imap.gmx.com",  # GMX Mail
     "zoho.com": "imap.zoho.com",  # Zoho Mail
 }
 
 
-@register_tool(tool_type=ToolType.EMAIL_LOGIN.type_name)
+@register_tool(tags=["email login"])
 def email_login_imap(email_address, email_password):
     """
     Use imap_tools package to log in to your email (the email that supports IMAP protocol) to verify and return the account object.
 
     Args:
         email_address (str): Email address that needs to be logged in and linked.
         email_password (str): Password for the email address that needs to be logged in and linked.
```

### Comparing `metagpt-0.7.7/metagpt/tools/libs/feature_engineering.py` & `metagpt-0.8.0/metagpt/tools/libs/feature_engineering.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,20 +15,19 @@
 from pandas.core.dtypes.common import is_object_dtype
 from sklearn.feature_selection import VarianceThreshold
 from sklearn.model_selection import KFold
 from sklearn.preprocessing import KBinsDiscretizer, PolynomialFeatures
 
 from metagpt.tools.libs.data_preprocess import MLProcess
 from metagpt.tools.tool_registry import register_tool
-from metagpt.tools.tool_type import ToolType
 
-TOOL_TYPE = ToolType.FEATURE_ENGINEERING.type_name
+TAGS = ["feature engineering", "machine learning"]
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class PolynomialExpansion(MLProcess):
     """
     Add polynomial and interaction features from selected numeric columns to input DataFrame.
     """
 
     def __init__(self, cols: list, label_col: str, degree: int = 2):
         """
@@ -63,15 +62,15 @@
         column_name = self.poly.get_feature_names_out(self.cols)
         ts_data = pd.DataFrame(ts_data, index=df.index, columns=column_name)
         new_df = df.drop(self.cols, axis=1)
         new_df = pd.concat([new_df, ts_data], axis=1)
         return new_df
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class CatCount(MLProcess):
     """
     Add value counts of a categorical column as new feature.
     """
 
     def __init__(self, col: str):
         """
@@ -88,15 +87,15 @@
 
     def transform(self, df: pd.DataFrame) -> pd.DataFrame:
         new_df = df.copy()
         new_df[f"{self.col}_cnt"] = new_df[self.col].map(self.encoder_dict)
         return new_df
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class TargetMeanEncoder(MLProcess):
     """
     Encode a categorical column by the mean of the label column, and adds the result as a new feature.
     """
 
     def __init__(self, col: str, label: str):
         """
@@ -115,15 +114,15 @@
 
     def transform(self, df: pd.DataFrame) -> pd.DataFrame:
         new_df = df.copy()
         new_df[f"{self.col}_target_mean"] = new_df[self.col].map(self.encoder_dict)
         return new_df
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class KFoldTargetMeanEncoder(MLProcess):
     """
     Add a new feature to the DataFrame by k-fold mean encoding of a categorical column using the label column.
     """
 
     def __init__(self, col: str, label: str, n_splits: int = 5, random_state: int = 2021):
         """
@@ -155,15 +154,15 @@
 
     def transform(self, df: pd.DataFrame) -> pd.DataFrame:
         new_df = df.copy()
         new_df[f"{self.col}_kf_target_mean"] = new_df[self.col].map(self.encoder_dict)
         return new_df
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class CatCross(MLProcess):
     """
     Add pairwise crossed features and convert them to numerical features.
     """
 
     def __init__(self, cols: list, max_cat_num: int = 100):
         """
@@ -212,15 +211,15 @@
             new_df[new_col] = pd.Series(zip(new_df[comb[0]], new_df[comb[1]])).map(_map)
             # set the unknown value to a new number
             new_df[new_col].fillna(max(_map.values()) + 1, inplace=True)
             new_df[new_col] = new_df[new_col].astype(int)
         return new_df
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class GroupStat(MLProcess):
     """
     Aggregate specified column in a DataFrame grouped by another column, adding new features named '<agg_col>_<agg_func>_by_<group_col>'.
     """
 
     def __init__(self, group_col: str, agg_col: str, agg_funcs: list):
         """
@@ -244,15 +243,15 @@
         self.group_df = group_df
 
     def transform(self, df: pd.DataFrame) -> pd.DataFrame:
         new_df = df.merge(self.group_df, on=self.group_col, how="left")
         return new_df
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class SplitBins(MLProcess):
     """
     Inplace binning of continuous data into intervals, returning integer-encoded bin identifiers directly.
     """
 
     def __init__(self, cols: list, strategy: str = "quantile"):
         """
@@ -272,15 +271,15 @@
 
     def transform(self, df: pd.DataFrame) -> pd.DataFrame:
         new_df = df.copy()
         new_df[self.cols] = self.encoder.transform(new_df[self.cols].fillna(0))
         return new_df
 
 
-# @register_tool(tool_type=TOOL_TYPE)
+# @register_tool(tags=TAGS)
 class ExtractTimeComps(MLProcess):
     """
     Extract time components from a datetime column and add them as new features.
     """
 
     def __init__(self, time_col: str, time_comps: list):
         """
@@ -312,15 +311,15 @@
             time_comps_df["dayofweek"] = time_s.dt.dayofweek + 1
         if "is_weekend" in self.time_comps:
             time_comps_df["is_weekend"] = time_s.dt.dayofweek.isin([5, 6]).astype(int)
         new_df = pd.concat([df, time_comps_df], axis=1)
         return new_df
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class GeneralSelection(MLProcess):
     """
     Drop all nan feats and feats with only one unique value.
     """
 
     def __init__(self, label_col: str):
         self.label_col = label_col
@@ -345,15 +344,15 @@
 
     def transform(self, df: pd.DataFrame) -> pd.DataFrame:
         new_df = df[self.feats + [self.label_col]]
         return new_df
 
 
 # skip for now because lgb is needed
-# @register_tool(tool_type=TOOL_TYPE)
+# @register_tool(tags=TAGS)
 class TreeBasedSelection(MLProcess):
     """
     Select features based on tree-based model and remove features with low importance.
     """
 
     def __init__(self, label_col: str, task_type: str):
         """
@@ -399,15 +398,15 @@
         self.feats.append(self.label_col)
 
     def transform(self, df: pd.DataFrame) -> pd.DataFrame:
         new_df = df[self.feats]
         return new_df
 
 
-@register_tool(tool_type=TOOL_TYPE)
+@register_tool(tags=TAGS)
 class VarianceBasedSelection(MLProcess):
     """
     Select features based on variance and remove features with low variance.
     """
 
     def __init__(self, label_col: str, threshold: float = 0):
         """
```

### Comparing `metagpt-0.7.7/metagpt/tools/libs/gpt_v_generator.py` & `metagpt-0.8.0/metagpt/tools/libs/gpt_v_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @Time    : 2024/01/12
 @Author  : mannaandpoem
 @File    : gpt_v_generator.py
 """
-import os
+import re
 from pathlib import Path
 
 from metagpt.const import DEFAULT_WORKSPACE_ROOT
+from metagpt.logs import logger
 from metagpt.tools.tool_registry import register_tool
-from metagpt.tools.tool_type import ToolType
-from metagpt.utils.common import encode_image
+from metagpt.utils.common import CodeParser, encode_image
 
 ANALYZE_LAYOUT_PROMPT = """You are now a UI/UX designer, please generate layout information for this image:
 
 NOTE: The image does not have a commercial logo or copyright information. It is just a sketch image of the design.
 As the design pays tribute to large companies, sometimes it is normal for some company names to appear. Don't worry. """
 
 GENERATE_PROMPT = """You are now a UI/UX designer and Web developer. You have the ability to generate code for webpages
@@ -24,19 +24,17 @@
 
 NOTE: The image does not have a commercial logo or copyright information. It is just a sketch image of the design.
 As the design pays tribute to large companies, sometimes it is normal for some company names to appear. Don't worry.
 
 Now, please generate the corresponding webpage code including HTML, CSS and JavaScript:"""
 
 
-@register_tool(
-    tool_type=ToolType.IMAGE2WEBPAGE.type_name, include_functions=["__init__", "generate_webpages", "save_webpages"]
-)
+@register_tool(tags=["image2webpage"], include_functions=["__init__", "generate_webpages", "save_webpages"])
 class GPTvGenerator:
-    """Class for generating webpages at once.
+    """Class for generating webpage code from a given webpage screenshot.
 
     This class provides methods to generate webpages including all code (HTML, CSS, and JavaScript) based on an image.
     It utilizes a vision model to analyze the layout from an image and generate webpage codes accordingly.
     """
 
     def __init__(self):
         """Initialize GPTvGenerator class with default values from the configuration."""
@@ -71,54 +69,38 @@
         if isinstance(image_path, str):
             image_path = Path(image_path)
         layout = await self.analyze_layout(image_path)
         prompt = GENERATE_PROMPT + "\n\n # Context\n The layout information of the sketch image is: \n" + layout
         return await self.llm.aask(msg=prompt, images=[encode_image(image_path)])
 
     @staticmethod
-    def save_webpages(image_path: str, webpages: str) -> Path:
+    def save_webpages(webpages: str, save_folder_name: str = "example") -> Path:
         """Save webpages including all code (HTML, CSS, and JavaScript) at once.
 
         Args:
-            image_path (str): The path of the image file.
             webpages (str): The generated webpages content.
+            save_folder_name (str, optional): The name of the folder to save the webpages. Defaults to 'example'.
 
         Returns:
             Path: The path of the saved webpages.
         """
         # Create a folder called webpages in the workspace directory to store HTML, CSS, and JavaScript files
-        webpages_path = DEFAULT_WORKSPACE_ROOT / "webpages" / Path(image_path).stem
-        os.makedirs(webpages_path, exist_ok=True)
+        webpages_path = DEFAULT_WORKSPACE_ROOT / "webpages" / save_folder_name
+        logger.info(f"code will be saved at {webpages_path}")
+        webpages_path.mkdir(parents=True, exist_ok=True)
 
         index_path = webpages_path / "index.html"
-        try:
-            index = webpages.split("```html")[1].split("```")[0]
-            style_path = None
-            if "styles.css" in index:
-                style_path = webpages_path / "styles.css"
-            elif "style.css" in index:
-                style_path = webpages_path / "style.css"
-            style = webpages.split("```css")[1].split("```")[0] if style_path else ""
-
-            js_path = None
-            if "scripts.js" in index:
-                js_path = webpages_path / "scripts.js"
-            elif "script.js" in index:
-                js_path = webpages_path / "script.js"
-
-            js = webpages.split("```javascript")[1].split("```")[0] if js_path else ""
-        except IndexError:
-            raise ValueError(f"No html or css or js code found in the result. \nWebpages: {webpages}")
-
-        try:
-            with open(index_path, "w", encoding="utf-8") as f:
-                f.write(index)
-            if style_path:
-                with open(style_path, "w", encoding="utf-8") as f:
-                    f.write(style)
-            if js_path:
-                with open(js_path, "w", encoding="utf-8") as f:
-                    f.write(js)
-        except FileNotFoundError as e:
-            raise FileNotFoundError(f"Cannot save the webpages to {str(webpages_path)}") from e
+        index_path.write_text(CodeParser.parse_code(block=None, text=webpages, lang="html"))
+
+        extract_and_save_code(folder=webpages_path, text=webpages, pattern="styles?.css", language="css")
+
+        extract_and_save_code(folder=webpages_path, text=webpages, pattern="scripts?.js", language="javascript")
 
         return webpages_path
+
+
+def extract_and_save_code(folder, text, pattern, language):
+    word = re.search(pattern, text)
+    if word:
+        path = folder / word.group(0)
+        code = CodeParser.parse_code(block=None, text=text, lang=language)
+        path.write_text(code, encoding="utf-8")
```

### Comparing `metagpt-0.7.7/metagpt/tools/libs/sd_engine.py` & `metagpt-0.8.0/metagpt/tools/libs/sd_engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,17 @@
 import json
 from os.path import join
 
 import requests
 from aiohttp import ClientSession
 from PIL import Image, PngImagePlugin
 
-#
 from metagpt.const import SD_OUTPUT_FILE_REPO, SOURCE_ROOT
 from metagpt.logs import logger
 from metagpt.tools.tool_registry import register_tool
-from metagpt.tools.tool_type import ToolType
 
 payload = {
     "prompt": "",
     "negative_prompt": "(easynegative:0.8),black, dark,Low resolution",
     "override_settings": {"sd_model_checkpoint": "galaxytimemachinesGTM_photoV20"},
     "seed": -1,
     "batch_size": 1,
@@ -51,15 +49,15 @@
     "alwayson_scripts": {},
 }
 
 default_negative_prompt = "(easynegative:0.8),black, dark,Low resolution"
 
 
 @register_tool(
-    tool_type=ToolType.STABLE_DIFFUSION.type_name,
+    tags=["text2image", "multimodal"],
     include_functions=["__init__", "simple_run_t2i", "run_t2i", "construct_payload", "save"],
 )
 class SDEngine:
     """Generate image using stable diffusion model.
 
     This class provides methods to interact with a stable diffusion service to generate images based on text inputs.
     """
```

### Comparing `metagpt-0.7.7/metagpt/tools/libs/web_scraping.py` & `metagpt-0.8.0/metagpt/tools/libs/web_scraping.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from metagpt.tools.tool_registry import register_tool
-from metagpt.tools.tool_type import ToolType
 from metagpt.tools.web_browser_engine_playwright import PlaywrightWrapper
 
 
-@register_tool(tool_type=ToolType.WEBSCRAPING.type_name)
+@register_tool(tags=["web scraping", "web"])
 async def scrape_web_playwright(url):
     """
     Asynchronously Scrape and save the HTML structure and inner text content of a web page using Playwright.
 
     Args:
         url (str): The main URL to fetch inner text from.
```

### Comparing `metagpt-0.7.7/metagpt/tools/metagpt_oas3_api_svc.py` & `metagpt-0.8.0/metagpt/tools/metagpt_oas3_api_svc.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/metagpt_text_to_image.py` & `metagpt-0.8.0/metagpt/tools/metagpt_text_to_image.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/moderation.py` & `metagpt-0.8.0/metagpt/tools/moderation.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/openai_text_to_embedding.py` & `metagpt-0.8.0/metagpt/tools/openai_text_to_embedding.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/openai_text_to_image.py` & `metagpt-0.8.0/metagpt/tools/openai_text_to_image.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/openapi_v3_hello.py` & `metagpt-0.8.0/metagpt/tools/openapi_v3_hello.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/prompt_writer.py` & `metagpt-0.8.0/metagpt/tools/prompt_writer.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/search_engine.py` & `metagpt-0.8.0/metagpt/tools/search_engine.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/search_engine_ddg.py` & `metagpt-0.8.0/metagpt/tools/search_engine_ddg.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/search_engine_googleapi.py` & `metagpt-0.8.0/metagpt/tools/search_engine_googleapi.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/search_engine_meilisearch.py` & `metagpt-0.8.0/metagpt/tools/search_engine_meilisearch.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/search_engine_serpapi.py` & `metagpt-0.8.0/metagpt/tools/search_engine_serpapi.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/search_engine_serper.py` & `metagpt-0.8.0/metagpt/tools/search_engine_serper.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/tool_convert.py` & `metagpt-0.8.0/metagpt/tools/tool_convert.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,61 @@
 import inspect
 
 from metagpt.utils.parse_docstring import GoogleDocstringParser, remove_spaces
 
+PARSER = GoogleDocstringParser
 
-def convert_code_to_tool_schema(obj, include: list[str] = []):
+
+def convert_code_to_tool_schema(obj, include: list[str] = None):
     docstring = inspect.getdoc(obj)
     assert docstring, "no docstring found for the objects, skip registering"
 
     if inspect.isclass(obj):
         schema = {"type": "class", "description": remove_spaces(docstring), "methods": {}}
         for name, method in inspect.getmembers(obj, inspect.isfunction):
+            if name.startswith("_") and name != "__init__":  # skip private methodss
+                continue
             if include and name not in include:
                 continue
             # method_doc = inspect.getdoc(method)
             method_doc = get_class_method_docstring(obj, name)
             if method_doc:
                 schema["methods"][name] = function_docstring_to_schema(method, method_doc)
 
     elif inspect.isfunction(obj):
         schema = function_docstring_to_schema(obj, docstring)
 
     return schema
 
 
-def function_docstring_to_schema(fn_obj, docstring):
-    function_type = "function" if not inspect.iscoroutinefunction(fn_obj) else "async_function"
-    return {"type": function_type, **docstring_to_schema(docstring)}
+def function_docstring_to_schema(fn_obj, docstring) -> dict:
+    """
+    Converts a function's docstring into a schema dictionary.
+
+    Args:
+        fn_obj: The function object.
+        docstring: The docstring of the function.
+
+    Returns:
+        A dictionary representing the schema of the function's docstring.
+        The dictionary contains the following keys:
+        - 'type': The type of the function ('function' or 'async_function').
+        - 'description': The first section of the docstring describing the function overall. Provided to LLMs for both recommending and using the function.
+        - 'signature': The signature of the function, which helps LLMs understand how to call the function.
+        - 'parameters': Docstring section describing parameters including args and returns, served as extra details for LLM perception.
+    """
+    signature = inspect.signature(fn_obj)
 
+    docstring = remove_spaces(docstring)
 
-def docstring_to_schema(docstring: str):
-    if docstring is None:
-        return {}
-
-    parser = GoogleDocstringParser(docstring=docstring)
-
-    # 匹配简介部分
-    description = parser.parse_desc()
-
-    # 匹配Args部分
-    params = parser.parse_params()
-    parameter_schema = {"properties": {}, "required": []}
-    for param in params:
-        param_name, param_type, param_desc = param
-        # check required or optional
-        is_optional, param_type = parser.check_and_parse_optional(param_type)
-        if not is_optional:
-            parameter_schema["required"].append(param_name)
-        # type and desc
-        param_dict = {"type": param_type, "description": remove_spaces(param_desc)}
-        # match Default for optional args
-        has_default_val, default_val = parser.check_and_parse_default_value(param_desc)
-        if has_default_val:
-            param_dict["default"] = default_val
-        # match Enum
-        has_enum, enum_vals = parser.check_and_parse_enum(param_desc)
-        if has_enum:
-            param_dict["enum"] = enum_vals
-        # add to parameter schema
-        parameter_schema["properties"].update({param_name: param_dict})
-
-    # 匹配Returns部分
-    returns = parser.parse_returns()
-
-    # 构建YAML字典
-    schema = {
-        "description": description,
-        "parameters": parameter_schema,
-    }
-    if returns:
-        schema["returns"] = [{"type": ret[0], "description": remove_spaces(ret[1])} for ret in returns]
+    overall_desc, param_desc = PARSER.parse(docstring)
 
-    return schema
+    function_type = "function" if not inspect.iscoroutinefunction(fn_obj) else "async_function"
+
+    return {"type": function_type, "description": overall_desc, "signature": str(signature), "parameters": param_desc}
 
 
 def get_class_method_docstring(cls, method_name):
     """Retrieve a method's docstring, searching the class hierarchy if necessary."""
     for base_class in cls.__mro__:
         if method_name in base_class.__dict__:
             method = base_class.__dict__[method_name]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `metagpt-0.7.7/metagpt/tools/tool_type.py` & `metagpt-0.8.0/metagpt/strategy/task_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,80 @@
 from enum import Enum
 
-from metagpt.prompts.tool_types import (
+from pydantic import BaseModel
+
+from metagpt.prompts.task_type import (
     DATA_PREPROCESS_PROMPT,
     EDA_PROMPT,
     FEATURE_ENGINEERING_PROMPT,
     IMAGE2WEBPAGE_PROMPT,
     MODEL_EVALUATE_PROMPT,
     MODEL_TRAIN_PROMPT,
 )
-from metagpt.tools.tool_data_type import ToolTypeDef
 
 
-class ToolType(Enum):
-    EDA = ToolTypeDef(
+class TaskTypeDef(BaseModel):
+    name: str
+    desc: str = ""
+    guidance: str = ""
+
+
+class TaskType(Enum):
+    """By identifying specific types of tasks, we can inject human priors (guidance) to help task solving"""
+
+    EDA = TaskTypeDef(
         name="eda",
         desc="For performing exploratory data analysis",
-        usage_prompt=EDA_PROMPT,
+        guidance=EDA_PROMPT,
     )
-    DATA_PREPROCESS = ToolTypeDef(
-        name="data_preprocess",
-        desc="Only for changing value inplace.",
-        usage_prompt=DATA_PREPROCESS_PROMPT,
+    DATA_PREPROCESS = TaskTypeDef(
+        name="data preprocessing",
+        desc="For preprocessing dataset in a data analysis or machine learning task ONLY,"
+        "general data operation doesn't fall into this type",
+        guidance=DATA_PREPROCESS_PROMPT,
     )
-    EMAIL_LOGIN = ToolTypeDef(
-        name="email_login",
-        desc="For logging to an email.",
-    )
-    FEATURE_ENGINEERING = ToolTypeDef(
-        name="feature_engineering",
+    FEATURE_ENGINEERING = TaskTypeDef(
+        name="feature engineering",
         desc="Only for creating new columns for input data.",
-        usage_prompt=FEATURE_ENGINEERING_PROMPT,
+        guidance=FEATURE_ENGINEERING_PROMPT,
     )
-    MODEL_TRAIN = ToolTypeDef(
-        name="model_train",
+    MODEL_TRAIN = TaskTypeDef(
+        name="model train",
         desc="Only for training model.",
-        usage_prompt=MODEL_TRAIN_PROMPT,
+        guidance=MODEL_TRAIN_PROMPT,
     )
-    MODEL_EVALUATE = ToolTypeDef(
-        name="model_evaluate",
+    MODEL_EVALUATE = TaskTypeDef(
+        name="model evaluate",
         desc="Only for evaluating model.",
-        usage_prompt=MODEL_EVALUATE_PROMPT,
-    )
-    STABLE_DIFFUSION = ToolTypeDef(
-        name="stable_diffusion",
-        desc="Related to text2image, image2image using stable diffusion model.",
+        guidance=MODEL_EVALUATE_PROMPT,
     )
-    IMAGE2WEBPAGE = ToolTypeDef(
+    IMAGE2WEBPAGE = TaskTypeDef(
         name="image2webpage",
         desc="For converting image into webpage code.",
-        usage_prompt=IMAGE2WEBPAGE_PROMPT,
+        guidance=IMAGE2WEBPAGE_PROMPT,
     )
-    WEBSCRAPING = ToolTypeDef(
-        name="web_scraping",
+    OTHER = TaskTypeDef(name="other", desc="Any tasks not in the defined categories")
+
+    # Legacy TaskType to support tool recommendation using type match. You don't need to define task types if you have no human priors to inject.
+    TEXT2IMAGE = TaskTypeDef(
+        name="text2image",
+        desc="Related to text2image, image2image using stable diffusion model.",
+    )
+    WEBSCRAPING = TaskTypeDef(
+        name="web scraping",
         desc="For scraping data from web pages.",
     )
-    OTHER = ToolTypeDef(name="other", desc="Any tools not in the defined categories")
-
-    def __missing__(self, key):
-        return self.OTHER
+    EMAIL_LOGIN = TaskTypeDef(
+        name="email login",
+        desc="For logging to an email.",
+    )
 
     @property
     def type_name(self):
         return self.value.name
+
+    @classmethod
+    def get_type(cls, type_name):
+        for member in cls:
+            if member.type_name == type_name:
+                return member.value
+        return None
```

### Comparing `metagpt-0.7.7/metagpt/tools/translator.py` & `metagpt-0.8.0/metagpt/tools/translator.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/ut_writer.py` & `metagpt-0.8.0/metagpt/tools/ut_writer.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/web_browser_engine.py` & `metagpt-0.8.0/metagpt/tools/web_browser_engine.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/web_browser_engine_playwright.py` & `metagpt-0.8.0/metagpt/tools/web_browser_engine_playwright.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/tools/web_browser_engine_selenium.py` & `metagpt-0.8.0/metagpt/tools/web_browser_engine_selenium.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 class WDMHttpProxyClient(WDMHttpClient):
     def __init__(self, proxy: str = None):
         super().__init__()
         self.proxy = proxy
 
     def get(self, url, **kwargs):
         if "proxies" not in kwargs and self.proxy:
-            kwargs["proxies"] = {"all_proxy": self.proxy}
+            kwargs["proxies"] = {"all": self.proxy}
         return super().get(url, **kwargs)
 
 
 def _gen_get_driver_func(browser_type, *args, executable_path=None, proxy=None):
     WebDriver = getattr(importlib.import_module(f"selenium.webdriver.{browser_type}.webdriver"), "WebDriver")
     Service = getattr(importlib.import_module(f"selenium.webdriver.{browser_type}.service"), "Service")
     Options = getattr(importlib.import_module(f"selenium.webdriver.{browser_type}.options"), "Options")
```

### Comparing `metagpt-0.7.7/metagpt/utils/ahttp_client.py` & `metagpt-0.8.0/metagpt/utils/ahttp_client.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/common.py` & `metagpt-0.8.0/metagpt/utils/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 import ast
 import base64
 import contextlib
 import csv
 import importlib
 import inspect
 import json
+import mimetypes
 import os
 import platform
 import re
 import sys
 import traceback
-import typing
 from io import BytesIO
 from pathlib import Path
-from typing import Any, Callable, List, Tuple, Union
+from typing import Any, Callable, List, Literal, Tuple, Union
+from urllib.parse import quote, unquote
 
 import aiofiles
 import chardet
 import loguru
 import requests
 from PIL import Image
 from pydantic_core import to_jsonable_python
@@ -358,24 +359,14 @@
     pattern = r"Send To:\s*([A-Za-z]+)\s*?"
     recipient = re.search(pattern, text)
     if recipient:
         return recipient.group(1)
     return ""
 
 
-def create_func_call_config(func_schema: dict) -> dict:
-    """Create new function call config"""
-    tools = [{"type": "function", "function": func_schema}]
-    tool_choice = {"type": "function", "function": {"name": func_schema["name"]}}
-    return {
-        "tools": tools,
-        "tool_choice": tool_choice,
-    }
-
-
 def remove_comments(code_str: str) -> str:
     """Remove comments from code."""
     pattern = r"(\".*?\"|\'.*?\')|(\#.*?$)"
 
     def replace_func(match):
         if match.group(2) is not None:
             return ""
@@ -430,31 +421,117 @@
             return True
     return False
 
 
 def any_to_name(val):
     """
     Convert a value to its name by extracting the last part of the dotted path.
+    """
+    return any_to_str(val).split(".")[-1]
+
 
-    :param val: The value to convert.
+def concat_namespace(*args, delimiter: str = ":") -> str:
+    """Concatenate fields to create a unique namespace prefix.
 
-    :return: The name of the value.
+    Example:
+        >>> concat_namespace('prefix', 'field1', 'field2', delimiter=":")
+        'prefix:field1:field2'
     """
-    return any_to_str(val).split(".")[-1]
+    return delimiter.join(str(value) for value in args)
 
 
-def concat_namespace(*args) -> str:
-    return ":".join(str(value) for value in args)
+def split_namespace(ns_class_name: str, delimiter: str = ":", maxsplit: int = 1) -> List[str]:
+    """Split a namespace-prefixed name into its namespace-prefix and name parts.
 
+    Example:
+        >>> split_namespace('prefix:classname')
+        ['prefix', 'classname']
 
-def split_namespace(ns_class_name: str) -> List[str]:
-    return ns_class_name.split(":")
+        >>> split_namespace('prefix:module:class', delimiter=":", maxsplit=2)
+        ['prefix', 'module', 'class']
+    """
+    return ns_class_name.split(delimiter, maxsplit=maxsplit)
+
+
+def auto_namespace(name: str, delimiter: str = ":") -> str:
+    """Automatically handle namespace-prefixed names.
+
+    If the input name is empty, returns a default namespace prefix and name.
+    If the input name is not namespace-prefixed, adds a default namespace prefix.
+    Otherwise, returns the input name unchanged.
 
+    Example:
+        >>> auto_namespace('classname')
+        '?:classname'
 
-def general_after_log(i: "loguru.Logger", sec_format: str = "%0.3f") -> typing.Callable[["RetryCallState"], None]:
+        >>> auto_namespace('prefix:classname')
+        'prefix:classname'
+
+        >>> auto_namespace('')
+        '?:?'
+
+        >>> auto_namespace('?:custom')
+        '?:custom'
+    """
+    if not name:
+        return f"?{delimiter}?"
+    v = split_namespace(name, delimiter=delimiter)
+    if len(v) < 2:
+        return f"?{delimiter}{name}"
+    return name
+
+
+def add_affix(text: str, affix: Literal["brace", "url", "none"] = "brace"):
+    """Add affix to encapsulate data.
+
+    Example:
+        >>> add_affix("data", affix="brace")
+        '{data}'
+
+        >>> add_affix("example.com", affix="url")
+        '%7Bexample.com%7D'
+
+        >>> add_affix("text", affix="none")
+        'text'
+    """
+    mappings = {
+        "brace": lambda x: "{" + x + "}",
+        "url": lambda x: quote("{" + x + "}"),
+    }
+    encoder = mappings.get(affix, lambda x: x)
+    return encoder(text)
+
+
+def remove_affix(text, affix: Literal["brace", "url", "none"] = "brace"):
+    """Remove affix to extract encapsulated data.
+
+    Args:
+        text (str): The input text with affix to be removed.
+        affix (str, optional): The type of affix used. Defaults to "brace".
+            Supported affix types: "brace" for removing curly braces, "url" for URL decoding within curly braces.
+
+    Returns:
+        str: The text with affix removed.
+
+    Example:
+        >>> remove_affix('{data}', affix="brace")
+        'data'
+
+        >>> remove_affix('%7Bexample.com%7D', affix="url")
+        'example.com'
+
+        >>> remove_affix('text', affix="none")
+        'text'
+    """
+    mappings = {"brace": lambda x: x[1:-1], "url": lambda x: unquote(x)[1:-1]}
+    decoder = mappings.get(affix, lambda x: x)
+    return decoder(text)
+
+
+def general_after_log(i: "loguru.Logger", sec_format: str = "%0.3f") -> Callable[["RetryCallState"], None]:
     """
     Generates a logging function to be used after a call is retried.
 
     This generated function logs an error message with the outcome of the retried function call. It includes
     the name of the function, the time taken for the call in seconds (formatted according to `sec_format`),
     the number of attempts made, and the exception raised, if any.
 
@@ -640,20 +717,68 @@
                 subfolder_files = list_files(root=file_path)
                 files.extend(subfolder_files)
     except Exception as e:
         logger.error(f"Error: {e}")
     return files
 
 
+def parse_json_code_block(markdown_text: str) -> List[str]:
+    json_blocks = re.findall(r"```json(.*?)```", markdown_text, re.DOTALL)
+    return [v.strip() for v in json_blocks]
+
+
+def remove_white_spaces(v: str) -> str:
+    return re.sub(r"(?<!['\"])\s|(?<=['\"])\s", "", v)
+
+
+async def aread_bin(filename: str | Path) -> bytes:
+    """Read binary file asynchronously.
+
+    Args:
+        filename (Union[str, Path]): The name or path of the file to be read.
+
+    Returns:
+        bytes: The content of the file as bytes.
+
+    Example:
+        >>> content = await aread_bin('example.txt')
+        b'This is the content of the file.'
+
+        >>> content = await aread_bin(Path('example.txt'))
+        b'This is the content of the file.'
+    """
+    async with aiofiles.open(str(filename), mode="rb") as reader:
+        content = await reader.read()
+    return content
+
+
+async def awrite_bin(filename: str | Path, data: bytes):
+    """Write binary file asynchronously.
+
+    Args:
+        filename (Union[str, Path]): The name or path of the file to be written.
+        data (bytes): The binary data to be written to the file.
+
+    Example:
+        >>> await awrite_bin('output.bin', b'This is binary data.')
+
+        >>> await awrite_bin(Path('output.bin'), b'Another set of binary data.')
+    """
+    pathname = Path(filename)
+    pathname.parent.mkdir(parents=True, exist_ok=True)
+    async with aiofiles.open(str(pathname), mode="wb") as writer:
+        await writer.write(data)
+
+
 def is_coroutine_func(func: Callable) -> bool:
     return inspect.iscoroutinefunction(func)
 
 
 def load_mc_skills_code(skill_names: list[str] = None, skills_dir: Path = None) -> list[str]:
-    """load mincraft skill from js files"""
+    """load minecraft skill from js files"""
     if not skills_dir:
         skills_dir = Path(__file__).parent.absolute()
     if skill_names is None:
         skill_names = [skill[:-3] for skill in os.listdir(f"{skills_dir}") if skill.endswith(".js")]
     skills = [skills_dir.joinpath(f"{skill_name}.js").read_text() for skill_name in skill_names]
     return skills
 
@@ -680,7 +805,36 @@
         img = Image.open(BytesIO(resp.content))
     else:
         # image b64_json
         b64_data = re.sub("^data:image/.+;base64,", "", img_url_or_b64)
         img_data = BytesIO(base64.b64decode(b64_data))
         img = Image.open(img_data)
     return img
+
+
+def log_and_reraise(retry_state: RetryCallState):
+    logger.error(f"Retry attempts exhausted. Last exception: {retry_state.outcome.exception()}")
+    logger.warning(
+        """
+Recommend going to https://deepwisdom.feishu.cn/wiki/MsGnwQBjiif9c3koSJNcYaoSnu4#part-XdatdVlhEojeAfxaaEZcMV3ZniQ
+See FAQ 5.8
+"""
+    )
+    raise retry_state.outcome.exception()
+
+
+def get_markdown_codeblock_type(filename: str) -> str:
+    """Return the markdown code-block type corresponding to the file extension."""
+    mime_type, _ = mimetypes.guess_type(filename)
+    mappings = {
+        "text/x-shellscript": "bash",
+        "text/x-c++src": "cpp",
+        "text/css": "css",
+        "text/html": "html",
+        "text/x-java": "java",
+        "application/javascript": "javascript",
+        "application/json": "json",
+        "text/x-python": "python",
+        "text/x-ruby": "ruby",
+        "application/sql": "sql",
+    }
+    return mappings.get(mime_type, "text")
```

### Comparing `metagpt-0.7.7/metagpt/utils/custom_decoder.py` & `metagpt-0.8.0/metagpt/utils/custom_decoder.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/dependency_file.py` & `metagpt-0.8.0/metagpt/utils/dependency_file.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/exceptions.py` & `metagpt-0.8.0/metagpt/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/file.py` & `metagpt-0.8.0/metagpt/utils/file.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/file_repository.py` & `metagpt-0.8.0/metagpt/utils/file_repository.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/git_repository.py` & `metagpt-0.8.0/metagpt/utils/git_repository.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/highlight.py` & `metagpt-0.8.0/metagpt/utils/highlight.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/human_interaction.py` & `metagpt-0.8.0/metagpt/utils/human_interaction.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/json_to_markdown.py` & `metagpt-0.8.0/metagpt/utils/json_to_markdown.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/make_sk_kernel.py` & `metagpt-0.8.0/metagpt/utils/make_sk_kernel.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/mermaid.py` & `metagpt-0.8.0/metagpt/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/mmdc_ink.py` & `metagpt-0.8.0/metagpt/utils/mmdc_ink.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/mmdc_playwright.py` & `metagpt-0.8.0/metagpt/utils/mmdc_playwright.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/mmdc_pyppeteer.py` & `metagpt-0.8.0/metagpt/utils/mmdc_pyppeteer.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/parse_html.py` & `metagpt-0.8.0/metagpt/utils/parse_html.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/project_repo.py` & `metagpt-0.8.0/metagpt/utils/project_repo.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     SEQ_FLOW_FILE_REPO,
     SYSTEM_DESIGN_FILE_REPO,
     SYSTEM_DESIGN_PDF_FILE_REPO,
     TASK_FILE_REPO,
     TASK_PDF_FILE_REPO,
     TEST_CODES_FILE_REPO,
     TEST_OUTPUTS_FILE_REPO,
+    VISUAL_GRAPH_REPO_FILE_REPO,
 )
 from metagpt.utils.file_repository import FileRepository
 from metagpt.utils.git_repository import GitRepository
 
 
 class DocFileRepositories(FileRepository):
     prd: FileRepository
@@ -65,27 +66,29 @@
     seq_flow: FileRepository
     system_design: FileRepository
     prd: FileRepository
     api_spec_and_task: FileRepository
     code_summary: FileRepository
     sd_output: FileRepository
     code_plan_and_change: FileRepository
+    graph_repo: FileRepository
 
     def __init__(self, git_repo):
         super().__init__(git_repo=git_repo, relative_path=RESOURCES_FILE_REPO)
 
         self.competitive_analysis = git_repo.new_file_repository(relative_path=COMPETITIVE_ANALYSIS_FILE_REPO)
         self.data_api_design = git_repo.new_file_repository(relative_path=DATA_API_DESIGN_FILE_REPO)
         self.seq_flow = git_repo.new_file_repository(relative_path=SEQ_FLOW_FILE_REPO)
         self.system_design = git_repo.new_file_repository(relative_path=SYSTEM_DESIGN_PDF_FILE_REPO)
         self.prd = git_repo.new_file_repository(relative_path=PRD_PDF_FILE_REPO)
         self.api_spec_and_task = git_repo.new_file_repository(relative_path=TASK_PDF_FILE_REPO)
         self.code_summary = git_repo.new_file_repository(relative_path=CODE_SUMMARIES_PDF_FILE_REPO)
         self.sd_output = git_repo.new_file_repository(relative_path=SD_OUTPUT_FILE_REPO)
         self.code_plan_and_change = git_repo.new_file_repository(relative_path=CODE_PLAN_AND_CHANGE_PDF_FILE_REPO)
+        self.graph_repo = git_repo.new_file_repository(relative_path=VISUAL_GRAPH_REPO_FILE_REPO)
 
 
 class ProjectRepo(FileRepository):
     def __init__(self, root: str | Path | GitRepository):
         if isinstance(root, str) or isinstance(root, Path):
             git_repo_ = GitRepository(local_path=Path(root))
         elif isinstance(root, GitRepository):
@@ -129,14 +132,15 @@
         git_workdir = self.git_repo.workdir
         src_workdir = git_workdir / git_workdir.name
         if not src_workdir.exists():
             return False
         code_files = self.with_src_path(path=git_workdir / git_workdir.name).srcs.all_files
         if not code_files:
             return False
+        return bool(code_files)
 
     def with_src_path(self, path: str | Path) -> ProjectRepo:
         try:
             self._srcs_path = Path(path).relative_to(self.workdir)
         except ValueError:
             self._srcs_path = Path(path)
         return self
```

### Comparing `metagpt-0.7.7/metagpt/utils/pycst.py` & `metagpt-0.8.0/metagpt/utils/pycst.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/read_document.py` & `metagpt-0.8.0/metagpt/utils/read_document.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/recovery_util.py` & `metagpt-0.8.0/metagpt/utils/recovery_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,9 +50,9 @@
     save_path.mkdir(parents=True, exist_ok=True)
 
     plan = role.planner.plan.dict()
 
     with open(save_path / "plan.json", "w", encoding="utf-8") as plan_file:
         json.dump(plan, plan_file, indent=4, ensure_ascii=False)
 
-    save_code_file(name=Path(record_time) / "history_nb", code_context=role.execute_code.nb, file_format="ipynb")
+    save_code_file(name=Path(record_time), code_context=role.execute_code.nb, file_format="ipynb")
     return save_path
```

### Comparing `metagpt-0.7.7/metagpt/utils/redis.py` & `metagpt-0.8.0/metagpt/utils/redis.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/repair_llm_raw_output.py` & `metagpt-0.8.0/metagpt/utils/repair_llm_raw_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
         output = output[1:]
         logger.info(f"repair_json_format: {'[{'}")
     elif output.endswith("}]"):
         output = output[:-1]
         logger.info(f"repair_json_format: {'}]'}")
     elif output.startswith("{") and output.endswith("]"):
         output = output[:-1] + "}"
+
     # remove comments in output json string, after json value content, maybe start with #, maybe start with //
     arr = output.split("\n")
     new_arr = []
     for json_line in arr:
         # look for # or // comments and make sure they are not inside the string value
         comment_index = -1
         for match in re.finditer(r"(\".*?\"|\'.*?\')|(#|//)", json_line):
@@ -204,14 +205,25 @@
             # problem, redundant char `}`
             new_line = line.replace("}", "")
         elif line.endswith("},") and output.endswith("},"):
             new_line = line[:-1]
         elif (rline[col_no] in ["'", '"']) and (line.startswith('"') or line.startswith("'")) and "," not in line:
             # problem, `"""` or `'''` without `,`
             new_line = f",{line}"
+        elif col_no - 1 >= 0 and rline[col_no - 1] in ['"', "'"]:
+            # backslash problem like \" in the output
+            char = rline[col_no - 1]
+            nearest_char_idx = rline[col_no:].find(char)
+            new_line = (
+                rline[: col_no - 1]
+                + "\\"
+                + rline[col_no - 1 : col_no + nearest_char_idx]
+                + "\\"
+                + rline[col_no + nearest_char_idx :]
+            )
         elif '",' not in line and "," not in line and '"' not in line:
             new_line = f'{line}",'
         elif not line.endswith(","):
             # problem, miss char `,` at the end.
             new_line = f"{line},"
         elif "," in line and len(line) == 1:
             new_line = f'"{line}'
@@ -324,12 +336,14 @@
     For openai models, they will always return state number. But for open llm models, the instruction result maybe a
     long text contain target number, so here add a extraction to improve success rate.
 
     Args:
         content (str): llm's output from `Role._think`
     """
     content = content.strip()  # deal the output cases like " 0", "0\n" and so on.
-    pattern = r"([0-9])"  # TODO find the number using a more proper method not just extract from content using pattern
+    pattern = (
+        r"(?<!-)[0-9]"  # TODO find the number using a more proper method not just extract from content using pattern
+    )
     matches = re.findall(pattern, content, re.DOTALL)
     matches = list(set(matches))
     state = matches[0] if len(matches) > 0 else "-1"
     return state
```

### Comparing `metagpt-0.7.7/metagpt/utils/s3.py` & `metagpt-0.8.0/metagpt/utils/s3.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/save_code.py` & `metagpt-0.8.0/metagpt/utils/save_code.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/serialize.py` & `metagpt-0.8.0/metagpt/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/singleton.py` & `metagpt-0.8.0/metagpt/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/text.py` & `metagpt-0.8.0/metagpt/utils/text.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt/utils/yaml_model.py` & `metagpt-0.8.0/metagpt/utils/yaml_model.py`

 * *Files identical despite different names*

### Comparing `metagpt-0.7.7/metagpt.egg-info/PKG-INFO` & `metagpt-0.8.0/metagpt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: metagpt
-Version: 0.7.7
+Version: 0.8.0
 Summary: The Multi-Agent Framework
 Home-page: https://github.com/geekan/MetaGPT
 Author: Alexander Wu
 Author-email: alexanderwu@deepwisdom.ai
 License: MIT
 Keywords: metagpt multi-agent multi-role programming gpt llm metaprogramming
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: selenium
 Provides-Extra: search-google
 Provides-Extra: search-ddg
 Provides-Extra: ocr
+Provides-Extra: rag
 Provides-Extra: test
 Provides-Extra: pyppeteer
 Provides-Extra: dev
 License-File: LICENSE
 
 
 # MetaGPT: The Multi-Agent Framework
@@ -42,15 +43,17 @@
 <p align="center">
    <a href="https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/geekan/MetaGPT"><img src="https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode" alt="Open in Dev Containers"></a>
    <a href="https://codespaces.new/geekan/MetaGPT"><img src="https://img.shields.io/badge/Github_Codespace-Open-blue?logo=github" alt="Open in GitHub Codespaces"></a>
    <a href="https://huggingface.co/spaces/deepwisdom/MetaGPT" target="_blank"><img alt="Hugging Face" src="https://img.shields.io/badge/%F0%9F%A4%97%20-Hugging%20Face-blue?color=blue&logoColor=white" /></a>
 </p>
 
 ## News
-🚀 March. 01, 2024: Our Data Interpreter paper is on arxiv. Find all design and benchmark details [here](https://arxiv.org/abs/2402.18679)!
+🚀 Mar. 29, 2024: [v0.8.0](https://github.com/geekan/MetaGPT/releases/tag/v0.8.0) released. Now you can use Data Interpreter via pypi package import. Meanwhile, we integrated RAG module and supported multiple new LLMs.
+
+🚀 Mar. 14, 2024: Our **Data Interpreter** paper is on [arxiv](https://arxiv.org/abs/2402.18679). Check the [example](https://docs.deepwisdom.ai/main/en/DataInterpreter/) and [code](https://github.com/geekan/MetaGPT/tree/main/examples/di)!
 
 🚀 Feb. 08, 2024: [v0.7.0](https://github.com/geekan/MetaGPT/releases/tag/v0.7.0) released, supporting assigning different LLMs to different Roles. We also introduced [Data Interpreter](https://github.com/geekan/MetaGPT/blob/main/examples/di/README.md), a powerful agent capable of solving a wide range of real-world problems.
 
 🚀 Jan. 16, 2024: Our paper [MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework
 ](https://arxiv.org/abs/2308.00352) accepted for oral presentation **(top 1.2%)** at ICLR 2024, **ranking #1** in the LLM-based Agent category.
 
 🚀 Jan. 03, 2024: [v0.6.0](https://github.com/geekan/MetaGPT/releases/tag/v0.6.0) released, new features include serialization, upgraded OpenAI package and supported multiple LLM, provided [minimal example for debate](https://github.com/geekan/MetaGPT/blob/main/examples/debate_simple.py) etc.
@@ -71,57 +74,77 @@
 2. Internally, MetaGPT includes **product managers / architects / project managers / engineers.** It provides the entire process of a **software company along with carefully orchestrated SOPs.**
    1. `Code = SOP(Team)` is the core philosophy. We materialize SOP and apply it to teams composed of LLMs.
 
 ![A software company consists of LLM-based roles](docs/resources/software_company_cd.jpeg)
 
 <p align="center">Software Company Multi-Agent Schematic (Gradually Implementing)</p>
 
-## Install
+## Get Started
 
-### Pip installation
+### Installation
 
 > Ensure that Python 3.9+ is installed on your system. You can check this by using: `python --version`.  
 > You can use conda like this: `conda create -n metagpt python=3.9 && conda activate metagpt`
 
 ```bash
-pip install metagpt
-metagpt --init-config  # create ~/.metagpt/config2.yaml, modify it to your own config
+pip install --upgrade metagpt
+# or `pip install --upgrade git+https://github.com/geekan/MetaGPT.git`
+# or `git clone https://github.com/geekan/MetaGPT && cd MetaGPT && pip install --upgrade -e .`
+```
+
+For detailed installation guidance, please refer to [cli_install](https://docs.deepwisdom.ai/main/en/guide/get_started/installation.html#install-stable-version)
+ or [docker_install](https://docs.deepwisdom.ai/main/en/guide/get_started/installation.html#install-with-docker)
+
+### Configuration
+
+You can init the config of MetaGPT by running the following command, or manually create `~/.metagpt/config2.yaml` file:
+```bash
+# Check https://docs.deepwisdom.ai/main/en/guide/get_started/configuration.html for more details
+metagpt --init-config  # it will create ~/.metagpt/config2.yaml, just modify it to your needs
+```
+
+You can configure `~/.metagpt/config2.yaml` according to the [example](https://github.com/geekan/MetaGPT/blob/main/config/config2.example.yaml) and [doc](https://docs.deepwisdom.ai/main/en/guide/get_started/configuration.html):
+
+```yaml
+llm:
+  api_type: "openai"  # or azure / ollama / open_llm etc. Check LLMType for more options
+  model: "gpt-4-turbo-preview"  # or gpt-3.5-turbo-1106 / gpt-4-1106-preview
+  base_url: "https://api.openai.com/v1"  # or forward url / other llm url
+  api_key: "YOUR_API_KEY"
+```
+
+### Usage
+
+After installation, you can use MetaGPT at CLI
+
+```bash
 metagpt "Create a 2048 game"  # this will create a repo in ./workspace
 ```
 
-or you can use it as library
+or use it as library
 
 ```python
 from metagpt.software_company import generate_repo, ProjectRepo
 repo: ProjectRepo = generate_repo("Create a 2048 game")  # or ProjectRepo("<path>")
 print(repo)  # it will print the repo structure with files
 ```
 
-detail installation please refer to [cli_install](https://docs.deepwisdom.ai/main/en/guide/get_started/installation.html#install-stable-version)
+You can also use its [Data Interpreter](https://github.com/geekan/MetaGPT/tree/main/examples/di)
+
+```python
+import asyncio
+from metagpt.roles.di.data_interpreter import DataInterpreter
 
-### Docker installation
-> Note: In the Windows, you need to replace "/opt/metagpt" with a directory that Docker has permission to create, such as "D:\Users\x\metagpt"
+async def main():
+    di = DataInterpreter()
+    await di.run("Run data analysis on sklearn Iris dataset, include a plot")
 
-```bash
-# Step 1: Download metagpt official image and prepare config2.yaml
-docker pull metagpt/metagpt:latest
-mkdir -p /opt/metagpt/{config,workspace}
-docker run --rm metagpt/metagpt:latest cat /app/metagpt/config/config2.yaml > /opt/metagpt/config/config2.yaml
-vim /opt/metagpt/config/config2.yaml # Change the config
-
-# Step 2: Run metagpt demo with container
-docker run --rm \
-    --privileged \
-    -v /opt/metagpt/config/config2.yaml:/app/metagpt/config/config2.yaml \
-    -v /opt/metagpt/workspace:/app/metagpt/workspace \
-    metagpt/metagpt:latest \
-    metagpt "Create a 2048 game"
+asyncio.run(main())  # or await main() in a jupyter notebook setting
 ```
 
-detail installation please refer to [docker_install](https://docs.deepwisdom.ai/main/en/guide/get_started/installation.html#install-with-docker)
 
 ### QuickStart & Demo Video
 - Try it on [MetaGPT Huggingface Space](https://huggingface.co/spaces/deepwisdom/MetaGPT)
 - [Matthew Berman: How To Install MetaGPT - Build A Startup With One Prompt!!](https://youtu.be/uT75J_KG_aY)
 - [Official Demo Video](https://github.com/geekan/MetaGPT/assets/2707039/5e8c1062-8c35-440f-bb20-2b0320f8d27d)
 
 https://github.com/geekan/MetaGPT/assets/34952977/34345016-5d13-489d-b9f9-b82ace413419
@@ -133,14 +156,15 @@
 - 🔎 [What can MetaGPT do?](https://docs.deepwisdom.ai/main/en/guide/get_started/introduction.html)
 - 🛠 How to build your own agents? 
   - [MetaGPT Usage & Development Guide | Agent 101](https://docs.deepwisdom.ai/main/en/guide/tutorials/agent_101.html)
   - [MetaGPT Usage & Development Guide | MultiAgent 101](https://docs.deepwisdom.ai/main/en/guide/tutorials/multi_agent_101.html)
 - 🧑‍💻 Contribution
   - [Develop Roadmap](docs/ROADMAP.md)
 - 🔖 Use Cases
+  - [Data Interpreter](https://docs.deepwisdom.ai/main/en/guide/use_cases/agent/interpreter/intro.html)
   - [Debate](https://docs.deepwisdom.ai/main/en/guide/use_cases/multi_agent/debate.html)
   - [Researcher](https://docs.deepwisdom.ai/main/en/guide/use_cases/agent/researcher.html)
   - [Recepit Assistant](https://docs.deepwisdom.ai/main/en/guide/use_cases/agent/receipt_assistant.html)
 - ❓ [FAQs](https://docs.deepwisdom.ai/main/en/guide/faq.html)
 
 ## Support
 
@@ -156,19 +180,31 @@
 - **Email:** alexanderwu@deepwisdom.ai
 - **GitHub Issues:** For more technical inquiries, you can also create a new issue in our [GitHub repository](https://github.com/geekan/metagpt/issues).
 
 We will respond to all questions within 2-3 business days.
 
 ## Citation
 
-For now, cite the [arXiv paper](https://arxiv.org/abs/2308.00352):
+To stay updated with the latest research and development, follow [@MetaGPT_](https://twitter.com/MetaGPT_) on Twitter. 
+
+To cite [MetaGPT](https://arxiv.org/abs/2308.00352) or [Data Interpreter](https://arxiv.org/abs/2402.18679) in publications, please use the following BibTeX entries.
 
 ```bibtex
 @misc{hong2023metagpt,
       title={MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework}, 
       author={Sirui Hong and Mingchen Zhuge and Jonathan Chen and Xiawu Zheng and Yuheng Cheng and Ceyao Zhang and Jinlin Wang and Zili Wang and Steven Ka Shing Yau and Zijuan Lin and Liyang Zhou and Chenyu Ran and Lingfeng Xiao and Chenglin Wu and Jürgen Schmidhuber},
       year={2023},
       eprint={2308.00352},
       archivePrefix={arXiv},
       primaryClass={cs.AI}
 }
+@misc{hong2024data,
+      title={Data Interpreter: An LLM Agent For Data Science}, 
+      author={Sirui Hong and Yizhang Lin and Bang Liu and Bangbang Liu and Binhao Wu and Danyang Li and Jiaqi Chen and Jiayi Zhang and Jinlin Wang and Li Zhang and Lingyao Zhang and Min Yang and Mingchen Zhuge and Taicheng Guo and Tuo Zhou and Wei Tao and Wenyi Wang and Xiangru Tang and Xiangtao Lu and Xiawu Zheng and Xinbing Liang and Yaying Fei and Yuheng Cheng and Zongze Xu and Chenglin Wu},
+      year={2024},
+      eprint={2402.18679},
+      archivePrefix={arXiv},
+      primaryClass={cs.AI}
+}
+
 ```
+
```

#### html2text {}

```diff
@@ -1,35 +1,39 @@
-Metadata-Version: 2.1 Name: metagpt Version: 0.7.7 Summary: The Multi-Agent
+Metadata-Version: 2.1 Name: metagpt Version: 0.8.0 Summary: The Multi-Agent
 Framework Home-page: https://github.com/geekan/MetaGPT Author: Alexander Wu
 Author-email: alexanderwu@deepwisdom.ai License: MIT Keywords: metagpt multi-
 agent multi-role programming gpt llm metaprogramming Requires-Python: >=3.9
 Description-Content-Type: text/markdown Provides-Extra: selenium Provides-
 Extra: search-google Provides-Extra: search-ddg Provides-Extra: ocr Provides-
-Extra: test Provides-Extra: pyppeteer Provides-Extra: dev License-File: LICENSE
-# MetaGPT: The Multi-Agent Framework
+Extra: rag Provides-Extra: test Provides-Extra: pyppeteer Provides-Extra: dev
+License-File: LICENSE # MetaGPT: The Multi-Agent Framework
 [MetaGPT logo: Enable GPT to work in software company, collaborating to tackle
                              more complex tasks.]
    AAssssiiggnn ddiiffffeerreenntt rroolleess ttoo GGPPTTss ttoo ffoorrmm aa ccoollllaabboorraattiivvee eennttiittyy ffoorr ccoommpplleexx
                                     ttaasskkss..
 _[_C_N_ _d_o_c_]_[_E_N_ _d_o_c_]_[_J_A_ _d_o_c_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]_[_r_o_a_d_m_a_p_]_[_D_i_s_c_o_r_d_ _F_o_l_l_o_w_]_[_T_w_i_t_t_e_r_ _F_o_l_l_o_w_]
        _[_O_p_e_n_ _i_n_ _D_e_v_ _C_o_n_t_a_i_n_e_r_s_]_[_O_p_e_n_ _i_n_ _G_i_t_H_u_b_ _C_o_d_e_s_p_a_c_e_s_]_[_H_u_g_g_i_n_g_ _F_a_c_e_]
-## News ð March. 01, 2024: Our Data Interpreter paper is on arxiv. Find all
-design and benchmark details [here](https://arxiv.org/abs/2402.18679)! ð
-Feb. 08, 2024: [v0.7.0](https://github.com/geekan/MetaGPT/releases/tag/v0.7.0)
-released, supporting assigning different LLMs to different Roles. We also
-introduced [Data Interpreter](https://github.com/geekan/MetaGPT/blob/main/
-examples/di/README.md), a powerful agent capable of solving a wide range of
-real-world problems. ð Jan. 16, 2024: Our paper [MetaGPT: Meta Programming
-for A Multi-Agent Collaborative Framework ](https://arxiv.org/abs/2308.00352)
-accepted for oral presentation **(top 1.2%)** at ICLR 2024, **ranking #1** in
-the LLM-based Agent category. ð Jan. 03, 2024: [v0.6.0](https://github.com/
-geekan/MetaGPT/releases/tag/v0.6.0) released, new features include
-serialization, upgraded OpenAI package and supported multiple LLM, provided
-[minimal example for debate](https://github.com/geekan/MetaGPT/blob/main/
-examples/debate_simple.py) etc. ð Dec. 15, 2023: [v0.5.0](https://
+## News ð Mar. 29, 2024: [v0.8.0](https://github.com/geekan/MetaGPT/
+releases/tag/v0.8.0) released. Now you can use Data Interpreter via pypi
+package import. Meanwhile, we integrated RAG module and supported multiple new
+LLMs. ð Mar. 14, 2024: Our **Data Interpreter** paper is on [arxiv](https://
+arxiv.org/abs/2402.18679). Check the [example](https://docs.deepwisdom.ai/main/
+en/DataInterpreter/) and [code](https://github.com/geekan/MetaGPT/tree/main/
+examples/di)! ð Feb. 08, 2024: [v0.7.0](https://github.com/geekan/MetaGPT/
+releases/tag/v0.7.0) released, supporting assigning different LLMs to different
+Roles. We also introduced [Data Interpreter](https://github.com/geekan/MetaGPT/
+blob/main/examples/di/README.md), a powerful agent capable of solving a wide
+range of real-world problems. ð Jan. 16, 2024: Our paper [MetaGPT: Meta
+Programming for A Multi-Agent Collaborative Framework ](https://arxiv.org/abs/
+2308.00352) accepted for oral presentation **(top 1.2%)** at ICLR 2024,
+**ranking #1** in the LLM-based Agent category. ð Jan. 03, 2024: [v0.6.0]
+(https://github.com/geekan/MetaGPT/releases/tag/v0.6.0) released, new features
+include serialization, upgraded OpenAI package and supported multiple LLM,
+provided [minimal example for debate](https://github.com/geekan/MetaGPT/blob/
+main/examples/debate_simple.py) etc. ð Dec. 15, 2023: [v0.5.0](https://
 github.com/geekan/MetaGPT/releases/tag/v0.5.0) released, introducing some
 experimental features such as **incremental development**, **multilingual**,
 **multiple programming languages**, etc. ð¥ Nov. 08, 2023: MetaGPT is
 selected into [Open100: Top 100 Open Source achievements](https://
 www.benchcouncil.org/evaluation/opencs/annual.html). ð¥ Sep. 01, 2023:
 MetaGPT tops GitHub Trending Monthly for the **17th time** in August 2023. ð
 Jun. 30, 2023: MetaGPT is now open source. ð Apr. 24, 2023: First line of
@@ -39,63 +43,82 @@
 etc.** 2. Internally, MetaGPT includes **product managers / architects /
 project managers / engineers.** It provides the entire process of a **software
 company along with carefully orchestrated SOPs.** 1. `Code = SOP(Team)` is the
 core philosophy. We materialize SOP and apply it to teams composed of LLMs. ![A
 software company consists of LLM-based roles](docs/resources/
 software_company_cd.jpeg)
         Software Company Multi-Agent Schematic (Gradually Implementing)
-## Install ### Pip installation > Ensure that Python 3.9+ is installed on your
+## Get Started ### Installation > Ensure that Python 3.9+ is installed on your
 system. You can check this by using: `python --version`. > You can use conda
 like this: `conda create -n metagpt python=3.9 && conda activate metagpt`
-```bash pip install metagpt metagpt --init-config # create ~/.metagpt/
-config2.yaml, modify it to your own config metagpt "Create a 2048 game" # this
-will create a repo in ./workspace ``` or you can use it as library ```python
-from metagpt.software_company import generate_repo, ProjectRepo repo:
-ProjectRepo = generate_repo("Create a 2048 game") # or ProjectRepo("") print
-(repo) # it will print the repo structure with files ``` detail installation
-please refer to [cli_install](https://docs.deepwisdom.ai/main/en/guide/
-get_started/installation.html#install-stable-version) ### Docker installation >
-Note: In the Windows, you need to replace "/opt/metagpt" with a directory that
-Docker has permission to create, such as "D:\Users\x\metagpt" ```bash # Step 1:
-Download metagpt official image and prepare config2.yaml docker pull metagpt/
-metagpt:latest mkdir -p /opt/metagpt/{config,workspace} docker run --rm
-metagpt/metagpt:latest cat /app/metagpt/config/config2.yaml > /opt/metagpt/
-config/config2.yaml vim /opt/metagpt/config/config2.yaml # Change the config #
-Step 2: Run metagpt demo with container docker run --rm \ --privileged \ -v /
-opt/metagpt/config/config2.yaml:/app/metagpt/config/config2.yaml \ -v /opt/
-metagpt/workspace:/app/metagpt/workspace \ metagpt/metagpt:latest \ metagpt
-"Create a 2048 game" ``` detail installation please refer to [docker_install]
-(https://docs.deepwisdom.ai/main/en/guide/get_started/
-installation.html#install-with-docker) ### QuickStart & Demo Video - Try it on
-[MetaGPT Huggingface Space](https://huggingface.co/spaces/deepwisdom/MetaGPT) -
-[Matthew Berman: How To Install MetaGPT - Build A Startup With One Prompt!!]
-(https://youtu.be/uT75J_KG_aY) - [Official Demo Video](https://github.com/
-geekan/MetaGPT/assets/2707039/5e8c1062-8c35-440f-bb20-2b0320f8d27d) https://
+```bash pip install --upgrade metagpt # or `pip install --upgrade git+https://
+github.com/geekan/MetaGPT.git` # or `git clone https://github.com/geekan/
+MetaGPT && cd MetaGPT && pip install --upgrade -e .` ``` For detailed
+installation guidance, please refer to [cli_install](https://
+docs.deepwisdom.ai/main/en/guide/get_started/installation.html#install-stable-
+version) or [docker_install](https://docs.deepwisdom.ai/main/en/guide/
+get_started/installation.html#install-with-docker) ### Configuration You can
+init the config of MetaGPT by running the following command, or manually create
+`~/.metagpt/config2.yaml` file: ```bash # Check https://docs.deepwisdom.ai/
+main/en/guide/get_started/configuration.html for more details metagpt --init-
+config # it will create ~/.metagpt/config2.yaml, just modify it to your needs
+``` You can configure `~/.metagpt/config2.yaml` according to the [example]
+(https://github.com/geekan/MetaGPT/blob/main/config/config2.example.yaml) and
+[doc](https://docs.deepwisdom.ai/main/en/guide/get_started/configuration.html):
+```yaml llm: api_type: "openai" # or azure / ollama / open_llm etc. Check
+LLMType for more options model: "gpt-4-turbo-preview" # or gpt-3.5-turbo-1106 /
+gpt-4-1106-preview base_url: "https://api.openai.com/v1" # or forward url /
+other llm url api_key: "YOUR_API_KEY" ``` ### Usage After installation, you can
+use MetaGPT at CLI ```bash metagpt "Create a 2048 game" # this will create a
+repo in ./workspace ``` or use it as library ```python from
+metagpt.software_company import generate_repo, ProjectRepo repo: ProjectRepo =
+generate_repo("Create a 2048 game") # or ProjectRepo("") print(repo) # it will
+print the repo structure with files ``` You can also use its [Data Interpreter]
+(https://github.com/geekan/MetaGPT/tree/main/examples/di) ```python import
+asyncio from metagpt.roles.di.data_interpreter import DataInterpreter async def
+main(): di = DataInterpreter() await di.run("Run data analysis on sklearn Iris
+dataset, include a plot") asyncio.run(main()) # or await main() in a jupyter
+notebook setting ``` ### QuickStart & Demo Video - Try it on [MetaGPT
+Huggingface Space](https://huggingface.co/spaces/deepwisdom/MetaGPT) - [Matthew
+Berman: How To Install MetaGPT - Build A Startup With One Prompt!!](https://
+youtu.be/uT75J_KG_aY) - [Official Demo Video](https://github.com/geekan/
+MetaGPT/assets/2707039/5e8c1062-8c35-440f-bb20-2b0320f8d27d) https://
 github.com/geekan/MetaGPT/assets/34952977/34345016-5d13-489d-b9f9-b82ace413419
 ## Tutorial - ð [Online Document](https://docs.deepwisdom.ai/main/en/) -
 ð» [Usage](https://docs.deepwisdom.ai/main/en/guide/get_started/
 quickstart.html) - ð [What can MetaGPT do?](https://docs.deepwisdom.ai/main/
 en/guide/get_started/introduction.html) - ð  How to build your own agents? -
 [MetaGPT Usage & Development Guide | Agent 101](https://docs.deepwisdom.ai/
 main/en/guide/tutorials/agent_101.html) - [MetaGPT Usage & Development Guide |
 MultiAgent 101](https://docs.deepwisdom.ai/main/en/guide/tutorials/
 multi_agent_101.html) - ð§âð» Contribution - [Develop Roadmap](docs/
-ROADMAP.md) - ð Use Cases - [Debate](https://docs.deepwisdom.ai/main/en/
-guide/use_cases/multi_agent/debate.html) - [Researcher](https://
-docs.deepwisdom.ai/main/en/guide/use_cases/agent/researcher.html) - [Recepit
-Assistant](https://docs.deepwisdom.ai/main/en/guide/use_cases/agent/
-receipt_assistant.html) - â [FAQs](https://docs.deepwisdom.ai/main/en/guide/
-faq.html) ## Support ### Discard Join US ð¢ Join Our [Discord Channel](https:
-//discord.gg/ZRHeExS6xv)! Looking forward to seeing you there! ð ### Contact
-Information If you have any questions or feedback about this project, please
-feel free to contact us. We highly appreciate your suggestions! - **Email:**
-alexanderwu@deepwisdom.ai - **GitHub Issues:** For more technical inquiries,
-you can also create a new issue in our [GitHub repository](https://github.com/
-geekan/metagpt/issues). We will respond to all questions within 2-3 business
-days. ## Citation For now, cite the [arXiv paper](https://arxiv.org/abs/
-2308.00352): ```bibtex @misc{hong2023metagpt, title={MetaGPT: Meta Programming
-for A Multi-Agent Collaborative Framework}, author={Sirui Hong and Mingchen
-Zhuge and Jonathan Chen and Xiawu Zheng and Yuheng Cheng and Ceyao Zhang and
-Jinlin Wang and Zili Wang and Steven Ka Shing Yau and Zijuan Lin and Liyang
-Zhou and Chenyu Ran and Lingfeng Xiao and Chenglin Wu and JÃ¼rgen Schmidhuber},
-year={2023}, eprint={2308.00352}, archivePrefix={arXiv}, primaryClass={cs.AI} }
-```
+ROADMAP.md) - ð Use Cases - [Data Interpreter](https://docs.deepwisdom.ai/
+main/en/guide/use_cases/agent/interpreter/intro.html) - [Debate](https://
+docs.deepwisdom.ai/main/en/guide/use_cases/multi_agent/debate.html) -
+[Researcher](https://docs.deepwisdom.ai/main/en/guide/use_cases/agent/
+researcher.html) - [Recepit Assistant](https://docs.deepwisdom.ai/main/en/
+guide/use_cases/agent/receipt_assistant.html) - â [FAQs](https://
+docs.deepwisdom.ai/main/en/guide/faq.html) ## Support ### Discard Join US ð¢
+Join Our [Discord Channel](https://discord.gg/ZRHeExS6xv)! Looking forward to
+seeing you there! ð ### Contact Information If you have any questions or
+feedback about this project, please feel free to contact us. We highly
+appreciate your suggestions! - **Email:** alexanderwu@deepwisdom.ai - **GitHub
+Issues:** For more technical inquiries, you can also create a new issue in our
+[GitHub repository](https://github.com/geekan/metagpt/issues). We will respond
+to all questions within 2-3 business days. ## Citation To stay updated with the
+latest research and development, follow [@MetaGPT_](https://twitter.com/
+MetaGPT_) on Twitter. To cite [MetaGPT](https://arxiv.org/abs/2308.00352) or
+[Data Interpreter](https://arxiv.org/abs/2402.18679) in publications, please
+use the following BibTeX entries. ```bibtex @misc{hong2023metagpt, title=
+{MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework}, author=
+{Sirui Hong and Mingchen Zhuge and Jonathan Chen and Xiawu Zheng and Yuheng
+Cheng and Ceyao Zhang and Jinlin Wang and Zili Wang and Steven Ka Shing Yau and
+Zijuan Lin and Liyang Zhou and Chenyu Ran and Lingfeng Xiao and Chenglin Wu and
+JÃ¼rgen Schmidhuber}, year={2023}, eprint={2308.00352}, archivePrefix={arXiv},
+primaryClass={cs.AI} } @misc{hong2024data, title={Data Interpreter: An LLM
+Agent For Data Science}, author={Sirui Hong and Yizhang Lin and Bang Liu and
+Bangbang Liu and Binhao Wu and Danyang Li and Jiaqi Chen and Jiayi Zhang and
+Jinlin Wang and Li Zhang and Lingyao Zhang and Min Yang and Mingchen Zhuge and
+Taicheng Guo and Tuo Zhou and Wei Tao and Wenyi Wang and Xiangru Tang and
+Xiangtao Lu and Xiawu Zheng and Xinbing Liang and Yaying Fei and Yuheng Cheng
+and Zongze Xu and Chenglin Wu}, year={2024}, eprint={2402.18679},
+archivePrefix={arXiv}, primaryClass={cs.AI} } ```
```

### Comparing `metagpt-0.7.7/setup.py` & `metagpt-0.8.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,45 +23,55 @@
 requirements = (here / "requirements.txt").read_text(encoding="utf-8").splitlines()
 
 
 extras_require = {
     "selenium": ["selenium>4", "webdriver_manager", "beautifulsoup4"],
     "search-google": ["google-api-python-client==2.94.0"],
     "search-ddg": ["duckduckgo-search~=4.1.1"],
-    "ocr": ["paddlepaddle==2.4.2", "paddleocr>=2.0.1", "tabulate==0.9.0"],
+    "ocr": ["paddlepaddle==2.4.2", "paddleocr~=2.7.3", "tabulate==0.9.0"],
+    "rag": [
+        "llama-index-core==0.10.15",
+        "llama-index-embeddings-azure-openai==0.1.6",
+        "llama-index-embeddings-openai==0.1.5",
+        "llama-index-llms-azure-openai==0.1.4",
+        "llama-index-readers-file==0.1.4",
+        "llama-index-retrievers-bm25==0.1.3",
+        "llama-index-vector-stores-faiss==0.1.1",
+        "llama-index-vector-stores-elasticsearch==0.1.6",
+        "llama-index-vector-stores-chroma==0.1.6",
+    ],
 }
 
 extras_require["test"] = [
     *set(i for j in extras_require.values() for i in j),
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
     "pytest-mock",
     "pytest-html",
     "pytest-xdist",
     "pytest-timeout",
     "connexion[uvicorn]~=3.0.5",
     "azure-cognitiveservices-speech~=1.31.0",
     "aioboto3~=11.3.0",
-    "chromadb==0.4.14",
     "gradio==3.0.0",
     "grpcio-status==1.48.2",
     "pylint==3.0.3",
     "pybrowsers",
 ]
 
 extras_require["pyppeteer"] = [
     "pyppeteer>=1.0.2"
 ]  # pyppeteer is unmaintained and there are conflicts with dependencies
 extras_require["dev"] = (["pylint~=3.0.3", "black~=23.3.0", "isort~=5.12.0", "pre-commit~=3.6.0"],)
 
 
 setup(
     name="metagpt",
-    version="0.7.7",
+    version="0.8.0",
     description="The Multi-Agent Framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/geekan/MetaGPT",
     author="Alexander Wu",
     author_email="alexanderwu@deepwisdom.ai",
     license="MIT",
```

