# Comparing `tmp/semantic_kernel-0.1.0.dev0.tar.gz` & `tmp/semantic_kernel-0.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.1.0.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.2.0.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.1.0.dev0.tar` & `semantic_kernel-0.2.0.dev0.tar`

### file list

```diff
@@ -1,88 +1,87 @@
--rw-r--r--   0        0        0     1141 2023-01-27 22:17:02.142058 semantic_kernel-0.1.0.dev0/LICENSE
--rw-r--r--   0        0        0      613 2023-04-06 23:28:27.129015 semantic_kernel-0.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     2368 2023-04-07 20:25:34.545940 semantic_kernel-0.1.0.dev0/README.md
--rw-r--r--   0        0        0     1571 2023-04-06 23:28:27.130010 semantic_kernel-0.1.0.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-06 23:28:27.130010 semantic_kernel-0.1.0.dev0/semantic_kernel/ai/ai_exception.py
--rw-r--r--   0        0        0      495 2023-04-06 23:28:27.131011 semantic_kernel-0.1.0.dev0/semantic_kernel/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1129 2023-04-06 23:28:27.131011 semantic_kernel-0.1.0.dev0/semantic_kernel/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1332 2023-04-06 23:28:27.131011 semantic_kernel-0.1.0.dev0/semantic_kernel/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-06 23:28:27.132012 semantic_kernel-0.1.0.dev0/semantic_kernel/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      479 2023-04-06 23:28:27.132012 semantic_kernel-0.1.0.dev0/semantic_kernel/ai/embeddings/embedding_index_base.py
--rw-r--r--   0        0        0      817 2023-04-06 23:28:27.133010 semantic_kernel-0.1.0.dev0/semantic_kernel/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2771 2023-04-07 20:20:53.481793 semantic_kernel-0.1.0.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2763 2023-04-07 20:20:53.481793 semantic_kernel-0.1.0.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2758 2023-04-07 20:20:53.481793 semantic_kernel-0.1.0.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     4007 2023-04-07 20:20:53.483403 semantic_kernel-0.1.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     4441 2023-04-07 20:20:53.484320 semantic_kernel-0.1.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2427 2023-04-07 20:20:53.485320 semantic_kernel-0.1.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0      476 2023-04-06 23:28:27.135522 semantic_kernel-0.1.0.dev0/semantic_kernel/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      383 2023-04-06 23:28:27.136521 semantic_kernel-0.1.0.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2072 2023-04-06 23:28:27.136521 semantic_kernel-0.1.0.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     4641 2023-04-06 23:28:27.137521 semantic_kernel-0.1.0.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2403 2023-04-06 23:28:27.137521 semantic_kernel-0.1.0.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     5613 2023-04-06 23:28:27.138525 semantic_kernel-0.1.0.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0    10609 2023-04-06 23:28:27.138525 semantic_kernel-0.1.0.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     2342 2023-04-06 23:28:27.139523 semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_base.py
--rw-r--r--   0        0        0     3097 2023-04-06 23:28:27.139523 semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_builder.py
--rw-r--r--   0        0        0     9136 2023-04-06 23:28:27.140524 semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_config.py
--rw-r--r--   0        0        0     1626 2023-04-06 23:28:27.140524 semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      710 2023-04-06 23:28:27.141523 semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_extensions/__init__.py
--rw-r--r--   0        0        0      210 2023-04-06 23:28:27.141523 semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
--rw-r--r--   0        0        0     2374 2023-04-06 23:28:27.141523 semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_extensions/import_skills.py
--rw-r--r--   0        0        0     2323 2023-04-06 23:28:27.142522 semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_extensions/inline_definition.py
--rw-r--r--   0        0        0     1531 2023-04-06 23:28:27.142522 semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
--rw-r--r--   0        0        0      160 2023-04-06 23:28:27.143521 semantic_kernel-0.1.0.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     1174 2023-04-06 23:28:27.143521 semantic_kernel-0.1.0.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     1598 2023-04-06 23:28:27.143521 semantic_kernel-0.1.0.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0      299 2023-04-06 23:28:27.144521 semantic_kernel-0.1.0.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1137 2023-04-06 23:28:27.144521 semantic_kernel-0.1.0.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     2499 2023-04-06 23:28:27.144521 semantic_kernel-0.1.0.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     1237 2023-04-06 23:28:27.145522 semantic_kernel-0.1.0.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0      836 2023-04-06 23:28:27.145522 semantic_kernel-0.1.0.dev0/semantic_kernel/memory/storage/data_entry.py
--rw-r--r--   0        0        0      953 2023-04-06 23:28:27.145522 semantic_kernel-0.1.0.dev0/semantic_kernel/memory/storage/data_store_base.py
--rw-r--r--   0        0        0     1989 2023-04-06 23:28:27.145522 semantic_kernel-0.1.0.dev0/semantic_kernel/memory/storage/volatile_data_store.py
--rw-r--r--   0        0        0     4050 2023-04-06 23:28:27.146521 semantic_kernel-0.1.0.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2328 2023-04-06 23:28:27.146521 semantic_kernel-0.1.0.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-06 23:28:27.146521 semantic_kernel-0.1.0.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     8966 2023-04-06 23:28:27.147521 semantic_kernel-0.1.0.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-06 23:28:27.147521 semantic_kernel-0.1.0.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7322 2023-04-06 23:28:27.147521 semantic_kernel-0.1.0.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    13154 2023-04-06 23:28:27.148522 semantic_kernel-0.1.0.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     5681 2023-04-06 23:28:27.148522 semantic_kernel-0.1.0.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      919 2023-04-06 23:28:27.149523 semantic_kernel-0.1.0.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      673 2023-04-06 23:28:27.149523 semantic_kernel-0.1.0.dev0/semantic_kernel/reliability/retry_mechanism.py
--rw-r--r--   0        0        0     2101 2023-04-06 23:28:27.150523 semantic_kernel-0.1.0.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-06 23:28:27.150523 semantic_kernel-0.1.0.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-06 23:28:27.151524 semantic_kernel-0.1.0.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     3437 2023-04-06 23:28:27.151524 semantic_kernel-0.1.0.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-06 23:28:27.152522 semantic_kernel-0.1.0.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-06 23:28:27.152522 semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-06 23:28:27.153521 semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     1717 2023-04-06 23:28:27.154523 semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-06 23:28:27.154523 semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-06 23:28:27.155525 semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-06 23:28:27.155525 semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-06 23:28:27.156525 semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-06 23:28:27.156525 semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-06 23:28:27.156525 semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-06 23:28:27.157522 semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0      830 2023-04-06 23:28:27.158522 semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-06 23:28:27.158522 semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4590 2023-04-06 23:28:27.159522 semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-06 23:28:27.159522 semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-06 23:28:27.160524 semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-06 23:28:27.160524 semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-06 23:28:27.160524 semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-06 23:28:27.161522 semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-06 23:28:27.161522 semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-06 23:28:27.162539 semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-06 23:28:27.162539 semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-06 23:28:27.163522 semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-06 23:28:27.163522 semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     1115 2023-04-06 23:28:27.157522 semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0     7637 2023-04-06 23:28:27.164523 semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      403 2023-04-06 23:28:27.164523 semantic_kernel-0.1.0.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2436 2023-04-06 23:28:27.165522 semantic_kernel-0.1.0.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-06 23:28:27.165522 semantic_kernel-0.1.0.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-06 23:28:27.165522 semantic_kernel-0.1.0.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     2942 1970-01-01 00:00:00.000000 semantic_kernel-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0      632 2023-04-10 18:26:09.498820 semantic_kernel-0.2.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     3551 2023-04-10 18:26:09.496820 semantic_kernel-0.2.0.dev0/README.md
+-rw-r--r--   0        0        0     1571 2023-04-06 23:28:27.130010 semantic_kernel-0.2.0.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-06 23:28:27.130010 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/ai_exception.py
+-rw-r--r--   0        0        0      495 2023-04-06 23:28:27.131011 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1129 2023-04-06 23:28:27.131011 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1332 2023-04-06 23:28:27.131011 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-06 23:28:27.132012 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      479 2023-04-06 23:28:27.132012 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/embeddings/embedding_index_base.py
+-rw-r--r--   0        0        0      817 2023-04-06 23:28:27.133010 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2771 2023-04-07 20:20:53.481793 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2763 2023-04-07 20:20:53.481793 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2758 2023-04-07 20:20:53.481793 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     4007 2023-04-07 20:20:53.483403 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     4441 2023-04-07 20:20:53.484320 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     2427 2023-04-07 20:20:53.485320 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0      476 2023-04-06 23:28:27.135522 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      383 2023-04-06 23:28:27.136521 semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2072 2023-04-07 23:02:47.633613 semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     4641 2023-04-06 23:28:27.137521 semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2403 2023-04-06 23:28:27.137521 semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     5613 2023-04-06 23:28:27.138525 semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0    10609 2023-04-06 23:28:27.138525 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     2342 2023-04-06 23:28:27.139523 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_base.py
+-rw-r--r--   0        0        0     3097 2023-04-06 23:28:27.139523 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_builder.py
+-rw-r--r--   0        0        0     9134 2023-04-10 18:26:09.500824 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_config.py
+-rw-r--r--   0        0        0     1626 2023-04-06 23:28:27.140524 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      710 2023-04-06 23:28:27.141523 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/__init__.py
+-rw-r--r--   0        0        0      210 2023-04-06 23:28:27.141523 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
+-rw-r--r--   0        0        0     2374 2023-04-06 23:28:27.141523 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/import_skills.py
+-rw-r--r--   0        0        0     2323 2023-04-06 23:28:27.142522 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/inline_definition.py
+-rw-r--r--   0        0        0     1531 2023-04-06 23:28:27.142522 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
+-rw-r--r--   0        0        0      160 2023-04-06 23:28:27.143521 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     1174 2023-04-06 23:28:27.143521 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     1598 2023-04-06 23:28:27.143521 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0      299 2023-04-06 23:28:27.144521 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1137 2023-04-06 23:28:27.144521 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     2499 2023-04-06 23:28:27.144521 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     1237 2023-04-06 23:28:27.145522 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0      836 2023-04-06 23:28:27.145522 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/storage/data_entry.py
+-rw-r--r--   0        0        0      953 2023-04-06 23:28:27.145522 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/storage/data_store_base.py
+-rw-r--r--   0        0        0     1989 2023-04-06 23:28:27.145522 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/storage/volatile_data_store.py
+-rw-r--r--   0        0        0     4050 2023-04-06 23:28:27.146521 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2328 2023-04-06 23:28:27.146521 semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-06 23:28:27.146521 semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     8966 2023-04-06 23:28:27.147521 semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-06 23:28:27.147521 semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7322 2023-04-06 23:28:27.147521 semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    16307 2023-04-10 18:26:09.500824 semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6960 2023-04-10 18:26:09.501831 semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      919 2023-04-06 23:28:27.149523 semantic_kernel-0.2.0.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      673 2023-04-06 23:28:27.149523 semantic_kernel-0.2.0.dev0/semantic_kernel/reliability/retry_mechanism.py
+-rw-r--r--   0        0        0     2101 2023-04-06 23:28:27.150523 semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-06 23:28:27.150523 semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-06 23:28:27.151524 semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     3437 2023-04-06 23:28:27.151524 semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-06 23:28:27.152522 semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0      322 2023-04-06 23:28:27.152522 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0     2053 2023-04-06 23:28:27.153521 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     1717 2023-04-06 23:28:27.154523 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0     1026 2023-04-06 23:28:27.154523 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     2104 2023-04-06 23:28:27.155525 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1345 2023-04-06 23:28:27.155525 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      858 2023-04-06 23:28:27.156525 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      837 2023-04-06 23:28:27.156525 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     6056 2023-04-06 23:28:27.156525 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      803 2023-04-06 23:28:27.157522 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0      830 2023-04-06 23:28:27.158522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-06 23:28:27.158522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4566 2023-04-10 18:26:09.501831 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2653 2023-04-06 23:28:27.159522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-06 23:28:27.160524 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1534 2023-04-06 23:28:27.160524 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2274 2023-04-06 23:28:27.160524 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2517 2023-04-06 23:28:27.161522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6535 2023-04-06 23:28:27.161522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6051 2023-04-06 23:28:27.162539 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-06 23:28:27.162539 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3043 2023-04-06 23:28:27.163522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-06 23:28:27.163522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     1115 2023-04-06 23:28:27.157522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0     7637 2023-04-06 23:28:27.164523 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      403 2023-04-06 23:28:27.164523 semantic_kernel-0.2.0.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2436 2023-04-06 23:28:27.165522 semantic_kernel-0.2.0.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-06 23:28:27.165522 semantic_kernel-0.2.0.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-06 23:28:27.165522 semantic_kernel-0.2.0.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     4165 1970-01-01 00:00:00.000000 semantic_kernel-0.2.0.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.1.0.dev0/pyproject.toml` & `semantic_kernel-0.2.0.dev0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.1.0.dev"
+version = "0.2.0.dev"
 description = ""
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.24.2"
 openai = "^0.27.0"
 aiofiles = "^23.1.0"
+asyncio = "^3.4.3"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.21.0"
 black = {version = "^23.1.0", allow-prereleases = true}
 ipykernel = "^6.21.1"
 pytest = "7.2.0"
 ruff = "^0.0.257"
```

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/ai/ai_exception.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/ai/chat_request_settings.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/ai/complete_request_settings.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/complete_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/ai/open_ai/__init__.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_base.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_builder.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_builder.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_config.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     def add_text_backend(
         self,
         service_id: str,
         backend: Union[
             TextCompletionClientBase, Callable[["KernelBase"], TextCompletionClientBase]
         ],
-        overwrite: bool = False,
+        overwrite: bool = True,
     ) -> "KernelConfig":
         if not service_id:
             raise ValueError("service_id must be a non-empty string")
         if not overwrite and service_id in self._text_backends:
             raise ValueError(
                 f"Text backend with service_id '{service_id}' already exists"
             )
@@ -94,15 +94,15 @@
 
     def add_chat_backend(
         self,
         service_id: str,
         backend: Union[
             ChatCompletionClientBase, Callable[["KernelBase"], ChatCompletionClientBase]
         ],
-        overwrite: bool = False,
+        overwrite: bool = True,
     ) -> "KernelConfig":
         if not service_id:
             raise ValueError("service_id must be a non-empty string")
         if not overwrite and service_id in self._chat_backends:
             raise ValueError(
                 f"Chat backend with service_id '{service_id}' already exists"
             )
```

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_extensions/__init__.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_extensions/import_skills.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/import_skills.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_extensions/inline_definition.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/inline_definition.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/kernel_extensions/memory_configuration.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/memory_configuration.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/memory/storage/data_entry.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/storage/data_entry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/memory/storage/data_store_base.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/storage/data_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/memory/storage/volatile_data_store.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/storage/volatile_data_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from enum import Enum
 from logging import Logger
+import threading
 from typing import Any, Callable, List, Optional, cast
+import asyncio
 
 from semantic_kernel.ai.chat_completion_client_base import ChatCompletionClientBase
 from semantic_kernel.ai.chat_request_settings import ChatRequestSettings
 from semantic_kernel.ai.complete_request_settings import CompleteRequestSettings
 from semantic_kernel.ai.text_completion_client_base import TextCompletionClientBase
 from semantic_kernel.kernel_exception import KernelException
 from semantic_kernel.memory.null_memory import NullMemory
@@ -26,14 +28,32 @@
 from semantic_kernel.skill_definition.read_only_skill_collection_base import (
     ReadOnlySkillCollectionBase,
 )
 from semantic_kernel.utils.null_logger import NullLogger
 
 
 class SKFunction(SKFunctionBase):
+    """
+    Semantic Kernel function.
+    """
+
+    class RunThread(threading.Thread):
+        """
+        Async code wrapper to allow running async code inside external
+        event loops such as Jupyter notebooks.
+        """
+
+        def __init__(self, code):
+            self.code = code
+            self.result = None
+            super().__init__()
+
+        def run(self):
+            self.result = asyncio.run(self.code)
+
     _parameters: List[ParameterView]
     _delegate_type: DelegateTypes
     _function: Callable[..., Any]
     _skill_collection: Optional[ReadOnlySkillCollectionBase]
     _log: Logger
     _ai_backend: Optional[TextCompletionClientBase]
     _ai_request_settings: CompleteRequestSettings
@@ -236,14 +256,70 @@
             name=self.name,
             skill_name=self.skill_name,
             description=self.description,
             is_semantic=self.is_semantic,
             parameters=self._parameters,
         )
 
+    def __call__(
+        self,
+        input: Optional[str] = None,
+        context: Optional[SKContext] = None,
+        settings: Optional[CompleteRequestSettings] = None,
+        log: Optional[Logger] = None,
+    ) -> SKContext:
+        return self.invoke(input=input, context=context, settings=settings, log=log)
+
+    def invoke(
+        self,
+        input: Optional[str] = None,
+        context: Optional[SKContext] = None,
+        settings: Optional[CompleteRequestSettings] = None,
+        log: Optional[Logger] = None,
+    ) -> SKContext:
+        if context is None:
+            if self._skill_collection is None:
+                raise ValueError("Skill collection cannot be `None`")
+            assert self._skill_collection is not None
+
+            context = SKContext(
+                ContextVariables(""),
+                NullMemory.instance,  # type: ignore
+                self._skill_collection,
+                log if log is not None else self._log,
+                # TODO: ctoken?
+            )
+
+        if input is not None:
+            context.variables.update(input)
+
+        # Check if there is an event loop
+        try:
+            loop = asyncio.get_running_loop()
+        except RuntimeError:
+            loop = None
+
+        # Handle "asyncio.run() cannot be called from a running event loop"
+        if loop and loop.is_running():
+            if self.is_semantic:
+                thread = self.RunThread(self._invoke_semantic_async(context, settings))
+                thread.start()
+                thread.join()
+                return thread.result
+            else:
+                thread = self.RunThread(self._invoke_native_async(context))
+                thread.start()
+                thread.join()
+                return thread.result
+        else:
+            if self.is_semantic:
+                return asyncio.run(self._invoke_semantic_async(context, settings))
+            else:
+                return asyncio.run(self._invoke_native_async(context))
+
     async def invoke_async(
         self,
         input: Optional[str] = None,
         context: Optional[SKContext] = None,
         settings: Optional[CompleteRequestSettings] = None,
         log: Optional[Logger] = None,
     ) -> SKContext:
@@ -264,26 +340,44 @@
             context.variables.update(input)
 
         if self.is_semantic:
             return await self._invoke_semantic_async(context, settings)
         else:
             return await self._invoke_native_async(context)
 
-    async def invoke_with_custom_input_async(
+    def invoke_with_vars(
+        self,
+        input: ContextVariables,
+        memory: Optional[SemanticTextMemoryBase] = None,
+        log: Optional[Logger] = None,
+    ) -> SKContext:
+        tmp_context = SKContext(
+            variables=input,
+            skill_collection=self._skill_collection,
+            memory=memory if memory is not None else NullMemory.instance,
+            logger=log if log is not None else self._log,
+        )
+
+        try:
+            return self.invoke(input=None, context=tmp_context, log=log)
+        except Exception as e:
+            tmp_context.fail(str(e), e)
+            return tmp_context
+
+    async def invoke_with_vars_async(
         self,
         input: ContextVariables,
-        memory: SemanticTextMemoryBase,
-        skills: ReadOnlySkillCollectionBase,
+        memory: Optional[SemanticTextMemoryBase] = None,
         log: Optional[Logger] = None,
     ) -> SKContext:
         tmp_context = SKContext(
-            input,
-            memory,
-            skills,
-            log if log is not None else self._log,
+            variables=input,
+            skill_collection=self._skill_collection,
+            memory=memory if memory is not None else NullMemory.instance,
+            logger=log if log is not None else self._log,
         )
 
         try:
             return await self.invoke_async(input=None, context=tmp_context, log=log)
         except Exception as e:
             tmp_context.fail(str(e), e)
             return tmp_context
```

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -91,14 +91,38 @@
 
         Returns:
             FunctionView -- The function description.
         """
         pass
 
     @abstractmethod
+    def invoke(
+        self,
+        input: Optional[str] = None,
+        context: Optional[SKContext] = None,
+        settings: Optional[CompleteRequestSettings] = None,
+        log: Optional[Logger] = None
+        # TODO: ctoken
+    ) -> SKContext:
+        """
+        Invokes the function with an explicit string input
+
+        Keyword Arguments:
+            input {str} -- The explicit string input (default: {None})
+            context {SKContext} -- The context to use
+            settings {CompleteRequestSettings} -- LLM completion settings
+            log {Logger} -- Application logger
+
+        Returns:
+            SKContext -- The updated context, potentially a new one if
+            context switching is implemented.
+        """
+        pass
+
+    @abstractmethod
     async def invoke_async(
         self,
         input: Optional[str] = None,
         context: Optional[SKContext] = None,
         settings: Optional[CompleteRequestSettings] = None,
         log: Optional[Logger] = None
         # TODO: ctoken
@@ -115,28 +139,47 @@
         Returns:
             SKContext -- The updated context, potentially a new one if
             context switching is implemented.
         """
         pass
 
     @abstractmethod
-    async def invoke_with_custom_input_async(
+    def invoke_with_vars(
+        self,
+        input: ContextVariables,
+        memory: Optional[SemanticTextMemoryBase] = None,
+        log: Optional[Logger] = None,
+    ) -> SKContext:
+        """
+        Invokes the function with a custom input
+
+        Arguments:
+            input {ContextVariables} -- The custom input
+            memory {SemanticTextMemoryBase} -- The memory to use
+            log {Logger} -- Application logger
+
+        Returns:
+            SKContext -- The updated context, potentially a new one if
+            context switching is implemented.
+        """
+        pass
+
+    @abstractmethod
+    async def invoke_with_vars_async(
         self,
         input: ContextVariables,
-        memory: SemanticTextMemoryBase,
-        skills: "ReadOnlySkillCollectionBase",
+        memory: Optional[SemanticTextMemoryBase] = None,
         log: Optional[Logger] = None,
     ) -> SKContext:
         """
         Invokes the function with a custom input
 
         Arguments:
             input {ContextVariables} -- The custom input
             memory {SemanticTextMemoryBase} -- The memory to use
-            skills {ReadOnlySkillCollectionBase} -- The skill collection to use
             log {Logger} -- Application logger
 
         Returns:
             SKContext -- The updated context, potentially a new one if
             context switching is implemented.
         """
         pass
```

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/reliability/retry_mechanism.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/reliability/retry_mechanism.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/parameter_view.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,16 +92,16 @@
         variables_clone = context.variables.clone()
 
         if len(self._tokens) > 1:
             self.log.debug(f"Passing variable/value: `{self._tokens[1].content}`")
             input_value = self._tokens[1].render(variables_clone)
             variables_clone.update(input_value)
 
-        result = await function.invoke_with_custom_input_async(
-            variables_clone, context.memory, context.skills, self.log
+        result = await function.invoke_with_vars_async(
+            variables_clone, context.memory, self.log
         )
 
         if result.error_occurred:
             error_msg = (
                 f"Function `{f_block.content}` execution failed. "
                 f"{result.last_exception.__class__.__name__}: "
                 f"{result.last_error_description}"
```

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/utils/settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.1.0.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.2.0.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

