# Comparing `tmp/swarms-4.7.1.tar.gz` & `tmp/swarms-4.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-4.7.1.tar", max compression
+gzip compressed data, was "swarms-4.7.3.tar", max compression
```

## Comparing `swarms-4.7.1.tar` & `swarms-4.7.3.tar`

### file list

```diff
@@ -1,250 +1,247 @@
--rw-r--r--   0        0        0    15674 2024-03-27 19:29:36.857220 swarms-4.7.1/LICENSE
--rw-r--r--   0        0        0    33330 2024-03-30 07:41:47.541395 swarms-4.7.1/README.md
--rw-r--r--   0        0        0     1670 2024-04-02 02:12:15.451445 swarms-4.7.1/pyproject.toml
--rw-r--r--   0        0        0      638 2024-03-27 19:58:17.440677 swarms-4.7.1/swarms/__init__.py
--rw-r--r--   0        0        0     6148 2024-03-15 22:19:20.999687 swarms-4.7.1/swarms/agents/.DS_Store
--rw-r--r--   0        0        0      864 2024-03-15 22:19:21.000202 swarms-4.7.1/swarms/agents/__init__.py
--rw-r--r--   0        0        0      881 2024-03-15 22:19:21.001107 swarms-4.7.1/swarms/agents/agent_wrapper.py
--rw-r--r--   0        0        0     3342 2024-03-21 23:46:38.264917 swarms-4.7.1/swarms/agents/base.py
--rw-r--r--   0        0        0     4201 2024-03-15 22:19:21.002271 swarms-4.7.1/swarms/agents/developer_agents.py
--rw-r--r--   0        0        0     2950 2024-03-27 19:12:09.754781 swarms-4.7.1/swarms/agents/omni_modal_agent.py
--rw-r--r--   0        0        0     3503 2024-03-15 22:19:21.004191 swarms-4.7.1/swarms/agents/simple_agent.py
--rw-r--r--   0        0        0      484 2024-03-15 22:19:21.004680 swarms-4.7.1/swarms/agents/stopping_conditions.py
--rw-r--r--   0        0        0     4971 2024-03-24 05:09:57.079682 swarms-4.7.1/swarms/agents/tool_agent.py
--rw-r--r--   0        0        0     5634 2024-03-27 19:12:09.755579 swarms-4.7.1/swarms/agents/worker_agent.py
--rw-r--r--   0        0        0      167 2024-03-15 22:19:21.006869 swarms-4.7.1/swarms/artifacts/__init__.py
--rw-r--r--   0        0        0     1675 2024-03-15 22:19:21.007269 swarms-4.7.1/swarms/artifacts/base_artifact.py
--rw-r--r--   0        0        0     2299 2024-03-27 19:27:30.716559 swarms-4.7.1/swarms/artifacts/text_artifact.py
--rw-r--r--   0        0        0        0 2024-03-15 22:19:21.010058 swarms-4.7.1/swarms/cli/__init__.py
--rw-r--r--   0        0        0     1384 2024-03-15 22:19:21.010779 swarms-4.7.1/swarms/cli/_cli.py
--rw-r--r--   0        0        0      332 2024-03-15 22:19:21.011154 swarms-4.7.1/swarms/cli/run_file.py
--rw-r--r--   0        0        0      621 2024-03-27 19:12:09.649116 swarms-4.7.1/swarms/memory/__init__.py
--rw-r--r--   0        0        0      433 2024-03-15 22:19:21.012591 swarms-4.7.1/swarms/memory/action_subtask.py
--rw-r--r--   0        0        0     3475 2024-03-15 22:19:21.012989 swarms-4.7.1/swarms/memory/base_db.py
--rw-r--r--   0        0        0     2827 2024-03-24 05:47:02.683694 swarms-4.7.1/swarms/memory/base_vectordb.py
--rw-r--r--   0        0        0     5867 2024-03-27 19:12:09.756589 swarms-4.7.1/swarms/memory/chroma_db.py
--rw-r--r--   0        0        0     2770 2024-03-15 22:19:21.014207 swarms-4.7.1/swarms/memory/cosine_similarity.py
--rw-r--r--   0        0        0     2895 2024-03-15 22:19:21.014370 swarms-4.7.1/swarms/memory/dict_internal_memory.py
--rw-r--r--   0        0        0     3336 2024-03-15 22:19:21.014516 swarms-4.7.1/swarms/memory/dict_shared_memory.py
--rw-r--r--   0        0        0     6125 2024-03-27 19:12:09.757820 swarms-4.7.1/swarms/memory/lanchain_chroma.py
--rw-r--r--   0        0        0     4497 2024-03-27 19:12:09.758770 swarms-4.7.1/swarms/memory/pg.py
--rw-r--r--   0        0        0     7651 2024-03-15 22:19:21.015872 swarms-4.7.1/swarms/memory/pinecone.py
--rw-r--r--   0        0        0     5738 2024-03-27 19:12:09.759612 swarms-4.7.1/swarms/memory/qdrant.py
--rw-r--r--   0        0        0     5603 2024-03-15 22:19:21.016770 swarms-4.7.1/swarms/memory/short_term_memory.py
--rw-r--r--   0        0        0     3841 2024-03-15 22:19:21.017420 swarms-4.7.1/swarms/memory/sqlite.py
--rw-r--r--   0        0        0     2936 2024-03-15 22:19:21.018457 swarms-4.7.1/swarms/memory/utils.py
--rw-r--r--   0        0        0     3371 2024-03-15 22:19:21.018970 swarms-4.7.1/swarms/memory/visual_memory.py
--rw-r--r--   0        0        0     6135 2024-03-15 22:19:21.019639 swarms-4.7.1/swarms/memory/weaviate_db.py
--rw-r--r--   0        0        0     2517 2024-04-02 02:11:29.866899 swarms-4.7.1/swarms/models/__init__.py
--rw-r--r--   0        0        0     2074 2024-03-27 19:58:17.874104 swarms-4.7.1/swarms/models/base_embedding_model.py
--rw-r--r--   0        0        0    13240 2024-03-15 22:19:21.021853 swarms-4.7.1/swarms/models/base_llm.py
--rw-r--r--   0        0        0    12728 2024-03-15 22:19:21.022342 swarms-4.7.1/swarms/models/base_multimodal_model.py
--rw-r--r--   0        0        0     2487 2024-03-15 22:19:21.023152 swarms-4.7.1/swarms/models/base_tts.py
--rw-r--r--   0        0        0     3171 2024-03-15 22:19:21.023526 swarms-4.7.1/swarms/models/base_ttv.py
--rw-r--r--   0        0        0    16953 2024-03-15 22:19:21.027265 swarms-4.7.1/swarms/models/cog_vlm.py
--rw-r--r--   0        0        0    10864 2024-03-15 22:19:21.028441 swarms-4.7.1/swarms/models/dalle3.py
--rw-r--r--   0        0        0     6643 2024-03-15 22:19:21.029941 swarms-4.7.1/swarms/models/distilled_whisperx.py
--rw-r--r--   0        0        0      682 2024-03-15 22:19:21.031788 swarms-4.7.1/swarms/models/embeddings_base.py
--rw-r--r--   0        0        0     2734 2024-03-15 22:19:21.032242 swarms-4.7.1/swarms/models/fire_function.py
--rw-r--r--   0        0        0     3022 2024-03-15 22:19:21.032963 swarms-4.7.1/swarms/models/fuyu.py
--rw-r--r--   0        0        0     7814 2024-03-15 22:19:21.033722 swarms-4.7.1/swarms/models/gemini.py
--rw-r--r--   0        0        0     2818 2024-03-15 22:19:21.034812 swarms-4.7.1/swarms/models/gpt4_sam.py
--rw-r--r--   0        0        0    14282 2024-03-15 22:19:21.035054 swarms-4.7.1/swarms/models/gpt4_vision_api.py
--rw-r--r--   0        0        0    13034 2024-03-15 22:19:21.035781 swarms-4.7.1/swarms/models/huggingface.py
--rw-r--r--   0        0        0     1968 2024-03-15 22:19:21.036059 swarms-4.7.1/swarms/models/huggingface_pipeline.py
--rw-r--r--   0        0        0     5623 2024-03-15 22:19:21.036228 swarms-4.7.1/swarms/models/idefics.py
--rw-r--r--   0        0        0     7996 2024-03-15 22:19:21.036860 swarms-4.7.1/swarms/models/jina_embeds.py
--rw-r--r--   0        0        0    10752 2024-04-02 02:09:16.602464 swarms-4.7.1/swarms/models/kosmos_two.py
--rw-r--r--   0        0        0     1448 2024-03-15 22:19:21.037679 swarms-4.7.1/swarms/models/layoutlm_document_qa.py
--rw-r--r--   0        0        0     6529 2024-03-15 22:19:21.038086 swarms-4.7.1/swarms/models/llama_function_caller.py
--rw-r--r--   0        0        0     2762 2024-03-15 22:19:21.038340 swarms-4.7.1/swarms/models/llava.py
--rw-r--r--   0        0        0     4597 2024-03-15 22:19:21.038513 swarms-4.7.1/swarms/models/medical_sam.py
--rw-r--r--   0        0        0     4324 2024-03-15 22:19:21.038800 swarms-4.7.1/swarms/models/mistral.py
--rw-r--r--   0        0        0      244 2024-03-24 04:08:38.359236 swarms-4.7.1/swarms/models/mistral_model_api.py
--rw-r--r--   0        0        0     2155 2024-03-15 22:19:21.039343 swarms-4.7.1/swarms/models/mixtral.py
--rw-r--r--   0        0        0     2056 2024-03-15 22:19:21.041522 swarms-4.7.1/swarms/models/moondream_mm.py
--rw-r--r--   0        0        0     6470 2024-03-15 22:19:21.041916 swarms-4.7.1/swarms/models/mpt.py
--rw-r--r--   0        0        0     2823 2024-03-15 22:19:21.042535 swarms-4.7.1/swarms/models/nougat.py
--rw-r--r--   0        0        0     2366 2024-03-15 22:19:21.043550 swarms-4.7.1/swarms/models/open_dalle.py
--rw-r--r--   0        0        0    20443 2024-03-21 23:46:38.329902 swarms-4.7.1/swarms/models/openai_embeddings.py
--rw-r--r--   0        0        0     3175 2024-03-15 22:19:21.045986 swarms-4.7.1/swarms/models/openai_tts.py
--rw-r--r--   0        0        0     6133 2024-03-21 23:46:38.330900 swarms-4.7.1/swarms/models/palm.py
--rw-r--r--   0        0        0     1101 2024-03-21 23:46:38.332006 swarms-4.7.1/swarms/models/popular_llms.py
--rw-r--r--   0        0        0     4843 2024-03-15 22:19:21.048155 swarms-4.7.1/swarms/models/qwen.py
--rw-r--r--   0        0        0     3547 2024-03-15 22:19:21.049332 swarms-4.7.1/swarms/models/sam.py
--rw-r--r--   0        0        0    12871 2024-03-15 22:19:21.050598 swarms-4.7.1/swarms/models/sampling_params.py
--rw-r--r--   0        0        0     7709 2024-03-15 22:19:21.050811 swarms-4.7.1/swarms/models/speecht5.py
--rw-r--r--   0        0        0     8318 2024-03-21 23:46:38.332831 swarms-4.7.1/swarms/models/ssd_1b.py
--rw-r--r--   0        0        0     5189 2024-03-15 22:19:21.051613 swarms-4.7.1/swarms/models/stable_diffusion.py
--rw-r--r--   0        0        0     1794 2024-03-15 22:19:21.052816 swarms-4.7.1/swarms/models/timm.py
--rw-r--r--   0        0        0     3990 2024-03-23 22:42:41.705709 swarms-4.7.1/swarms/models/together.py
--rw-r--r--   0        0        0      148 2024-03-15 22:19:21.053560 swarms-4.7.1/swarms/models/trocr.py
--rw-r--r--   0        0        0      592 2024-03-15 22:19:21.054281 swarms-4.7.1/swarms/models/types.py
--rw-r--r--   0        0        0     1499 2024-03-15 22:19:21.054547 swarms-4.7.1/swarms/models/ultralytics_model.py
--rw-r--r--   0        0        0     1731 2024-03-15 22:19:21.054977 swarms-4.7.1/swarms/models/vilt.py
--rw-r--r--   0        0        0     2846 2024-03-15 22:19:21.055732 swarms-4.7.1/swarms/models/vip_llava.py
--rw-r--r--   0        0        0     7678 2024-03-15 22:19:21.056747 swarms-4.7.1/swarms/models/wizard_storytelling.py
--rw-r--r--   0        0        0     9576 2024-03-15 22:19:21.057712 swarms-4.7.1/swarms/models/yarn_mistral.py
--rw-r--r--   0        0        0     2943 2024-03-15 22:19:21.058472 swarms-4.7.1/swarms/models/yi_200k.py
--rw-r--r--   0        0        0     3681 2024-03-15 22:19:21.059936 swarms-4.7.1/swarms/models/zeroscope.py
--rw-r--r--   0        0        0      775 2024-03-15 22:19:21.060753 swarms-4.7.1/swarms/prompts/__init__.py
--rw-r--r--   0        0        0    11320 2024-03-15 22:19:21.061563 swarms-4.7.1/swarms/prompts/accountant_swarm_prompts.py
--rw-r--r--   0        0        0     9156 2024-03-15 22:19:21.062133 swarms-4.7.1/swarms/prompts/aga.py
--rw-r--r--   0        0        0     1451 2024-03-15 22:19:21.062911 swarms-4.7.1/swarms/prompts/agent_output_parser.py
--rw-r--r--   0        0        0     2705 2024-03-15 22:19:21.063538 swarms-4.7.1/swarms/prompts/agent_prompt.py
--rw-r--r--   0        0        0     6886 2024-03-15 22:19:21.064160 swarms-4.7.1/swarms/prompts/agent_prompts.py
--rw-r--r--   0        0        0     7145 2024-03-15 22:19:21.065128 swarms-4.7.1/swarms/prompts/agent_system_prompts.py
--rw-r--r--   0        0        0     5233 2024-03-15 22:19:21.065787 swarms-4.7.1/swarms/prompts/ai_research_team.py
--rw-r--r--   0        0        0    13981 2024-03-15 22:19:21.066513 swarms-4.7.1/swarms/prompts/autobloggen.py
--rw-r--r--   0        0        0     5605 2024-03-15 22:19:21.068224 swarms-4.7.1/swarms/prompts/autoswarm.py
--rw-r--r--   0        0        0     7542 2024-03-15 22:19:21.068567 swarms-4.7.1/swarms/prompts/base.py
--rw-r--r--   0        0        0     3801 2024-03-15 22:19:21.068894 swarms-4.7.1/swarms/prompts/chat_prompt.py
--rw-r--r--   0        0        0     2235 2024-03-15 22:19:21.069096 swarms-4.7.1/swarms/prompts/code_interpreter.py
--rw-r--r--   0        0        0     4106 2024-03-15 22:19:21.069652 swarms-4.7.1/swarms/prompts/code_spawner.py
--rw-r--r--   0        0        0     1566 2024-03-15 22:19:21.069820 swarms-4.7.1/swarms/prompts/debate.py
--rw-r--r--   0        0        0     7044 2024-03-15 22:19:21.070670 swarms-4.7.1/swarms/prompts/documentation.py
--rw-r--r--   0        0        0     1767 2024-03-15 22:19:21.071442 swarms-4.7.1/swarms/prompts/education.py
--rw-r--r--   0        0        0     4180 2024-03-15 22:19:21.071791 swarms-4.7.1/swarms/prompts/finance_agent_prompt.py
--rw-r--r--   0        0        0     4117 2024-03-15 22:19:21.072144 swarms-4.7.1/swarms/prompts/growth_agent_prompt.py
--rw-r--r--   0        0        0      880 2024-03-15 22:19:21.072694 swarms-4.7.1/swarms/prompts/idea2img.py
--rw-r--r--   0        0        0     3346 2024-03-15 22:19:21.072990 swarms-4.7.1/swarms/prompts/legal_agent_prompt.py
--rw-r--r--   0        0        0     4785 2024-03-15 22:19:21.073912 swarms-4.7.1/swarms/prompts/logistics.py
--rw-r--r--   0        0        0    10662 2024-03-15 22:19:21.074621 swarms-4.7.1/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
--rw-r--r--   0        0        0     3511 2024-03-15 22:19:21.075295 swarms-4.7.1/swarms/prompts/multi_modal_prompts.py
--rw-r--r--   0        0        0     3225 2024-03-15 22:19:21.075646 swarms-4.7.1/swarms/prompts/multi_modal_visual_prompts.py
--rw-r--r--   0        0        0     3454 2024-03-15 22:19:21.076012 swarms-4.7.1/swarms/prompts/operations_agent_prompt.py
--rw-r--r--   0        0        0        0 2024-03-15 22:19:21.076143 swarms-4.7.1/swarms/prompts/orchestrator_prompt.py
--rw-r--r--   0        0        0     2149 2024-03-15 22:19:21.076733 swarms-4.7.1/swarms/prompts/personal_stylist.py
--rw-r--r--   0        0        0     8333 2024-03-15 22:19:21.077280 swarms-4.7.1/swarms/prompts/product_agent_prompt.py
--rw-r--r--   0        0        0    10144 2024-03-15 22:19:21.078026 swarms-4.7.1/swarms/prompts/programming.py
--rw-r--r--   0        0        0     2128 2024-03-15 22:19:21.078275 swarms-4.7.1/swarms/prompts/project_manager.py
--rw-r--r--   0        0        0    13215 2024-03-15 22:19:21.078885 swarms-4.7.1/swarms/prompts/python.py
--rw-r--r--   0        0        0     2960 2024-03-15 22:19:21.079805 swarms-4.7.1/swarms/prompts/react.py
--rw-r--r--   0        0        0        0 2024-03-15 22:19:21.080059 swarms-4.7.1/swarms/prompts/refiner_agent_prompt.py
--rw-r--r--   0        0        0     5126 2024-03-15 22:19:21.080659 swarms-4.7.1/swarms/prompts/sales.py
--rw-r--r--   0        0        0     5013 2024-03-15 22:19:21.081280 swarms-4.7.1/swarms/prompts/sales_prompts.py
--rw-r--r--   0        0        0     7573 2024-03-15 22:19:21.082529 swarms-4.7.1/swarms/prompts/schema_generator.py
--rw-r--r--   0        0        0     2679 2024-03-15 22:19:21.083072 swarms-4.7.1/swarms/prompts/security_team.py
--rw-r--r--   0        0        0     3264 2024-03-15 22:19:21.083517 swarms-4.7.1/swarms/prompts/self_operating_prompt.py
--rw-r--r--   0        0        0     4147 2024-03-15 22:19:21.084066 swarms-4.7.1/swarms/prompts/sop_generator_agent_prompt.py
--rw-r--r--   0        0        0     4640 2024-03-15 22:19:21.084386 swarms-4.7.1/swarms/prompts/summaries_prompts.py
--rw-r--r--   0        0        0     3984 2024-03-15 22:19:21.084631 swarms-4.7.1/swarms/prompts/support_agent_prompt.py
--rw-r--r--   0        0        0     4280 2024-03-15 22:19:21.085244 swarms-4.7.1/swarms/prompts/swarm_manager_agent.py
--rw-r--r--   0        0        0      728 2024-03-15 22:19:21.085725 swarms-4.7.1/swarms/prompts/task_assignment_prompt.py
--rw-r--r--   0        0        0     4271 2024-03-15 22:19:21.086266 swarms-4.7.1/swarms/prompts/tests.py
--rw-r--r--   0        0        0     4288 2024-03-15 22:19:21.086625 swarms-4.7.1/swarms/prompts/tools.py
--rw-r--r--   0        0        0     2398 2024-03-15 22:19:21.087352 swarms-4.7.1/swarms/prompts/urban_planning.py
--rw-r--r--   0        0        0     3675 2024-03-15 22:19:21.087654 swarms-4.7.1/swarms/prompts/visual_cot.py
--rw-r--r--   0        0        0     2792 2024-03-21 23:46:38.334043 swarms-4.7.1/swarms/prompts/worker_prompt.py
--rw-r--r--   0        0        0     2349 2024-03-15 22:19:21.088382 swarms-4.7.1/swarms/prompts/xray_swarm_prompt.py
--rw-r--r--   0        0        0     3785 2024-03-27 19:58:17.513026 swarms-4.7.1/swarms/structs/__init__.py
--rw-r--r--   0        0        0    47441 2024-03-30 18:48:29.907000 swarms-4.7.1/swarms/structs/agent.py
--rw-r--r--   0        0        0      574 2024-03-15 22:19:21.092491 swarms-4.7.1/swarms/structs/agent_job.py
--rw-r--r--   0        0        0     2923 2024-03-27 19:58:17.509429 swarms-4.7.1/swarms/structs/agent_process.py
--rw-r--r--   0        0        0     3732 2024-03-15 22:19:21.092747 swarms-4.7.1/swarms/structs/async_workflow.py
--rw-r--r--   0        0        0     7951 2024-03-27 19:47:31.068918 swarms-4.7.1/swarms/structs/auto_swarm.py
--rw-r--r--   0        0        0    11735 2024-03-15 22:19:21.093292 swarms-4.7.1/swarms/structs/autoscaler.py
--rw-r--r--   0        0        0    12262 2024-03-15 22:19:21.093668 swarms-4.7.1/swarms/structs/base.py
--rw-r--r--   0        0        0    19105 2024-03-30 07:40:24.964542 swarms-4.7.1/swarms/structs/base_swarm.py
--rw-r--r--   0        0        0    12486 2024-03-27 19:12:09.737934 swarms-4.7.1/swarms/structs/base_workflow.py
--rw-r--r--   0        0        0     1056 2024-03-15 22:19:21.095125 swarms-4.7.1/swarms/structs/block_wrapper.py
--rw-r--r--   0        0        0      629 2024-03-15 22:19:21.095875 swarms-4.7.1/swarms/structs/blockdevice.py
--rw-r--r--   0        0        0     3178 2024-03-15 22:19:21.096348 swarms-4.7.1/swarms/structs/blocksdict.py
--rw-r--r--   0        0        0     4887 2024-03-15 22:19:21.096911 swarms-4.7.1/swarms/structs/blockslist.py
--rw-r--r--   0        0        0     5364 2024-03-15 22:19:21.097555 swarms-4.7.1/swarms/structs/company.py
--rw-r--r--   0        0        0     4515 2024-03-15 22:19:21.097858 swarms-4.7.1/swarms/structs/concurrent_workflow.py
--rw-r--r--   0        0        0    14023 2024-03-27 19:26:23.824143 swarms-4.7.1/swarms/structs/conversation.py
--rw-r--r--   0        0        0    12615 2024-03-15 22:19:21.099092 swarms-4.7.1/swarms/structs/debate.py
--rw-r--r--   0        0        0     3041 2024-03-15 22:19:21.099360 swarms-4.7.1/swarms/structs/document.py
--rw-r--r--   0        0        0     5433 2024-03-15 22:19:21.099780 swarms-4.7.1/swarms/structs/graph_workflow.py
--rw-r--r--   0        0        0     5066 2024-03-15 22:19:21.100307 swarms-4.7.1/swarms/structs/groupchat.py
--rw-r--r--   0        0        0     1951 2024-03-15 22:19:21.100923 swarms-4.7.1/swarms/structs/load_balancer.py
--rw-r--r--   0        0        0     4545 2024-03-15 22:19:21.101122 swarms-4.7.1/swarms/structs/long_swarm.py
--rw-r--r--   0        0        0     7072 2024-03-15 22:19:21.101824 swarms-4.7.1/swarms/structs/majority_voting.py
--rw-r--r--   0        0        0      582 2024-03-15 22:19:21.101971 swarms-4.7.1/swarms/structs/message.py
--rw-r--r--   0        0        0     7384 2024-03-15 22:19:21.102439 swarms-4.7.1/swarms/structs/message_pool.py
--rw-r--r--   0        0        0     5771 2024-03-15 22:19:21.102829 swarms-4.7.1/swarms/structs/model_parallizer.py
--rw-r--r--   0        0        0    10524 2024-03-26 17:51:23.615677 swarms-4.7.1/swarms/structs/multi_agent_collab.py
--rw-r--r--   0        0        0     5623 2024-03-15 22:19:21.103669 swarms-4.7.1/swarms/structs/multi_process_workflow.py
--rw-r--r--   0        0        0     5386 2024-03-15 22:19:21.103964 swarms-4.7.1/swarms/structs/multi_threaded_workflow.py
--rw-r--r--   0        0        0     2883 2024-03-15 22:19:21.104315 swarms-4.7.1/swarms/structs/nonlinear_workflow.py
--rw-r--r--   0        0        0      364 2024-03-26 04:56:18.014859 swarms-4.7.1/swarms/structs/omni_agent_types.py
--rw-r--r--   0        0        0      778 2024-03-15 22:19:21.104929 swarms-4.7.1/swarms/structs/plan.py
--rw-r--r--   0        0        0     5466 2024-03-30 18:05:25.777384 swarms-4.7.1/swarms/structs/rearrange.py
--rw-r--r--   0        0        0     2813 2024-03-27 19:12:09.704075 swarms-4.7.1/swarms/structs/recursive_workflow.py
--rw-r--r--   0        0        0     4182 2024-03-21 23:46:38.336523 swarms-4.7.1/swarms/structs/schemas.py
--rw-r--r--   0        0        0     8094 2024-03-15 22:19:21.106433 swarms-4.7.1/swarms/structs/sequential_workflow.py
--rw-r--r--   0        0        0     2337 2024-03-27 19:47:31.068657 swarms-4.7.1/swarms/structs/sermon_swarm.py
--rw-r--r--   0        0        0     2894 2024-04-02 02:08:38.776074 swarms-4.7.1/swarms/structs/stackoverflow_swarm.py
--rw-r--r--   0        0        0      704 2024-03-27 19:12:09.672624 swarms-4.7.1/swarms/structs/step.py
--rw-r--r--   0        0        0    10756 2024-03-27 19:12:09.673443 swarms-4.7.1/swarms/structs/swarm_net.py
--rw-r--r--   0        0        0     5182 2024-03-27 19:47:31.068788 swarms-4.7.1/swarms/structs/swarm_redis_registry.py
--rw-r--r--   0        0        0     6470 2024-03-15 22:19:21.109619 swarms-4.7.1/swarms/structs/swarming_architectures.py
--rw-r--r--   0        0        0     8311 2024-03-15 22:19:21.109964 swarms-4.7.1/swarms/structs/task.py
--rw-r--r--   0        0        0     1989 2024-03-27 19:12:09.705030 swarms-4.7.1/swarms/structs/task_queue_base.py
--rw-r--r--   0        0        0     3427 2024-03-15 22:19:21.111077 swarms-4.7.1/swarms/structs/team.py
--rw-r--r--   0        0        0     3545 2024-03-15 22:19:21.112074 swarms-4.7.1/swarms/structs/utils.py
--rw-r--r--   0        0        0      891 2024-03-27 19:12:09.674045 swarms-4.7.1/swarms/telemetry/__init__.py
--rw-r--r--   0        0        0      513 2024-03-27 19:12:09.674581 swarms-4.7.1/swarms/telemetry/auto_upgrade_swarms.py
--rw-r--r--   0        0        0      335 2024-03-15 22:19:21.113472 swarms-4.7.1/swarms/telemetry/bootup.py
--rw-r--r--   0        0        0     1087 2024-03-15 22:19:21.113750 swarms-4.7.1/swarms/telemetry/check_update.py
--rw-r--r--   0        0        0      807 2024-03-15 22:19:21.114471 swarms-4.7.1/swarms/telemetry/log_all.py
--rw-r--r--   0        0        0      496 2024-03-22 00:42:19.696403 swarms-4.7.1/swarms/telemetry/sentry_active.py
--rw-r--r--   0        0        0     2729 2024-03-15 22:19:21.115547 swarms-4.7.1/swarms/telemetry/sys_info.py
--rw-r--r--   0        0        0     1996 2024-03-27 19:12:09.675144 swarms-4.7.1/swarms/telemetry/user_utils.py
--rw-r--r--   0        0        0      805 2024-03-21 23:46:38.337818 swarms-4.7.1/swarms/tools/__init__.py
--rw-r--r--   0        0        0     3038 2024-03-15 22:19:21.119284 swarms-4.7.1/swarms/tools/code_executor.py
--rw-r--r--   0        0        0     3614 2024-03-15 22:19:21.119730 swarms-4.7.1/swarms/tools/exec_tool.py
--rw-r--r--   0        0        0    14523 2024-03-24 05:11:17.316917 swarms-4.7.1/swarms/tools/format_tools.py
--rw-r--r--   0        0        0     2469 2024-03-24 05:13:04.696739 swarms-4.7.1/swarms/tools/logits_processor.py
--rw-r--r--   0        0        0      157 2024-03-24 04:12:12.223834 swarms-4.7.1/swarms/tools/tool.py
--rw-r--r--   0        0        0     6165 2024-03-15 22:19:21.121316 swarms-4.7.1/swarms/tools/tool_utils.py
--rw-r--r--   0        0        0     5466 2024-03-15 22:19:21.122024 swarms-4.7.1/swarms/utils/README.md
--rw-r--r--   0        0        0     2691 2024-03-27 19:41:15.064545 swarms-4.7.1/swarms/utils/__init__.py
--rw-r--r--   0        0        0     3537 2024-03-15 22:19:21.122933 swarms-4.7.1/swarms/utils/apa.py
--rw-r--r--   0        0        0     6071 2024-03-15 22:19:21.123535 swarms-4.7.1/swarms/utils/check_function_result.py
--rw-r--r--   0        0        0     1008 2024-03-15 22:19:21.124143 swarms-4.7.1/swarms/utils/class_args_wrapper.py
--rw-r--r--   0        0        0     6674 2024-03-15 22:19:21.125150 swarms-4.7.1/swarms/utils/code_interpreter.py
--rw-r--r--   0        0        0     1264 2024-03-15 22:19:21.125539 swarms-4.7.1/swarms/utils/concurrent_utils.py
--rw-r--r--   0        0        0      808 2024-03-15 22:19:21.126204 swarms-4.7.1/swarms/utils/csv_and_pandas.py
--rw-r--r--   0        0        0     1887 2024-03-15 22:19:21.126685 swarms-4.7.1/swarms/utils/data_to_text.py
--rw-r--r--   0        0        0     2451 2024-03-15 22:19:21.127334 swarms-4.7.1/swarms/utils/decorators.py
--rw-r--r--   0        0        0     2342 2024-03-15 22:19:21.127636 swarms-4.7.1/swarms/utils/device_checker_cuda.py
--rw-r--r--   0        0        0     1311 2024-03-15 22:19:21.127902 swarms-4.7.1/swarms/utils/disable_logging.py
--rw-r--r--   0        0        0      890 2024-03-15 22:19:21.128555 swarms-4.7.1/swarms/utils/download_img.py
--rw-r--r--   0        0        0      690 2024-03-15 22:19:21.129208 swarms-4.7.1/swarms/utils/download_weights_from_url.py
--rw-r--r--   0        0        0     1127 2024-03-15 22:19:21.129540 swarms-4.7.1/swarms/utils/execute_futures.py
--rw-r--r--   0        0        0     3472 2024-03-15 22:19:21.130035 swarms-4.7.1/swarms/utils/execution_sandbox.py
--rw-r--r--   0        0        0     1113 2024-03-15 22:19:21.130281 swarms-4.7.1/swarms/utils/exponential_backoff.py
--rw-r--r--   0        0        0      854 2024-03-15 22:19:21.130759 swarms-4.7.1/swarms/utils/fetch_init_params.py
--rw-r--r--   0        0        0      500 2024-03-15 22:19:21.131255 swarms-4.7.1/swarms/utils/file_extension_seach.py
--rw-r--r--   0        0        0     3286 2024-03-15 22:19:21.131635 swarms-4.7.1/swarms/utils/file_processing.py
--rw-r--r--   0        0        0      644 2024-03-15 22:19:21.131989 swarms-4.7.1/swarms/utils/find_img_path.py
--rw-r--r--   0        0        0     1411 2024-03-15 22:19:21.132408 swarms-4.7.1/swarms/utils/function_calling_utils.py
--rw-r--r--   0        0        0     4184 2024-03-15 22:19:21.132807 swarms-4.7.1/swarms/utils/get_logger.py
--rw-r--r--   0        0        0      363 2024-03-15 22:19:21.133103 swarms-4.7.1/swarms/utils/hash.py
--rw-r--r--   0        0        0     2228 2024-03-15 22:19:21.133717 swarms-4.7.1/swarms/utils/inference_convert_utils.py
--rw-r--r--   0        0        0     2872 2024-03-15 22:19:21.133992 swarms-4.7.1/swarms/utils/json_output_parser.py
--rw-r--r--   0        0        0     1316 2024-03-21 23:46:38.581600 swarms-4.7.1/swarms/utils/json_utils.py
--rw-r--r--   0        0        0     1837 2024-03-15 22:19:21.134782 swarms-4.7.1/swarms/utils/jsonl_utils.py
--rw-r--r--   0        0        0      932 2024-03-15 22:19:21.135261 swarms-4.7.1/swarms/utils/llm_metrics_decorator.py
--rw-r--r--   0        0        0     1915 2024-03-15 22:19:21.135427 swarms-4.7.1/swarms/utils/load_model_torch.py
--rw-r--r--   0        0        0     2261 2024-03-15 22:19:21.136053 swarms-4.7.1/swarms/utils/logger.py
--rw-r--r--   0        0        0    16348 2024-03-26 17:55:25.494840 swarms-4.7.1/swarms/utils/loggers.py
--rw-r--r--   0        0        0      453 2024-03-27 19:12:09.738695 swarms-4.7.1/swarms/utils/loguru_logger.py
--rw-r--r--   0        0        0     6723 2024-03-27 19:12:09.739420 swarms-4.7.1/swarms/utils/main.py
--rw-r--r--   0        0        0      711 2024-03-27 19:12:09.676603 swarms-4.7.1/swarms/utils/markdown_message.py
--rw-r--r--   0        0        0     1461 2024-03-15 22:19:21.138609 swarms-4.7.1/swarms/utils/math_eval.py
--rw-r--r--   0        0        0     1097 2024-03-15 22:19:21.139027 swarms-4.7.1/swarms/utils/pandas_to_str.py
--rw-r--r--   0        0        0      600 2024-03-15 22:19:21.139501 swarms-4.7.1/swarms/utils/parse_code.py
--rw-r--r--   0        0        0     1199 2024-03-15 22:19:21.140224 swarms-4.7.1/swarms/utils/pdf_to_text.py
--rw-r--r--   0        0        0      778 2024-03-15 22:19:21.140973 swarms-4.7.1/swarms/utils/prep_torch_model_inference.py
--rw-r--r--   0        0        0     1353 2024-03-15 22:19:21.141276 swarms-4.7.1/swarms/utils/remove_json_whitespace.py
--rw-r--r--   0        0        0     1300 2024-03-15 22:19:21.141589 swarms-4.7.1/swarms/utils/save_logs.py
--rw-r--r--   0        0        0     4804 2024-03-21 23:46:38.340334 swarms-4.7.1/swarms/utils/serializable.py
--rw-r--r--   0        0        0     3034 2024-03-15 22:19:21.143281 swarms-4.7.1/swarms/utils/supervision_visualizer.py
--rw-r--r--   0        0        0      245 2024-03-15 22:19:21.144185 swarms-4.7.1/swarms/utils/torch_utils.py
--rw-r--r--   0        0        0     1308 2024-03-15 22:19:21.144686 swarms-4.7.1/swarms/utils/try_except_wrapper.py
--rw-r--r--   0        0        0     2692 2024-03-15 22:19:21.145401 swarms-4.7.1/swarms/utils/yaml_output_parser.py
--rw-r--r--   0        0        0    35842 1970-01-01 00:00:00.000000 swarms-4.7.1/setup.py
--rw-r--r--   0        0        0    34893 1970-01-01 00:00:00.000000 swarms-4.7.1/PKG-INFO
+-rw-r--r--   0        0        0    15674 2024-03-27 19:29:36.857220 swarms-4.7.3/LICENSE
+-rw-r--r--   0        0        0    33330 2024-03-30 07:41:47.541395 swarms-4.7.3/README.md
+-rw-r--r--   0        0        0     1615 2024-04-02 02:27:15.683808 swarms-4.7.3/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-04-02 02:14:02.744354 swarms-4.7.3/swarms/__init__.py
+-rw-r--r--   0        0        0     6148 2024-03-15 22:19:20.999687 swarms-4.7.3/swarms/agents/.DS_Store
+-rw-r--r--   0        0        0      864 2024-03-15 22:19:21.000202 swarms-4.7.3/swarms/agents/__init__.py
+-rw-r--r--   0        0        0      881 2024-03-15 22:19:21.001107 swarms-4.7.3/swarms/agents/agent_wrapper.py
+-rw-r--r--   0        0        0     3342 2024-03-21 23:46:38.264917 swarms-4.7.3/swarms/agents/base.py
+-rw-r--r--   0        0        0     4201 2024-03-15 22:19:21.002271 swarms-4.7.3/swarms/agents/developer_agents.py
+-rw-r--r--   0        0        0     2950 2024-03-27 19:12:09.754781 swarms-4.7.3/swarms/agents/omni_modal_agent.py
+-rw-r--r--   0        0        0     3503 2024-03-15 22:19:21.004191 swarms-4.7.3/swarms/agents/simple_agent.py
+-rw-r--r--   0        0        0      484 2024-03-15 22:19:21.004680 swarms-4.7.3/swarms/agents/stopping_conditions.py
+-rw-r--r--   0        0        0     4971 2024-03-24 05:09:57.079682 swarms-4.7.3/swarms/agents/tool_agent.py
+-rw-r--r--   0        0        0     5634 2024-03-27 19:12:09.755579 swarms-4.7.3/swarms/agents/worker_agent.py
+-rw-r--r--   0        0        0      167 2024-03-15 22:19:21.006869 swarms-4.7.3/swarms/artifacts/__init__.py
+-rw-r--r--   0        0        0     1675 2024-03-15 22:19:21.007269 swarms-4.7.3/swarms/artifacts/base_artifact.py
+-rw-r--r--   0        0        0     2299 2024-03-27 19:27:30.716559 swarms-4.7.3/swarms/artifacts/text_artifact.py
+-rw-r--r--   0        0        0      621 2024-03-27 19:12:09.649116 swarms-4.7.3/swarms/memory/__init__.py
+-rw-r--r--   0        0        0      433 2024-03-15 22:19:21.012591 swarms-4.7.3/swarms/memory/action_subtask.py
+-rw-r--r--   0        0        0     3475 2024-03-15 22:19:21.012989 swarms-4.7.3/swarms/memory/base_db.py
+-rw-r--r--   0        0        0     2827 2024-03-24 05:47:02.683694 swarms-4.7.3/swarms/memory/base_vectordb.py
+-rw-r--r--   0        0        0     5867 2024-03-27 19:12:09.756589 swarms-4.7.3/swarms/memory/chroma_db.py
+-rw-r--r--   0        0        0     2770 2024-03-15 22:19:21.014207 swarms-4.7.3/swarms/memory/cosine_similarity.py
+-rw-r--r--   0        0        0     2895 2024-03-15 22:19:21.014370 swarms-4.7.3/swarms/memory/dict_internal_memory.py
+-rw-r--r--   0        0        0     3336 2024-03-15 22:19:21.014516 swarms-4.7.3/swarms/memory/dict_shared_memory.py
+-rw-r--r--   0        0        0     6125 2024-03-27 19:12:09.757820 swarms-4.7.3/swarms/memory/lanchain_chroma.py
+-rw-r--r--   0        0        0     4497 2024-03-27 19:12:09.758770 swarms-4.7.3/swarms/memory/pg.py
+-rw-r--r--   0        0        0     7651 2024-03-15 22:19:21.015872 swarms-4.7.3/swarms/memory/pinecone.py
+-rw-r--r--   0        0        0     5738 2024-03-27 19:12:09.759612 swarms-4.7.3/swarms/memory/qdrant.py
+-rw-r--r--   0        0        0     5603 2024-03-15 22:19:21.016770 swarms-4.7.3/swarms/memory/short_term_memory.py
+-rw-r--r--   0        0        0     3841 2024-03-15 22:19:21.017420 swarms-4.7.3/swarms/memory/sqlite.py
+-rw-r--r--   0        0        0     2936 2024-03-15 22:19:21.018457 swarms-4.7.3/swarms/memory/utils.py
+-rw-r--r--   0        0        0     3371 2024-03-15 22:19:21.018970 swarms-4.7.3/swarms/memory/visual_memory.py
+-rw-r--r--   0        0        0     6135 2024-03-15 22:19:21.019639 swarms-4.7.3/swarms/memory/weaviate_db.py
+-rw-r--r--   0        0        0     2410 2024-04-02 02:22:10.686547 swarms-4.7.3/swarms/models/__init__.py
+-rw-r--r--   0        0        0     2074 2024-03-27 19:58:17.874104 swarms-4.7.3/swarms/models/base_embedding_model.py
+-rw-r--r--   0        0        0    13240 2024-03-15 22:19:21.021853 swarms-4.7.3/swarms/models/base_llm.py
+-rw-r--r--   0        0        0    12728 2024-03-15 22:19:21.022342 swarms-4.7.3/swarms/models/base_multimodal_model.py
+-rw-r--r--   0        0        0     2487 2024-03-15 22:19:21.023152 swarms-4.7.3/swarms/models/base_tts.py
+-rw-r--r--   0        0        0     3171 2024-03-15 22:19:21.023526 swarms-4.7.3/swarms/models/base_ttv.py
+-rw-r--r--   0        0        0    16953 2024-03-15 22:19:21.027265 swarms-4.7.3/swarms/models/cog_vlm.py
+-rw-r--r--   0        0        0    10864 2024-03-15 22:19:21.028441 swarms-4.7.3/swarms/models/dalle3.py
+-rw-r--r--   0        0        0     6643 2024-03-15 22:19:21.029941 swarms-4.7.3/swarms/models/distilled_whisperx.py
+-rw-r--r--   0        0        0      682 2024-03-15 22:19:21.031788 swarms-4.7.3/swarms/models/embeddings_base.py
+-rw-r--r--   0        0        0     2734 2024-03-15 22:19:21.032242 swarms-4.7.3/swarms/models/fire_function.py
+-rw-r--r--   0        0        0     3022 2024-03-15 22:19:21.032963 swarms-4.7.3/swarms/models/fuyu.py
+-rw-r--r--   0        0        0     7814 2024-03-15 22:19:21.033722 swarms-4.7.3/swarms/models/gemini.py
+-rw-r--r--   0        0        0     2818 2024-03-15 22:19:21.034812 swarms-4.7.3/swarms/models/gpt4_sam.py
+-rw-r--r--   0        0        0    14282 2024-03-15 22:19:21.035054 swarms-4.7.3/swarms/models/gpt4_vision_api.py
+-rw-r--r--   0        0        0    13034 2024-03-15 22:19:21.035781 swarms-4.7.3/swarms/models/huggingface.py
+-rw-r--r--   0        0        0     1968 2024-03-15 22:19:21.036059 swarms-4.7.3/swarms/models/huggingface_pipeline.py
+-rw-r--r--   0        0        0     5623 2024-03-15 22:19:21.036228 swarms-4.7.3/swarms/models/idefics.py
+-rw-r--r--   0        0        0     7996 2024-03-15 22:19:21.036860 swarms-4.7.3/swarms/models/jina_embeds.py
+-rw-r--r--   0        0        0    10752 2024-04-02 02:09:16.602464 swarms-4.7.3/swarms/models/kosmos_two.py
+-rw-r--r--   0        0        0     1448 2024-03-15 22:19:21.037679 swarms-4.7.3/swarms/models/layoutlm_document_qa.py
+-rw-r--r--   0        0        0     6529 2024-03-15 22:19:21.038086 swarms-4.7.3/swarms/models/llama_function_caller.py
+-rw-r--r--   0        0        0     2762 2024-03-15 22:19:21.038340 swarms-4.7.3/swarms/models/llava.py
+-rw-r--r--   0        0        0     4597 2024-03-15 22:19:21.038513 swarms-4.7.3/swarms/models/medical_sam.py
+-rw-r--r--   0        0        0     4324 2024-03-15 22:19:21.038800 swarms-4.7.3/swarms/models/mistral.py
+-rw-r--r--   0        0        0      244 2024-03-24 04:08:38.359236 swarms-4.7.3/swarms/models/mistral_model_api.py
+-rw-r--r--   0        0        0     2155 2024-03-15 22:19:21.039343 swarms-4.7.3/swarms/models/mixtral.py
+-rw-r--r--   0        0        0     2056 2024-03-15 22:19:21.041522 swarms-4.7.3/swarms/models/moondream_mm.py
+-rw-r--r--   0        0        0     6470 2024-03-15 22:19:21.041916 swarms-4.7.3/swarms/models/mpt.py
+-rw-r--r--   0        0        0     2823 2024-03-15 22:19:21.042535 swarms-4.7.3/swarms/models/nougat.py
+-rw-r--r--   0        0        0     2366 2024-03-15 22:19:21.043550 swarms-4.7.3/swarms/models/open_dalle.py
+-rw-r--r--   0        0        0    20443 2024-03-21 23:46:38.329902 swarms-4.7.3/swarms/models/openai_embeddings.py
+-rw-r--r--   0        0        0     3175 2024-03-15 22:19:21.045986 swarms-4.7.3/swarms/models/openai_tts.py
+-rw-r--r--   0        0        0     6133 2024-03-21 23:46:38.330900 swarms-4.7.3/swarms/models/palm.py
+-rw-r--r--   0        0        0     1101 2024-03-21 23:46:38.332006 swarms-4.7.3/swarms/models/popular_llms.py
+-rw-r--r--   0        0        0     4843 2024-03-15 22:19:21.048155 swarms-4.7.3/swarms/models/qwen.py
+-rw-r--r--   0        0        0     3547 2024-03-15 22:19:21.049332 swarms-4.7.3/swarms/models/sam.py
+-rw-r--r--   0        0        0    12871 2024-03-15 22:19:21.050598 swarms-4.7.3/swarms/models/sampling_params.py
+-rw-r--r--   0        0        0     7709 2024-03-15 22:19:21.050811 swarms-4.7.3/swarms/models/speecht5.py
+-rw-r--r--   0        0        0     8318 2024-03-21 23:46:38.332831 swarms-4.7.3/swarms/models/ssd_1b.py
+-rw-r--r--   0        0        0     5189 2024-03-15 22:19:21.051613 swarms-4.7.3/swarms/models/stable_diffusion.py
+-rw-r--r--   0        0        0     1794 2024-03-15 22:19:21.052816 swarms-4.7.3/swarms/models/timm.py
+-rw-r--r--   0        0        0     3990 2024-03-23 22:42:41.705709 swarms-4.7.3/swarms/models/together.py
+-rw-r--r--   0        0        0      148 2024-03-15 22:19:21.053560 swarms-4.7.3/swarms/models/trocr.py
+-rw-r--r--   0        0        0      592 2024-03-15 22:19:21.054281 swarms-4.7.3/swarms/models/types.py
+-rw-r--r--   0        0        0     1499 2024-03-15 22:19:21.054547 swarms-4.7.3/swarms/models/ultralytics_model.py
+-rw-r--r--   0        0        0     1731 2024-03-15 22:19:21.054977 swarms-4.7.3/swarms/models/vilt.py
+-rw-r--r--   0        0        0     2846 2024-03-15 22:19:21.055732 swarms-4.7.3/swarms/models/vip_llava.py
+-rw-r--r--   0        0        0     7678 2024-03-15 22:19:21.056747 swarms-4.7.3/swarms/models/wizard_storytelling.py
+-rw-r--r--   0        0        0     9576 2024-03-15 22:19:21.057712 swarms-4.7.3/swarms/models/yarn_mistral.py
+-rw-r--r--   0        0        0     2943 2024-03-15 22:19:21.058472 swarms-4.7.3/swarms/models/yi_200k.py
+-rw-r--r--   0        0        0     3681 2024-03-15 22:19:21.059936 swarms-4.7.3/swarms/models/zeroscope.py
+-rw-r--r--   0        0        0      775 2024-03-15 22:19:21.060753 swarms-4.7.3/swarms/prompts/__init__.py
+-rw-r--r--   0        0        0    11320 2024-03-15 22:19:21.061563 swarms-4.7.3/swarms/prompts/accountant_swarm_prompts.py
+-rw-r--r--   0        0        0     9156 2024-03-15 22:19:21.062133 swarms-4.7.3/swarms/prompts/aga.py
+-rw-r--r--   0        0        0     1451 2024-03-15 22:19:21.062911 swarms-4.7.3/swarms/prompts/agent_output_parser.py
+-rw-r--r--   0        0        0     2705 2024-03-15 22:19:21.063538 swarms-4.7.3/swarms/prompts/agent_prompt.py
+-rw-r--r--   0        0        0     6886 2024-03-15 22:19:21.064160 swarms-4.7.3/swarms/prompts/agent_prompts.py
+-rw-r--r--   0        0        0     7145 2024-03-15 22:19:21.065128 swarms-4.7.3/swarms/prompts/agent_system_prompts.py
+-rw-r--r--   0        0        0     5233 2024-03-15 22:19:21.065787 swarms-4.7.3/swarms/prompts/ai_research_team.py
+-rw-r--r--   0        0        0    13981 2024-03-15 22:19:21.066513 swarms-4.7.3/swarms/prompts/autobloggen.py
+-rw-r--r--   0        0        0     5605 2024-03-15 22:19:21.068224 swarms-4.7.3/swarms/prompts/autoswarm.py
+-rw-r--r--   0        0        0     7542 2024-03-15 22:19:21.068567 swarms-4.7.3/swarms/prompts/base.py
+-rw-r--r--   0        0        0     3801 2024-03-15 22:19:21.068894 swarms-4.7.3/swarms/prompts/chat_prompt.py
+-rw-r--r--   0        0        0     2235 2024-03-15 22:19:21.069096 swarms-4.7.3/swarms/prompts/code_interpreter.py
+-rw-r--r--   0        0        0     4106 2024-03-15 22:19:21.069652 swarms-4.7.3/swarms/prompts/code_spawner.py
+-rw-r--r--   0        0        0     1566 2024-03-15 22:19:21.069820 swarms-4.7.3/swarms/prompts/debate.py
+-rw-r--r--   0        0        0     7044 2024-03-15 22:19:21.070670 swarms-4.7.3/swarms/prompts/documentation.py
+-rw-r--r--   0        0        0     1767 2024-03-15 22:19:21.071442 swarms-4.7.3/swarms/prompts/education.py
+-rw-r--r--   0        0        0     4180 2024-03-15 22:19:21.071791 swarms-4.7.3/swarms/prompts/finance_agent_prompt.py
+-rw-r--r--   0        0        0     4117 2024-03-15 22:19:21.072144 swarms-4.7.3/swarms/prompts/growth_agent_prompt.py
+-rw-r--r--   0        0        0      880 2024-03-15 22:19:21.072694 swarms-4.7.3/swarms/prompts/idea2img.py
+-rw-r--r--   0        0        0     3346 2024-03-15 22:19:21.072990 swarms-4.7.3/swarms/prompts/legal_agent_prompt.py
+-rw-r--r--   0        0        0     4785 2024-03-15 22:19:21.073912 swarms-4.7.3/swarms/prompts/logistics.py
+-rw-r--r--   0        0        0    10662 2024-03-15 22:19:21.074621 swarms-4.7.3/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
+-rw-r--r--   0        0        0     3511 2024-03-15 22:19:21.075295 swarms-4.7.3/swarms/prompts/multi_modal_prompts.py
+-rw-r--r--   0        0        0     3225 2024-03-15 22:19:21.075646 swarms-4.7.3/swarms/prompts/multi_modal_visual_prompts.py
+-rw-r--r--   0        0        0     3454 2024-03-15 22:19:21.076012 swarms-4.7.3/swarms/prompts/operations_agent_prompt.py
+-rw-r--r--   0        0        0        0 2024-03-15 22:19:21.076143 swarms-4.7.3/swarms/prompts/orchestrator_prompt.py
+-rw-r--r--   0        0        0     2149 2024-03-15 22:19:21.076733 swarms-4.7.3/swarms/prompts/personal_stylist.py
+-rw-r--r--   0        0        0     8333 2024-03-15 22:19:21.077280 swarms-4.7.3/swarms/prompts/product_agent_prompt.py
+-rw-r--r--   0        0        0    10144 2024-03-15 22:19:21.078026 swarms-4.7.3/swarms/prompts/programming.py
+-rw-r--r--   0        0        0     2128 2024-03-15 22:19:21.078275 swarms-4.7.3/swarms/prompts/project_manager.py
+-rw-r--r--   0        0        0    13215 2024-03-15 22:19:21.078885 swarms-4.7.3/swarms/prompts/python.py
+-rw-r--r--   0        0        0     2960 2024-03-15 22:19:21.079805 swarms-4.7.3/swarms/prompts/react.py
+-rw-r--r--   0        0        0        0 2024-03-15 22:19:21.080059 swarms-4.7.3/swarms/prompts/refiner_agent_prompt.py
+-rw-r--r--   0        0        0     5126 2024-03-15 22:19:21.080659 swarms-4.7.3/swarms/prompts/sales.py
+-rw-r--r--   0        0        0     5013 2024-03-15 22:19:21.081280 swarms-4.7.3/swarms/prompts/sales_prompts.py
+-rw-r--r--   0        0        0     7573 2024-03-15 22:19:21.082529 swarms-4.7.3/swarms/prompts/schema_generator.py
+-rw-r--r--   0        0        0     2679 2024-03-15 22:19:21.083072 swarms-4.7.3/swarms/prompts/security_team.py
+-rw-r--r--   0        0        0     3264 2024-03-15 22:19:21.083517 swarms-4.7.3/swarms/prompts/self_operating_prompt.py
+-rw-r--r--   0        0        0     4147 2024-03-15 22:19:21.084066 swarms-4.7.3/swarms/prompts/sop_generator_agent_prompt.py
+-rw-r--r--   0        0        0     4640 2024-03-15 22:19:21.084386 swarms-4.7.3/swarms/prompts/summaries_prompts.py
+-rw-r--r--   0        0        0     3984 2024-03-15 22:19:21.084631 swarms-4.7.3/swarms/prompts/support_agent_prompt.py
+-rw-r--r--   0        0        0     4280 2024-03-15 22:19:21.085244 swarms-4.7.3/swarms/prompts/swarm_manager_agent.py
+-rw-r--r--   0        0        0      728 2024-03-15 22:19:21.085725 swarms-4.7.3/swarms/prompts/task_assignment_prompt.py
+-rw-r--r--   0        0        0     4271 2024-03-15 22:19:21.086266 swarms-4.7.3/swarms/prompts/tests.py
+-rw-r--r--   0        0        0     4288 2024-03-15 22:19:21.086625 swarms-4.7.3/swarms/prompts/tools.py
+-rw-r--r--   0        0        0     2398 2024-03-15 22:19:21.087352 swarms-4.7.3/swarms/prompts/urban_planning.py
+-rw-r--r--   0        0        0     3675 2024-03-15 22:19:21.087654 swarms-4.7.3/swarms/prompts/visual_cot.py
+-rw-r--r--   0        0        0     2792 2024-03-21 23:46:38.334043 swarms-4.7.3/swarms/prompts/worker_prompt.py
+-rw-r--r--   0        0        0     2349 2024-03-15 22:19:21.088382 swarms-4.7.3/swarms/prompts/xray_swarm_prompt.py
+-rw-r--r--   0        0        0     3785 2024-03-27 19:58:17.513026 swarms-4.7.3/swarms/structs/__init__.py
+-rw-r--r--   0        0        0    47441 2024-03-30 18:48:29.907000 swarms-4.7.3/swarms/structs/agent.py
+-rw-r--r--   0        0        0      574 2024-03-15 22:19:21.092491 swarms-4.7.3/swarms/structs/agent_job.py
+-rw-r--r--   0        0        0     2923 2024-03-27 19:58:17.509429 swarms-4.7.3/swarms/structs/agent_process.py
+-rw-r--r--   0        0        0     3732 2024-03-15 22:19:21.092747 swarms-4.7.3/swarms/structs/async_workflow.py
+-rw-r--r--   0        0        0     7951 2024-03-27 19:47:31.068918 swarms-4.7.3/swarms/structs/auto_swarm.py
+-rw-r--r--   0        0        0    11735 2024-03-15 22:19:21.093292 swarms-4.7.3/swarms/structs/autoscaler.py
+-rw-r--r--   0        0        0    12262 2024-03-15 22:19:21.093668 swarms-4.7.3/swarms/structs/base.py
+-rw-r--r--   0        0        0    19105 2024-03-30 07:40:24.964542 swarms-4.7.3/swarms/structs/base_swarm.py
+-rw-r--r--   0        0        0    12486 2024-03-27 19:12:09.737934 swarms-4.7.3/swarms/structs/base_workflow.py
+-rw-r--r--   0        0        0     1056 2024-03-15 22:19:21.095125 swarms-4.7.3/swarms/structs/block_wrapper.py
+-rw-r--r--   0        0        0      629 2024-03-15 22:19:21.095875 swarms-4.7.3/swarms/structs/blockdevice.py
+-rw-r--r--   0        0        0     3178 2024-03-15 22:19:21.096348 swarms-4.7.3/swarms/structs/blocksdict.py
+-rw-r--r--   0        0        0     4887 2024-03-15 22:19:21.096911 swarms-4.7.3/swarms/structs/blockslist.py
+-rw-r--r--   0        0        0     5364 2024-03-15 22:19:21.097555 swarms-4.7.3/swarms/structs/company.py
+-rw-r--r--   0        0        0     4515 2024-03-15 22:19:21.097858 swarms-4.7.3/swarms/structs/concurrent_workflow.py
+-rw-r--r--   0        0        0    14023 2024-03-27 19:26:23.824143 swarms-4.7.3/swarms/structs/conversation.py
+-rw-r--r--   0        0        0    12615 2024-03-15 22:19:21.099092 swarms-4.7.3/swarms/structs/debate.py
+-rw-r--r--   0        0        0     3041 2024-03-15 22:19:21.099360 swarms-4.7.3/swarms/structs/document.py
+-rw-r--r--   0        0        0     5433 2024-03-15 22:19:21.099780 swarms-4.7.3/swarms/structs/graph_workflow.py
+-rw-r--r--   0        0        0     5066 2024-03-15 22:19:21.100307 swarms-4.7.3/swarms/structs/groupchat.py
+-rw-r--r--   0        0        0     1951 2024-03-15 22:19:21.100923 swarms-4.7.3/swarms/structs/load_balancer.py
+-rw-r--r--   0        0        0     4545 2024-03-15 22:19:21.101122 swarms-4.7.3/swarms/structs/long_swarm.py
+-rw-r--r--   0        0        0     7072 2024-03-15 22:19:21.101824 swarms-4.7.3/swarms/structs/majority_voting.py
+-rw-r--r--   0        0        0      582 2024-03-15 22:19:21.101971 swarms-4.7.3/swarms/structs/message.py
+-rw-r--r--   0        0        0     7384 2024-03-15 22:19:21.102439 swarms-4.7.3/swarms/structs/message_pool.py
+-rw-r--r--   0        0        0     5771 2024-03-15 22:19:21.102829 swarms-4.7.3/swarms/structs/model_parallizer.py
+-rw-r--r--   0        0        0    10524 2024-03-26 17:51:23.615677 swarms-4.7.3/swarms/structs/multi_agent_collab.py
+-rw-r--r--   0        0        0     5623 2024-03-15 22:19:21.103669 swarms-4.7.3/swarms/structs/multi_process_workflow.py
+-rw-r--r--   0        0        0     5386 2024-03-15 22:19:21.103964 swarms-4.7.3/swarms/structs/multi_threaded_workflow.py
+-rw-r--r--   0        0        0     2883 2024-03-15 22:19:21.104315 swarms-4.7.3/swarms/structs/nonlinear_workflow.py
+-rw-r--r--   0        0        0      364 2024-03-26 04:56:18.014859 swarms-4.7.3/swarms/structs/omni_agent_types.py
+-rw-r--r--   0        0        0      778 2024-03-15 22:19:21.104929 swarms-4.7.3/swarms/structs/plan.py
+-rw-r--r--   0        0        0     5466 2024-03-30 18:05:25.777384 swarms-4.7.3/swarms/structs/rearrange.py
+-rw-r--r--   0        0        0     2813 2024-03-27 19:12:09.704075 swarms-4.7.3/swarms/structs/recursive_workflow.py
+-rw-r--r--   0        0        0     4182 2024-03-21 23:46:38.336523 swarms-4.7.3/swarms/structs/schemas.py
+-rw-r--r--   0        0        0     8094 2024-03-15 22:19:21.106433 swarms-4.7.3/swarms/structs/sequential_workflow.py
+-rw-r--r--   0        0        0     2337 2024-03-27 19:47:31.068657 swarms-4.7.3/swarms/structs/sermon_swarm.py
+-rw-r--r--   0        0        0     2894 2024-04-02 02:08:38.776074 swarms-4.7.3/swarms/structs/stackoverflow_swarm.py
+-rw-r--r--   0        0        0      704 2024-03-27 19:12:09.672624 swarms-4.7.3/swarms/structs/step.py
+-rw-r--r--   0        0        0    10756 2024-03-27 19:12:09.673443 swarms-4.7.3/swarms/structs/swarm_net.py
+-rw-r--r--   0        0        0     5182 2024-03-27 19:47:31.068788 swarms-4.7.3/swarms/structs/swarm_redis_registry.py
+-rw-r--r--   0        0        0     6470 2024-03-15 22:19:21.109619 swarms-4.7.3/swarms/structs/swarming_architectures.py
+-rw-r--r--   0        0        0     8311 2024-03-15 22:19:21.109964 swarms-4.7.3/swarms/structs/task.py
+-rw-r--r--   0        0        0     1989 2024-03-27 19:12:09.705030 swarms-4.7.3/swarms/structs/task_queue_base.py
+-rw-r--r--   0        0        0     3427 2024-03-15 22:19:21.111077 swarms-4.7.3/swarms/structs/team.py
+-rw-r--r--   0        0        0     3545 2024-03-15 22:19:21.112074 swarms-4.7.3/swarms/structs/utils.py
+-rw-r--r--   0        0        0      891 2024-03-27 19:12:09.674045 swarms-4.7.3/swarms/telemetry/__init__.py
+-rw-r--r--   0        0        0      513 2024-03-27 19:12:09.674581 swarms-4.7.3/swarms/telemetry/auto_upgrade_swarms.py
+-rw-r--r--   0        0        0      384 2024-04-02 02:13:55.447849 swarms-4.7.3/swarms/telemetry/bootup.py
+-rw-r--r--   0        0        0     1087 2024-03-15 22:19:21.113750 swarms-4.7.3/swarms/telemetry/check_update.py
+-rw-r--r--   0        0        0      807 2024-03-15 22:19:21.114471 swarms-4.7.3/swarms/telemetry/log_all.py
+-rw-r--r--   0        0        0      496 2024-03-22 00:42:19.696403 swarms-4.7.3/swarms/telemetry/sentry_active.py
+-rw-r--r--   0        0        0     2729 2024-03-15 22:19:21.115547 swarms-4.7.3/swarms/telemetry/sys_info.py
+-rw-r--r--   0        0        0     1996 2024-03-27 19:12:09.675144 swarms-4.7.3/swarms/telemetry/user_utils.py
+-rw-r--r--   0        0        0      805 2024-03-21 23:46:38.337818 swarms-4.7.3/swarms/tools/__init__.py
+-rw-r--r--   0        0        0     3038 2024-03-15 22:19:21.119284 swarms-4.7.3/swarms/tools/code_executor.py
+-rw-r--r--   0        0        0     3614 2024-03-15 22:19:21.119730 swarms-4.7.3/swarms/tools/exec_tool.py
+-rw-r--r--   0        0        0    14523 2024-03-24 05:11:17.316917 swarms-4.7.3/swarms/tools/format_tools.py
+-rw-r--r--   0        0        0     2469 2024-03-24 05:13:04.696739 swarms-4.7.3/swarms/tools/logits_processor.py
+-rw-r--r--   0        0        0      157 2024-03-24 04:12:12.223834 swarms-4.7.3/swarms/tools/tool.py
+-rw-r--r--   0        0        0     6165 2024-03-15 22:19:21.121316 swarms-4.7.3/swarms/tools/tool_utils.py
+-rw-r--r--   0        0        0     5466 2024-03-15 22:19:21.122024 swarms-4.7.3/swarms/utils/README.md
+-rw-r--r--   0        0        0     2691 2024-03-27 19:41:15.064545 swarms-4.7.3/swarms/utils/__init__.py
+-rw-r--r--   0        0        0     3537 2024-03-15 22:19:21.122933 swarms-4.7.3/swarms/utils/apa.py
+-rw-r--r--   0        0        0     6071 2024-03-15 22:19:21.123535 swarms-4.7.3/swarms/utils/check_function_result.py
+-rw-r--r--   0        0        0     1008 2024-03-15 22:19:21.124143 swarms-4.7.3/swarms/utils/class_args_wrapper.py
+-rw-r--r--   0        0        0     6674 2024-03-15 22:19:21.125150 swarms-4.7.3/swarms/utils/code_interpreter.py
+-rw-r--r--   0        0        0     1264 2024-03-15 22:19:21.125539 swarms-4.7.3/swarms/utils/concurrent_utils.py
+-rw-r--r--   0        0        0      808 2024-03-15 22:19:21.126204 swarms-4.7.3/swarms/utils/csv_and_pandas.py
+-rw-r--r--   0        0        0     1887 2024-03-15 22:19:21.126685 swarms-4.7.3/swarms/utils/data_to_text.py
+-rw-r--r--   0        0        0     2451 2024-03-15 22:19:21.127334 swarms-4.7.3/swarms/utils/decorators.py
+-rw-r--r--   0        0        0     2342 2024-03-15 22:19:21.127636 swarms-4.7.3/swarms/utils/device_checker_cuda.py
+-rw-r--r--   0        0        0     1311 2024-03-15 22:19:21.127902 swarms-4.7.3/swarms/utils/disable_logging.py
+-rw-r--r--   0        0        0      890 2024-03-15 22:19:21.128555 swarms-4.7.3/swarms/utils/download_img.py
+-rw-r--r--   0        0        0      690 2024-03-15 22:19:21.129208 swarms-4.7.3/swarms/utils/download_weights_from_url.py
+-rw-r--r--   0        0        0     1127 2024-03-15 22:19:21.129540 swarms-4.7.3/swarms/utils/execute_futures.py
+-rw-r--r--   0        0        0     3472 2024-03-15 22:19:21.130035 swarms-4.7.3/swarms/utils/execution_sandbox.py
+-rw-r--r--   0        0        0     1113 2024-03-15 22:19:21.130281 swarms-4.7.3/swarms/utils/exponential_backoff.py
+-rw-r--r--   0        0        0      854 2024-03-15 22:19:21.130759 swarms-4.7.3/swarms/utils/fetch_init_params.py
+-rw-r--r--   0        0        0      500 2024-03-15 22:19:21.131255 swarms-4.7.3/swarms/utils/file_extension_seach.py
+-rw-r--r--   0        0        0     3286 2024-03-15 22:19:21.131635 swarms-4.7.3/swarms/utils/file_processing.py
+-rw-r--r--   0        0        0      644 2024-03-15 22:19:21.131989 swarms-4.7.3/swarms/utils/find_img_path.py
+-rw-r--r--   0        0        0     1411 2024-03-15 22:19:21.132408 swarms-4.7.3/swarms/utils/function_calling_utils.py
+-rw-r--r--   0        0        0     4184 2024-03-15 22:19:21.132807 swarms-4.7.3/swarms/utils/get_logger.py
+-rw-r--r--   0        0        0      363 2024-03-15 22:19:21.133103 swarms-4.7.3/swarms/utils/hash.py
+-rw-r--r--   0        0        0     2228 2024-03-15 22:19:21.133717 swarms-4.7.3/swarms/utils/inference_convert_utils.py
+-rw-r--r--   0        0        0     2872 2024-03-15 22:19:21.133992 swarms-4.7.3/swarms/utils/json_output_parser.py
+-rw-r--r--   0        0        0     1316 2024-03-21 23:46:38.581600 swarms-4.7.3/swarms/utils/json_utils.py
+-rw-r--r--   0        0        0     1837 2024-03-15 22:19:21.134782 swarms-4.7.3/swarms/utils/jsonl_utils.py
+-rw-r--r--   0        0        0      932 2024-03-15 22:19:21.135261 swarms-4.7.3/swarms/utils/llm_metrics_decorator.py
+-rw-r--r--   0        0        0     1915 2024-03-15 22:19:21.135427 swarms-4.7.3/swarms/utils/load_model_torch.py
+-rw-r--r--   0        0        0     2261 2024-03-15 22:19:21.136053 swarms-4.7.3/swarms/utils/logger.py
+-rw-r--r--   0        0        0    16348 2024-03-26 17:55:25.494840 swarms-4.7.3/swarms/utils/loggers.py
+-rw-r--r--   0        0        0      453 2024-03-27 19:12:09.738695 swarms-4.7.3/swarms/utils/loguru_logger.py
+-rw-r--r--   0        0        0     6723 2024-03-27 19:12:09.739420 swarms-4.7.3/swarms/utils/main.py
+-rw-r--r--   0        0        0      711 2024-03-27 19:12:09.676603 swarms-4.7.3/swarms/utils/markdown_message.py
+-rw-r--r--   0        0        0     1461 2024-03-15 22:19:21.138609 swarms-4.7.3/swarms/utils/math_eval.py
+-rw-r--r--   0        0        0     1097 2024-03-15 22:19:21.139027 swarms-4.7.3/swarms/utils/pandas_to_str.py
+-rw-r--r--   0        0        0      600 2024-03-15 22:19:21.139501 swarms-4.7.3/swarms/utils/parse_code.py
+-rw-r--r--   0        0        0     1199 2024-03-15 22:19:21.140224 swarms-4.7.3/swarms/utils/pdf_to_text.py
+-rw-r--r--   0        0        0      778 2024-03-15 22:19:21.140973 swarms-4.7.3/swarms/utils/prep_torch_model_inference.py
+-rw-r--r--   0        0        0     1353 2024-03-15 22:19:21.141276 swarms-4.7.3/swarms/utils/remove_json_whitespace.py
+-rw-r--r--   0        0        0     1300 2024-03-15 22:19:21.141589 swarms-4.7.3/swarms/utils/save_logs.py
+-rw-r--r--   0        0        0     4804 2024-03-21 23:46:38.340334 swarms-4.7.3/swarms/utils/serializable.py
+-rw-r--r--   0        0        0     3034 2024-03-15 22:19:21.143281 swarms-4.7.3/swarms/utils/supervision_visualizer.py
+-rw-r--r--   0        0        0      245 2024-03-15 22:19:21.144185 swarms-4.7.3/swarms/utils/torch_utils.py
+-rw-r--r--   0        0        0     1308 2024-03-15 22:19:21.144686 swarms-4.7.3/swarms/utils/try_except_wrapper.py
+-rw-r--r--   0        0        0     2692 2024-03-15 22:19:21.145401 swarms-4.7.3/swarms/utils/yaml_output_parser.py
+-rw-r--r--   0        0        0    35720 1970-01-01 00:00:00.000000 swarms-4.7.3/setup.py
+-rw-r--r--   0        0        0    34893 1970-01-01 00:00:00.000000 swarms-4.7.3/PKG-INFO
```

### Comparing `swarms-4.7.1/LICENSE` & `swarms-4.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/README.md` & `swarms-4.7.3/README.md`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/pyproject.toml` & `swarms-4.7.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "swarms"
-version = "4.7.1"
+version = "4.7.3"
 description = "Swarms - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/swarms"
 documentation = "https://swarms.apac.ai"  
 readme = "README.md" 
 repository = "https://github.com/kyegomez/swarms"
@@ -64,11 +64,7 @@
 fixable = ["ALL"]
 unfixable = []
 
 [tool.black]
 line-length = 70
 target-version = ['py38']
 preview = true
-
-
-[tool.poetry.scripts]
-swarms = 'swarms.cli._cli:main'
```

### Comparing `swarms-4.7.1/swarms/__init__.py` & `swarms-4.7.3/swarms/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import os
 
 from swarms.telemetry.bootup import bootup  # noqa: E402, F403
 from swarms.telemetry.sentry_active import activate_sentry
 
-os.environ["WANDB_SILENT"] = "true"
-
 bootup()
 activate_sentry()
 
 
 from swarms.agents import *  # noqa: E402, F403
 from swarms.artifacts import *  # noqa: E402, F403
 from swarms.memory import *  # noqa: E402, F403
```

### Comparing `swarms-4.7.1/swarms/agents/.DS_Store` & `swarms-4.7.3/swarms/agents/.DS_Store`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/agents/__init__.py` & `swarms-4.7.3/swarms/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/agents/agent_wrapper.py` & `swarms-4.7.3/swarms/agents/agent_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/agents/base.py` & `swarms-4.7.3/swarms/agents/base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/agents/developer_agents.py` & `swarms-4.7.3/swarms/agents/developer_agents.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/agents/omni_modal_agent.py` & `swarms-4.7.3/swarms/agents/omni_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/agents/simple_agent.py` & `swarms-4.7.3/swarms/agents/simple_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/agents/tool_agent.py` & `swarms-4.7.3/swarms/agents/tool_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/agents/worker_agent.py` & `swarms-4.7.3/swarms/agents/worker_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/artifacts/base_artifact.py` & `swarms-4.7.3/swarms/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/artifacts/text_artifact.py` & `swarms-4.7.3/swarms/artifacts/text_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/__init__.py` & `swarms-4.7.3/swarms/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/base_db.py` & `swarms-4.7.3/swarms/memory/base_db.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/base_vectordb.py` & `swarms-4.7.3/swarms/memory/base_vectordb.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/chroma_db.py` & `swarms-4.7.3/swarms/memory/chroma_db.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/cosine_similarity.py` & `swarms-4.7.3/swarms/memory/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/dict_internal_memory.py` & `swarms-4.7.3/swarms/memory/dict_internal_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/dict_shared_memory.py` & `swarms-4.7.3/swarms/memory/dict_shared_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/lanchain_chroma.py` & `swarms-4.7.3/swarms/memory/lanchain_chroma.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/pg.py` & `swarms-4.7.3/swarms/memory/pg.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/pinecone.py` & `swarms-4.7.3/swarms/memory/pinecone.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/qdrant.py` & `swarms-4.7.3/swarms/memory/qdrant.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/short_term_memory.py` & `swarms-4.7.3/swarms/memory/short_term_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/sqlite.py` & `swarms-4.7.3/swarms/memory/sqlite.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/utils.py` & `swarms-4.7.3/swarms/memory/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/visual_memory.py` & `swarms-4.7.3/swarms/memory/visual_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/memory/weaviate_db.py` & `swarms-4.7.3/swarms/memory/weaviate_db.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/__init__.py` & `swarms-4.7.3/swarms/models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     OpenAILLM as OpenAI,
 )
 from swarms.models.popular_llms import (
     ReplicateLLM as Replicate,
 )
 from swarms.models.qwen import QwenVLMultiModal  # noqa: E402
 
-from swarms.models.sam_supervision import SegmentAnythingMarkGenerator
 from swarms.models.sampling_params import SamplingParams, SamplingType
 from swarms.models.together import TogetherLLM  # noqa: E402
 from swarms.models.types import (  # noqa: E402
     AudioModality,
     ImageModality,
     MultimodalData,
     TextModality,
@@ -70,15 +69,14 @@
     "OpenAI",
     "OpenAIChat",
     "OpenAITTS",
     "QwenVLMultiModal",
     "Replicate",
     "SamplingParams",
     "SamplingType",
-    "SegmentAnythingMarkGenerator",
     "TextModality",
     "TogetherLLM",
     "Vilt",
     "AudioModality",
     "ImageModality",
     "VideoModality",
 ]
```

### Comparing `swarms-4.7.1/swarms/models/base_embedding_model.py` & `swarms-4.7.3/swarms/models/base_embedding_model.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/base_llm.py` & `swarms-4.7.3/swarms/models/base_llm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/base_multimodal_model.py` & `swarms-4.7.3/swarms/models/base_multimodal_model.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/base_tts.py` & `swarms-4.7.3/swarms/models/base_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/base_ttv.py` & `swarms-4.7.3/swarms/models/base_ttv.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/cog_vlm.py` & `swarms-4.7.3/swarms/models/cog_vlm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/dalle3.py` & `swarms-4.7.3/swarms/models/dalle3.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/distilled_whisperx.py` & `swarms-4.7.3/swarms/models/distilled_whisperx.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/embeddings_base.py` & `swarms-4.7.3/swarms/models/embeddings_base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/fire_function.py` & `swarms-4.7.3/swarms/models/fire_function.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/fuyu.py` & `swarms-4.7.3/swarms/models/fuyu.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/gemini.py` & `swarms-4.7.3/swarms/models/gemini.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/gpt4_sam.py` & `swarms-4.7.3/swarms/models/gpt4_sam.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/gpt4_vision_api.py` & `swarms-4.7.3/swarms/models/gpt4_vision_api.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/huggingface.py` & `swarms-4.7.3/swarms/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/huggingface_pipeline.py` & `swarms-4.7.3/swarms/models/huggingface_pipeline.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/idefics.py` & `swarms-4.7.3/swarms/models/idefics.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/jina_embeds.py` & `swarms-4.7.3/swarms/models/jina_embeds.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/kosmos_two.py` & `swarms-4.7.3/swarms/models/kosmos_two.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/layoutlm_document_qa.py` & `swarms-4.7.3/swarms/models/layoutlm_document_qa.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/llama_function_caller.py` & `swarms-4.7.3/swarms/models/llama_function_caller.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/llava.py` & `swarms-4.7.3/swarms/models/llava.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/medical_sam.py` & `swarms-4.7.3/swarms/models/medical_sam.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/mistral.py` & `swarms-4.7.3/swarms/models/mistral.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/mixtral.py` & `swarms-4.7.3/swarms/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/moondream_mm.py` & `swarms-4.7.3/swarms/models/moondream_mm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/mpt.py` & `swarms-4.7.3/swarms/models/mpt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/nougat.py` & `swarms-4.7.3/swarms/models/nougat.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/open_dalle.py` & `swarms-4.7.3/swarms/models/open_dalle.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/openai_embeddings.py` & `swarms-4.7.3/swarms/models/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/openai_tts.py` & `swarms-4.7.3/swarms/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/palm.py` & `swarms-4.7.3/swarms/models/palm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/popular_llms.py` & `swarms-4.7.3/swarms/models/popular_llms.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/qwen.py` & `swarms-4.7.3/swarms/models/qwen.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/sam.py` & `swarms-4.7.3/swarms/models/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/sampling_params.py` & `swarms-4.7.3/swarms/models/sampling_params.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/speecht5.py` & `swarms-4.7.3/swarms/models/speecht5.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/ssd_1b.py` & `swarms-4.7.3/swarms/models/ssd_1b.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/stable_diffusion.py` & `swarms-4.7.3/swarms/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/timm.py` & `swarms-4.7.3/swarms/models/timm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/together.py` & `swarms-4.7.3/swarms/models/together.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/types.py` & `swarms-4.7.3/swarms/models/types.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/ultralytics_model.py` & `swarms-4.7.3/swarms/models/ultralytics_model.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/vilt.py` & `swarms-4.7.3/swarms/models/vilt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/vip_llava.py` & `swarms-4.7.3/swarms/models/vip_llava.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/wizard_storytelling.py` & `swarms-4.7.3/swarms/models/wizard_storytelling.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/yarn_mistral.py` & `swarms-4.7.3/swarms/models/yarn_mistral.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/yi_200k.py` & `swarms-4.7.3/swarms/models/yi_200k.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/models/zeroscope.py` & `swarms-4.7.3/swarms/models/zeroscope.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/__init__.py` & `swarms-4.7.3/swarms/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/accountant_swarm_prompts.py` & `swarms-4.7.3/swarms/prompts/accountant_swarm_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/aga.py` & `swarms-4.7.3/swarms/prompts/aga.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/agent_output_parser.py` & `swarms-4.7.3/swarms/prompts/agent_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/agent_prompt.py` & `swarms-4.7.3/swarms/prompts/agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/agent_prompts.py` & `swarms-4.7.3/swarms/prompts/agent_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/agent_system_prompts.py` & `swarms-4.7.3/swarms/prompts/agent_system_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/ai_research_team.py` & `swarms-4.7.3/swarms/prompts/ai_research_team.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/autobloggen.py` & `swarms-4.7.3/swarms/prompts/autobloggen.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/autoswarm.py` & `swarms-4.7.3/swarms/prompts/autoswarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/base.py` & `swarms-4.7.3/swarms/prompts/base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/chat_prompt.py` & `swarms-4.7.3/swarms/prompts/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/code_interpreter.py` & `swarms-4.7.3/swarms/prompts/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/code_spawner.py` & `swarms-4.7.3/swarms/prompts/code_spawner.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/debate.py` & `swarms-4.7.3/swarms/prompts/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/documentation.py` & `swarms-4.7.3/swarms/prompts/documentation.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/education.py` & `swarms-4.7.3/swarms/prompts/education.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/finance_agent_prompt.py` & `swarms-4.7.3/swarms/prompts/finance_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/growth_agent_prompt.py` & `swarms-4.7.3/swarms/prompts/growth_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/idea2img.py` & `swarms-4.7.3/swarms/prompts/idea2img.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/legal_agent_prompt.py` & `swarms-4.7.3/swarms/prompts/legal_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/logistics.py` & `swarms-4.7.3/swarms/prompts/logistics.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/multi_modal_autonomous_instruction_prompt.py` & `swarms-4.7.3/swarms/prompts/multi_modal_autonomous_instruction_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/multi_modal_prompts.py` & `swarms-4.7.3/swarms/prompts/multi_modal_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/multi_modal_visual_prompts.py` & `swarms-4.7.3/swarms/prompts/multi_modal_visual_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/operations_agent_prompt.py` & `swarms-4.7.3/swarms/prompts/operations_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/personal_stylist.py` & `swarms-4.7.3/swarms/prompts/personal_stylist.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/product_agent_prompt.py` & `swarms-4.7.3/swarms/prompts/product_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/programming.py` & `swarms-4.7.3/swarms/prompts/programming.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/project_manager.py` & `swarms-4.7.3/swarms/prompts/project_manager.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/python.py` & `swarms-4.7.3/swarms/prompts/python.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/react.py` & `swarms-4.7.3/swarms/prompts/react.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/sales.py` & `swarms-4.7.3/swarms/prompts/sales.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/sales_prompts.py` & `swarms-4.7.3/swarms/prompts/sales_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/schema_generator.py` & `swarms-4.7.3/swarms/prompts/schema_generator.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/security_team.py` & `swarms-4.7.3/swarms/prompts/security_team.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/self_operating_prompt.py` & `swarms-4.7.3/swarms/prompts/self_operating_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/sop_generator_agent_prompt.py` & `swarms-4.7.3/swarms/prompts/sop_generator_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/summaries_prompts.py` & `swarms-4.7.3/swarms/prompts/summaries_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/support_agent_prompt.py` & `swarms-4.7.3/swarms/prompts/support_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/swarm_manager_agent.py` & `swarms-4.7.3/swarms/prompts/swarm_manager_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/task_assignment_prompt.py` & `swarms-4.7.3/swarms/prompts/task_assignment_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/tests.py` & `swarms-4.7.3/swarms/prompts/tests.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/tools.py` & `swarms-4.7.3/swarms/prompts/tools.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/urban_planning.py` & `swarms-4.7.3/swarms/prompts/urban_planning.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/visual_cot.py` & `swarms-4.7.3/swarms/prompts/visual_cot.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/worker_prompt.py` & `swarms-4.7.3/swarms/prompts/worker_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/prompts/xray_swarm_prompt.py` & `swarms-4.7.3/swarms/prompts/xray_swarm_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/__init__.py` & `swarms-4.7.3/swarms/structs/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/agent.py` & `swarms-4.7.3/swarms/structs/agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/agent_job.py` & `swarms-4.7.3/swarms/structs/agent_job.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/agent_process.py` & `swarms-4.7.3/swarms/structs/agent_process.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/async_workflow.py` & `swarms-4.7.3/swarms/structs/async_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/auto_swarm.py` & `swarms-4.7.3/swarms/structs/auto_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/autoscaler.py` & `swarms-4.7.3/swarms/structs/autoscaler.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/base.py` & `swarms-4.7.3/swarms/structs/base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/base_swarm.py` & `swarms-4.7.3/swarms/structs/base_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/base_workflow.py` & `swarms-4.7.3/swarms/structs/base_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/block_wrapper.py` & `swarms-4.7.3/swarms/structs/block_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/blockdevice.py` & `swarms-4.7.3/swarms/structs/blockdevice.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/blocksdict.py` & `swarms-4.7.3/swarms/structs/blocksdict.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/blockslist.py` & `swarms-4.7.3/swarms/structs/blockslist.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/company.py` & `swarms-4.7.3/swarms/structs/company.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/concurrent_workflow.py` & `swarms-4.7.3/swarms/structs/concurrent_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/conversation.py` & `swarms-4.7.3/swarms/structs/conversation.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/debate.py` & `swarms-4.7.3/swarms/structs/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/document.py` & `swarms-4.7.3/swarms/structs/document.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/graph_workflow.py` & `swarms-4.7.3/swarms/structs/graph_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/groupchat.py` & `swarms-4.7.3/swarms/structs/groupchat.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/load_balancer.py` & `swarms-4.7.3/swarms/structs/load_balancer.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/long_swarm.py` & `swarms-4.7.3/swarms/structs/long_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/majority_voting.py` & `swarms-4.7.3/swarms/structs/majority_voting.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/message.py` & `swarms-4.7.3/swarms/structs/message.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/message_pool.py` & `swarms-4.7.3/swarms/structs/message_pool.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/model_parallizer.py` & `swarms-4.7.3/swarms/structs/model_parallizer.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/multi_agent_collab.py` & `swarms-4.7.3/swarms/structs/multi_agent_collab.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/multi_process_workflow.py` & `swarms-4.7.3/swarms/structs/multi_process_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/multi_threaded_workflow.py` & `swarms-4.7.3/swarms/structs/multi_threaded_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/nonlinear_workflow.py` & `swarms-4.7.3/swarms/structs/nonlinear_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/plan.py` & `swarms-4.7.3/swarms/structs/plan.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/rearrange.py` & `swarms-4.7.3/swarms/structs/rearrange.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/recursive_workflow.py` & `swarms-4.7.3/swarms/structs/recursive_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/schemas.py` & `swarms-4.7.3/swarms/structs/schemas.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/sequential_workflow.py` & `swarms-4.7.3/swarms/structs/sequential_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/sermon_swarm.py` & `swarms-4.7.3/swarms/structs/sermon_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/stackoverflow_swarm.py` & `swarms-4.7.3/swarms/structs/stackoverflow_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/step.py` & `swarms-4.7.3/swarms/structs/step.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/swarm_net.py` & `swarms-4.7.3/swarms/structs/swarm_net.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/swarm_redis_registry.py` & `swarms-4.7.3/swarms/structs/swarm_redis_registry.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/swarming_architectures.py` & `swarms-4.7.3/swarms/structs/swarming_architectures.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/task.py` & `swarms-4.7.3/swarms/structs/task.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/task_queue_base.py` & `swarms-4.7.3/swarms/structs/task_queue_base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/team.py` & `swarms-4.7.3/swarms/structs/team.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/structs/utils.py` & `swarms-4.7.3/swarms/structs/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/telemetry/__init__.py` & `swarms-4.7.3/swarms/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/telemetry/auto_upgrade_swarms.py` & `swarms-4.7.3/swarms/telemetry/auto_upgrade_swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/telemetry/check_update.py` & `swarms-4.7.3/swarms/telemetry/check_update.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/telemetry/log_all.py` & `swarms-4.7.3/swarms/telemetry/log_all.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/telemetry/sys_info.py` & `swarms-4.7.3/swarms/telemetry/sys_info.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/telemetry/user_utils.py` & `swarms-4.7.3/swarms/telemetry/user_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/tools/__init__.py` & `swarms-4.7.3/swarms/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/tools/code_executor.py` & `swarms-4.7.3/swarms/tools/code_executor.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/tools/exec_tool.py` & `swarms-4.7.3/swarms/tools/exec_tool.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/tools/format_tools.py` & `swarms-4.7.3/swarms/tools/format_tools.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/tools/logits_processor.py` & `swarms-4.7.3/swarms/tools/logits_processor.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/tools/tool_utils.py` & `swarms-4.7.3/swarms/tools/tool_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/README.md` & `swarms-4.7.3/swarms/utils/README.md`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/__init__.py` & `swarms-4.7.3/swarms/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/apa.py` & `swarms-4.7.3/swarms/utils/apa.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/check_function_result.py` & `swarms-4.7.3/swarms/utils/check_function_result.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/class_args_wrapper.py` & `swarms-4.7.3/swarms/utils/class_args_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/code_interpreter.py` & `swarms-4.7.3/swarms/utils/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/concurrent_utils.py` & `swarms-4.7.3/swarms/utils/concurrent_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/csv_and_pandas.py` & `swarms-4.7.3/swarms/utils/csv_and_pandas.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/data_to_text.py` & `swarms-4.7.3/swarms/utils/data_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/decorators.py` & `swarms-4.7.3/swarms/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/device_checker_cuda.py` & `swarms-4.7.3/swarms/utils/device_checker_cuda.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/disable_logging.py` & `swarms-4.7.3/swarms/utils/disable_logging.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/download_img.py` & `swarms-4.7.3/swarms/utils/download_img.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/download_weights_from_url.py` & `swarms-4.7.3/swarms/utils/download_weights_from_url.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/execute_futures.py` & `swarms-4.7.3/swarms/utils/execute_futures.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/execution_sandbox.py` & `swarms-4.7.3/swarms/utils/execution_sandbox.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/exponential_backoff.py` & `swarms-4.7.3/swarms/utils/exponential_backoff.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/fetch_init_params.py` & `swarms-4.7.3/swarms/utils/fetch_init_params.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/file_processing.py` & `swarms-4.7.3/swarms/utils/file_processing.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/find_img_path.py` & `swarms-4.7.3/swarms/utils/find_img_path.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/function_calling_utils.py` & `swarms-4.7.3/swarms/utils/function_calling_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/get_logger.py` & `swarms-4.7.3/swarms/utils/get_logger.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/inference_convert_utils.py` & `swarms-4.7.3/swarms/utils/inference_convert_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/json_output_parser.py` & `swarms-4.7.3/swarms/utils/json_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/json_utils.py` & `swarms-4.7.3/swarms/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/jsonl_utils.py` & `swarms-4.7.3/swarms/utils/jsonl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/llm_metrics_decorator.py` & `swarms-4.7.3/swarms/utils/llm_metrics_decorator.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/load_model_torch.py` & `swarms-4.7.3/swarms/utils/load_model_torch.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/logger.py` & `swarms-4.7.3/swarms/utils/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/loggers.py` & `swarms-4.7.3/swarms/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/main.py` & `swarms-4.7.3/swarms/utils/main.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/markdown_message.py` & `swarms-4.7.3/swarms/utils/markdown_message.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/math_eval.py` & `swarms-4.7.3/swarms/utils/math_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/pandas_to_str.py` & `swarms-4.7.3/swarms/utils/pandas_to_str.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/parse_code.py` & `swarms-4.7.3/swarms/utils/parse_code.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/pdf_to_text.py` & `swarms-4.7.3/swarms/utils/pdf_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/prep_torch_model_inference.py` & `swarms-4.7.3/swarms/utils/prep_torch_model_inference.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/remove_json_whitespace.py` & `swarms-4.7.3/swarms/utils/remove_json_whitespace.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/save_logs.py` & `swarms-4.7.3/swarms/utils/save_logs.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/serializable.py` & `swarms-4.7.3/swarms/utils/serializable.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/supervision_visualizer.py` & `swarms-4.7.3/swarms/utils/supervision_visualizer.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/try_except_wrapper.py` & `swarms-4.7.3/swarms/utils/try_except_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/swarms/utils/yaml_output_parser.py` & `swarms-4.7.3/swarms/utils/yaml_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-4.7.1/setup.py` & `swarms-4.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['swarms',
  'swarms.agents',
  'swarms.artifacts',
- 'swarms.cli',
  'swarms.memory',
  'swarms.models',
  'swarms.prompts',
  'swarms.structs',
  'swarms.telemetry',
  'swarms.tools',
  'swarms.utils']
@@ -34,29 +33,25 @@
  'rich==13.5.2',
  'sentry-sdk',
  'tenacity==8.2.3',
  'toml',
  'torch>=2.1.1,<3.0',
  'transformers>=4.39.0,<5.0.0']
 
-entry_points = \
-{'console_scripts': ['swarms = swarms.cli._cli:main']}
-
 setup_kwargs = {
     'name': 'swarms',
-    'version': '4.7.1',
+    'version': '4.7.3',
     'description': 'Swarms - Pytorch',
     'long_description': '![Swarming banner icon](images/swarmslogobanner.png)\n\n<div align="center">\n\nOrchestrate swarms of agents for production-grade applications.\n\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/swarms)](https://libraries.io/github/kyegomez/swarms) [![Downloads](https://static.pepy.tech/badge/swarms/month)](https://pepy.tech/project/swarms)\n\n[![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)\n\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)\n\n</div>\n\nIndividual agents are barely being deployd into production because of 5 suffocating challanges: short memory, single task threading, hallucinations, high cost, and lack of collaboration.  With Multi-agent collaboration, you can effectively eliminate all of these issues. Swarms provides you with simple, reliable, and agile primitives to build your own Swarm for your specific use case. Now, Swarms is being used in production by RBC, John Deere, and many AI startups. To learn more about the unparalled benefits about multi-agent collaboration check out this github repository for research papers or book a call with me!\n\n----\n\n## Install\n`pip3 install -U swarms`\n\n---\n\n## Usage\n\n\nRun example in Collab: <a target="_blank" href="https://colab.research.google.com/github/kyegomez/swarms/blob/master/playground/swarms_example.ipynb">\n<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n\n### `Agent`\nA fully plug-and-play autonomous agent powered by an LLM extended by a long-term memory database, and equipped with function calling for tool usage! By passing in an LLM, you can create a fully autonomous agent with extreme customization and reliability, ready for real-world task automation!\n\nFeatures:\n\n✅ Any LLM / Any framework\n\n✅ Extremely customize-able with max loops, autosaving, import docs (PDFS, TXT, CSVs, etc), tool usage, etc etc\n\n✅ Long term memory database with RAG (ChromaDB, Pinecone, Qdrant)\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, autosave=True, dashboard=True)\n\n# Run the workflow on a task\nagent.run("Generate a 10,000 word blog on health and wellness.")\n```\n\n\n### `ToolAgent`\nToolAgent is an agent that can use tools through JSON function calling. It intakes any open source model from huggingface and is extremely modular and plug in and play. We need help adding general support to all models soon.\n\n\n```python\nfrom pydantic import BaseModel, Field\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nfrom swarms import ToolAgent\nfrom swarms.utils.json_utils import base_model_to_json\n\n# Load the pre-trained model and tokenizer\nmodel = AutoModelForCausalLM.from_pretrained(\n    "databricks/dolly-v2-12b",\n    load_in_4bit=True,\n    device_map="auto",\n)\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = base_model_to_json(Schema)\n\n# Define the task to generate a person\'s information\ntask = (\n    "Generate a person\'s information based on the following schema:"\n)\n\n# Create an instance of the ToolAgent class\nagent = ToolAgent(\n    name="dolly-function-agent",\n    description="Ana gent to create a child data",\n    model=model,\n    tokenizer=tokenizer,\n    json_schema=tool_schema,\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n```\n\n\n### `Worker`\nThe `Worker` is a simple all-in-one agent equipped with an LLM, tools, and RAG for low level tasks.\n\n✅ Plug in and Play LLM. Utilize any LLM from anywhere and any framework\n\n✅ Reliable RAG: Utilizes FAISS for efficient RAG but it\'s modular so you can use any DB.\n\n✅ Multi-Step Parallel Function Calling: Use any tool\n\n```python\n# Importing necessary modules\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import OpenAIChat, Worker, tool\n\n# Loading environment variables from .env file\nload_dotenv()\n\n# Retrieving the OpenAI API key from environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Create a tool\n@tool\ndef search_api(query: str):\n    pass\n\n\n# Creating a Worker instance\nworker = Worker(\n    name="My Worker",\n    role="Worker",\n    human_in_the_loop=False,\n    tools=[search_api],\n    temperature=0.5,\n    llm=OpenAIChat(openai_api_key=api_key),\n)\n\n# Running the worker with a prompt\nout = worker.run("Hello, how are you? Create an image of how your are doing!")\n\n# Printing the output\nprint(out)\n```\n\n------\n\n\n# `Agent` with Long Term Memory\n`Agent` equipped with quasi-infinite long term memory. Great for long document understanding, analysis, and retrieval.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n# `Agent` with Long Term Memory ++ Tools!\nAn LLM equipped with long term memory and tools, a full stack agent capable of automating all and any digital tasks given a good prompt.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat, tool\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initialize a tool\n@tool\ndef search_api(query: str):\n    # Add your logic here\n    return query\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n    tools=[search_api],\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n\n\n\n\n\n\n----\n\n### `SequentialWorkflow`\nSequential Workflow enables you to sequentially execute tasks with `Agent` and then pass the output into the next agent and onwards until you have specified your max loops. `SequentialWorkflow` is wonderful for real-world business tasks like sending emails, summarizing documents, and analyzing data.\n\n\n✅  Save and Restore Workflow states!\n\n✅  Multi-Modal Support for Visual Chaining\n\n✅  Utilizes Agent class\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, SequentialWorkflow\n\nload_dotenv()\n\n# Load the environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Initialize the language agent\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n# Initialize the agent with the language agent\nagent1 = Agent(llm=llm, max_loops=1)\n\n# Create another agent for a different task\nagent2 = Agent(llm=llm, max_loops=1)\n\n# Create another agent for a different task\nagent3 = Agent(llm=llm, max_loops=1)\n\n# Create the workflow\nworkflow = SequentialWorkflow(max_loops=1)\n\n# Add tasks to the workflow\nworkflow.add(\n    agent1,\n    "Generate a 10,000 word blog on health and wellness.",\n)\n\n# Suppose the next task takes the output of the first task as input\nworkflow.add(\n    agent2,\n    "Summarize the generated blog",\n)\n\n# Run the workflow\nworkflow.run()\n\n# Output the results\nfor task in workflow.tasks:\n    print(f"Task: {task.description}, Result: {task.result}")\n```\n\n\n\n### `ConcurrentWorkflow`\n`ConcurrentWorkflow` runs all the tasks all at the same time with the inputs you give it!\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, ConcurrentWorkflow, OpenAIChat, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = ConcurrentWorkflow(max_workers=5)\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(tasks=[task1, task2, task3])\n\n# Run the workflow\nworkflow.run()\n```\n\n### `RecursiveWorkflow`\n`RecursiveWorkflow` will keep executing the tasks until a specific token like <DONE> is located inside the text!\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, RecursiveWorkflow, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = RecursiveWorkflow(stop_token="<DONE>")\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(task1)\nworkflow.add(task2)\nworkflow.add(task3)\n\n# Run the workflow\nworkflow.run()\n```\n\n\n\n### `ModelParallelizer`\nThe ModelParallelizer allows you to run multiple models concurrently, comparing their outputs. This feature enables you to easily compare the performance and results of different models, helping you make informed decisions about which model to use for your specific task.\n\nPlug-and-Play Integration: The structure provides a seamless integration with various models, including OpenAIChat, Anthropic, Mixtral, and Gemini. You can easily plug in any of these models and start using them without the need for extensive modifications or setup.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Anthropic, Gemini, Mixtral, ModelParallelizer, OpenAIChat\n\nload_dotenv()\n\n# API Keys\nanthropic_api_key = os.getenv("ANTHROPIC_API_KEY")\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Initialize the models\nllm = OpenAIChat(openai_api_key=openai_api_key)\nanthropic = Anthropic(anthropic_api_key=anthropic_api_key)\nmixtral = Mixtral()\ngemini = Gemini(gemini_api_key=gemini_api_key)\n\n# Initialize the parallelizer\nllms = [llm, anthropic, mixtral, gemini]\nparallelizer = ModelParallelizer(llms)\n\n# Set the task\ntask = "Generate a 10,000 word blog on health and wellness."\n\n# Run the task\nout = parallelizer.run(task)\n\n# Print the responses 1 by 1\nfor i in range(len(out)):\n    print(f"Response from LLM {i}: {out[i]}")\n```\n\n\n### Simple Conversational Agent\nA Plug in and play conversational agent with `GPT4`, `Mixytral`, or any of our models\n\n- Reliable conversational structure to hold messages together with dynamic handling for long context conversations and interactions with auto chunking\n- Reliable, this simple system will always provide responses you want.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Conversation, OpenAIChat\n\nconv = Conversation(\n    time_enabled=True,\n)\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(openai_api_key=api_key, model_name="gpt-4")\n\n\n# Run the language model in a loop\ndef interactive_conversation(llm):\n    conv = Conversation()\n    while True:\n        user_input = input("User: ")\n        conv.add("user", user_input)\n        if user_input.lower() == "quit":\n            break\n        task = conv.return_history_as_string()  # Get the conversation history\n        out = llm(task)\n        conv.add("assistant", out)\n        print(\n            f"Assistant: {out}",\n        )\n    conv.display_conversation()\n    conv.export_conversation("conversation.txt")\n\n\n# Replace with your LLM instance\ninteractive_conversation(llm)\n```\n\n\n### `SwarmNetwork`\n`SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.\n\n✅ Efficient Task Management: SwarmNetwork\'s intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.\n\n✅ Scalability: SwarmNetwork can dynamically scale the number of agents based on the number of pending tasks. This means it can handle an increase in workload by adding more agents, and conserve resources when the workload is low by reducing the number of agents.\n\n✅ Versatile Deployment Options: With SwarmNetwork, each agent can be run on its own thread, process, container, machine, or even cluster. This provides a high degree of flexibility and allows for deployment that best suits the user\'s needs and infrastructure.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat, SwarmNetwork\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5,\n    openai_api_key=api_key,\n)\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, agent_name="Social Media Manager")\nagent2 = Agent(llm=llm, max_loops=1, agent_name=" Product Manager")\nagent3 = Agent(llm=llm, max_loops=1, agent_name="SEO Manager")\n\n\n# Load the swarmnet with the agents\nswarmnet = SwarmNetwork(\n    agents=[agent, agent2, agent3],\n)\n\n# List the agents in the swarm network\nout = swarmnet.list_agents()\nprint(out)\n\n# Run the workflow on a task\nout = swarmnet.run_single_agent(\n    agent2.id, "Generate a 10,000 word blog on health and wellness."\n)\nprint(out)\n\n\n# Run all the agents in the swarm network on a task\nout = swarmnet.run_many_agents("Generate a 10,000 word blog on health and wellness.")\nprint(out)\n```\n\n\n### `Task`\n`Task` is a simple structure for task execution with the `Agent`. Imagine zapier for LLM-based workflow automation\n\n✅ Task is a structure for task execution with the Agent. \n\n✅ Tasks can have descriptions, scheduling, triggers, actions, conditions, dependencies, priority, and a history. \n\n✅ The Task structure allows for efficient workflow automation with LLM-based agents.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.structs import Agent, OpenAIChat, Task\n\n# Load the environment variables\nload_dotenv()\n\n\n# Define a function to be used as the action\ndef my_action():\n    print("Action executed")\n\n\n# Define a function to be used as the condition\ndef my_condition():\n    print("Condition checked")\n    return True\n\n\n# Create an agent\nagent = Agent(\n    llm=OpenAIChat(openai_api_key=os.environ["OPENAI_API_KEY"]),\n    max_loops=1,\n    dashboard=False,\n)\n\n# Create a task\ntask = Task(\n    description=(\n        "Generate a report on the top 3 biggest expenses for small"\n        " businesses and how businesses can save 20%"\n    ),\n    agent=agent,\n)\n\n# Set the action and condition\ntask.set_action(my_action)\ntask.set_condition(my_condition)\n\n# Execute the task\nprint("Executing task...")\ntask.run()\n\n# Check if the task is completed\nif task.is_completed():\n    print("Task completed")\nelse:\n    print("Task not completed")\n\n# Output the result of the task\nprint(f"Task result: {task.result}")\n```\n\n---\n\n\n\n### `BlockList`\n- Modularity and Flexibility: BlocksList allows users to create custom swarms by adding or removing different classes or functions as blocks. This means users can easily tailor the functionality of their swarm to suit their specific needs.\n\n- Ease of Management: With methods to add, remove, update, and retrieve blocks, BlocksList provides a straightforward way to manage the components of a swarm. This makes it easier to maintain and update the swarm over time.\n\n- Enhanced Searchability: BlocksList offers methods to get blocks by various attributes such as name, type, ID, and parent-related properties. This makes it easier for users to find and work with specific blocks in a large and complex swarm.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\nfrom pydantic import BaseModel\nfrom swarms import BlocksList, Gemini, GPT4VisionAPI, Mixtral, OpenAI, ToolAgent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the environment variables\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Tool Agent\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n# Convert the schema to a JSON string\njson_schema = base_model_to_json(Schema)\n\n\ntoolagent = ToolAgent(model=model, tokenizer=tokenizer, json_schema=json_schema)\n\n# Blocks List which enables you to build custom swarms by adding classes or functions\nswarm = BlocksList(\n    "SocialMediaSwarm",\n    "A swarm of social media agents",\n    [\n        OpenAI(openai_api_key=openai_api_key),\n        Mixtral(),\n        GPT4VisionAPI(openai_api_key=openai_api_key),\n        Gemini(gemini_api_key=gemini_api_key),\n    ],\n)\n\n\n# Add the new block to the swarm\nswarm.add(toolagent)\n\n# Remove a block from the swarm\nswarm.remove(toolagent)\n\n# Update a block in the swarm\nswarm.update(toolagent)\n\n# Get a block at a specific index\nblock_at_index = swarm.get(0)\n\n# Get all blocks in the swarm\nall_blocks = swarm.get_all()\n\n# Get blocks by name\nopenai_blocks = swarm.get_by_name("OpenAI")\n\n# Get blocks by type\ngpt4_blocks = swarm.get_by_type("GPT4VisionAPI")\n\n# Get blocks by ID\nblock_by_id = swarm.get_by_id(toolagent.id)\n\n# Get blocks by parent\nblocks_by_parent = swarm.get_by_parent(swarm)\n\n# Get blocks by parent ID\nblocks_by_parent_id = swarm.get_by_parent_id(swarm.id)\n\n# Get blocks by parent name\nblocks_by_parent_name = swarm.get_by_parent_name(swarm.name)\n\n# Get blocks by parent type\nblocks_by_parent_type = swarm.get_by_parent_type(type(swarm).__name__)\n\n# Get blocks by parent description\nblocks_by_parent_description = swarm.get_by_parent_description(swarm.description)\n\n# Run the block in the swarm\ninference = swarm.run_block(toolagent, "Hello World")\nprint(inference)\n```\n\n\n## Majority Voting\nMultiple-agents will evaluate an idea based off of an parsing or evaluation function. From papers like "[More agents is all you need](https://arxiv.org/pdf/2402.05120.pdf)\n\n```python\nfrom swarms import Agent, MajorityVoting, ChromaDB, Anthropic\n\n# Initialize the llm\nllm = Anthropic()\n\n# Agents\nagent1 = Agent(\n    llm = llm,\n    system_prompt="You are the leader of the Progressive Party. What is your stance on healthcare?",\n    agent_name="Progressive Leader",\n    agent_description="Leader of the Progressive Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent2 = Agent(\n    llm=llm,\n    agent_name="Conservative Leader",\n    agent_description="Leader of the Conservative Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent3 = Agent(\n    llm=llm,\n    agent_name="Libertarian Leader",\n    agent_description="Leader of the Libertarian Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\n# Initialize the majority voting\nmv = MajorityVoting(\n    agents=[agent1, agent2, agent3],\n    output_parser=llm.majority_voting,\n    autosave=False,\n    verbose=True,\n)\n\n\n# Start the majority voting\nmv.run("What is your stance on healthcare?")\n```\n\n## Real-World Deployment\n\n### Multi-Agent Swarm for Logistics\nHere\'s a production grade swarm ready for real-world deployment in a factory and logistics settings like warehouses. This swarm can automate 3 costly and inefficient workflows, safety checks, productivity checks, and warehouse security.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models import GPT4VisionAPI\nfrom swarms.prompts.logistics import (\n    Efficiency_Agent_Prompt,\n    Health_Security_Agent_Prompt,\n    Productivity_Agent_Prompt,\n    Quality_Control_Agent_Prompt,\n    Safety_Agent_Prompt,\n    Security_Agent_Prompt,\n    Sustainability_Agent_Prompt,\n)\nfrom swarms.structs import Agent\n\n# Load ENV\nload_dotenv()\napi_key = os.getenv("OPENAI_API_KEY")\n\n# GPT4VisionAPI\nllm = GPT4VisionAPI(openai_api_key=api_key)\n\n# Image for analysis\nfactory_image = "factory_image1.jpg"\n\n# Initialize agents with respective prompts\nhealth_security_agent = Agent(\n    llm=llm,\n    sop=Health_Security_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Quality control agent\nquality_control_agent = Agent(\n    llm=llm,\n    sop=Quality_Control_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Productivity Agent\nproductivity_agent = Agent(\n    llm=llm,\n    sop=Productivity_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Initiailize safety agent\nsafety_agent = Agent(llm=llm, sop=Safety_Agent_Prompt, max_loops=1, multi_modal=True)\n\n# Init the security agent\nsecurity_agent = Agent(\n    llm=llm, sop=Security_Agent_Prompt, max_loops=1, multi_modal=True\n)\n\n\n# Initialize sustainability agent\nsustainability_agent = Agent(\n    llm=llm,\n    sop=Sustainability_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Initialize efficincy agent\nefficiency_agent = Agent(\n    llm=llm,\n    sop=Efficiency_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Run agents with respective tasks on the same image\nhealth_analysis = health_security_agent.run(\n    "Analyze the safety of this factory", factory_image\n)\nquality_analysis = quality_control_agent.run(\n    "Examine product quality in the factory", factory_image\n)\nproductivity_analysis = productivity_agent.run(\n    "Evaluate factory productivity", factory_image\n)\nsafety_analysis = safety_agent.run(\n    "Inspect the factory\'s adherence to safety standards",\n    factory_image,\n)\nsecurity_analysis = security_agent.run(\n    "Assess the factory\'s security measures and systems",\n    factory_image,\n)\nsustainability_analysis = sustainability_agent.run(\n    "Examine the factory\'s sustainability practices", factory_image\n)\nefficiency_analysis = efficiency_agent.run(\n    "Analyze the efficiency of the factory\'s manufacturing process",\n    factory_image,\n)\n```\n---\n\n\n## `Multi Modal Autonomous Agents`\nRun the agent with multiple modalities useful for various real-world tasks in manufacturing, logistics, and health.\n\n```python\n# Description: This is an example of how to use the Agent class to run a multi-modal workflow\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models.gpt4_vision_api import GPT4VisionAPI\nfrom swarms.structs import Agent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = GPT4VisionAPI(\n    openai_api_key=api_key,\n    max_tokens=500,\n)\n\n# Initialize the task\ntask = (\n    "Analyze this image of an assembly line and identify any issues such as"\n    " misaligned parts, defects, or deviations from the standard assembly"\n    " process. IF there is anything unsafe in the image, explain why it is"\n    " unsafe and how it could be improved."\n)\nimg = "assembly_line.jpg"\n\n## Initialize the workflow\nagent = Agent(\n    llm=llm, max_loops="auto", autosave=True, dashboard=True, multi_modal=True\n)\n\n# Run the workflow on a task\nagent.run(task=task, img=img)\n```\n----\n\n\n## Build your own LLMs, Agents, and Swarms!\n\n### Swarms Compliant Model Interface\n```python\nfrom swarms import AbstractLLM\n\nclass vLLMLM(AbstractLLM):\n    def __init__(self, model_name=\'default_model\', tensor_parallel_size=1, *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.model_name = model_name\n        self.tensor_parallel_size = tensor_parallel_size\n        # Add any additional initialization here\n    \n    def run(self, task: str):\n        pass\n\n# Example\nmodel = vLLMLM("mistral")\n\n# Run the model\nout = model("Analyze these financial documents and summarize of them")\nprint(out)\n\n```\n\n\n### Swarms Compliant Agent Interface\n\n```python\nfrom swarms import Agent\n\n\nclass MyCustomAgent(Agent):\n\n\xa0 \xa0 def __init__(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 super().__init__(*args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Custom initialization logic\n\n\xa0 \xa0 def custom_method(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Implement custom logic here\n\n\xa0 \xa0 \xa0 \xa0 pass\n\n\xa0 \xa0 def run(self, task, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Customize the run method\n\n\xa0 \xa0 \xa0 \xa0 response = super().run(task, *args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Additional custom logic\n\n\xa0 \xa0 \xa0 \xa0 return response`\n\n# Model\nagent = MyCustomAgent()\n\n# Run the agent\nout = agent("Analyze and summarize these financial documents: ")\nprint(out)\n\n```\n\n\n### Compliant Interface for Multi-Agent Collaboration\n\n```python\nfrom swarms import AutoSwarm, AutoSwarmRouter, BaseSwarm\n\n\n# Build your own Swarm\nclass MySwarm(BaseSwarm):\n    def __init__(self, name="kyegomez/myswarm", *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.name = name\n\n    def run(self, task: str, *args, **kwargs):\n        # Add your multi-agent logic here\n        # agent 1\n        # agent 2\n        # agent 3\n        return "output of the swarm"\n\n\n# Add your custom swarm to the AutoSwarmRouter\nrouter = AutoSwarmRouter(\n    swarms=[MySwarm]\n)\n\n\n# Create an AutoSwarm instance\nautoswarm = AutoSwarm(\n    name="kyegomez/myswarm",\n    description="A simple API to build and run swarms",\n    verbose=True,\n    router=router,\n)\n\n\n# Run the AutoSwarm\nautoswarm.run("Analyze these financial data and give me a summary")\n\n\n```\n\n---\n\n## Documentation\nDocumentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)\n\n----\n\n## 🫶 Contributions:\n\nThe easiest way to contribute is to pick any issue with the `good first issue` tag 💪. Read the Contributing guidelines [here](/CONTRIBUTING.md). Bug Report? [File here](https://github.com/swarms/gateway/issues) | Feature Request? [File here](https://github.com/swarms/gateway/issues)\n\nSwarms is an open-source project, and contributions are VERY welcome. If you want to contribute, you can create new features, fix bugs, or improve the infrastructure. Please refer to the [CONTRIBUTING.md](https://github.com/kyegomez/swarms/blob/master/CONTRIBUTING.md) and our [contributing board](https://github.com/users/kyegomez/projects/1) to participate in Roadmap discussions!\n\n<a href="https://github.com/kyegomez/swarms/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=kyegomez/swarms" />\n</a>\n\n----\n\n## Community\n\nJoin our growing community around the world, for real-time support, ideas, and discussions on Swarms 😊 \n\n- View our official [Blog](https://swarms.apac.ai)\n- Chat live with us on [Discord](https://discord.gg/kS3rwKs3ZC)\n- Follow us on [Twitter](https://twitter.com/kyegomez)\n- Connect with us on [LinkedIn](https://www.linkedin.com/company/the-swarm-corporation)\n- Visit us on [YouTube](https://www.youtube.com/channel/UC9yXyitkbU_WSy7bd_41SqQ)\n- [Join the Swarms community on Discord!](https://discord.gg/AJazBmhKnr)\n- Join our Swarms Community Gathering every Thursday at 1pm NYC Time to unlock the potential of autonomous agents in automating your daily tasks [Sign up here](https://lu.ma/5p2jnc2v)\n\n---\n\n## Discovery Call\nBook a discovery call to learn how Swarms can lower your operating costs by 40% with swarms of autonomous agents in lightspeed. [Click here to book a time that works for you!](https://calendly.com/swarm-corp/30min?month=2023-11)\n\n\n\n## Accelerate Backlog\nHelp us accelerate our backlog by supporting us financially! Note, we\'re an open source corporation and so all the revenue we generate is through donations at the moment ;)\n\n<a href="https://polar.sh/kyegomez"><img src="https://polar.sh/embed/fund-our-backlog.svg?org=kyegomez" /></a>\n\n\n## File Structure\nThe swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs`\xa0that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.\n\n```sh\n├── __init__.py\n├── agents\n├── artifacts\n├── chunkers\n├── cli\n├── loaders\n├── memory\n├── models\n├── prompts\n├── structs\n├── telemetry\n├── tokenizers\n├── tools\n├── utils\n└── workers\n```\n\n## Docker Instructions\n\nThis application uses Docker with CUDA support. To build and run the Docker container, follow these steps:\n\n### Prerequisites\n\n- Make sure you have [Docker installed](https://docs.docker.com/get-docker/) on your machine.\n- Ensure your machine has an NVIDIA GPU and [NVIDIA Docker support](https://github.com/NVIDIA/nvidia-docker) installed.\n\n### Building the Docker Image\n\nTo build the Docker image, navigate to the root directory containing the `Dockerfile` and run the following command:\n\n```bash\ndocker build --gpus all -t swarms\n``` \n### Running the Docker Container\nTo run the Docker container, use the following command:\n\n`docker run --gpus all -p 4000:80 swarms`\n\nReplace swarms with the name of your Docker image, and replace 4000:80 with your actual port mapping. The format is hostPort:containerPort.\n\nNow, your application should be running with CUDA support!\n\n\n## Swarm Newsletter 🤖 🤖 🤖 📧 \nSign up to the Swarm newsletter to receive  updates on the latest Autonomous agent research papers, step by step guides on creating multi-agent app, and much more Swarmie goodiness 😊\n\n\n[CLICK HERE TO SIGNUP](https://docs.google.com/forms/d/e/1FAIpQLSfqxI2ktPR9jkcIwzvHL0VY6tEIuVPd-P2fOWKnd6skT9j1EQ/viewform?usp=sf_link)\n\n# License\nApache License\n\n\n\n',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/swarms',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'entry_points': entry_points,
     'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `swarms-4.7.1/PKG-INFO` & `swarms-4.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 4.7.1
+Version: 4.7.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering,swarms,agents
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.9,<4.0
```

