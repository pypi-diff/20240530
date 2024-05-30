# Comparing `tmp/swarms-5.0.8.tar.gz` & `tmp/swarms-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-5.0.8.tar", max compression
+gzip compressed data, was "swarms-5.1.3.tar", max compression
```

## Comparing `swarms-5.0.8.tar` & `swarms-5.1.3.tar`

### file list

```diff
@@ -1,213 +1,219 @@
--rw-r--r--   0        0        0    15674 2024-05-20 23:12:19.525914 swarms-5.0.8/LICENSE
--rw-r--r--   0        0        0    33743 2024-05-25 00:26:35.052802 swarms-5.0.8/README.md
--rw-r--r--   0        0        0     1790 2024-05-27 04:35:03.351567 swarms-5.0.8/pyproject.toml
--rw-r--r--   0        0        0      590 2024-05-20 23:12:19.584595 swarms-5.0.8/swarms/__init__.py
--rw-r--r--   0        0        0      864 2024-05-20 23:12:19.584679 swarms-5.0.8/swarms/agents/__init__.py
--rw-r--r--   0        0        0      881 2024-05-20 23:12:19.584738 swarms-5.0.8/swarms/agents/agent_wrapper.py
--rw-r--r--   0        0        0     3342 2024-05-20 23:12:19.584796 swarms-5.0.8/swarms/agents/base.py
--rw-r--r--   0        0        0     4201 2024-05-20 23:12:19.584880 swarms-5.0.8/swarms/agents/developer_agents.py
--rw-r--r--   0        0        0     2950 2024-05-20 23:12:19.584947 swarms-5.0.8/swarms/agents/omni_modal_agent.py
--rw-r--r--   0        0        0     3491 2024-05-20 23:12:19.585001 swarms-5.0.8/swarms/agents/simple_agent.py
--rw-r--r--   0        0        0      484 2024-05-20 23:12:19.585048 swarms-5.0.8/swarms/agents/stopping_conditions.py
--rw-r--r--   0        0        0     4940 2024-05-20 23:12:19.585129 swarms-5.0.8/swarms/agents/tool_agent.py
--rw-r--r--   0        0        0     5504 2024-05-20 23:12:19.585192 swarms-5.0.8/swarms/agents/worker_agent.py
--rw-r--r--   0        0        0      167 2024-05-20 23:12:19.585283 swarms-5.0.8/swarms/artifacts/__init__.py
--rw-r--r--   0        0        0     1675 2024-05-20 23:12:19.585343 swarms-5.0.8/swarms/artifacts/base_artifact.py
--rw-r--r--   0        0        0     2299 2024-05-20 23:12:19.585425 swarms-5.0.8/swarms/artifacts/text_artifact.py
--rw-r--r--   0        0        0      613 2024-05-20 23:12:19.585515 swarms-5.0.8/swarms/memory/__init__.py
--rw-r--r--   0        0        0      433 2024-05-20 23:12:19.585565 swarms-5.0.8/swarms/memory/action_subtask.py
--rw-r--r--   0        0        0     3475 2024-05-20 23:12:19.585621 swarms-5.0.8/swarms/memory/base_db.py
--rw-r--r--   0        0        0     2823 2024-05-20 23:12:19.585702 swarms-5.0.8/swarms/memory/base_vectordb.py
--rw-r--r--   0        0        0     2895 2024-05-20 23:12:19.585767 swarms-5.0.8/swarms/memory/dict_internal_memory.py
--rw-r--r--   0        0        0     3306 2024-05-20 23:12:19.585826 swarms-5.0.8/swarms/memory/dict_shared_memory.py
--rw-r--r--   0        0        0     5499 2024-05-20 23:12:19.585895 swarms-5.0.8/swarms/memory/short_term_memory.py
--rw-r--r--   0        0        0     3371 2024-05-20 23:12:19.585978 swarms-5.0.8/swarms/memory/visual_memory.py
--rw-r--r--   0        0        0     2392 2024-05-21 05:06:54.045652 swarms-5.0.8/swarms/models/__init__.py
--rw-r--r--   0        0        0     2052 2024-05-21 00:48:59.027928 swarms-5.0.8/swarms/models/base_embedding_model.py
--rw-r--r--   0        0        0    13168 2024-05-20 23:12:19.586207 swarms-5.0.8/swarms/models/base_llm.py
--rw-r--r--   0        0        0    12604 2024-05-20 23:12:19.586302 swarms-5.0.8/swarms/models/base_multimodal_model.py
--rw-r--r--   0        0        0     2475 2024-05-20 23:12:19.586361 swarms-5.0.8/swarms/models/base_tts.py
--rw-r--r--   0        0        0     3163 2024-05-20 23:12:19.586416 swarms-5.0.8/swarms/models/base_ttv.py
--rw-r--r--   0        0        0    16743 2024-05-20 23:12:19.586490 swarms-5.0.8/swarms/models/cog_vlm.py
--rw-r--r--   0        0        0    10760 2024-05-20 23:12:19.586608 swarms-5.0.8/swarms/models/dalle3.py
--rw-r--r--   0        0        0     6449 2024-05-20 23:12:19.586690 swarms-5.0.8/swarms/models/distilled_whisperx.py
--rw-r--r--   0        0        0      682 2024-05-20 23:12:19.586747 swarms-5.0.8/swarms/models/embeddings_base.py
--rw-r--r--   0        0        0     3022 2024-05-20 23:12:19.586804 swarms-5.0.8/swarms/models/fuyu.py
--rw-r--r--   0        0        0     7762 2024-05-20 23:12:19.586891 swarms-5.0.8/swarms/models/gemini.py
--rw-r--r--   0        0        0    14236 2024-05-20 23:12:19.586973 swarms-5.0.8/swarms/models/gpt4_vision_api.py
--rw-r--r--   0        0        0    12996 2024-05-20 23:12:19.587047 swarms-5.0.8/swarms/models/huggingface.py
--rw-r--r--   0        0        0     1826 2024-05-20 23:12:19.587108 swarms-5.0.8/swarms/models/huggingface_pipeline.py
--rw-r--r--   0        0        0     5601 2024-05-20 23:12:19.587202 swarms-5.0.8/swarms/models/idefics.py
--rw-r--r--   0        0        0    10672 2024-05-20 23:12:19.587276 swarms-5.0.8/swarms/models/kosmos_two.py
--rw-r--r--   0        0        0     1448 2024-05-20 23:12:19.587347 swarms-5.0.8/swarms/models/layoutlm_document_qa.py
--rw-r--r--   0        0        0     2599 2024-05-21 05:06:21.835242 swarms-5.0.8/swarms/models/llama3_hosted.py
--rw-r--r--   0        0        0     6581 2024-05-20 23:12:19.587506 swarms-5.0.8/swarms/models/llama_function_caller.py
--rw-r--r--   0        0        0     2762 2024-05-20 23:12:19.587573 swarms-5.0.8/swarms/models/llava.py
--rw-r--r--   0        0        0     2056 2024-05-20 23:12:19.587792 swarms-5.0.8/swarms/models/moondream_mm.py
--rw-r--r--   0        0        0     2881 2024-05-20 23:12:19.587858 swarms-5.0.8/swarms/models/nougat.py
--rw-r--r--   0        0        0     2366 2024-05-20 23:12:19.587917 swarms-5.0.8/swarms/models/open_dalle.py
--rw-r--r--   0        0        0     2464 2024-05-20 23:12:19.587972 swarms-5.0.8/swarms/models/open_router.py
--rw-r--r--   0        0        0      106 2024-05-20 23:12:19.588047 swarms-5.0.8/swarms/models/openai_embeddings.py
--rw-r--r--   0        0        0     3167 2024-05-20 23:12:19.588099 swarms-5.0.8/swarms/models/openai_tts.py
--rw-r--r--   0        0        0       93 2024-05-20 23:12:19.588149 swarms-5.0.8/swarms/models/palm.py
--rw-r--r--   0        0        0     2160 2024-05-20 23:12:19.588204 swarms-5.0.8/swarms/models/popular_llms.py
--rw-r--r--   0        0        0     4813 2024-05-20 23:12:19.588296 swarms-5.0.8/swarms/models/qwen.py
--rw-r--r--   0        0        0     3561 2024-05-20 23:12:19.588355 swarms-5.0.8/swarms/models/sam.py
--rw-r--r--   0        0        0    12675 2024-05-20 23:12:19.588421 swarms-5.0.8/swarms/models/sampling_params.py
--rw-r--r--   0        0        0     8244 2024-05-20 23:12:19.588474 swarms-5.0.8/swarms/models/ssd_1b.py
--rw-r--r--   0        0        0     3948 2024-05-20 23:12:19.588553 swarms-5.0.8/swarms/models/together.py
--rw-r--r--   0        0        0      592 2024-05-20 23:12:19.588607 swarms-5.0.8/swarms/models/types.py
--rw-r--r--   0        0        0     1731 2024-05-20 23:12:19.588664 swarms-5.0.8/swarms/models/vilt.py
--rw-r--r--   0        0        0     2846 2024-05-20 23:12:19.588711 swarms-5.0.8/swarms/models/vip_llava.py
--rw-r--r--   0        0        0     3666 2024-05-20 23:12:19.588784 swarms-5.0.8/swarms/models/zeroscope.py
--rw-r--r--   0        0        0        0 2024-05-20 23:12:19.588836 swarms-5.0.8/swarms/prebuilt_swarms/__init__.py
--rw-r--r--   0        0        0      692 2024-05-20 23:12:19.588923 swarms-5.0.8/swarms/prompts/__init__.py
--rw-r--r--   0        0        0    11320 2024-05-20 23:12:19.588988 swarms-5.0.8/swarms/prompts/accountant_swarm_prompts.py
--rw-r--r--   0        0        0     9156 2024-05-20 23:12:19.589069 swarms-5.0.8/swarms/prompts/aga.py
--rw-r--r--   0        0        0     1451 2024-05-20 23:12:19.589128 swarms-5.0.8/swarms/prompts/agent_output_parser.py
--rw-r--r--   0        0        0     2705 2024-05-20 23:12:19.589180 swarms-5.0.8/swarms/prompts/agent_prompt.py
--rw-r--r--   0        0        0     6886 2024-05-20 23:12:19.589236 swarms-5.0.8/swarms/prompts/agent_prompts.py
--rw-r--r--   0        0        0     7113 2024-05-20 23:12:19.589316 swarms-5.0.8/swarms/prompts/agent_system_prompts.py
--rw-r--r--   0        0        0     5233 2024-05-20 23:12:19.589377 swarms-5.0.8/swarms/prompts/ai_research_team.py
--rw-r--r--   0        0        0     1148 2024-05-20 23:12:19.589426 swarms-5.0.8/swarms/prompts/aot_prompt.py
--rw-r--r--   0        0        0    13981 2024-05-20 23:12:19.589498 swarms-5.0.8/swarms/prompts/autobloggen.py
--rw-r--r--   0        0        0     5605 2024-05-20 23:12:19.589584 swarms-5.0.8/swarms/prompts/autoswarm.py
--rw-r--r--   0        0        0     7542 2024-05-20 23:12:19.589647 swarms-5.0.8/swarms/prompts/base.py
--rw-r--r--   0        0        0     3801 2024-05-20 23:12:19.589703 swarms-5.0.8/swarms/prompts/chat_prompt.py
--rw-r--r--   0        0        0     2235 2024-05-20 23:12:19.589756 swarms-5.0.8/swarms/prompts/code_interpreter.py
--rw-r--r--   0        0        0     4106 2024-05-20 23:12:19.589834 swarms-5.0.8/swarms/prompts/code_spawner.py
--rw-r--r--   0        0        0     1566 2024-05-20 23:12:19.589885 swarms-5.0.8/swarms/prompts/debate.py
--rw-r--r--   0        0        0     7157 2024-05-23 01:40:32.871666 swarms-5.0.8/swarms/prompts/documentation.py
--rw-r--r--   0        0        0     1767 2024-05-20 23:12:19.590009 swarms-5.0.8/swarms/prompts/education.py
--rw-r--r--   0        0        0     4180 2024-05-20 23:12:19.590089 swarms-5.0.8/swarms/prompts/finance_agent_prompt.py
--rw-r--r--   0        0        0     4117 2024-05-20 23:12:19.590152 swarms-5.0.8/swarms/prompts/growth_agent_prompt.py
--rw-r--r--   0        0        0      880 2024-05-20 23:12:19.590207 swarms-5.0.8/swarms/prompts/idea2img.py
--rw-r--r--   0        0        0     3346 2024-05-20 23:12:19.590267 swarms-5.0.8/swarms/prompts/legal_agent_prompt.py
--rw-r--r--   0        0        0     4785 2024-05-20 23:12:19.590358 swarms-5.0.8/swarms/prompts/logistics.py
--rw-r--r--   0        0        0     3374 2024-05-20 23:12:19.590418 swarms-5.0.8/swarms/prompts/meta_system_prompt.py
--rw-r--r--   0        0        0    10662 2024-05-20 23:12:19.590489 swarms-5.0.8/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
--rw-r--r--   0        0        0     3511 2024-05-20 23:12:19.590550 swarms-5.0.8/swarms/prompts/multi_modal_prompts.py
--rw-r--r--   0        0        0     3225 2024-05-20 23:12:19.590626 swarms-5.0.8/swarms/prompts/multi_modal_visual_prompts.py
--rw-r--r--   0        0        0     3454 2024-05-20 23:12:19.590685 swarms-5.0.8/swarms/prompts/operations_agent_prompt.py
--rw-r--r--   0        0        0     2149 2024-05-20 23:12:19.590738 swarms-5.0.8/swarms/prompts/personal_stylist.py
--rw-r--r--   0        0        0     8333 2024-05-20 23:12:19.590803 swarms-5.0.8/swarms/prompts/product_agent_prompt.py
--rw-r--r--   0        0        0    10144 2024-05-20 23:12:19.590895 swarms-5.0.8/swarms/prompts/programming.py
--rw-r--r--   0        0        0     2128 2024-05-20 23:12:19.590958 swarms-5.0.8/swarms/prompts/project_manager.py
--rw-r--r--   0        0        0    13215 2024-05-20 23:12:19.591020 swarms-5.0.8/swarms/prompts/python.py
--rw-r--r--   0        0        0     2960 2024-05-20 23:12:19.591076 swarms-5.0.8/swarms/prompts/react.py
--rw-r--r--   0        0        0        0 2024-05-20 23:12:19.591117 swarms-5.0.8/swarms/prompts/refiner_agent_prompt.py
--rw-r--r--   0        0        0     5126 2024-05-20 23:12:19.591208 swarms-5.0.8/swarms/prompts/sales.py
--rw-r--r--   0        0        0     5013 2024-05-20 23:12:19.591263 swarms-5.0.8/swarms/prompts/sales_prompts.py
--rw-r--r--   0        0        0     2679 2024-05-20 23:12:19.591326 swarms-5.0.8/swarms/prompts/security_team.py
--rw-r--r--   0        0        0     3252 2024-05-20 23:12:19.591419 swarms-5.0.8/swarms/prompts/self_operating_prompt.py
--rw-r--r--   0        0        0     4147 2024-05-20 23:12:19.591487 swarms-5.0.8/swarms/prompts/sop_generator_agent_prompt.py
--rw-r--r--   0        0        0     4640 2024-05-20 23:12:19.591551 swarms-5.0.8/swarms/prompts/summaries_prompts.py
--rw-r--r--   0        0        0     3984 2024-05-20 23:12:19.591612 swarms-5.0.8/swarms/prompts/support_agent_prompt.py
--rw-r--r--   0        0        0     4280 2024-05-20 23:12:19.591714 swarms-5.0.8/swarms/prompts/swarm_manager_agent.py
--rw-r--r--   0        0        0      728 2024-05-20 23:12:19.591774 swarms-5.0.8/swarms/prompts/task_assignment_prompt.py
--rw-r--r--   0        0        0     4271 2024-05-20 23:12:19.591847 swarms-5.0.8/swarms/prompts/tests.py
--rw-r--r--   0        0        0     6576 2024-05-24 17:56:40.206770 swarms-5.0.8/swarms/prompts/tools.py
--rw-r--r--   0        0        0     2398 2024-05-20 23:12:19.592013 swarms-5.0.8/swarms/prompts/urban_planning.py
--rw-r--r--   0        0        0     3675 2024-05-20 23:12:19.592103 swarms-5.0.8/swarms/prompts/visual_cot.py
--rw-r--r--   0        0        0     5554 2024-05-20 23:12:19.592180 swarms-5.0.8/swarms/prompts/worker_prompt.py
--rw-r--r--   0        0        0     2349 2024-05-20 23:12:19.592230 swarms-5.0.8/swarms/prompts/xray_swarm_prompt.py
--rw-r--r--   0        0        0        0 2024-05-21 03:27:54.652576 swarms-5.0.8/swarms/schemas/__init__.py
--rw-r--r--   0        0        0     3168 2024-05-24 00:43:53.750806 swarms-5.0.8/swarms/schemas/hass_agent_schema.py
--rw-r--r--   0        0        0      182 2024-05-21 05:06:25.218133 swarms-5.0.8/swarms/schemas/plan.py
--rw-r--r--   0        0        0     6764 2024-05-20 23:12:19.594641 swarms-5.0.8/swarms/schemas/schemas.py
--rw-r--r--   0        0        0      709 2024-05-20 23:12:19.594792 swarms-5.0.8/swarms/schemas/step.py
--rw-r--r--   0        0        0     4084 2024-05-24 14:40:28.251160 swarms-5.0.8/swarms/structs/__init__.py
--rw-r--r--   0        0        0    61682 2024-05-25 00:11:23.269052 swarms-5.0.8/swarms/structs/agent.py
--rw-r--r--   0        0        0      574 2024-05-20 23:12:19.592548 swarms-5.0.8/swarms/structs/agent_job.py
--rw-r--r--   0        0        0     2937 2024-05-20 23:12:19.592611 swarms-5.0.8/swarms/structs/agent_process.py
--rw-r--r--   0        0        0     3777 2024-05-20 23:12:19.592668 swarms-5.0.8/swarms/structs/async_workflow.py
--rw-r--r--   0        0        0     6624 2024-05-20 23:12:19.592755 swarms-5.0.8/swarms/structs/auto_swarm.py
--rw-r--r--   0        0        0    12437 2024-05-20 23:12:19.592817 swarms-5.0.8/swarms/structs/base_structure.py
--rw-r--r--   0        0        0    19446 2024-05-20 23:12:19.592905 swarms-5.0.8/swarms/structs/base_swarm.py
--rw-r--r--   0        0        0    12161 2024-05-20 23:12:19.593000 swarms-5.0.8/swarms/structs/base_workflow.py
--rw-r--r--   0        0        0     5265 2024-05-21 00:48:59.119899 swarms-5.0.8/swarms/structs/company.py
--rw-r--r--   0        0        0     6181 2024-05-25 00:30:33.743749 swarms-5.0.8/swarms/structs/concurrent_workflow.py
--rw-r--r--   0        0        0    14685 2024-05-20 23:12:19.593392 swarms-5.0.8/swarms/structs/conversation.py
--rw-r--r--   0        0        0    12608 2024-05-20 23:12:19.593456 swarms-5.0.8/swarms/structs/debate.py
--rw-r--r--   0        0        0     4834 2024-05-20 23:12:19.593607 swarms-5.0.8/swarms/structs/groupchat.py
--rw-r--r--   0        0        0     8721 2024-05-27 04:34:55.663377 swarms-5.0.8/swarms/structs/hiearchical_swarm.py
--rw-r--r--   0        0        0     7012 2024-05-20 23:12:19.593787 swarms-5.0.8/swarms/structs/majority_voting.py
--rw-r--r--   0        0        0      621 2024-05-21 05:06:56.355487 swarms-5.0.8/swarms/structs/message.py
--rw-r--r--   0        0        0     7397 2024-05-20 23:12:19.593913 swarms-5.0.8/swarms/structs/message_pool.py
--rw-r--r--   0        0        0      855 2024-05-20 23:12:19.593973 swarms-5.0.8/swarms/structs/meta_system_prompt.py
--rw-r--r--   0        0        0     8193 2024-05-24 00:28:06.786449 swarms-5.0.8/swarms/structs/multi_agent_collab.py
--rw-r--r--   0        0        0     5623 2024-05-20 23:12:19.594191 swarms-5.0.8/swarms/structs/multi_process_workflow.py
--rw-r--r--   0        0        0     5272 2024-05-20 23:12:19.594250 swarms-5.0.8/swarms/structs/multi_threaded_workflow.py
--rw-r--r--   0        0        0      371 2024-05-20 23:12:19.594301 swarms-5.0.8/swarms/structs/omni_agent_types.py
--rw-r--r--   0        0        0     9900 2024-05-21 03:26:12.085452 swarms-5.0.8/swarms/structs/rearrange.py
--rw-r--r--   0        0        0     3011 2024-05-20 23:12:19.594499 swarms-5.0.8/swarms/structs/recursive_workflow.py
--rw-r--r--   0        0        0     3256 2024-05-20 23:12:19.594554 swarms-5.0.8/swarms/structs/round_robin.py
--rw-r--r--   0        0        0     2956 2024-05-20 23:12:19.594695 swarms-5.0.8/swarms/structs/sequential_workflow.py
--rw-r--r--   0        0        0     2442 2024-05-20 23:12:19.594743 swarms-5.0.8/swarms/structs/sermon_swarm.py
--rw-r--r--   0        0        0     1396 2024-05-23 01:40:40.668233 swarms-5.0.8/swarms/structs/society_of_agents.py
--rw-r--r--   0        0        0    11249 2024-05-24 16:15:05.490950 swarms-5.0.8/swarms/structs/swarm_load_balancer.py
--rw-r--r--   0        0        0    10684 2024-05-20 23:12:19.594876 swarms-5.0.8/swarms/structs/swarm_net.py
--rw-r--r--   0        0        0     6426 2024-05-20 23:12:19.594944 swarms-5.0.8/swarms/structs/swarming_architectures.py
--rw-r--r--   0        0        0     8251 2024-05-20 23:12:19.595011 swarms-5.0.8/swarms/structs/task.py
--rw-r--r--   0        0        0     1989 2024-05-20 23:12:19.595073 swarms-5.0.8/swarms/structs/task_queue_base.py
--rw-r--r--   0        0        0     3829 2024-05-24 20:02:02.841193 swarms-5.0.8/swarms/structs/tree_of_thoughts.py
--rw-r--r--   0        0        0     3646 2024-05-23 01:40:40.674259 swarms-5.0.8/swarms/structs/utils.py
--rw-r--r--   0        0        0     7403 2024-05-20 23:12:19.595210 swarms-5.0.8/swarms/structs/yaml_model.py
--rw-r--r--   0        0        0      891 2024-05-20 23:12:19.595297 swarms-5.0.8/swarms/telemetry/__init__.py
--rw-r--r--   0        0        0      513 2024-05-20 23:12:19.595348 swarms-5.0.8/swarms/telemetry/auto_upgrade_swarms.py
--rw-r--r--   0        0        0      385 2024-05-20 23:12:19.595426 swarms-5.0.8/swarms/telemetry/bootup.py
--rw-r--r--   0        0        0     1073 2024-05-20 23:12:19.595476 swarms-5.0.8/swarms/telemetry/check_update.py
--rw-r--r--   0        0        0      807 2024-05-20 23:12:19.595528 swarms-5.0.8/swarms/telemetry/log_all.py
--rw-r--r--   0        0        0      496 2024-05-20 23:12:19.595576 swarms-5.0.8/swarms/telemetry/sentry_active.py
--rw-r--r--   0        0        0     2675 2024-05-20 23:12:19.595649 swarms-5.0.8/swarms/telemetry/sys_info.py
--rw-r--r--   0        0        0     1879 2024-05-20 23:12:19.595698 swarms-5.0.8/swarms/telemetry/user_utils.py
--rw-r--r--   0        0        0     1457 2024-05-25 00:11:23.032620 swarms-5.0.8/swarms/tools/__init__.py
--rw-r--r--   0        0        0    13754 2024-05-25 00:08:34.660101 swarms-5.0.8/swarms/tools/base_tool.py
--rw-r--r--   0        0        0     6258 2024-05-25 00:03:55.372791 swarms-5.0.8/swarms/tools/func_calling_executor.py
--rw-r--r--   0        0        0     1115 2024-05-25 00:08:48.921190 swarms-5.0.8/swarms/tools/func_to_str.py
--rw-r--r--   0        0        0      773 2024-05-25 00:03:54.059716 swarms-5.0.8/swarms/tools/function_util.py
--rw-r--r--   0        0        0    14241 2024-05-20 23:12:19.596094 swarms-5.0.8/swarms/tools/json_former.py
--rw-r--r--   0        0        0     1316 2024-05-20 23:12:19.596178 swarms-5.0.8/swarms/tools/json_utils.py
--rw-r--r--   0        0        0     2455 2024-05-20 23:12:19.596226 swarms-5.0.8/swarms/tools/logits_processor.py
--rw-r--r--   0        0        0      978 2024-05-20 23:12:19.596325 swarms-5.0.8/swarms/tools/openai_func_calling_schema_pydantic.py
--rw-r--r--   0        0        0     2578 2024-05-25 00:03:55.373001 swarms-5.0.8/swarms/tools/openai_tool_creator_decorator.py
--rw-r--r--   0        0        0      205 2024-05-25 00:23:02.813589 swarms-5.0.8/swarms/tools/prebuilt/__init__.py
--rw-r--r--   0        0        0     6653 2024-05-20 23:12:19.595923 swarms-5.0.8/swarms/tools/prebuilt/code_interpreter.py
--rw-r--r--   0        0        0     1461 2024-05-20 23:12:19.596276 swarms-5.0.8/swarms/tools/prebuilt/math_eval.py
--rw-r--r--   0        0        0    15564 2024-05-20 23:12:19.596483 swarms-5.0.8/swarms/tools/py_func_to_openai_func_str.py
--rw-r--r--   0        0        0     3183 2024-05-25 00:08:48.931693 swarms-5.0.8/swarms/tools/pydantic_to_json.py
--rw-r--r--   0        0        0     7179 2024-05-24 17:56:40.227742 swarms-5.0.8/swarms/tools/tool_utils.py
--rw-r--r--   0        0        0     5466 2024-05-20 23:12:19.596758 swarms-5.0.8/swarms/utils/README.md
--rw-r--r--   0        0        0     1983 2024-05-25 00:11:23.037330 swarms-5.0.8/swarms/utils/__init__.py
--rw-r--r--   0        0        0     3507 2024-05-20 23:12:19.596872 swarms-5.0.8/swarms/utils/apa.py
--rw-r--r--   0        0        0     6065 2024-05-20 23:12:19.596962 swarms-5.0.8/swarms/utils/check_function_result.py
--rw-r--r--   0        0        0     1008 2024-05-20 23:12:19.597020 swarms-5.0.8/swarms/utils/class_args_wrapper.py
--rw-r--r--   0        0        0     1234 2024-05-20 23:12:19.597075 swarms-5.0.8/swarms/utils/concurrent_utils.py
--rw-r--r--   0        0        0     1865 2024-05-20 23:12:19.597130 swarms-5.0.8/swarms/utils/data_to_text.py
--rw-r--r--   0        0        0     2451 2024-05-20 23:12:19.597203 swarms-5.0.8/swarms/utils/decorators.py
--rw-r--r--   0        0        0     1311 2024-05-20 23:12:19.597263 swarms-5.0.8/swarms/utils/disable_logging.py
--rw-r--r--   0        0        0      890 2024-05-20 23:12:19.597318 swarms-5.0.8/swarms/utils/download_img.py
--rw-r--r--   0        0        0     1127 2024-05-20 23:12:19.597370 swarms-5.0.8/swarms/utils/execute_futures.py
--rw-r--r--   0        0        0     1113 2024-05-20 23:12:19.597441 swarms-5.0.8/swarms/utils/exponential_backoff.py
--rw-r--r--   0        0        0      854 2024-05-20 23:12:19.597496 swarms-5.0.8/swarms/utils/fetch_init_params.py
--rw-r--r--   0        0        0      500 2024-05-20 23:12:19.597550 swarms-5.0.8/swarms/utils/file_extension_seach.py
--rw-r--r--   0        0        0     3266 2024-05-20 23:12:19.597606 swarms-5.0.8/swarms/utils/file_processing.py
--rw-r--r--   0        0        0      630 2024-05-20 23:12:19.597693 swarms-5.0.8/swarms/utils/find_img_path.py
--rw-r--r--   0        0        0     4184 2024-05-20 23:12:19.597767 swarms-5.0.8/swarms/utils/get_logger.py
--rw-r--r--   0        0        0     4232 2024-05-20 23:12:19.597842 swarms-5.0.8/swarms/utils/get_total_gpus.py
--rw-r--r--   0        0        0     2848 2024-05-20 23:12:19.597905 swarms-5.0.8/swarms/utils/json_output_parser.py
--rw-r--r--   0        0        0     1831 2024-05-20 23:12:19.597994 swarms-5.0.8/swarms/utils/jsonl_utils.py
--rw-r--r--   0        0        0      932 2024-05-20 23:12:19.598063 swarms-5.0.8/swarms/utils/llm_metrics_decorator.py
--rw-r--r--   0        0        0     2209 2024-05-20 23:12:19.598133 swarms-5.0.8/swarms/utils/logger.py
--rw-r--r--   0        0        0    16186 2024-05-20 23:12:19.598202 swarms-5.0.8/swarms/utils/loggers.py
--rw-r--r--   0        0        0      453 2024-05-20 23:12:19.598285 swarms-5.0.8/swarms/utils/loguru_logger.py
--rw-r--r--   0        0        0      711 2024-05-20 23:12:19.598349 swarms-5.0.8/swarms/utils/markdown_message.py
--rw-r--r--   0        0        0     2173 2024-05-26 03:54:20.425670 swarms-5.0.8/swarms/utils/optimized_loop.py
--rw-r--r--   0        0        0      600 2024-05-20 23:12:19.598408 swarms-5.0.8/swarms/utils/parse_code.py
--rw-r--r--   0        0        0     1177 2024-05-20 23:12:19.598470 swarms-5.0.8/swarms/utils/pdf_to_text.py
--rw-r--r--   0        0        0     1353 2024-05-20 23:12:19.598561 swarms-5.0.8/swarms/utils/remove_json_whitespace.py
--rw-r--r--   0        0        0     1278 2024-05-20 23:12:19.598619 swarms-5.0.8/swarms/utils/save_logs.py
--rw-r--r--   0        0        0     4774 2024-05-20 23:12:19.598696 swarms-5.0.8/swarms/utils/serializable.py
--rw-r--r--   0        0        0     1315 2024-05-20 23:12:19.598755 swarms-5.0.8/swarms/utils/try_except_wrapper.py
--rw-r--r--   0        0        0     2668 2024-05-20 23:12:19.598843 swarms-5.0.8/swarms/utils/yaml_output_parser.py
--rw-r--r--   0        0        0    35249 1970-01-01 00:00:00.000000 swarms-5.0.8/PKG-INFO
+-rw-r--r--   0        0        0    15674 2024-05-20 23:12:19.525914 swarms-5.1.3/LICENSE
+-rw-r--r--   0        0        0    33743 2024-05-25 00:26:35.052802 swarms-5.1.3/README.md
+-rw-r--r--   0        0        0     1790 2024-05-30 19:50:22.087043 swarms-5.1.3/pyproject.toml
+-rw-r--r--   0        0        0      590 2024-05-20 23:12:19.584595 swarms-5.1.3/swarms/__init__.py
+-rw-r--r--   0        0        0      864 2024-05-20 23:12:19.584679 swarms-5.1.3/swarms/agents/__init__.py
+-rw-r--r--   0        0        0      881 2024-05-20 23:12:19.584738 swarms-5.1.3/swarms/agents/agent_wrapper.py
+-rw-r--r--   0        0        0     3342 2024-05-20 23:12:19.584796 swarms-5.1.3/swarms/agents/base.py
+-rw-r--r--   0        0        0     4201 2024-05-20 23:12:19.584880 swarms-5.1.3/swarms/agents/developer_agents.py
+-rw-r--r--   0        0        0     2950 2024-05-20 23:12:19.584947 swarms-5.1.3/swarms/agents/omni_modal_agent.py
+-rw-r--r--   0        0        0     3491 2024-05-20 23:12:19.585001 swarms-5.1.3/swarms/agents/simple_agent.py
+-rw-r--r--   0        0        0      484 2024-05-20 23:12:19.585048 swarms-5.1.3/swarms/agents/stopping_conditions.py
+-rw-r--r--   0        0        0     4940 2024-05-20 23:12:19.585129 swarms-5.1.3/swarms/agents/tool_agent.py
+-rw-r--r--   0        0        0     5504 2024-05-20 23:12:19.585192 swarms-5.1.3/swarms/agents/worker_agent.py
+-rw-r--r--   0        0        0      167 2024-05-20 23:12:19.585283 swarms-5.1.3/swarms/artifacts/__init__.py
+-rw-r--r--   0        0        0     1675 2024-05-20 23:12:19.585343 swarms-5.1.3/swarms/artifacts/base_artifact.py
+-rw-r--r--   0        0        0     2299 2024-05-20 23:12:19.585425 swarms-5.1.3/swarms/artifacts/text_artifact.py
+-rw-r--r--   0        0        0      241 2024-05-27 18:13:38.292135 swarms-5.1.3/swarms/marketplace/__init__.py
+-rw-r--r--   0        0        0     1809 2024-05-27 17:53:43.733672 swarms-5.1.3/swarms/marketplace/add_all_swarms.py
+-rw-r--r--   0        0        0     8335 2024-05-27 18:00:05.308232 swarms-5.1.3/swarms/marketplace/agricultural_optimization.py
+-rw-r--r--   0        0        0      613 2024-05-20 23:12:19.585515 swarms-5.1.3/swarms/memory/__init__.py
+-rw-r--r--   0        0        0      433 2024-05-20 23:12:19.585565 swarms-5.1.3/swarms/memory/action_subtask.py
+-rw-r--r--   0        0        0     3475 2024-05-20 23:12:19.585621 swarms-5.1.3/swarms/memory/base_db.py
+-rw-r--r--   0        0        0     2823 2024-05-20 23:12:19.585702 swarms-5.1.3/swarms/memory/base_vectordb.py
+-rw-r--r--   0        0        0     2895 2024-05-20 23:12:19.585767 swarms-5.1.3/swarms/memory/dict_internal_memory.py
+-rw-r--r--   0        0        0     3306 2024-05-20 23:12:19.585826 swarms-5.1.3/swarms/memory/dict_shared_memory.py
+-rw-r--r--   0        0        0     5499 2024-05-20 23:12:19.585895 swarms-5.1.3/swarms/memory/short_term_memory.py
+-rw-r--r--   0        0        0     3371 2024-05-20 23:12:19.585978 swarms-5.1.3/swarms/memory/visual_memory.py
+-rw-r--r--   0        0        0     2392 2024-05-21 05:06:54.045652 swarms-5.1.3/swarms/models/__init__.py
+-rw-r--r--   0        0        0     2052 2024-05-21 00:48:59.027928 swarms-5.1.3/swarms/models/base_embedding_model.py
+-rw-r--r--   0        0        0    13168 2024-05-20 23:12:19.586207 swarms-5.1.3/swarms/models/base_llm.py
+-rw-r--r--   0        0        0    12604 2024-05-20 23:12:19.586302 swarms-5.1.3/swarms/models/base_multimodal_model.py
+-rw-r--r--   0        0        0     2475 2024-05-20 23:12:19.586361 swarms-5.1.3/swarms/models/base_tts.py
+-rw-r--r--   0        0        0     3163 2024-05-20 23:12:19.586416 swarms-5.1.3/swarms/models/base_ttv.py
+-rw-r--r--   0        0        0    16743 2024-05-20 23:12:19.586490 swarms-5.1.3/swarms/models/cog_vlm.py
+-rw-r--r--   0        0        0    10760 2024-05-20 23:12:19.586608 swarms-5.1.3/swarms/models/dalle3.py
+-rw-r--r--   0        0        0     6449 2024-05-20 23:12:19.586690 swarms-5.1.3/swarms/models/distilled_whisperx.py
+-rw-r--r--   0        0        0      682 2024-05-20 23:12:19.586747 swarms-5.1.3/swarms/models/embeddings_base.py
+-rw-r--r--   0        0        0     3022 2024-05-20 23:12:19.586804 swarms-5.1.3/swarms/models/fuyu.py
+-rw-r--r--   0        0        0     7762 2024-05-20 23:12:19.586891 swarms-5.1.3/swarms/models/gemini.py
+-rw-r--r--   0        0        0    14273 2024-05-27 18:58:25.544867 swarms-5.1.3/swarms/models/gpt4_vision_api.py
+-rw-r--r--   0        0        0    12996 2024-05-20 23:12:19.587047 swarms-5.1.3/swarms/models/huggingface.py
+-rw-r--r--   0        0        0     1826 2024-05-20 23:12:19.587108 swarms-5.1.3/swarms/models/huggingface_pipeline.py
+-rw-r--r--   0        0        0     5601 2024-05-20 23:12:19.587202 swarms-5.1.3/swarms/models/idefics.py
+-rw-r--r--   0        0        0    10672 2024-05-20 23:12:19.587276 swarms-5.1.3/swarms/models/kosmos_two.py
+-rw-r--r--   0        0        0     1448 2024-05-20 23:12:19.587347 swarms-5.1.3/swarms/models/layoutlm_document_qa.py
+-rw-r--r--   0        0        0     2599 2024-05-21 05:06:21.835242 swarms-5.1.3/swarms/models/llama3_hosted.py
+-rw-r--r--   0        0        0     6581 2024-05-20 23:12:19.587506 swarms-5.1.3/swarms/models/llama_function_caller.py
+-rw-r--r--   0        0        0     2762 2024-05-20 23:12:19.587573 swarms-5.1.3/swarms/models/llava.py
+-rw-r--r--   0        0        0     2056 2024-05-20 23:12:19.587792 swarms-5.1.3/swarms/models/moondream_mm.py
+-rw-r--r--   0        0        0     2881 2024-05-20 23:12:19.587858 swarms-5.1.3/swarms/models/nougat.py
+-rw-r--r--   0        0        0     2366 2024-05-20 23:12:19.587917 swarms-5.1.3/swarms/models/open_dalle.py
+-rw-r--r--   0        0        0     2464 2024-05-20 23:12:19.587972 swarms-5.1.3/swarms/models/open_router.py
+-rw-r--r--   0        0        0      106 2024-05-20 23:12:19.588047 swarms-5.1.3/swarms/models/openai_embeddings.py
+-rw-r--r--   0        0        0     3167 2024-05-20 23:12:19.588099 swarms-5.1.3/swarms/models/openai_tts.py
+-rw-r--r--   0        0        0       93 2024-05-20 23:12:19.588149 swarms-5.1.3/swarms/models/palm.py
+-rw-r--r--   0        0        0     2228 2024-05-30 19:26:31.558067 swarms-5.1.3/swarms/models/popular_llms.py
+-rw-r--r--   0        0        0     4813 2024-05-20 23:12:19.588296 swarms-5.1.3/swarms/models/qwen.py
+-rw-r--r--   0        0        0     3561 2024-05-20 23:12:19.588355 swarms-5.1.3/swarms/models/sam.py
+-rw-r--r--   0        0        0    12675 2024-05-20 23:12:19.588421 swarms-5.1.3/swarms/models/sampling_params.py
+-rw-r--r--   0        0        0     8244 2024-05-20 23:12:19.588474 swarms-5.1.3/swarms/models/ssd_1b.py
+-rw-r--r--   0        0        0     3948 2024-05-20 23:12:19.588553 swarms-5.1.3/swarms/models/together.py
+-rw-r--r--   0        0        0      592 2024-05-20 23:12:19.588607 swarms-5.1.3/swarms/models/types.py
+-rw-r--r--   0        0        0     1731 2024-05-20 23:12:19.588664 swarms-5.1.3/swarms/models/vilt.py
+-rw-r--r--   0        0        0     2846 2024-05-20 23:12:19.588711 swarms-5.1.3/swarms/models/vip_llava.py
+-rw-r--r--   0        0        0     3666 2024-05-20 23:12:19.588784 swarms-5.1.3/swarms/models/zeroscope.py
+-rw-r--r--   0        0        0      692 2024-05-20 23:12:19.588923 swarms-5.1.3/swarms/prompts/__init__.py
+-rw-r--r--   0        0        0    11320 2024-05-20 23:12:19.588988 swarms-5.1.3/swarms/prompts/accountant_swarm_prompts.py
+-rw-r--r--   0        0        0     9156 2024-05-20 23:12:19.589069 swarms-5.1.3/swarms/prompts/aga.py
+-rw-r--r--   0        0        0     1451 2024-05-20 23:12:19.589128 swarms-5.1.3/swarms/prompts/agent_output_parser.py
+-rw-r--r--   0        0        0     2705 2024-05-20 23:12:19.589180 swarms-5.1.3/swarms/prompts/agent_prompt.py
+-rw-r--r--   0        0        0     6886 2024-05-20 23:12:19.589236 swarms-5.1.3/swarms/prompts/agent_prompts.py
+-rw-r--r--   0        0        0     7113 2024-05-20 23:12:19.589316 swarms-5.1.3/swarms/prompts/agent_system_prompts.py
+-rw-r--r--   0        0        0     5233 2024-05-20 23:12:19.589377 swarms-5.1.3/swarms/prompts/ai_research_team.py
+-rw-r--r--   0        0        0     1148 2024-05-20 23:12:19.589426 swarms-5.1.3/swarms/prompts/aot_prompt.py
+-rw-r--r--   0        0        0    13981 2024-05-20 23:12:19.589498 swarms-5.1.3/swarms/prompts/autobloggen.py
+-rw-r--r--   0        0        0     5605 2024-05-20 23:12:19.589584 swarms-5.1.3/swarms/prompts/autoswarm.py
+-rw-r--r--   0        0        0     7542 2024-05-20 23:12:19.589647 swarms-5.1.3/swarms/prompts/base.py
+-rw-r--r--   0        0        0     3801 2024-05-20 23:12:19.589703 swarms-5.1.3/swarms/prompts/chat_prompt.py
+-rw-r--r--   0        0        0     2235 2024-05-20 23:12:19.589756 swarms-5.1.3/swarms/prompts/code_interpreter.py
+-rw-r--r--   0        0        0     4106 2024-05-20 23:12:19.589834 swarms-5.1.3/swarms/prompts/code_spawner.py
+-rw-r--r--   0        0        0     1566 2024-05-20 23:12:19.589885 swarms-5.1.3/swarms/prompts/debate.py
+-rw-r--r--   0        0        0     7157 2024-05-23 01:40:32.871666 swarms-5.1.3/swarms/prompts/documentation.py
+-rw-r--r--   0        0        0     1767 2024-05-20 23:12:19.590009 swarms-5.1.3/swarms/prompts/education.py
+-rw-r--r--   0        0        0     4180 2024-05-20 23:12:19.590089 swarms-5.1.3/swarms/prompts/finance_agent_prompt.py
+-rw-r--r--   0        0        0     4117 2024-05-20 23:12:19.590152 swarms-5.1.3/swarms/prompts/growth_agent_prompt.py
+-rw-r--r--   0        0        0      880 2024-05-20 23:12:19.590207 swarms-5.1.3/swarms/prompts/idea2img.py
+-rw-r--r--   0        0        0     3346 2024-05-20 23:12:19.590267 swarms-5.1.3/swarms/prompts/legal_agent_prompt.py
+-rw-r--r--   0        0        0     4785 2024-05-20 23:12:19.590358 swarms-5.1.3/swarms/prompts/logistics.py
+-rw-r--r--   0        0        0     3374 2024-05-20 23:12:19.590418 swarms-5.1.3/swarms/prompts/meta_system_prompt.py
+-rw-r--r--   0        0        0    10662 2024-05-20 23:12:19.590489 swarms-5.1.3/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
+-rw-r--r--   0        0        0     3511 2024-05-20 23:12:19.590550 swarms-5.1.3/swarms/prompts/multi_modal_prompts.py
+-rw-r--r--   0        0        0     3225 2024-05-20 23:12:19.590626 swarms-5.1.3/swarms/prompts/multi_modal_visual_prompts.py
+-rw-r--r--   0        0        0     3454 2024-05-20 23:12:19.590685 swarms-5.1.3/swarms/prompts/operations_agent_prompt.py
+-rw-r--r--   0        0        0     2149 2024-05-20 23:12:19.590738 swarms-5.1.3/swarms/prompts/personal_stylist.py
+-rw-r--r--   0        0        0     8333 2024-05-20 23:12:19.590803 swarms-5.1.3/swarms/prompts/product_agent_prompt.py
+-rw-r--r--   0        0        0    10144 2024-05-20 23:12:19.590895 swarms-5.1.3/swarms/prompts/programming.py
+-rw-r--r--   0        0        0     2128 2024-05-20 23:12:19.590958 swarms-5.1.3/swarms/prompts/project_manager.py
+-rw-r--r--   0        0        0    13215 2024-05-20 23:12:19.591020 swarms-5.1.3/swarms/prompts/python.py
+-rw-r--r--   0        0        0     2960 2024-05-20 23:12:19.591076 swarms-5.1.3/swarms/prompts/react.py
+-rw-r--r--   0        0        0        0 2024-05-20 23:12:19.591117 swarms-5.1.3/swarms/prompts/refiner_agent_prompt.py
+-rw-r--r--   0        0        0     5126 2024-05-20 23:12:19.591208 swarms-5.1.3/swarms/prompts/sales.py
+-rw-r--r--   0        0        0     5013 2024-05-20 23:12:19.591263 swarms-5.1.3/swarms/prompts/sales_prompts.py
+-rw-r--r--   0        0        0     2679 2024-05-20 23:12:19.591326 swarms-5.1.3/swarms/prompts/security_team.py
+-rw-r--r--   0        0        0     3252 2024-05-20 23:12:19.591419 swarms-5.1.3/swarms/prompts/self_operating_prompt.py
+-rw-r--r--   0        0        0     4147 2024-05-20 23:12:19.591487 swarms-5.1.3/swarms/prompts/sop_generator_agent_prompt.py
+-rw-r--r--   0        0        0     4640 2024-05-20 23:12:19.591551 swarms-5.1.3/swarms/prompts/summaries_prompts.py
+-rw-r--r--   0        0        0     3984 2024-05-20 23:12:19.591612 swarms-5.1.3/swarms/prompts/support_agent_prompt.py
+-rw-r--r--   0        0        0     4280 2024-05-20 23:12:19.591714 swarms-5.1.3/swarms/prompts/swarm_manager_agent.py
+-rw-r--r--   0        0        0      728 2024-05-20 23:12:19.591774 swarms-5.1.3/swarms/prompts/task_assignment_prompt.py
+-rw-r--r--   0        0        0     4271 2024-05-20 23:12:19.591847 swarms-5.1.3/swarms/prompts/tests.py
+-rw-r--r--   0        0        0     6576 2024-05-24 17:56:40.206770 swarms-5.1.3/swarms/prompts/tools.py
+-rw-r--r--   0        0        0     2398 2024-05-20 23:12:19.592013 swarms-5.1.3/swarms/prompts/urban_planning.py
+-rw-r--r--   0        0        0     3675 2024-05-20 23:12:19.592103 swarms-5.1.3/swarms/prompts/visual_cot.py
+-rw-r--r--   0        0        0     5554 2024-05-20 23:12:19.592180 swarms-5.1.3/swarms/prompts/worker_prompt.py
+-rw-r--r--   0        0        0     2349 2024-05-20 23:12:19.592230 swarms-5.1.3/swarms/prompts/xray_swarm_prompt.py
+-rw-r--r--   0        0        0        0 2024-05-21 03:27:54.652576 swarms-5.1.3/swarms/schemas/__init__.py
+-rw-r--r--   0        0        0     3168 2024-05-24 00:43:53.750806 swarms-5.1.3/swarms/schemas/hass_agent_schema.py
+-rw-r--r--   0        0        0      182 2024-05-21 05:06:25.218133 swarms-5.1.3/swarms/schemas/plan.py
+-rw-r--r--   0        0        0     6764 2024-05-20 23:12:19.594641 swarms-5.1.3/swarms/schemas/schemas.py
+-rw-r--r--   0        0        0      709 2024-05-20 23:12:19.594792 swarms-5.1.3/swarms/schemas/step.py
+-rw-r--r--   0        0        0     4084 2024-05-24 14:40:28.251160 swarms-5.1.3/swarms/structs/__init__.py
+-rw-r--r--   0        0        0    57349 2024-05-29 00:04:03.308368 swarms-5.1.3/swarms/structs/agent.py
+-rw-r--r--   0        0        0      574 2024-05-20 23:12:19.592548 swarms-5.1.3/swarms/structs/agent_job.py
+-rw-r--r--   0        0        0     2937 2024-05-20 23:12:19.592611 swarms-5.1.3/swarms/structs/agent_process.py
+-rw-r--r--   0        0        0     3777 2024-05-20 23:12:19.592668 swarms-5.1.3/swarms/structs/async_workflow.py
+-rw-r--r--   0        0        0     8028 2024-05-27 18:13:39.873463 swarms-5.1.3/swarms/structs/auto_swarm.py
+-rw-r--r--   0        0        0    12437 2024-05-20 23:12:19.592817 swarms-5.1.3/swarms/structs/base_structure.py
+-rw-r--r--   0        0        0    19446 2024-05-20 23:12:19.592905 swarms-5.1.3/swarms/structs/base_swarm.py
+-rw-r--r--   0        0        0    12161 2024-05-20 23:12:19.593000 swarms-5.1.3/swarms/structs/base_workflow.py
+-rw-r--r--   0        0        0     5265 2024-05-21 00:48:59.119899 swarms-5.1.3/swarms/structs/company.py
+-rw-r--r--   0        0        0     6181 2024-05-25 00:30:33.743749 swarms-5.1.3/swarms/structs/concurrent_workflow.py
+-rw-r--r--   0        0        0    14685 2024-05-20 23:12:19.593392 swarms-5.1.3/swarms/structs/conversation.py
+-rw-r--r--   0        0        0    12608 2024-05-20 23:12:19.593456 swarms-5.1.3/swarms/structs/debate.py
+-rw-r--r--   0        0        0     4834 2024-05-20 23:12:19.593607 swarms-5.1.3/swarms/structs/groupchat.py
+-rw-r--r--   0        0        0     8721 2024-05-27 04:34:55.663377 swarms-5.1.3/swarms/structs/hiearchical_swarm.py
+-rw-r--r--   0        0        0     7012 2024-05-20 23:12:19.593787 swarms-5.1.3/swarms/structs/majority_voting.py
+-rw-r--r--   0        0        0      621 2024-05-21 05:06:56.355487 swarms-5.1.3/swarms/structs/message.py
+-rw-r--r--   0        0        0     7397 2024-05-20 23:12:19.593913 swarms-5.1.3/swarms/structs/message_pool.py
+-rw-r--r--   0        0        0      855 2024-05-20 23:12:19.593973 swarms-5.1.3/swarms/structs/meta_system_prompt.py
+-rw-r--r--   0        0        0     8193 2024-05-24 00:28:06.786449 swarms-5.1.3/swarms/structs/multi_agent_collab.py
+-rw-r--r--   0        0        0     5623 2024-05-20 23:12:19.594191 swarms-5.1.3/swarms/structs/multi_process_workflow.py
+-rw-r--r--   0        0        0     5272 2024-05-20 23:12:19.594250 swarms-5.1.3/swarms/structs/multi_threaded_workflow.py
+-rw-r--r--   0        0        0      371 2024-05-20 23:12:19.594301 swarms-5.1.3/swarms/structs/omni_agent_types.py
+-rw-r--r--   0        0        0     9900 2024-05-21 03:26:12.085452 swarms-5.1.3/swarms/structs/rearrange.py
+-rw-r--r--   0        0        0     3011 2024-05-20 23:12:19.594499 swarms-5.1.3/swarms/structs/recursive_workflow.py
+-rw-r--r--   0        0        0     3256 2024-05-20 23:12:19.594554 swarms-5.1.3/swarms/structs/round_robin.py
+-rw-r--r--   0        0        0      652 2024-05-30 19:26:33.653853 swarms-5.1.3/swarms/structs/scp.py
+-rw-r--r--   0        0        0     2956 2024-05-20 23:12:19.594695 swarms-5.1.3/swarms/structs/sequential_workflow.py
+-rw-r--r--   0        0        0     2442 2024-05-20 23:12:19.594743 swarms-5.1.3/swarms/structs/sermon_swarm.py
+-rw-r--r--   0        0        0     1396 2024-05-23 01:40:40.668233 swarms-5.1.3/swarms/structs/society_of_agents.py
+-rw-r--r--   0        0        0    11249 2024-05-24 16:15:05.490950 swarms-5.1.3/swarms/structs/swarm_load_balancer.py
+-rw-r--r--   0        0        0    10684 2024-05-20 23:12:19.594876 swarms-5.1.3/swarms/structs/swarm_net.py
+-rw-r--r--   0        0        0     6426 2024-05-20 23:12:19.594944 swarms-5.1.3/swarms/structs/swarming_architectures.py
+-rw-r--r--   0        0        0     8251 2024-05-20 23:12:19.595011 swarms-5.1.3/swarms/structs/task.py
+-rw-r--r--   0        0        0     1989 2024-05-20 23:12:19.595073 swarms-5.1.3/swarms/structs/task_queue_base.py
+-rw-r--r--   0        0        0     3829 2024-05-24 20:02:02.841193 swarms-5.1.3/swarms/structs/tree_of_thoughts.py
+-rw-r--r--   0        0        0     3646 2024-05-23 01:40:40.674259 swarms-5.1.3/swarms/structs/utils.py
+-rw-r--r--   0        0        0     7403 2024-05-20 23:12:19.595210 swarms-5.1.3/swarms/structs/yaml_model.py
+-rw-r--r--   0        0        0      891 2024-05-20 23:12:19.595297 swarms-5.1.3/swarms/telemetry/__init__.py
+-rw-r--r--   0        0        0      513 2024-05-20 23:12:19.595348 swarms-5.1.3/swarms/telemetry/auto_upgrade_swarms.py
+-rw-r--r--   0        0        0      385 2024-05-20 23:12:19.595426 swarms-5.1.3/swarms/telemetry/bootup.py
+-rw-r--r--   0        0        0     1073 2024-05-20 23:12:19.595476 swarms-5.1.3/swarms/telemetry/check_update.py
+-rw-r--r--   0        0        0      807 2024-05-20 23:12:19.595528 swarms-5.1.3/swarms/telemetry/log_all.py
+-rw-r--r--   0        0        0      496 2024-05-20 23:12:19.595576 swarms-5.1.3/swarms/telemetry/sentry_active.py
+-rw-r--r--   0        0        0     2675 2024-05-20 23:12:19.595649 swarms-5.1.3/swarms/telemetry/sys_info.py
+-rw-r--r--   0        0        0     1879 2024-05-20 23:12:19.595698 swarms-5.1.3/swarms/telemetry/user_utils.py
+-rw-r--r--   0        0        0     1607 2024-05-29 01:39:06.560756 swarms-5.1.3/swarms/tools/__init__.py
+-rw-r--r--   0        0        0    13754 2024-05-25 00:08:34.660101 swarms-5.1.3/swarms/tools/base_tool.py
+-rw-r--r--   0        0        0      586 2024-05-28 23:59:46.627698 swarms-5.1.3/swarms/tools/cohere_func_call_schema.py
+-rw-r--r--   0        0        0     8692 2024-05-29 00:01:20.565744 swarms-5.1.3/swarms/tools/func_calling_executor.py
+-rw-r--r--   0        0        0     2678 2024-05-28 23:06:05.558516 swarms-5.1.3/swarms/tools/func_calling_utils.py
+-rw-r--r--   0        0        0     1115 2024-05-25 00:08:48.921190 swarms-5.1.3/swarms/tools/func_to_str.py
+-rw-r--r--   0        0        0      773 2024-05-25 00:03:54.059716 swarms-5.1.3/swarms/tools/function_util.py
+-rw-r--r--   0        0        0    14241 2024-05-20 23:12:19.596094 swarms-5.1.3/swarms/tools/json_former.py
+-rw-r--r--   0        0        0     1316 2024-05-20 23:12:19.596178 swarms-5.1.3/swarms/tools/json_utils.py
+-rw-r--r--   0        0        0     2455 2024-05-20 23:12:19.596226 swarms-5.1.3/swarms/tools/logits_processor.py
+-rw-r--r--   0        0        0      978 2024-05-20 23:12:19.596325 swarms-5.1.3/swarms/tools/openai_func_calling_schema_pydantic.py
+-rw-r--r--   0        0        0     2578 2024-05-25 00:03:55.373001 swarms-5.1.3/swarms/tools/openai_tool_creator_decorator.py
+-rw-r--r--   0        0        0      205 2024-05-25 00:23:02.813589 swarms-5.1.3/swarms/tools/prebuilt/__init__.py
+-rw-r--r--   0        0        0     2452 2024-05-28 01:45:52.242620 swarms-5.1.3/swarms/tools/prebuilt/bing_api.py
+-rw-r--r--   0        0        0     7162 2024-05-28 23:06:05.570048 swarms-5.1.3/swarms/tools/prebuilt/code_interpreter.py
+-rw-r--r--   0        0        0     1461 2024-05-20 23:12:19.596276 swarms-5.1.3/swarms/tools/prebuilt/math_eval.py
+-rw-r--r--   0        0        0    15564 2024-05-20 23:12:19.596483 swarms-5.1.3/swarms/tools/py_func_to_openai_func_str.py
+-rw-r--r--   0        0        0     3183 2024-05-25 00:08:48.931693 swarms-5.1.3/swarms/tools/pydantic_to_json.py
+-rw-r--r--   0        0        0     7179 2024-05-24 17:56:40.227742 swarms-5.1.3/swarms/tools/tool_utils.py
+-rw-r--r--   0        0        0     5466 2024-05-20 23:12:19.596758 swarms-5.1.3/swarms/utils/README.md
+-rw-r--r--   0        0        0     1983 2024-05-25 00:11:23.037330 swarms-5.1.3/swarms/utils/__init__.py
+-rw-r--r--   0        0        0     3507 2024-05-20 23:12:19.596872 swarms-5.1.3/swarms/utils/apa.py
+-rw-r--r--   0        0        0     6065 2024-05-20 23:12:19.596962 swarms-5.1.3/swarms/utils/check_function_result.py
+-rw-r--r--   0        0        0     1008 2024-05-20 23:12:19.597020 swarms-5.1.3/swarms/utils/class_args_wrapper.py
+-rw-r--r--   0        0        0     1234 2024-05-20 23:12:19.597075 swarms-5.1.3/swarms/utils/concurrent_utils.py
+-rw-r--r--   0        0        0     1865 2024-05-20 23:12:19.597130 swarms-5.1.3/swarms/utils/data_to_text.py
+-rw-r--r--   0        0        0     2451 2024-05-20 23:12:19.597203 swarms-5.1.3/swarms/utils/decorators.py
+-rw-r--r--   0        0        0     1311 2024-05-20 23:12:19.597263 swarms-5.1.3/swarms/utils/disable_logging.py
+-rw-r--r--   0        0        0      890 2024-05-20 23:12:19.597318 swarms-5.1.3/swarms/utils/download_img.py
+-rw-r--r--   0        0        0     1127 2024-05-20 23:12:19.597370 swarms-5.1.3/swarms/utils/execute_futures.py
+-rw-r--r--   0        0        0     1113 2024-05-20 23:12:19.597441 swarms-5.1.3/swarms/utils/exponential_backoff.py
+-rw-r--r--   0        0        0      854 2024-05-20 23:12:19.597496 swarms-5.1.3/swarms/utils/fetch_init_params.py
+-rw-r--r--   0        0        0      500 2024-05-20 23:12:19.597550 swarms-5.1.3/swarms/utils/file_extension_seach.py
+-rw-r--r--   0        0        0     3266 2024-05-20 23:12:19.597606 swarms-5.1.3/swarms/utils/file_processing.py
+-rw-r--r--   0        0        0      630 2024-05-20 23:12:19.597693 swarms-5.1.3/swarms/utils/find_img_path.py
+-rw-r--r--   0        0        0     4184 2024-05-20 23:12:19.597767 swarms-5.1.3/swarms/utils/get_logger.py
+-rw-r--r--   0        0        0     4232 2024-05-20 23:12:19.597842 swarms-5.1.3/swarms/utils/get_total_gpus.py
+-rw-r--r--   0        0        0     2848 2024-05-20 23:12:19.597905 swarms-5.1.3/swarms/utils/json_output_parser.py
+-rw-r--r--   0        0        0     1831 2024-05-20 23:12:19.597994 swarms-5.1.3/swarms/utils/jsonl_utils.py
+-rw-r--r--   0        0        0      932 2024-05-20 23:12:19.598063 swarms-5.1.3/swarms/utils/llm_metrics_decorator.py
+-rw-r--r--   0        0        0     2209 2024-05-20 23:12:19.598133 swarms-5.1.3/swarms/utils/logger.py
+-rw-r--r--   0        0        0    16186 2024-05-20 23:12:19.598202 swarms-5.1.3/swarms/utils/loggers.py
+-rw-r--r--   0        0        0      453 2024-05-20 23:12:19.598285 swarms-5.1.3/swarms/utils/loguru_logger.py
+-rw-r--r--   0        0        0      711 2024-05-20 23:12:19.598349 swarms-5.1.3/swarms/utils/markdown_message.py
+-rw-r--r--   0        0        0     2179 2024-05-27 17:59:39.665558 swarms-5.1.3/swarms/utils/optimized_loop.py
+-rw-r--r--   0        0        0      600 2024-05-20 23:12:19.598408 swarms-5.1.3/swarms/utils/parse_code.py
+-rw-r--r--   0        0        0     1177 2024-05-20 23:12:19.598470 swarms-5.1.3/swarms/utils/pdf_to_text.py
+-rw-r--r--   0        0        0     1353 2024-05-20 23:12:19.598561 swarms-5.1.3/swarms/utils/remove_json_whitespace.py
+-rw-r--r--   0        0        0     1278 2024-05-20 23:12:19.598619 swarms-5.1.3/swarms/utils/save_logs.py
+-rw-r--r--   0        0        0     4774 2024-05-20 23:12:19.598696 swarms-5.1.3/swarms/utils/serializable.py
+-rw-r--r--   0        0        0     1315 2024-05-20 23:12:19.598755 swarms-5.1.3/swarms/utils/try_except_wrapper.py
+-rw-r--r--   0        0        0     2668 2024-05-20 23:12:19.598843 swarms-5.1.3/swarms/utils/yaml_output_parser.py
+-rw-r--r--   0        0        0    35249 1970-01-01 00:00:00.000000 swarms-5.1.3/PKG-INFO
```

### Comparing `swarms-5.0.8/LICENSE` & `swarms-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/README.md` & `swarms-5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/pyproject.toml` & `swarms-5.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "swarms"
-version = "5.0.8"
+version = "5.1.3"
 description = "Swarms - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/swarms"
 documentation = "https://swarms.world"
 readme = "README.md"
 repository = "https://github.com/kyegomez/swarms"
```

### Comparing `swarms-5.0.8/swarms/__init__.py` & `swarms-5.1.3/swarms/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/agents/__init__.py` & `swarms-5.1.3/swarms/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/agents/agent_wrapper.py` & `swarms-5.1.3/swarms/agents/agent_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/agents/base.py` & `swarms-5.1.3/swarms/agents/base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/agents/developer_agents.py` & `swarms-5.1.3/swarms/agents/developer_agents.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/agents/omni_modal_agent.py` & `swarms-5.1.3/swarms/agents/omni_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/agents/simple_agent.py` & `swarms-5.1.3/swarms/agents/simple_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/agents/tool_agent.py` & `swarms-5.1.3/swarms/agents/tool_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/agents/worker_agent.py` & `swarms-5.1.3/swarms/agents/worker_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/artifacts/base_artifact.py` & `swarms-5.1.3/swarms/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/artifacts/text_artifact.py` & `swarms-5.1.3/swarms/artifacts/text_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/memory/__init__.py` & `swarms-5.1.3/swarms/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/memory/base_db.py` & `swarms-5.1.3/swarms/memory/base_db.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/memory/base_vectordb.py` & `swarms-5.1.3/swarms/memory/base_vectordb.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/memory/dict_internal_memory.py` & `swarms-5.1.3/swarms/memory/dict_internal_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/memory/dict_shared_memory.py` & `swarms-5.1.3/swarms/memory/dict_shared_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/memory/short_term_memory.py` & `swarms-5.1.3/swarms/memory/short_term_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/memory/visual_memory.py` & `swarms-5.1.3/swarms/memory/visual_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/__init__.py` & `swarms-5.1.3/swarms/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/base_embedding_model.py` & `swarms-5.1.3/swarms/models/base_embedding_model.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/base_llm.py` & `swarms-5.1.3/swarms/models/base_llm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/base_multimodal_model.py` & `swarms-5.1.3/swarms/models/base_multimodal_model.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/base_tts.py` & `swarms-5.1.3/swarms/models/base_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/base_ttv.py` & `swarms-5.1.3/swarms/models/base_ttv.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/cog_vlm.py` & `swarms-5.1.3/swarms/models/cog_vlm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/dalle3.py` & `swarms-5.1.3/swarms/models/dalle3.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/distilled_whisperx.py` & `swarms-5.1.3/swarms/models/distilled_whisperx.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/embeddings_base.py` & `swarms-5.1.3/swarms/models/embeddings_base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/fuyu.py` & `swarms-5.1.3/swarms/models/fuyu.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/gemini.py` & `swarms-5.1.3/swarms/models/gemini.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/gpt4_vision_api.py` & `swarms-5.1.3/swarms/models/gpt4_vision_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,14 +164,15 @@
             )
 
             # Get the response as a JSON object
             response_json = response.json()
 
             # Return the JSON object if return_json is True
             if return_json is True:
+                print(response_json)
                 return response_json
             else:
                 return response_json["choices"][0]["message"]["content"]
 
         except Exception as error:
             logger.error(
                 f"Error with the request: {error}, make sure you"
```

### Comparing `swarms-5.0.8/swarms/models/huggingface.py` & `swarms-5.1.3/swarms/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/huggingface_pipeline.py` & `swarms-5.1.3/swarms/models/huggingface_pipeline.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/idefics.py` & `swarms-5.1.3/swarms/models/idefics.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/kosmos_two.py` & `swarms-5.1.3/swarms/models/kosmos_two.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/layoutlm_document_qa.py` & `swarms-5.1.3/swarms/models/layoutlm_document_qa.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/llama3_hosted.py` & `swarms-5.1.3/swarms/models/llama3_hosted.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/llama_function_caller.py` & `swarms-5.1.3/swarms/models/llama_function_caller.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/llava.py` & `swarms-5.1.3/swarms/models/llava.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/moondream_mm.py` & `swarms-5.1.3/swarms/models/moondream_mm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/nougat.py` & `swarms-5.1.3/swarms/models/nougat.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/open_dalle.py` & `swarms-5.1.3/swarms/models/open_dalle.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/open_router.py` & `swarms-5.1.3/swarms/models/open_router.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/openai_tts.py` & `swarms-5.1.3/swarms/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/popular_llms.py` & `swarms-5.1.3/swarms/models/popular_llms.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,18 +61,20 @@
 
 
 class OpenAIChatLLM(OpenAIChat):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def __call__(self, *args, **kwargs):
-        return self.invoke(*args, **kwargs)
+        out = self.invoke(*args, **kwargs)
+        return out.content.strip()
 
     def run(self, *args, **kwargs):
-        return self.invoke(*args, **kwargs)
+        out = self.invoke(*args, **kwargs)
+        return out.content.strip()
 
 
 class OctoAIChat(OctoAIEndpoint):
     def __call__(self, *args, **kwargs):
         return self.invoke(*args, **kwargs)
 
     def run(self, *args, **kwargs):
```

### Comparing `swarms-5.0.8/swarms/models/qwen.py` & `swarms-5.1.3/swarms/models/qwen.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/sam.py` & `swarms-5.1.3/swarms/models/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/sampling_params.py` & `swarms-5.1.3/swarms/models/sampling_params.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/ssd_1b.py` & `swarms-5.1.3/swarms/models/ssd_1b.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/together.py` & `swarms-5.1.3/swarms/models/together.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/types.py` & `swarms-5.1.3/swarms/models/types.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/vilt.py` & `swarms-5.1.3/swarms/models/vilt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/vip_llava.py` & `swarms-5.1.3/swarms/models/vip_llava.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/models/zeroscope.py` & `swarms-5.1.3/swarms/models/zeroscope.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/__init__.py` & `swarms-5.1.3/swarms/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/accountant_swarm_prompts.py` & `swarms-5.1.3/swarms/prompts/accountant_swarm_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/aga.py` & `swarms-5.1.3/swarms/prompts/aga.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/agent_output_parser.py` & `swarms-5.1.3/swarms/prompts/agent_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/agent_prompt.py` & `swarms-5.1.3/swarms/prompts/agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/agent_prompts.py` & `swarms-5.1.3/swarms/prompts/agent_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/agent_system_prompts.py` & `swarms-5.1.3/swarms/prompts/agent_system_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/ai_research_team.py` & `swarms-5.1.3/swarms/prompts/ai_research_team.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/aot_prompt.py` & `swarms-5.1.3/swarms/prompts/aot_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/autobloggen.py` & `swarms-5.1.3/swarms/prompts/autobloggen.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/autoswarm.py` & `swarms-5.1.3/swarms/prompts/autoswarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/base.py` & `swarms-5.1.3/swarms/prompts/base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/chat_prompt.py` & `swarms-5.1.3/swarms/prompts/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/code_interpreter.py` & `swarms-5.1.3/swarms/prompts/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/code_spawner.py` & `swarms-5.1.3/swarms/prompts/code_spawner.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/debate.py` & `swarms-5.1.3/swarms/prompts/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/documentation.py` & `swarms-5.1.3/swarms/prompts/documentation.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/education.py` & `swarms-5.1.3/swarms/prompts/education.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/finance_agent_prompt.py` & `swarms-5.1.3/swarms/prompts/finance_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/growth_agent_prompt.py` & `swarms-5.1.3/swarms/prompts/growth_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/idea2img.py` & `swarms-5.1.3/swarms/prompts/idea2img.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/legal_agent_prompt.py` & `swarms-5.1.3/swarms/prompts/legal_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/logistics.py` & `swarms-5.1.3/swarms/prompts/logistics.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/meta_system_prompt.py` & `swarms-5.1.3/swarms/prompts/meta_system_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/multi_modal_autonomous_instruction_prompt.py` & `swarms-5.1.3/swarms/prompts/multi_modal_autonomous_instruction_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/multi_modal_prompts.py` & `swarms-5.1.3/swarms/prompts/multi_modal_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/multi_modal_visual_prompts.py` & `swarms-5.1.3/swarms/prompts/multi_modal_visual_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/operations_agent_prompt.py` & `swarms-5.1.3/swarms/prompts/operations_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/personal_stylist.py` & `swarms-5.1.3/swarms/prompts/personal_stylist.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/product_agent_prompt.py` & `swarms-5.1.3/swarms/prompts/product_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/programming.py` & `swarms-5.1.3/swarms/prompts/programming.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/project_manager.py` & `swarms-5.1.3/swarms/prompts/project_manager.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/python.py` & `swarms-5.1.3/swarms/prompts/python.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/react.py` & `swarms-5.1.3/swarms/prompts/react.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/sales.py` & `swarms-5.1.3/swarms/prompts/sales.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/sales_prompts.py` & `swarms-5.1.3/swarms/prompts/sales_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/security_team.py` & `swarms-5.1.3/swarms/prompts/security_team.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/self_operating_prompt.py` & `swarms-5.1.3/swarms/prompts/self_operating_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/sop_generator_agent_prompt.py` & `swarms-5.1.3/swarms/prompts/sop_generator_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/summaries_prompts.py` & `swarms-5.1.3/swarms/prompts/summaries_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/support_agent_prompt.py` & `swarms-5.1.3/swarms/prompts/support_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/swarm_manager_agent.py` & `swarms-5.1.3/swarms/prompts/swarm_manager_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/task_assignment_prompt.py` & `swarms-5.1.3/swarms/prompts/task_assignment_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/tests.py` & `swarms-5.1.3/swarms/prompts/tests.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/tools.py` & `swarms-5.1.3/swarms/prompts/tools.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/urban_planning.py` & `swarms-5.1.3/swarms/prompts/urban_planning.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/visual_cot.py` & `swarms-5.1.3/swarms/prompts/visual_cot.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/worker_prompt.py` & `swarms-5.1.3/swarms/prompts/worker_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/prompts/xray_swarm_prompt.py` & `swarms-5.1.3/swarms/prompts/xray_swarm_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/schemas/hass_agent_schema.py` & `swarms-5.1.3/swarms/schemas/hass_agent_schema.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/schemas/schemas.py` & `swarms-5.1.3/swarms/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/schemas/step.py` & `swarms-5.1.3/swarms/schemas/step.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/__init__.py` & `swarms-5.1.3/swarms/structs/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/agent.py` & `swarms-5.1.3/swarms/structs/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,31 +19,33 @@
 from swarms.prompts.aot_prompt import algorithm_of_thoughts_sop
 from swarms.prompts.multi_modal_autonomous_instruction_prompt import (
     MULTI_MODAL_AUTO_AGENT_SYSTEM_PROMPT_1,
 )
 from swarms.structs.conversation import Conversation
 from swarms.structs.yaml_model import YamlModel
 from swarms.telemetry.user_utils import get_user_device_data
-from swarms.tools.base_tool import BaseTool
 from swarms.tools.prebuilt.code_interpreter import (
     SubprocessCodeInterpreter,
 )
 from swarms.tools.pydantic_to_json import (
-    base_model_to_openai_function,
     multi_base_model_to_openai_function,
 )
 from swarms.utils.data_to_text import data_to_text
 from swarms.utils.parse_code import extract_code_from_markdown
 from swarms.utils.pdf_to_text import pdf_to_text
 from swarms.tools.py_func_to_openai_func_str import (
     get_openai_function_schema_from_func,
 )
 from swarms.tools.func_calling_executor import openai_tool_executor
 from swarms.structs.base_structure import BaseStructure
 from swarms.prompts.tools import tool_sop_prompt
+from swarms.tools.func_calling_utils import (
+    pydantic_model_to_json_str,
+    prepare_output_for_output_model,
+)
 
 
 # Utils
 # Custom stopping condition
 def stop_when_repeats(response: str) -> bool:
     # Stop if the word stop appears in the response
     return "stop" in response.lower()
@@ -68,14 +70,18 @@
 
     Returns:
         str: A string representation of a UUID.
     """
     return str(uuid.uuid4())
 
 
+def exists(val):
+    return val is not None
+
+
 # Step ID generator
 def step_id():
     return str(uuid.uuid1())
 
 
 # Agent output types
 agent_output_type = Union[BaseModel, dict, str]
@@ -245,14 +251,15 @@
         tree_of_thoughts: bool = False,
         tool_choice: str = "auto",
         execute_tool: bool = False,
         rules: str = None,
         planning: Optional[str] = False,
         planning_prompt: Optional[str] = None,
         device: str = None,
+        custom_planning_prompt: str = None,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.id = id
         self.llm = llm
         self.template = template
@@ -343,20 +350,14 @@
         # If multimodal = yes then set the sop to the multimodal sop
         if self.multi_modal:
             self.sop = MULTI_MODAL_AUTO_AGENT_SYSTEM_PROMPT_1
 
         # Memory
         self.feedback = []
 
-        # Initialize the code executor
-        if self.code_interpreter is not False:
-            self.code_executor = SubprocessCodeInterpreter(
-                debug_mode=True,
-            )
-
         # If the preset stopping token is enabled then set the stopping token to the preset stopping token
         if preset_stopping_token is not None:
             self.stopping_token = "<DONE>"
 
         # If the system prompt is provided then set the system prompt
         # Initialize the short term memory
         self.short_memory = Conversation(
@@ -365,43 +366,34 @@
             user=user_name,
             rules=rules,
             *args,
             **kwargs,
         )
 
         # If the docs exist then ingest the docs
-        if self.docs:
+        if self.docs is not None:
             self.ingest_docs(self.docs)
 
         # If docs folder exists then get the docs from docs folder
         if self.docs_folder:
             self.get_docs_from_doc_folders()
 
         # If tokenizer and context length exists then:
         # if self.tokenizer and self.context_length:
         #     self.truncate_history()
 
         # If verbose is enabled then set the logger level to info
-        # if verbose:
+        # if verbose is not False:
         #     logger.setLevel(logging.INFO)
 
         if tools is not None:
 
             # Add the tool prompt to the memory
             self.short_memory.add(role="System", content=tool_sop_prompt())
 
-            # # BaseTool
-            # self.base_tool = BaseTool(
-            #     functions=tools,
-            #     verbose=verbose,
-            #     auto_execute_tool=execute_tool,
-            #     autocheck=True,
-            #     base_models=list_base_models,
-            # )
-
             # Print number of tools
             logger.info(f"Number of tools: {len(tools)}")
             logger.info(
                 "Tools provided, Automatically converting to OpenAI function"
             )
 
             # Now the names of the tools
@@ -426,63 +418,42 @@
                 self.short_memory.add(
                     role="System", content=tool_schema_list
                 )
 
             # Now create a function calling map for every tools
             self.function_map = {tool.__name__: tool for tool in tools}
 
-        # # If tools are provided then set the tool prompt by adding to sop
-        # if self.tools is not None:
-        #     if custom_tools_prompt is not None:
-        #         tools_prompt = custom_tools_prompt(tools=self.tools)
-
-        #         # Append the tools prompt to the short_term_memory
-        #         self.short_memory.add(
-        #             role=self.agent_name, content=tools_prompt
-        #         )
-
-        #     else:
-        #         # Default tool prompt
-        #         tools_prompt = tool_usage_worker_prompt(tools=self.tools)
-
-        #         # Append the tools prompt to the short_term_memory
-        #         self.short_memory.add(
-        #             role=self.agent_name, content=tools_prompt
-        #         )
-
         # Set the logger handler
-        if logger_handler:
+        if exists(logger_handler):
             logger.add(
                 f"{self.agent_name}.log",
                 level="INFO",
                 colorize=True,
                 format=("<green>{time}</green> <level>{message}</level>"),
                 backtrace=True,
                 diagnose=True,
             )
 
-        # logger.info("Creating Agent {}".format(self.agent_name))
-
         # If the tool types are provided
         if self.tool_schema is not None:
             # Log the tool schema
             logger.info(
                 "Tool schema provided, Automatically converting to OpenAI function"
             )
-            tool_schema_str = self.pydantic_model_to_json_str(
+            tool_schema_str = pydantic_model_to_json_str(
                 self.tool_schema, indent=4
             )
             logger.info(f"Tool Schema: {tool_schema_str}")
             # Add the tool schema to the short memory
             self.short_memory.add(
                 role=self.user_name, content=tool_schema_str
             )
 
         # If a list of tool schemas is provided
-        if self.list_base_models is not None:
+        if exists(self.list_base_models):
             logger.info(
                 "List of tool schemas provided, Automatically converting to OpenAI function"
             )
             tool_schemas = multi_base_model_to_openai_function(
                 self.list_base_models
             )
 
@@ -505,19 +476,19 @@
         # Return the history
         if return_history is True:
             logger.info(f"Beginning of Agent {self.agent_name} History")
             logger.info(self.short_memory.return_history_as_string())
             logger.info(f"End of Agent {self.agent_name} History")
 
         # If the user inputs a list of strings for the sop then join them and set the sop
-        if self.sop_list:
+        if exists(self.sop_list):
             self.sop = "\n".join(self.sop_list)
             self.short_memory.add(role=self.user_name, content=self.sop)
 
-        if self.sop is not None:
+        if exists(self.sop):
             self.short_memory.add(role=self.user_name, content=self.sop)
 
         # If the device is not provided then get the device data
 
     def set_system_prompt(self, system_prompt: str):
         """Set the system prompt"""
         self.system_prompt = system_prompt
@@ -611,19 +582,21 @@
         start_time = time.time()
         self.llm(text)
         end_time = time.time()
         return end_time - start_time
 
     # ############## TOKENIZER FUNCTIONS ##############
 
-    def add_message_to_memory(self, message: str):
+    def add_message_to_memory(self, message: str, *args, **kwargs):
         """Add the message to the memory"""
         try:
             logger.info(f"Adding message to memory: {message}")
-            self.short_memory.add(role=self.agent_name, content=message)
+            self.short_memory.add(
+                role=self.agent_name, content=message, *args, **kwargs
+            )
         except Exception as error:
             print(
                 colored(f"Error adding message to memory: {error}", "red")
             )
 
     def add_message_to_memory_and_truncate(self, message: str):
         """Add the message to the memory and truncate"""
@@ -721,145 +694,52 @@
             content (str, optional): The content to be streamed. Defaults to None.
         """
         for letter in content:
             print(letter, end="")
 
     ########################## FUNCTION CALLING ##########################
 
-    def json_str_to_json(self, json_str: str):
-        """Convert a JSON string to a JSON object"""
-        return json.loads(json_str)
-
-    def json_str_to_pydantic_model(self, json_str: str, model: BaseModel):
-        """Convert a JSON string to a Pydantic model"""
-        return model.model_validate_json(json_str)
-
-    def json_str_to_dict(self, json_str: str):
-        """Convert a JSON string to a dictionary"""
-        return json.loads(json_str)
-
-    def pydantic_model_to_json_str(
-        self, model: BaseModel, indent, *args, **kwargs
-    ):
-        return json.dumps(
-            base_model_to_openai_function(model),
-            indent=indent,
-            *args,
-            **kwargs,
-        )
-
-    def dict_to_json_str(self, dictionary: dict):
-        """Convert a dictionary to a JSON string"""
-        return json.dumps(dictionary)
-
-    def dict_to_pydantic_model(self, dictionary: dict, model: BaseModel):
-        """Convert a dictionary to a Pydantic model"""
-        return model.model_validate_json(dictionary)
-
-    # def prep_pydantic_model_for_str(self, model: BaseModel):
-    #     # Convert to Function
-    #     out = self.pydantic_model_to_json_str(model)
-
-    #     # return function_to_str(out)
-
-    def tool_schema_to_str(
-        self, tool_schema: BaseModel = None, *args, **kwargs
-    ):
-        """Convert a tool schema to a string"""
-        out = base_model_to_openai_function(tool_schema)
-        return str(out)
-
-    def tool_schemas_to_str(
-        self, tool_schemas: List[BaseModel] = None, *args, **kwargs
-    ):
-        """Convert a list of tool schemas to a string"""
-        out = multi_base_model_to_openai_function(tool_schemas)
-        return str(out)
-
-    def str_to_pydantic_model(self, string: str, model: BaseModel):
-        """Convert a string to a Pydantic model"""
-        return model.model_validate_json(string)
-
-    def list_str_to_pydantic_model(
-        self, list_str: List[str], model: BaseModel
-    ):
-        """Convert a list of strings to a Pydantic model"""
-        # return model.model_validate_json(list_str)
-        for string in list_str:
-            return model.model_validate_json(string)
-
-    def prepare_output_for_output_model(
-        self, output: agent_output_type = None
-    ):
-        """Prepare the output for the output model"""
-        if self.output_type == BaseModel:
-            return self.str_to_pydantic_model(output, self.output_type)
-        elif self.output_type == dict:
-            return self.dict_to_json_str(output)
-        elif self.output_type == str:
-            return output
-        else:
-            return output
-
-    ########################## FUNCTION CALLING ##########################
-
     def run(
         self,
         task: Optional[str] = None,
         img: Optional[str] = None,
         *args,
         **kwargs,
     ):
         """
         Run the autonomous agent loop
         """
         try:
             self.activate_autonomous_agent()
 
-            # Check if the task is not None
-            if task is not None:
-                self.short_memory.add(role=self.user_name, content=task)
+            # Add task to memory
+            self.short_memory.add(role=self.user_name, content=task)
 
+            # Set the loop count
             loop_count = 0
 
             # Clear the short memory
-            # self.short_memory.clear()
-            response = None
+            # response = None
 
-            while (
-                self.max_loops == "auto"
-                or loop_count < self.max_loops
-                # or self.custom_loop_condition()
-            ):
+            while self.max_loops == "auto" or loop_count < self.max_loops:
                 loop_count += 1
                 self.loop_count_print(loop_count, self.max_loops)
                 print("\n")
 
                 # Dynamic temperature
-                if self.dynamic_temperature_enabled:
+                if self.dynamic_temperature_enabled is True:
                     self.dynamic_temperature()
 
                 # Task prompt
                 task_prompt = self.short_memory.return_history_as_string()
 
                 attempt = 0
                 success = False
                 while attempt < self.retry_attempts and not success:
                     try:
-                        if self.planning is not False:
-                            plan = self.llm(self.planning_prompt)
-
-                            # Add the plan to the memory
-                            self.short_memory.add(
-                                role=self.agent_name, content=plan
-                            )
-
-                            task_prompt = (
-                                self.short_memory.return_history_as_string()
-                            )
 
                         response_args = (
                             (task_prompt, *args)
                             if img is None
                             else (task_prompt, img, *args)
                         )
                         response = self.llm(*response_args, **kwargs)
@@ -870,76 +750,18 @@
                         # Add the response to the memory
                         self.short_memory.add(
                             role=self.agent_name, content=response
                         )
 
                         # Check if tools is not None
                         if self.tools is not None:
+                            self.parse_and_execute_tools(response)
 
-                            # Extract json from markdown
-                            response = extract_code_from_markdown(response)
-
-                            # Try executing the tool
-                            if self.execute_tool is not False:
-                                try:
-                                    logger.info("Executing tool...")
-
-                                    # try to Execute the tool and return a string
-                                    out = openai_tool_executor(
-                                        tools=response,
-                                        function_map=self.function_map,
-                                        return_as_string=True,
-                                    )
-
-                                    print(f"Tool Output: {out}")
-
-                                    # Add the output to the memory
-                                    self.short_memory.add(
-                                        role=self.agent_name,
-                                        content=out,
-                                    )
-
-                                except Exception as error:
-                                    logger.error(
-                                        f"Error executing tool: {error}"
-                                    )
-                                    print(
-                                        colored(
-                                            f"Error executing tool: {error}",
-                                            "red",
-                                        )
-                                    )
-
-                        if self.code_interpreter:
-                            # Extract code from markdown
-                            extracted_code = extract_code_from_markdown(
-                                response
-                            )
-
-                            # Execute the code
-                            execution = SubprocessCodeInterpreter(
-                                debug_mode=True
-                            ).run(extracted_code)
-
-                            # Add the execution to the memory
-                            self.short_memory.add(
-                                role=self.agent_name,
-                                content=execution,
-                            )
-
-                            # Run the llm again
-                            response = self.llm(
-                                self.short_memory.return_history_as_string(),
-                                *args,
-                                **kwargs,
-                            )
-
-                            print(
-                                f"Response after code interpretation: {response}"
-                            )
+                        if exists(self.code_interpreter):
+                            self.code_interpreter_execution(response)
 
                         if self.evaluator:
                             evaluated_response = self.evaluator(response)
                             print(
                                 "Evaluated Response:"
                                 f" {evaluated_response}"
                             )
@@ -1033,15 +855,15 @@
                 logger.info("Applying output cleaner to response.")
                 response = self.output_cleaner(response)
                 logger.info(f"Response after output cleaner: {response}")
 
             # Prepare the output for the output model
             if self.output_type is not None:
                 # logger.info("Preparing output for output model.")
-                response = self.prepare_output_for_output_model(response)
+                response = prepare_output_for_output_model(response)
                 print(f"Response after output model: {response}")
 
             # print(response)
 
             return response
         except Exception as error:
             print(f"Error running agent: {error}")
@@ -1056,14 +878,48 @@
         """
         try:
             return self.run(task, img, *args, **kwargs)
         except Exception as error:
             logger.error(f"Error calling agent: {error}")
             raise error
 
+    def parse_and_execute_tools(self, response: str, *args, **kwargs):
+        # Extract json from markdown
+        response = extract_code_from_markdown(response)
+
+        # Try executing the tool
+        if self.execute_tool is not False:
+            try:
+                logger.info("Executing tool...")
+
+                # try to Execute the tool and return a string
+                out = openai_tool_executor(
+                    tools=response,
+                    function_map=self.function_map,
+                    *args,
+                    **kwargs,
+                )
+
+                print(f"Tool Output: {out}")
+
+                # Add the output to the memory
+                self.short_memory.add(
+                    role=self.agent_name,
+                    content=out,
+                )
+
+            except Exception as error:
+                logger.error(f"Error executing tool: {error}")
+                print(
+                    colored(
+                        f"Error executing tool: {error}",
+                        "red",
+                    )
+                )
+
     def long_term_memory_prompt(self, query: str, *args, **kwargs):
         """
         Generate the agent long term memory prompt
 
         Args:
             system_prompt (str): The system prompt
             history (List[str]): The history of the conversation
@@ -1086,14 +942,35 @@
 
         Returns:
             _type_: _description_
         """
         logger.info(f"Adding memory: {message}")
         return self.short_memory.add(role=self.agent_name, content=message)
 
+    def plan(self, task: str, *args, **kwargs):
+        """
+        Plan the task
+
+        Args:
+            task (str): The task to plan
+        """
+        try:
+            if exists(self.planning_prompt):
+                # Join the plan and the task
+                planning_prompt = f"{self.planning_prompt} {task}"
+                plan = self.llm(planning_prompt)
+
+            # Add the plan to the memory
+            self.short_memory.add(role=self.agent_name, content=plan)
+
+            return None
+        except Exception as error:
+            logger.error(f"Error planning task: {error}")
+            raise error
+
     async def run_concurrent(self, task: str, *args, **kwargs):
         """
         Run a task concurrently.
 
         Args:
             task (str): The task to run.
         """
@@ -1278,14 +1155,42 @@
         agent.run("Generate a report on Trump")
 
 
         """
         logger.info(f"Adding response filter: {filter_word}")
         self.reponse_filters.append(filter_word)
 
+    def code_interpreter_execution(
+        self, code: str, *args, **kwargs
+    ) -> str:
+        # Extract code from markdown
+        extracted_code = extract_code_from_markdown(code)
+
+        # Execute the code
+        execution = SubprocessCodeInterpreter(debug_mode=True).run(
+            extracted_code
+        )
+
+        # Add the execution to the memory
+        self.short_memory.add(
+            role=self.agent_name,
+            content=execution,
+        )
+
+        # Run the llm again
+        response = self.llm(
+            self.short_memory.return_history_as_string(),
+            *args,
+            **kwargs,
+        )
+
+        print(f"Response after code interpretation: {response}")
+
+        return response
+
     def apply_reponse_filters(self, response: str) -> str:
         """
         Apply the response filters to the response
 
         """
         logger.info(f"Applying response filters to response: {response}")
         for word in self.response_filters:
@@ -1635,20 +1540,27 @@
             self.short_memory.return_history_as_string()
         )
 
         # Now the logic that truncates the memory if it's more than the count
         if len(self.short_memory) > count:
             self.short_memory = self.short_memory[:count]
 
-    def add_tool(self, tool: BaseTool):
+    def add_tool(self, tool: Callable):
         return self.tools.append(tool)
 
-    def add_tools(self, tools: List[BaseTool]):
+    def add_tools(self, tools: List[Callable]):
         return self.tools.extend(tools)
 
+    def remove_tool(self, tool: Callable):
+        return self.tools.remove(tool)
+
+    def remove_tools(self, tools: List[Callable]):
+        for tool in tools:
+            self.tools.remove(tool)
+
     def get_docs_from_doc_folders(self):
         """Get the docs from the files"""
         try:
             logger.info("Getting docs from doc folders")
             # Get the list of files then extract them and add them to the memory
             files = os.listdir(self.docs_folder)
```

### Comparing `swarms-5.0.8/swarms/structs/agent_job.py` & `swarms-5.1.3/swarms/structs/agent_job.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/agent_process.py` & `swarms-5.1.3/swarms/structs/agent_process.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/async_workflow.py` & `swarms-5.1.3/swarms/structs/async_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/auto_swarm.py` & `swarms-5.1.3/swarms/structs/auto_swarm.py`

 * *Files 25% similar despite different names*

```diff
@@ -50,14 +50,18 @@
         self.custom_preprocess = custom_preprocess
         self.custom_postprocess = custom_postprocess
         self.custom_router = custom_router
 
         # Create a dictionary of swarms
         self.swarm_dict = {swarm.name: swarm for swarm in self.swarms}
 
+        logger.info(
+            f"AutoSwarmRouter has been initialized with {self.len_of_swarms()} swarms."
+        )
+
     def run(self, task: str = None, *args, **kwargs):
         try:
             """Run the swarm simulation and route the task to the appropriate swarm."""
 
             if self.custom_preprocess:
                 # If custom preprocess function is provided then run it
                 logger.info("Running custom preprocess function.")
@@ -88,14 +92,29 @@
 
             # If no match is found then return None
             raise ValueError(f"Swarm with name {self.name} not found.")
         except Exception as e:
             logger.error(f"Error: {e}")
             raise e
 
+    def len_of_swarms(self):
+        return print(len(self.swarms))
+
+    def list_available_swarms(self):
+        for swarm in self.swarms:
+            try:
+                logger.info(
+                    f"Swarm Name: {swarm.name} || Swarm Description: {swarm.description} "
+                )
+            except Exception as error:
+                logger.error(
+                    f"Error Detected You may not have swarms available: {error}"
+                )
+                raise error
+
 
 class AutoSwarm(BaseSwarm):
     """AutoSwarm class represents a swarm of agents that can be created automatically.
 
     Flow:
     name -> router -> swarm entry point
 
@@ -137,14 +156,27 @@
             custom_preprocess=custom_preprocess,
             custom_postprocess=custom_postprocess,
             custom_router=custom_router,
             *args,
             **kwargs,
         )
 
+        if name is None:
+            raise ValueError(
+                "A name must be provided for the AutoSwarm, what swarm do you want to use?"
+            )
+
+        if verbose is True:
+            self.init_logging()
+
+    def init_logging(self):
+        logger.info("AutoSwarm has been activated. Ready for usage.")
+
+    # def name_swarm_check(self, name: str = None):
+
     def run(self, task: str = None, *args, **kwargs):
         """Run the swarm simulation."""
         try:
             loop = 0
 
             while loop < self.max_loops:
                 if self.custom_preprocess:
@@ -171,7 +203,19 @@
 
                 return out
         except Exception as e:
             logger.error(
                 f"Error: {e} try optimizing the inputs and try again."
             )
             raise e
+
+    def list_all_swarms(self):
+        for swarm in self.swarms:
+            try:
+                logger.info(
+                    f"Swarm Name: {swarm.name} || Swarm Description: {swarm.description} "
+                )
+            except Exception as error:
+                logger.error(
+                    f"Error Detected You may not have swarms available: {error}"
+                )
+                raise error
```

### Comparing `swarms-5.0.8/swarms/structs/base_structure.py` & `swarms-5.1.3/swarms/structs/base_structure.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/base_swarm.py` & `swarms-5.1.3/swarms/structs/base_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/base_workflow.py` & `swarms-5.1.3/swarms/structs/base_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/company.py` & `swarms-5.1.3/swarms/structs/company.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/concurrent_workflow.py` & `swarms-5.1.3/swarms/structs/concurrent_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/conversation.py` & `swarms-5.1.3/swarms/structs/conversation.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/debate.py` & `swarms-5.1.3/swarms/structs/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/groupchat.py` & `swarms-5.1.3/swarms/structs/groupchat.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/hiearchical_swarm.py` & `swarms-5.1.3/swarms/structs/hiearchical_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/majority_voting.py` & `swarms-5.1.3/swarms/structs/majority_voting.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/message.py` & `swarms-5.1.3/swarms/structs/message.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/message_pool.py` & `swarms-5.1.3/swarms/structs/message_pool.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/meta_system_prompt.py` & `swarms-5.1.3/swarms/structs/meta_system_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/multi_agent_collab.py` & `swarms-5.1.3/swarms/structs/multi_agent_collab.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/multi_process_workflow.py` & `swarms-5.1.3/swarms/structs/multi_process_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/multi_threaded_workflow.py` & `swarms-5.1.3/swarms/structs/multi_threaded_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/rearrange.py` & `swarms-5.1.3/swarms/structs/rearrange.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/recursive_workflow.py` & `swarms-5.1.3/swarms/structs/recursive_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/round_robin.py` & `swarms-5.1.3/swarms/structs/round_robin.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/sequential_workflow.py` & `swarms-5.1.3/swarms/structs/sequential_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/sermon_swarm.py` & `swarms-5.1.3/swarms/structs/sermon_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/society_of_agents.py` & `swarms-5.1.3/swarms/structs/society_of_agents.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/swarm_load_balancer.py` & `swarms-5.1.3/swarms/structs/swarm_load_balancer.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/swarm_net.py` & `swarms-5.1.3/swarms/structs/swarm_net.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/swarming_architectures.py` & `swarms-5.1.3/swarms/structs/swarming_architectures.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/task.py` & `swarms-5.1.3/swarms/structs/task.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/task_queue_base.py` & `swarms-5.1.3/swarms/structs/task_queue_base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/tree_of_thoughts.py` & `swarms-5.1.3/swarms/structs/tree_of_thoughts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/utils.py` & `swarms-5.1.3/swarms/structs/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/structs/yaml_model.py` & `swarms-5.1.3/swarms/structs/yaml_model.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/telemetry/__init__.py` & `swarms-5.1.3/swarms/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/telemetry/auto_upgrade_swarms.py` & `swarms-5.1.3/swarms/telemetry/auto_upgrade_swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/telemetry/check_update.py` & `swarms-5.1.3/swarms/telemetry/check_update.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/telemetry/log_all.py` & `swarms-5.1.3/swarms/telemetry/log_all.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/telemetry/sys_info.py` & `swarms-5.1.3/swarms/telemetry/sys_info.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/telemetry/user_utils.py` & `swarms-5.1.3/swarms/telemetry/user_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/tools/__init__.py` & `swarms-5.1.3/swarms/tools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,18 @@
     get_required_params,
     Function,
     ToolFunction,
 )
 from swarms.tools.openai_tool_creator_decorator import tool
 from swarms.tools.base_tool import BaseTool
 from swarms.tools.prebuilt import *  # noqa: F403
-
+from swarms.tools.cohere_func_call_schema import (
+    CohereFuncSchema,
+    ParameterDefinition,
+)
 
 __all__ = [
     "BaseTool",
     "tool",
     "Function",
     "ToolFunction",
     "get_openai_function_schema_from_func",
@@ -44,8 +47,10 @@
     "_remove_a_key",
     "openai_tool_executor",
     "execute_tools",
     "extract_tool_commands",
     "parse_and_execute_tools",
     "scrape_tool_func_docs",
     "tool_find_by_name",
+    "CohereFuncSchema",
+    "ParameterDefinition",
 ]
```

### Comparing `swarms-5.0.8/swarms/tools/base_tool.py` & `swarms-5.1.3/swarms/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/tools/func_calling_executor.py` & `swarms-5.1.3/swarms/tools/func_calling_executor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,176 @@
 import concurrent.futures
 from typing import Callable, Any, Dict, List
 from swarms.utils.loguru_logger import logger
 
 
+# def openai_tool_executor(
+#     tools: List[Dict[str, Any]],
+#     function_map: Dict[str, Callable],
+#     verbose: bool = True,
+#     return_as_string: bool = False,
+#     *args,
+#     **kwargs,
+# ) -> Callable:
+#     """
+#     Creates a function that dynamically and concurrently executes multiple functions based on parameters specified
+#     in a list of tool dictionaries, with extensive error handling and validation.
+
+#     Args:
+#         tools (List[Dict[str, Any]]): A list of dictionaries, each containing configuration for a tool, including parameters.
+#         function_map (Dict[str, Callable]): A dictionary mapping function names to their corresponding callable functions.
+#         verbose (bool): If True, enables verbose logging.
+#         return_as_string (bool): If True, returns the results as a concatenated string.
+
+#     Returns:
+#         Callable: A function that, when called, executes the specified functions concurrently with the parameters given.
+
+#     Examples:
+#     >>> def test_function(param1: int, param2: str) -> str:
+#     ...     return f"Test function called with parameters: {param1}, {param2}"
+
+#     >>> tool_executor = openai_tool_executor(
+#     ...     tools=[
+#     ...         {
+#     ...             "type": "function",
+#     ...             "function": {
+#     ...                 "name": "test_function",
+#     ...                 "parameters": {
+#     ...                     "param1": 1,
+#     ...                     "param2": "example"
+#     ...                 }
+#     ...             }
+#     ...         }
+#     ...     ],
+#     ...     function_map={
+#     ...         "test_function": test_function
+#     ...     },
+#     ...     return_as_string=True
+#     ... )
+#     >>> results = tool_executor()
+#     >>> print(results)
+#     """
+
+#     def tool_executor():
+#         # Prepare tasks for concurrent execution
+#         results = []
+#         logger.info(f"Executing {len(tools)} tools concurrently.")
+#         with concurrent.futures.ThreadPoolExecutor() as executor:
+#             futures = []
+#             for tool in tools:
+#                 if tool.get("type") != "function":
+#                     continue  # Skip non-function tool entries
+
+#                 function_info = tool.get("function", {})
+#                 func_name = function_info.get("name")
+#                 logger.info(f"Executing function: {func_name}")
+
+#                 # Check if the function name is mapped to an actual function
+#                 if func_name not in function_map:
+#                     error_message = f"Function '{func_name}' not found in function map."
+#                     logger.error(error_message)
+#                     results.append(error_message)
+#                     continue
+
+#                 # Validate parameters
+#                 params = function_info.get("parameters", {})
+#                 if not params:
+#                     error_message = f"No parameters specified for function '{func_name}'."
+#                     logger.error(error_message)
+#                     results.append(error_message)
+#                     continue
+
+#                 # Submit the function for execution
+#                 try:
+#                     future = executor.submit(
+#                         function_map[func_name], **params
+#                     )
+#                     futures.append((func_name, future))
+#                 except Exception as e:
+#                     error_message = f"Failed to submit the function '{func_name}' for execution: {e}"
+#                     logger.error(error_message)
+#                     results.append(error_message)
+
+#             # Gather results from all futures
+#             for func_name, future in futures:
+#                 try:
+#                     result = future.result()  # Collect result from future
+#                     results.append(f"{func_name}: {result}")
+#                 except Exception as e:
+#                     error_message = f"Error during execution of function '{func_name}': {e}"
+#                     logger.error(error_message)
+#                     results.append(error_message)
+
+#         if return_as_string:
+#             return "\n".join(results)
+
+#         logger.info(f"Results: {results}")
+
+#         return results
+
+#     return tool_executor
+
+
 def openai_tool_executor(
     tools: List[Dict[str, Any]],
     function_map: Dict[str, Callable],
     verbose: bool = True,
     return_as_string: bool = False,
     *args,
     **kwargs,
 ) -> Callable:
-    """
-    Creates a function that dynamically and concurrently executes multiple functions based on parameters specified
-    in a list of tool dictionaries, with extensive error handling and validation.
-
-    Args:
-        tools (List[Dict[str, Any]]): A list of dictionaries, each containing configuration for a tool, including parameters.
-        function_map (Dict[str, Callable]): A dictionary mapping function names to their corresponding callable functions.
-        verbose (bool): If True, enables verbose logging.
-        return_as_string (bool): If True, returns the results as a concatenated string.
-
-    Returns:
-        Callable: A function that, when called, executes the specified functions concurrently with the parameters given.
-
-    Examples:
-    >>> def test_function(param1: int, param2: str) -> str:
-    ...     return f"Test function called with parameters: {param1}, {param2}"
-
-    >>> tool_executor = openai_tool_executor(
-    ...     tools=[
-    ...         {
-    ...             "type": "function",
-    ...             "function": {
-    ...                 "name": "test_function",
-    ...                 "parameters": {
-    ...                     "param1": 1,
-    ...                     "param2": "example"
-    ...                 }
-    ...             }
-    ...         }
-    ...     ],
-    ...     function_map={
-    ...         "test_function": test_function
-    ...     },
-    ...     return_as_string=True
-    ... )
-    >>> results = tool_executor()
-    >>> print(results)
-    """
-
     def tool_executor():
-        # Prepare tasks for concurrent execution
         results = []
         logger.info(f"Executing {len(tools)} tools concurrently.")
         with concurrent.futures.ThreadPoolExecutor() as executor:
             futures = []
             for tool in tools:
                 if tool.get("type") != "function":
-                    continue  # Skip non-function tool entries
+                    continue
 
                 function_info = tool.get("function", {})
                 func_name = function_info.get("name")
                 logger.info(f"Executing function: {func_name}")
 
-                # Check if the function name is mapped to an actual function
                 if func_name not in function_map:
                     error_message = f"Function '{func_name}' not found in function map."
                     logger.error(error_message)
                     results.append(error_message)
                     continue
 
-                # Validate parameters
                 params = function_info.get("parameters", {})
                 if not params:
                     error_message = f"No parameters specified for function '{func_name}'."
                     logger.error(error_message)
                     results.append(error_message)
                     continue
 
-                # Submit the function for execution
+                if "name" in params and params["name"] in function_map:
+                    try:
+                        result = function_map[params["name"]](**params)
+                        results.append(f"{params['name']}: {result}")
+                    except Exception as e:
+                        error_message = f"Failed to execute the function '{params['name']}': {e}"
+                        logger.error(error_message)
+                        results.append(error_message)
+                    continue
+
                 try:
                     future = executor.submit(
                         function_map[func_name], **params
                     )
                     futures.append((func_name, future))
                 except Exception as e:
                     error_message = f"Failed to submit the function '{func_name}' for execution: {e}"
                     logger.error(error_message)
                     results.append(error_message)
 
-            # Gather results from all futures
             for func_name, future in futures:
                 try:
-                    result = future.result()  # Collect result from future
+                    result = future.result()
                     results.append(f"{func_name}: {result}")
                 except Exception as e:
                     error_message = f"Error during execution of function '{func_name}': {e}"
                     logger.error(error_message)
                     results.append(error_message)
 
         if return_as_string:
@@ -106,71 +179,54 @@
         logger.info(f"Results: {results}")
 
         return results
 
     return tool_executor
 
 
-# # Example
-# @tool(
-#     name="test_function",
-#     description="A test function that takes two parameters and returns a string.",
-# )
-# def test_function(param1: int, param2: str) -> str:
-#     return f"Test function called with parameters: {param1}, {param2}"
+# function_schema = {
+#     "name": "execute",
+#     "description": "Executes code on the user's machine **in the users local environment** and returns the output",
+#     "parameters": {
+#         "type": "object",
+#         "properties": {
+#             "language": {
+#                 "type": "string",
+#                 "description": "The programming language (required parameter to the `execute` function)",
+#                 "enum": [
+#                     # This will be filled dynamically with the languages OI has access to.
+#                 ],
+#             },
+#             "code": {
+#                 "type": "string",
+#                 "description": "The code to execute (required)",
+#             },
+#         },
+#         "required": ["language", "code"],
+#     },
+# }
 
 
-# @tool(
-#     name="test_function2",
-#     description="A test function that takes two parameters and returns a string.",
-# )
-# def test_function2(param1: int, param2: str) -> str:
-#     return f"Test function 2 called with parameters: {param1}, {param2}"
+# def execute(language: str, code: str):
+#     """
+#     Executes code on the user's machine **in the users local environment** and returns the output
+
+#     Args:
+#         language (str): The programming language (required parameter to the `execute` function)
+#         code (str): The code to execute (required)
+
+#     Returns:
+#         str: The output of the code execution
+#     """
+#     # This function will be implemented by the user
+#     return "Code execution not implemented yet"
 
 
 # # Example execution
 # out = openai_tool_executor(
-#     tools=[
-#         {
-#             "type": "function",
-#             "function": {
-#                 "name": "test_function",
-#                 "parameters": {
-#                     "properties": {
-#                         "param1": {
-#                             "type": "int",
-#                             "description": "An integer parameter.",
-#                         },
-#                         "param2": {
-#                             "type": "str",
-#                             "description": "A string parameter.",
-#                         },
-#                     }
-#                 },
-#             },
-#         },
-#         {
-#             "type": "function",
-#             "function": {
-#                 "name": "test_function2",
-#                 "parameters": {
-#                     "properties": {
-#                         "param1": {
-#                             "type": "int",
-#                             "description": "An integer parameter.",
-#                         },
-#                         "param2": {
-#                             "type": "str",
-#                             "description": "A string parameter.",
-#                         },
-#                     }
-#                 },
-#             },
-#         },
-#     ],
+#     tools=[function_schema],
 #     function_map={
-#         "test_function": test_function,
-#         "test_function2": test_function2,
+#         "execute": execute,
 #     },
 #     return_as_string=True,
 # )
 # print(out)
```

### Comparing `swarms-5.0.8/swarms/tools/func_to_str.py` & `swarms-5.1.3/swarms/tools/func_to_str.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/tools/function_util.py` & `swarms-5.1.3/swarms/tools/function_util.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/tools/json_former.py` & `swarms-5.1.3/swarms/tools/json_former.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/tools/json_utils.py` & `swarms-5.1.3/swarms/tools/json_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/tools/logits_processor.py` & `swarms-5.1.3/swarms/tools/logits_processor.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/tools/openai_func_calling_schema_pydantic.py` & `swarms-5.1.3/swarms/tools/openai_func_calling_schema_pydantic.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/tools/openai_tool_creator_decorator.py` & `swarms-5.1.3/swarms/tools/openai_tool_creator_decorator.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/tools/prebuilt/code_interpreter.py` & `swarms-5.1.3/swarms/tools/prebuilt/code_interpreter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import queue
 import subprocess
 import threading
 import time
 import traceback
+from swarms.utils.loguru_logger import logger
 
 
 class SubprocessCodeInterpreter:
     """
     SubprocessCodeinterpreter is a base class for code interpreters that run code in a subprocess.
 
 
@@ -20,16 +21,26 @@
     Example:
     """
 
     def __init__(
         self,
         start_cmd: str = "python3",
         debug_mode: bool = False,
+        max_retries: int = 3,
+        verbose: bool = False,
+        retry_count: int = 0,
+        *args,
+        **kwargs,
     ):
         self.process = None
+        self.start_cmd = start_cmd
+        self.debug_mode = debug_mode
+        self.max_retries = max_retries
+        self.verbose = verbose
+        self.retry_count = retry_count
         self.output_queue = queue.Queue()
         self.done = threading.Event()
 
     def detect_active_line(self, line):
         """Detect if the line is an active line
 
         Args:
@@ -76,14 +87,15 @@
         self.process.terminate()
 
     def start_process(self):
         """start the subprocess"""
         if self.process:
             self.terminate()
 
+        logger.info(f"Starting subprocess with command: {self.start_cmd}")
         self.process = subprocess.Popen(
             self.start_cmd.split(),
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             text=True,
             bufsize=0,
@@ -96,62 +108,64 @@
         ).start()
         threading.Thread(
             target=self.handle_stream_output,
             args=(self.process.stderr, True),
             daemon=True,
         ).start()
 
+        return self.process
+
     def run(self, code: str):
         """Run the code in the subprocess
 
         Args:
             code (str): _description_
 
         Yields:
             _type_: _description_
         """
-        retry_count = 0
-        max_retries = 3
 
         # Setup
+        logger.info("Running code in subprocess")
         try:
             code = self.preprocess_code(code)
             if not self.process:
                 self.start_process()
         except BaseException:
             yield {"output": traceback.format_exc()}
             return
 
-        while retry_count <= max_retries:
+        while self.retry_count <= self.max_retries:
             if self.debug_mode:
                 print(f"Running code:\n{code}\n---")
 
             self.done.clear()
 
             try:
                 self.process.stdin.write(code + "\n")
                 self.process.stdin.flush()
                 break
             except BaseException:
-                if retry_count != 0:
+                if self.retry_count != 0:
                     # For UX, I like to hide this if it happens once. Obviously feels better to not see errors
                     # Most of the time it doesn't matter, but we should figure out why it happens frequently with:
                     # applescript
                     yield {"output": traceback.format_exc()}
                     yield {
                         "output": (
-                            "Retrying..." f" ({retry_count}/{max_retries})"
+                            "Retrying..."
+                            f" ({self.retry_count}/{self.max_retries})"
                         )
                     }
                     yield {"output": "Restarting process."}
 
                 self.start_process()
 
-                retry_count += 1
-                if retry_count > max_retries:
+                self.retry_count += 1
+                if self.retry_count > self.max_retries:
                     yield {
                         "output": (
                             "Maximum retries reached. Could not"
                             " execute code."
                         )
                     }
                     return
@@ -205,12 +219,12 @@
                 self.done.set()
             else:
                 self.output_queue.put({"output": line})
 
 
 # interpreter = SubprocessCodeInterpreter()
 # interpreter.start_cmd = "python3"
-# for output in interpreter.run("""
+# out = interpreter.run("""
 # print("hello")
 # print("world")
-# """):
-#     print(output)
+# """)
+# print(out)
```

### Comparing `swarms-5.0.8/swarms/tools/prebuilt/math_eval.py` & `swarms-5.1.3/swarms/tools/prebuilt/math_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/tools/py_func_to_openai_func_str.py` & `swarms-5.1.3/swarms/tools/py_func_to_openai_func_str.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/tools/pydantic_to_json.py` & `swarms-5.1.3/swarms/tools/pydantic_to_json.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/tools/tool_utils.py` & `swarms-5.1.3/swarms/tools/tool_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/README.md` & `swarms-5.1.3/swarms/utils/README.md`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/__init__.py` & `swarms-5.1.3/swarms/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/apa.py` & `swarms-5.1.3/swarms/utils/apa.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/check_function_result.py` & `swarms-5.1.3/swarms/utils/check_function_result.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/class_args_wrapper.py` & `swarms-5.1.3/swarms/utils/class_args_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/concurrent_utils.py` & `swarms-5.1.3/swarms/utils/concurrent_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/data_to_text.py` & `swarms-5.1.3/swarms/utils/data_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/decorators.py` & `swarms-5.1.3/swarms/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/disable_logging.py` & `swarms-5.1.3/swarms/utils/disable_logging.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/download_img.py` & `swarms-5.1.3/swarms/utils/download_img.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/execute_futures.py` & `swarms-5.1.3/swarms/utils/execute_futures.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/exponential_backoff.py` & `swarms-5.1.3/swarms/utils/exponential_backoff.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/fetch_init_params.py` & `swarms-5.1.3/swarms/utils/fetch_init_params.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/file_processing.py` & `swarms-5.1.3/swarms/utils/file_processing.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/find_img_path.py` & `swarms-5.1.3/swarms/utils/find_img_path.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/get_logger.py` & `swarms-5.1.3/swarms/utils/get_logger.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/get_total_gpus.py` & `swarms-5.1.3/swarms/utils/get_total_gpus.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/json_output_parser.py` & `swarms-5.1.3/swarms/utils/json_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/jsonl_utils.py` & `swarms-5.1.3/swarms/utils/jsonl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/llm_metrics_decorator.py` & `swarms-5.1.3/swarms/utils/llm_metrics_decorator.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/logger.py` & `swarms-5.1.3/swarms/utils/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/loggers.py` & `swarms-5.1.3/swarms/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/markdown_message.py` & `swarms-5.1.3/swarms/utils/markdown_message.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/optimized_loop.py` & `swarms-5.1.3/swarms/utils/optimized_loop.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import timeit
-from typing import Callable, Iterable, List, Optional, TypeVar, Union
+from typing import Callable, Iterable, List, Optional, TypeVar
 
-T = TypeVar('T')
-R = TypeVar('R')
+T = TypeVar("T")
+R = TypeVar("R")
 
-def optimized_loop(data: Iterable[T], 
-                   operation: Callable[[T], R], 
-                   condition: Optional[Callable[[T], bool]] = None) -> List[R]:
+
+def optimized_loop(
+    data: Iterable[T],
+    operation: Callable[[T], R],
+    condition: Optional[Callable[[T], bool]] = None,
+) -> List[R]:
     """
     Perform an optimized loop over the input data, applying an operation to each element.
     Optionally, filter elements based on a condition before applying the operation.
 
     Args:
         data (Iterable[T]): The input data to be processed. Can be any iterable type.
         operation (Callable[[T], R]): The operation to be applied to each element.
@@ -20,46 +23,57 @@
         List[R]: The result of applying the operation to the filtered elements.
     """
     if condition is not None:
         return [operation(x) for x in data if condition(x)]
     else:
         return [operation(x) for x in data]
 
+
 # Sample data, operation, and condition for benchmarking
 data = list(range(1000000))
-operation = lambda x: x * x
-condition = lambda x: x % 2 == 0
+
+
+def operation(x):
+    return x * x
+
+
+def condition(x):
+    return x % 2 == 0
+
 
 # Define a traditional loop for comparison
 def traditional_loop(data: Iterable[int]) -> List[int]:
     result = []
     for x in data:
         if x % 2 == 0:
             result.append(x * x)
     return result
 
+
 # Define a benchmarking function
 def benchmark():
     # Time the execution of the optimized loop
     optimized_time = timeit.timeit(
         stmt="optimized_loop(data, operation, condition)",
         setup="from __main__ import optimized_loop, data, operation, condition",
         globals=globals(),
-        number=10
+        number=10,
     )
 
     print(f"Optimized loop execution time: {optimized_time:.4f} seconds")
 
     # Time the execution of the traditional loop for comparison
     traditional_time = timeit.timeit(
         stmt="traditional_loop(data)",
         setup="from __main__ import traditional_loop, data",
         globals=globals(),
-        number=10
+        number=10,
+    )
+
+    print(
+        f"Traditional loop execution time: {traditional_time:.4f} seconds"
     )
 
-    print(f"Traditional loop execution time: {traditional_time:.4f} seconds")
 
 # Run the benchmark
 if __name__ == "__main__":
     benchmark()
-
```

### Comparing `swarms-5.0.8/swarms/utils/parse_code.py` & `swarms-5.1.3/swarms/utils/parse_code.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/pdf_to_text.py` & `swarms-5.1.3/swarms/utils/pdf_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/remove_json_whitespace.py` & `swarms-5.1.3/swarms/utils/remove_json_whitespace.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/save_logs.py` & `swarms-5.1.3/swarms/utils/save_logs.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/serializable.py` & `swarms-5.1.3/swarms/utils/serializable.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/try_except_wrapper.py` & `swarms-5.1.3/swarms/utils/try_except_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/swarms/utils/yaml_output_parser.py` & `swarms-5.1.3/swarms/utils/yaml_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.8/PKG-INFO` & `swarms-5.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 5.0.8
+Version: 5.1.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering,swarms,agents
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.10,<4.0
```

