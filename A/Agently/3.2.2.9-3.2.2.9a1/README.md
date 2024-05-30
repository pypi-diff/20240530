# Comparing `tmp/Agently-3.2.2.9.tar.gz` & `tmp/Agently-3.2.2.9a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Agently-3.2.2.9.tar", last modified: Wed May 29 15:57:16 2024, max compression
+gzip compressed data, was "Agently-3.2.2.9a1.tar", last modified: Wed May 29 15:53:36 2024, max compression
```

## Comparing `Agently-3.2.2.9.tar` & `Agently-3.2.2.9a1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.024047 Agently-3.2.2.9/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:15.993518 Agently-3.2.2.9/Agently/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:15.995044 Agently-3.2.2.9/Agently/Agent/
--rw-r--r--   0 moxin      (501) staff       (20)    14491 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Agent/Agent.py
--rw-r--r--   0 moxin      (501) staff       (20)     2437 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Agent/AgentFactory.py
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Agent/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:15.996004 Agently-3.2.2.9/Agently/Facility/
--rw-r--r--   0 moxin      (501) staff       (20)     1819 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Facility/FacilityManager.py
--rw-r--r--   0 moxin      (501) staff       (20)       44 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Facility/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:15.996484 Agently-3.2.2.9/Agently/Request/
--rw-r--r--   0 moxin      (501) staff       (20)    10000 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Request/Request.py
--rw-r--r--   0 moxin      (501) staff       (20)       28 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Request/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:15.996936 Agently-3.2.2.9/Agently/WebSocket/
--rw-r--r--   0 moxin      (501) staff       (20)     9550 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/WebSocket/WebSocket.py
--rw-r--r--   0 moxin      (501) staff       (20)       55 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/WebSocket/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:15.998466 Agently-3.2.2.9/Agently/Workflow/
--rw-r--r--   0 moxin      (501) staff       (20)     7650 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/Chunk.py
--rw-r--r--   0 moxin      (501) staff       (20)    16640 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/MainExecutor.py
--rw-r--r--   0 moxin      (501) staff       (20)     6775 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/Schema.py
--rw-r--r--   0 moxin      (501) staff       (20)     3222 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/Workflow.py
--rw-r--r--   0 moxin      (501) staff       (20)       57 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:15.999772 Agently-3.2.2.9/Agently/Workflow/executors/
--rw-r--r--   0 moxin      (501) staff       (20)       67 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/executors/StartExecutor.py
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/executors/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      245 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/executors/install.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.001091 Agently-3.2.2.9/Agently/Workflow/lib/
--rw-r--r--   0 moxin      (501) staff       (20)     1470 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/lib/BreakingHub.py
--rw-r--r--   0 moxin      (501) staff       (20)      656 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/lib/ChunkExecutorABC.py
--rw-r--r--   0 moxin      (501) staff       (20)      426 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/lib/ChunkExecutorManager.py
--rw-r--r--   0 moxin      (501) staff       (20)      500 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/lib/Store.py
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/lib/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      515 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/lib/constants.py
--rw-r--r--   0 moxin      (501) staff       (20)     2058 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/lib/painter.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.002687 Agently-3.2.2.9/Agently/Workflow/utils/
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     4599 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/utils/exec_tree.py
--rw-r--r--   0 moxin      (501) staff       (20)     1411 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/utils/find.py
--rw-r--r--   0 moxin      (501) staff       (20)      613 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/utils/logger.py
--rw-r--r--   0 moxin      (501) staff       (20)      892 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/utils/runtime_supports.py
--rw-r--r--   0 moxin      (501) staff       (20)      242 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/utils/verify.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.004162 Agently-3.2.2.9/Agently/Workflow/yamlflow/
--rw-r--r--   0 moxin      (501) staff       (20)       63 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/yamlflow/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.004908 Agently-3.2.2.9/Agently/Workflow/yamlflow/preset_chunks/
--rw-r--r--   0 moxin      (501) staff       (20)      500 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/yamlflow/preset_chunks/Print.py
--rw-r--r--   0 moxin      (501) staff       (20)      108 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/yamlflow/preset_chunks/Start.py
--rw-r--r--   0 moxin      (501) staff       (20)      289 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/yamlflow/preset_chunks/UserInput.py
--rw-r--r--   0 moxin      (501) staff       (20)      767 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/yamlflow/preset_chunks/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     5728 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/Workflow/yamlflow/yamlflow.py
--rw-r--r--   0 moxin      (501) staff       (20)      571 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      515 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/_global.py
--rw-r--r--   0 moxin      (501) staff       (20)      149 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/global_plugin_manager.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.005115 Agently-3.2.2.9/Agently/plugins/
--rw-r--r--   0 moxin      (501) staff       (20)     4920 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.010539 Agently-3.2.2.9/Agently/plugins/agent_component/
--rw-r--r--   0 moxin      (501) staff       (20)     2913 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/Decorator.py
--rw-r--r--   0 moxin      (501) staff       (20)     2074 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/EventListener.py
--rw-r--r--   0 moxin      (501) staff       (20)     5290 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/OpenAIAssistant.py
--rw-r--r--   0 moxin      (501) staff       (20)      785 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/ReplyReformer.py
--rw-r--r--   0 moxin      (501) staff       (20)     3050 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/Role.py
--rw-r--r--   0 moxin      (501) staff       (20)     4075 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/Search.py
--rw-r--r--   0 moxin      (501) staff       (20)     9781 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/Segment.py
--rw-r--r--   0 moxin      (501) staff       (20)     8280 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/Session.py
--rw-r--r--   0 moxin      (501) staff       (20)     3508 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/Status.py
--rw-r--r--   0 moxin      (501) staff       (20)     9970 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/Tool.py
--rw-r--r--   0 moxin      (501) staff       (20)     2977 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/UserInfo.py
--rw-r--r--   0 moxin      (501) staff       (20)     3849 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/YAMLLoader.py
--rw-r--r--   0 moxin      (501) staff       (20)     2220 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      505 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.012036 Agently-3.2.2.9/Agently/plugins/agent_component/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      588 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/utils/ComponentABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/agent_component/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.013076 Agently-3.2.2.9/Agently/plugins/facility/
--rw-r--r--   0 moxin      (501) staff       (20)     4633 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/facility/Embedding.py
--rw-r--r--   0 moxin      (501) staff       (20)     1874 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/facility/RoleManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     1216 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/facility/StatusManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/facility/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)       85 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/facility/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.013442 Agently-3.2.2.9/Agently/plugins/facility/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      266 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/facility/utils/FacilityABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       36 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/facility/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.016635 Agently-3.2.2.9/Agently/plugins/request/
--rw-r--r--   0 moxin      (501) staff       (20)    12099 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/request/AzureOpenAI.py
--rw-r--r--   0 moxin      (501) staff       (20)     8057 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/request/Claude.py
--rw-r--r--   0 moxin      (501) staff       (20)    10461 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/request/ERNIE.py
--rw-r--r--   0 moxin      (501) staff       (20)     7368 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/request/Google.py
--rw-r--r--   0 moxin      (501) staff       (20)     7769 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/request/Kimi.py
--rw-r--r--   0 moxin      (501) staff       (20)    12270 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/request/MiniMax.py
--rw-r--r--   0 moxin      (501) staff       (20)    13476 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/request/OAIClient.py
--rw-r--r--   0 moxin      (501) staff       (20)    11813 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/request/OpenAI.py
--rw-r--r--   0 moxin      (501) staff       (20)    12624 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/request/ZhipuAI.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/request/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      139 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/request/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.017260 Agently-3.2.2.9/Agently/plugins/request/utils/
--rw-r--r--   0 moxin      (501) staff       (20)     5307 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/request/utils/RequestABC.py
--rw-r--r--   0 moxin      (501) staff       (20)      162 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/request/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     2728 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/request/utils/format.py
--rw-r--r--   0 moxin      (501) staff       (20)     4455 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/request/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.017738 Agently-3.2.2.9/Agently/plugins/storage/
--rw-r--r--   0 moxin      (501) staff       (20)     3156 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/storage/FileStorage.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/storage/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      131 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/storage/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.018000 Agently-3.2.2.9/Agently/plugins/storage/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      745 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/storage/utils/StorageABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       34 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/storage/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.019482 Agently-3.2.2.9/Agently/plugins/tool/
--rw-r--r--   0 moxin      (501) staff       (20)     1828 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/tool/Code.py
--rw-r--r--   0 moxin      (501) staff       (20)     6400 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/tool/Web.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/tool/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      104 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/tool/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.019739 Agently-3.2.2.9/Agently/plugins/tool/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      443 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/tool/utils/ToolABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       28 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/plugins/tool/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      213 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/requirements.txt
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:16.023571 Agently-3.2.2.9/Agently/utils/
--rw-r--r--   0 moxin      (501) staff       (20)     2896 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/utils/AliasManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     6706 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/utils/DataOps.py
--rw-r--r--   0 moxin      (501) staff       (20)      323 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/utils/IdGenerator.py
--rw-r--r--   0 moxin      (501) staff       (20)     2282 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/utils/PluginManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     2418 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/utils/RuntimeCtx.py
--rw-r--r--   0 moxin      (501) staff       (20)     1934 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/utils/StorageDelegate.py
--rw-r--r--   0 moxin      (501) staff       (20)     4963 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/utils/ToolManager.py
--rw-r--r--   0 moxin      (501) staff       (20)      491 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     1928 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/utils/check_version.py
--rw-r--r--   0 moxin      (501) staff       (20)     2868 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/utils/load_json.py
--rw-r--r--   0 moxin      (501) staff       (20)     4328 2024-05-29 15:11:33.000000 Agently-3.2.2.9/Agently/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:57:15.994088 Agently-3.2.2.9/Agently.egg-info/
--rw-r--r--   0 moxin      (501) staff       (20)      848 2024-05-29 15:57:15.000000 Agently-3.2.2.9/Agently.egg-info/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)     3824 2024-05-29 15:57:15.000000 Agently-3.2.2.9/Agently.egg-info/SOURCES.txt
--rw-r--r--   0 moxin      (501) staff       (20)        1 2024-05-29 15:57:15.000000 Agently-3.2.2.9/Agently.egg-info/dependency_links.txt
--rw-r--r--   0 moxin      (501) staff       (20)      130 2024-05-29 15:57:15.000000 Agently-3.2.2.9/Agently.egg-info/requires.txt
--rw-r--r--   0 moxin      (501) staff       (20)        8 2024-05-29 15:57:15.000000 Agently-3.2.2.9/Agently.egg-info/top_level.txt
--rw-r--r--   0 moxin      (501) staff       (20)      848 2024-05-29 15:57:16.023858 Agently-3.2.2.9/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-05-29 15:57:16.024088 Agently-3.2.2.9/setup.cfg
--rw-------   0 moxin      (501) staff       (20)     1006 2024-05-29 15:57:10.000000 Agently-3.2.2.9/setup.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.359912 Agently-3.2.2.9a1/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.328159 Agently-3.2.2.9a1/Agently/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.329615 Agently-3.2.2.9a1/Agently/Agent/
+-rw-r--r--   0 moxin      (501) staff       (20)    14491 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Agent/Agent.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2437 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Agent/AgentFactory.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Agent/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.330717 Agently-3.2.2.9a1/Agently/Facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     1819 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Facility/FacilityManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)       44 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Facility/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.331097 Agently-3.2.2.9a1/Agently/Request/
+-rw-r--r--   0 moxin      (501) staff       (20)    10000 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Request/Request.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Request/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.331514 Agently-3.2.2.9a1/Agently/WebSocket/
+-rw-r--r--   0 moxin      (501) staff       (20)     9550 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/WebSocket/WebSocket.py
+-rw-r--r--   0 moxin      (501) staff       (20)       55 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/WebSocket/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.333120 Agently-3.2.2.9a1/Agently/Workflow/
+-rw-r--r--   0 moxin      (501) staff       (20)     7650 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/Chunk.py
+-rw-r--r--   0 moxin      (501) staff       (20)    16640 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/MainExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6775 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/Schema.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3222 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/Workflow.py
+-rw-r--r--   0 moxin      (501) staff       (20)       57 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.334395 Agently-3.2.2.9a1/Agently/Workflow/executors/
+-rw-r--r--   0 moxin      (501) staff       (20)       67 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/executors/StartExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/executors/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      245 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/executors/install.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.335401 Agently-3.2.2.9a1/Agently/Workflow/lib/
+-rw-r--r--   0 moxin      (501) staff       (20)     1470 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/lib/BreakingHub.py
+-rw-r--r--   0 moxin      (501) staff       (20)      656 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/lib/ChunkExecutorABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      426 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/lib/ChunkExecutorManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)      500 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/lib/Store.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/lib/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/lib/constants.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2058 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/lib/painter.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.337165 Agently-3.2.2.9a1/Agently/Workflow/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4599 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/utils/exec_tree.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1411 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/utils/find.py
+-rw-r--r--   0 moxin      (501) staff       (20)      613 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/utils/logger.py
+-rw-r--r--   0 moxin      (501) staff       (20)      892 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/utils/runtime_supports.py
+-rw-r--r--   0 moxin      (501) staff       (20)      242 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/utils/verify.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.338693 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/
+-rw-r--r--   0 moxin      (501) staff       (20)       63 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.339396 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/preset_chunks/
+-rw-r--r--   0 moxin      (501) staff       (20)      500 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/preset_chunks/Print.py
+-rw-r--r--   0 moxin      (501) staff       (20)      108 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/preset_chunks/Start.py
+-rw-r--r--   0 moxin      (501) staff       (20)      289 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/preset_chunks/UserInput.py
+-rw-r--r--   0 moxin      (501) staff       (20)      767 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/preset_chunks/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5728 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/yamlflow.py
+-rw-r--r--   0 moxin      (501) staff       (20)      571 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/_global.py
+-rw-r--r--   0 moxin      (501) staff       (20)      149 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/global_plugin_manager.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.339597 Agently-3.2.2.9a1/Agently/plugins/
+-rw-r--r--   0 moxin      (501) staff       (20)     4920 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.344391 Agently-3.2.2.9a1/Agently/plugins/agent_component/
+-rw-r--r--   0 moxin      (501) staff       (20)     2913 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/Decorator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2074 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/EventListener.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5290 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/OpenAIAssistant.py
+-rw-r--r--   0 moxin      (501) staff       (20)      785 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/ReplyReformer.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3050 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/Role.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4075 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/Search.py
+-rw-r--r--   0 moxin      (501) staff       (20)     9781 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/Segment.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8280 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/Session.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3508 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/Status.py
+-rw-r--r--   0 moxin      (501) staff       (20)     9970 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/Tool.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2977 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/UserInfo.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3849 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/YAMLLoader.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2220 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      505 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.345807 Agently-3.2.2.9a1/Agently/plugins/agent_component/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      588 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/utils/ComponentABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.346544 Agently-3.2.2.9a1/Agently/plugins/facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     4633 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/facility/Embedding.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1874 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/facility/RoleManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1216 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/facility/StatusManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/facility/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)       85 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/facility/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.346874 Agently-3.2.2.9a1/Agently/plugins/facility/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      266 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/facility/utils/FacilityABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       36 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/facility/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.352241 Agently-3.2.2.9a1/Agently/plugins/request/
+-rw-r--r--   0 moxin      (501) staff       (20)    12099 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/AzureOpenAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8057 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/Claude.py
+-rw-r--r--   0 moxin      (501) staff       (20)    10461 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/ERNIE.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7368 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/Google.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7769 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/Kimi.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12270 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/MiniMax.py
+-rw-r--r--   0 moxin      (501) staff       (20)    13476 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/OAIClient.py
+-rw-r--r--   0 moxin      (501) staff       (20)    11813 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/OpenAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12624 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/ZhipuAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      139 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.352786 Agently-3.2.2.9a1/Agently/plugins/request/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     5307 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/utils/RequestABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      162 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2728 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/utils/format.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4455 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.353285 Agently-3.2.2.9a1/Agently/plugins/storage/
+-rw-r--r--   0 moxin      (501) staff       (20)     3156 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/storage/FileStorage.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/storage/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      131 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/storage/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.353553 Agently-3.2.2.9a1/Agently/plugins/storage/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      745 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/storage/utils/StorageABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       34 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/storage/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.355134 Agently-3.2.2.9a1/Agently/plugins/tool/
+-rw-r--r--   0 moxin      (501) staff       (20)     1828 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/tool/Code.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6400 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/tool/Web.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/tool/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      104 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/tool/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.355409 Agently-3.2.2.9a1/Agently/plugins/tool/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      443 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/tool/utils/ToolABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/tool/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      213 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/requirements.txt
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.359394 Agently-3.2.2.9a1/Agently/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     2896 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/AliasManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6706 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/DataOps.py
+-rw-r--r--   0 moxin      (501) staff       (20)      323 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/IdGenerator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2282 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/PluginManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2418 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/RuntimeCtx.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1934 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/StorageDelegate.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4963 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/ToolManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)      491 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1928 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/check_version.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2868 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/load_json.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4328 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.328705 Agently-3.2.2.9a1/Agently.egg-info/
+-rw-r--r--   0 moxin      (501) staff       (20)      850 2024-05-29 15:53:36.000000 Agently-3.2.2.9a1/Agently.egg-info/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)     3824 2024-05-29 15:53:36.000000 Agently-3.2.2.9a1/Agently.egg-info/SOURCES.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        1 2024-05-29 15:53:36.000000 Agently-3.2.2.9a1/Agently.egg-info/dependency_links.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      130 2024-05-29 15:53:36.000000 Agently-3.2.2.9a1/Agently.egg-info/requires.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        8 2024-05-29 15:53:36.000000 Agently-3.2.2.9a1/Agently.egg-info/top_level.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      850 2024-05-29 15:53:36.359707 Agently-3.2.2.9a1/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-05-29 15:53:36.359960 Agently-3.2.2.9a1/setup.cfg
+-rw-------   0 moxin      (501) staff       (20)     1014 2024-05-29 15:13:08.000000 Agently-3.2.2.9a1/setup.py
```

### Comparing `Agently-3.2.2.9/Agently/Agent/Agent.py` & `Agently-3.2.2.9a1/Agently/Agent/Agent.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Agent/AgentFactory.py` & `Agently-3.2.2.9a1/Agently/Agent/AgentFactory.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Facility/FacilityManager.py` & `Agently-3.2.2.9a1/Agently/Facility/FacilityManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Request/Request.py` & `Agently-3.2.2.9a1/Agently/Request/Request.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/WebSocket/WebSocket.py` & `Agently-3.2.2.9a1/Agently/WebSocket/WebSocket.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Workflow/Chunk.py` & `Agently-3.2.2.9a1/Agently/Workflow/Chunk.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Workflow/MainExecutor.py` & `Agently-3.2.2.9a1/Agently/Workflow/MainExecutor.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Workflow/Schema.py` & `Agently-3.2.2.9a1/Agently/Workflow/Schema.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Workflow/Workflow.py` & `Agently-3.2.2.9a1/Agently/Workflow/Workflow.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Workflow/lib/BreakingHub.py` & `Agently-3.2.2.9a1/Agently/Workflow/lib/BreakingHub.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Workflow/lib/ChunkExecutorABC.py` & `Agently-3.2.2.9a1/Agently/Workflow/lib/ChunkExecutorABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Workflow/lib/constants.py` & `Agently-3.2.2.9a1/Agently/Workflow/lib/constants.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Workflow/lib/painter.py` & `Agently-3.2.2.9a1/Agently/Workflow/lib/painter.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Workflow/utils/exec_tree.py` & `Agently-3.2.2.9a1/Agently/Workflow/utils/exec_tree.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Workflow/utils/find.py` & `Agently-3.2.2.9a1/Agently/Workflow/utils/find.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Workflow/utils/logger.py` & `Agently-3.2.2.9a1/Agently/Workflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Workflow/utils/runtime_supports.py` & `Agently-3.2.2.9a1/Agently/Workflow/utils/runtime_supports.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Workflow/yamlflow/preset_chunks/__init__.py` & `Agently-3.2.2.9a1/Agently/Workflow/yamlflow/preset_chunks/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/Workflow/yamlflow/yamlflow.py` & `Agently-3.2.2.9a1/Agently/Workflow/yamlflow/yamlflow.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/__init__.py` & `Agently-3.2.2.9a1/Agently/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/_global.py` & `Agently-3.2.2.9a1/Agently/_global.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/__init__.py` & `Agently-3.2.2.9a1/Agently/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/agent_component/Decorator.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/Decorator.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/agent_component/EventListener.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/EventListener.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/agent_component/OpenAIAssistant.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/OpenAIAssistant.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/agent_component/ReplyReformer.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/ReplyReformer.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/agent_component/Role.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/Role.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/agent_component/Search.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/Search.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/agent_component/Segment.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/Segment.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/agent_component/Session.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/Session.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/agent_component/Status.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/Status.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/agent_component/Tool.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/Tool.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/agent_component/UserInfo.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/UserInfo.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/agent_component/YAMLLoader.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/YAMLLoader.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/agent_component/__init__.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/agent_component/utils/ComponentABC.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/utils/ComponentABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/facility/Embedding.py` & `Agently-3.2.2.9a1/Agently/plugins/facility/Embedding.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/facility/RoleManager.py` & `Agently-3.2.2.9a1/Agently/plugins/facility/RoleManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/facility/StatusManager.py` & `Agently-3.2.2.9a1/Agently/plugins/facility/StatusManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/facility/__init__.py` & `Agently-3.2.2.9a1/Agently/plugins/facility/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/request/AzureOpenAI.py` & `Agently-3.2.2.9a1/Agently/plugins/request/AzureOpenAI.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/request/Claude.py` & `Agently-3.2.2.9a1/Agently/plugins/request/Claude.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/request/ERNIE.py` & `Agently-3.2.2.9a1/Agently/plugins/request/ERNIE.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/request/Google.py` & `Agently-3.2.2.9a1/Agently/plugins/request/Google.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/request/Kimi.py` & `Agently-3.2.2.9a1/Agently/plugins/request/Kimi.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/request/MiniMax.py` & `Agently-3.2.2.9a1/Agently/plugins/request/MiniMax.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/request/OAIClient.py` & `Agently-3.2.2.9a1/Agently/plugins/request/OAIClient.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/request/OpenAI.py` & `Agently-3.2.2.9a1/Agently/plugins/request/OpenAI.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/request/ZhipuAI.py` & `Agently-3.2.2.9a1/Agently/plugins/request/ZhipuAI.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/request/__init__.py` & `Agently-3.2.2.9a1/Agently/plugins/request/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/request/utils/RequestABC.py` & `Agently-3.2.2.9a1/Agently/plugins/request/utils/RequestABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/request/utils/format.py` & `Agently-3.2.2.9a1/Agently/plugins/request/utils/format.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/request/utils/transform.py` & `Agently-3.2.2.9a1/Agently/plugins/request/utils/transform.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/storage/FileStorage.py` & `Agently-3.2.2.9a1/Agently/plugins/storage/FileStorage.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/storage/__init__.py` & `Agently-3.2.2.9a1/Agently/plugins/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/storage/utils/StorageABC.py` & `Agently-3.2.2.9a1/Agently/plugins/storage/utils/StorageABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/tool/Code.py` & `Agently-3.2.2.9a1/Agently/plugins/tool/Code.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/tool/Web.py` & `Agently-3.2.2.9a1/Agently/plugins/tool/Web.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/plugins/tool/__init__.py` & `Agently-3.2.2.9a1/Agently/plugins/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/utils/AliasManager.py` & `Agently-3.2.2.9a1/Agently/utils/AliasManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/utils/DataOps.py` & `Agently-3.2.2.9a1/Agently/utils/DataOps.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/utils/PluginManager.py` & `Agently-3.2.2.9a1/Agently/utils/PluginManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/utils/RuntimeCtx.py` & `Agently-3.2.2.9a1/Agently/utils/RuntimeCtx.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/utils/StorageDelegate.py` & `Agently-3.2.2.9a1/Agently/utils/StorageDelegate.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/utils/ToolManager.py` & `Agently-3.2.2.9a1/Agently/utils/ToolManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/utils/check_version.py` & `Agently-3.2.2.9a1/Agently/utils/check_version.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/utils/load_json.py` & `Agently-3.2.2.9a1/Agently/utils/load_json.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently/utils/transform.py` & `Agently-3.2.2.9a1/Agently/utils/transform.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/Agently.egg-info/PKG-INFO` & `Agently-3.2.2.9a1/Agently.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Agently
-Version: 3.2.2.9
+Version: 3.2.2.9a1
 Summary: Agently, a framework to build applications based on language model powered intelligent agents.
 Home-page: https://github.com/Maplemx/Agently
 Author: Maplemx
 Author-email: maplemx@gmail.com
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Agently-3.2.2.9/Agently.egg-info/SOURCES.txt` & `Agently-3.2.2.9a1/Agently.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.9/PKG-INFO` & `Agently-3.2.2.9a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Agently
-Version: 3.2.2.9
+Version: 3.2.2.9a1
 Summary: Agently, a framework to build applications based on language model powered intelligent agents.
 Home-page: https://github.com/Maplemx/Agently
 Author: Maplemx
 Author-email: maplemx@gmail.com
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Agently-3.2.2.9/setup.py` & `Agently-3.2.2.9a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 for requirement in origin_requirements:
     if not requirement.startswith("#"):
         requirements.append(requirement)
 
 
 setuptools.setup(
     name = "Agently",
-    version = "3.2.2.9",
+    version = "3.2.2.9-alpha-1",
     author = "Maplemx",
     author_email = "maplemx@gmail.com",
     description = "Agently, a framework to build applications based on language model powered intelligent agents.",
     long_description = "https://github.com/Maplemx/Agently",
     url = "https://github.com/Maplemx/Agently",
     license='Apache License, Version 2.0',
     #packages = ["Agently"],
```

